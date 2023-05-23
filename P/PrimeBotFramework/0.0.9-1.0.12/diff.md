# Comparing `tmp/PrimeBotFramework-0.0.9.tar.gz` & `tmp/PrimeBotFramework-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrimeBotFramework-0.0.9.tar", last modified: Tue Dec 20 17:49:26 2022, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-ceqp5mot/PrimeBotFramework-1.0.12.tar", last modified: Tue May 23 18:21:57 2023, max compression
```

## Comparing `PrimeBotFramework-0.0.9.tar` & `PrimeBotFramework-1.0.12.tar`

### file list

```diff
@@ -1,32 +1,49 @@
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.560529 PrimeBotFramework-0.0.9/
--rw-rw-rw-   0        0        0      868 2022-12-20 17:47:57.000000 PrimeBotFramework-0.0.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0       30 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3786 2022-12-20 17:49:26.559531 PrimeBotFramework-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.535594 PrimeBotFramework-0.0.9/PrimeBot/
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.548559 PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/
--rw-rw-rw-   0        0        0     1932 2022-12-20 17:44:24.000000 PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0        0        0      693 2022-12-20 17:45:49.000000 PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0        0        0      336 2022-12-20 17:44:43.000000 PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.549556 PrimeBotFramework-0.0.9/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0        0        0     2912 2022-12-20 11:57:30.000000 PrimeBotFramework-0.0.9/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.550554 PrimeBotFramework-0.0.9/PrimeBot/Documents/
--rw-rw-rw-   0        0        0     1115 2022-12-20 11:58:03.000000 PrimeBotFramework-0.0.9/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.553548 PrimeBotFramework-0.0.9/PrimeBot/Elastic/
--rw-rw-rw-   0        0        0     1292 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.554544 PrimeBotFramework-0.0.9/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0        0        0     9261 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.556540 PrimeBotFramework-0.0.9/PrimeBot/Mongo/
--rw-rw-rw-   0        0        0      431 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.557538 PrimeBotFramework-0.0.9/PrimeBot/Vault/
--rw-rw-rw-   0        0        0     2828 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.544569 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/
--rw-rw-rw-   0        0        0     3786 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2307 2022-12-20 13:06:05.000000 PrimeBotFramework-0.0.9/README.md
--rw-rw-rw-   0        0        0      213 2022-12-20 12:32:35.000000 PrimeBotFramework-0.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-12-20 17:49:26.560529 PrimeBotFramework-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      971 2022-12-20 17:46:18.000000 PrimeBotFramework-0.0.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/.pypirc
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/CHANGELOG.txt
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6609 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    26928 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/Pipfile.lock
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6609 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      817 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4332 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/setup.py
```

### Comparing `PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/__init__.py` & `PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,56 @@
-import requests
-from PrimeBot.CpfCnpj.model import Endereco, DadosEmpresa, Erro
-from PrimeBot.CpfCnpj.api_codes import Package, Error
-
-def set_token(token: str) -> None:
-    global TOKEN
-    TOKEN = token
-
-
-def consulta_cnpj(cnpj: str) -> dict:
-    base_url = "https://api.cpfcnpj.com.br/"
-    if not TOKEN:
-        raise Exception("Token não definido")
-    CALL_URL = f"{base_url}/{TOKEN}/{Package.CNPJ_C.value}/{cnpj}"
-    response = requests.get(CALL_URL)
-    response_json = response.json()
-    error_list = [
-        Error.CNPJ_INCOMPLETO.value,
-        Error.CNPJ_INVALIDO.value,
-        Error.CNPJ_INEXISTENTE.value,
-        Error.TOKEN_INVALIDO.value,
-        Error.FORNECEDOR_INDISPONIVEL.value,
-        Error.IMPOSSIVEL_CONSULTAR.value,
-        Error.CONTA_BLOQUEADA.value,
-        Error.CREDITOS_INSUFICIENTES.value,
-        Error.PACOTE_INVALIDO.value,
-    ]
-
-    if response_json["status"]:
-        endereco = response_json["matrizEndereco"]
-        resultado = DadosEmpresa(
-            razao_social=response_json["razao"],
-            situacao=response_json["situacao"]["nome"],
-            endereco= Endereco(
-                logradouro=endereco["logradouro"],
-                bairro=endereco["bairro"],
-                cep=endereco["cep"],
-                cidade=endereco["cidade"],
-                uf=endereco["uf"],
-            ),
-        )
-    elif response_json["erroCodigo"] == Error.BLACKLIST.value:
-        resultado = Erro(
-            erro=response_json["blacklist"]["motivo"],
-            codigo=response_json["erroCodigo"],
-        )
-    elif response_json["erroCodigo"] in error_list:
-        resultado = Erro(
-            erro=response_json["erro"],
-            codigo=response_json["erroCodigo"],
-        )
-    else:
-        resultado = Erro(
-            erro="Erro desconhecido",
-            codigo=999,
-        )
-
+import requests
+from PrimeBot.CpfCnpj.model import Endereco, DadosEmpresa
+from PrimeBot.CpfCnpj.api_codes import Package, Error
+
+def set_token(token: str) -> None:
+    global TOKEN
+    TOKEN = token
+
+
+def consulta_cnpj_pacote_C(cnpj: str) -> dict:
+    base_url = "https://api.cpfcnpj.com.br/"
+    if not TOKEN:
+        raise Exception("Token não definido")
+    CALL_URL = f"{base_url}/{TOKEN}/{Package.CNPJ_C.value}/{cnpj}"
+    response = requests.get(CALL_URL)
+    response_json = response.json()
+    error_list = [
+        Error.CNPJ_INCOMPLETO.value,
+        Error.CNPJ_INVALIDO.value,
+        Error.CNPJ_INEXISTENTE.value,
+        Error.TOKEN_INVALIDO.value,
+        Error.FORNECEDOR_INDISPONIVEL.value,
+        Error.IMPOSSIVEL_CONSULTAR.value,
+        Error.CONTA_BLOQUEADA.value,
+        Error.CREDITOS_INSUFICIENTES.value,
+        Error.PACOTE_INVALIDO.value,
+    ]
+
+    if response_json["status"]:
+        endereco = response_json["matrizEndereco"]
+        resultado = DadosEmpresa(
+            razao_social=response_json["razao"],
+            cnpj=response_json["cnpj"],
+            situacao=response_json["situacao"]["nome"],
+            endereco= Endereco(
+                logradouro=endereco["logradouro"],
+                bairro=endereco["bairro"],
+                cep=endereco["cep"],
+                cidade=endereco["cidade"],
+                uf=endereco["uf"],
+            ),
+            delay=response_json["delay"],
+            saldo=response_json["saldo"]
+        )
+    elif response_json["erroCodigo"] == Error.BLACKLIST.value:
+        erro=response_json["blacklist"]["motivo"]
+        codigo=response_json["erroCodigo"]
+        raise Exception(str(codigo) + ": " + erro)
+    elif response_json["erroCodigo"] in error_list:
+        erro=response_json["erro"]
+        codigo=response_json["erroCodigo"]
+        raise Exception(str(codigo) + ": " + erro)
+    else:
+        raise Exception("999: Erro desconhecido")
+
     return resultado.dict()
```

### Comparing `PrimeBotFramework-0.0.9/PrimeBot/DeathByCaptcha/__init__.py` & `PrimeBotFramework-1.0.12/PrimeBot/DeathByCaptcha/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from pathlib import Path
-import time
-import requests
-import json
-
-
-class DeathByCaptcha:
-    URL = "http://api.dbcapi.me/api/captcha"
-
-    def __init__(self,token):
-        self.token = token
-
-
-    def config_h_captcha(self,sitekey,pageurl,proxy="",proxytype=""):
-        self.sitekey = sitekey
-        self.pageurl = pageurl
-        self.proxytype = proxytype
-        self.proxy = proxy
-
-    # def config_img_captcha(self,token):
-    #     self.token = token
-
-    def resolve_HCaptcha(self,timeout=30):
-        hcaptcha_params = {
-            "proxy": self.proxy,
-            "proxytype": self.proxytype,
-            "sitekey": self.sitekey,
-            "pageurl": self.pageurl
-        }
-
-        payload = {
-            'authtoken': self.token,
-            'type': '7',
-            'hcaptcha_params': json.dumps(hcaptcha_params)
-        }
-
-        response = requests.request("POST", self.URL, data=payload)
-        if response.status_code != 200:
-            return Exception(response.text)
-        
-        data = {x.split('=')[0]:x.split('=')[1] for x in response.text.split("&")}
-        if data["is_correct"] == "0":
-            return Exception("Data Sent is not correct!")
-
-        return self.waitSolution(data["captcha"],timeout=timeout) 
-
-
-
-    def resolve_ImageCaptcha(self,captchaImage,timeout=30):
-        tempo = 0
-        while tempo < 30:
-            fName = Path(captchaImage).stem + Path(captchaImage).suffix
-            payload = {
-                'authtoken': self.token,
-            }
-            files=[
-                ('captchafile',(fName,open(captchaImage,'rb'),'application/octet-stream'))
-            ]
-
-            response = requests.request("POST", self.URL, data=payload,files=files)
-        
-            if response.status_code == 200:
-                break
-            else:
-                time.sleep(2)
-                tempo=tempo+2
-                
-        
-        if response.status_code != 200:
-            return Exception(response.text)
-
-        data = {x.split('=')[0]:x.split('=')[1] for x in response.text.split("&")}
-        if data["is_correct"] == "0":
-            return Exception("Data Sent is not correct!")
-        
-        return self.waitSolution(data["captcha"],timeout=timeout)
-        
-   
-    def waitSolution(self,captcha,timeout=30):
-        start = time.time()
-        response = requests.request("GET", f"{self.URL}/{captcha}")
-        data = {x.split('=')[0]:x.split('=')[1] for x in response.text.split("&")}
-        if data["is_correct"] == "0":
-            return Exception("Data received is not correct!")
-        if timeout <= 0:
-            return Exception("Timeout solving captcha")
-        if data["text"] == "":
-            count = time.time()- start
-            return self.waitSolution(captcha,timeout-count)
-        
+from pathlib import Path
+import time
+import requests
+import json
+
+
+class DeathByCaptcha:
+    URL = "http://api.dbcapi.me/api/captcha"
+
+    def __init__(self,token):
+        self.token = token
+
+
+    def config_h_captcha(self,sitekey,pageurl,proxy="",proxytype=""):
+        self.sitekey = sitekey
+        self.pageurl = pageurl
+        self.proxytype = proxytype
+        self.proxy = proxy
+
+    # def config_img_captcha(self,token):
+    #     self.token = token
+
+    def resolve_HCaptcha(self,timeout=30):
+        hcaptcha_params = {
+            "proxy": self.proxy,
+            "proxytype": self.proxytype,
+            "sitekey": self.sitekey,
+            "pageurl": self.pageurl
+        }
+
+        payload = {
+            'authtoken': self.token,
+            'type': '7',
+            'hcaptcha_params': json.dumps(hcaptcha_params)
+        }
+
+        response = requests.request("POST", self.URL, data=payload)
+        if response.status_code != 200:
+            return Exception(response.text)
+        
+        data = {x.split('=')[0]:x.split('=')[1] for x in response.text.split("&")}
+        if data["is_correct"] == "0":
+            return Exception("Data Sent is not correct!")
+
+        return self.waitSolution(data["captcha"],timeout=timeout) 
+
+
+
+    def resolve_ImageCaptcha(self,captchaImage,timeout=30):
+        tempo = 0
+        while tempo < 30:
+            fName = Path(captchaImage).stem + Path(captchaImage).suffix
+            payload = {
+                'authtoken': self.token,
+            }
+            files=[
+                ('captchafile',(fName,open(captchaImage,'rb'),'application/octet-stream'))
+            ]
+
+            response = requests.request("POST", self.URL, data=payload,files=files)
+        
+            if response.status_code == 200:
+                break
+            else:
+                time.sleep(2)
+                tempo=tempo+2
+                
+        
+        if response.status_code != 200:
+            return Exception(response.text)
+
+        data = {x.split('=')[0]:x.split('=')[1] for x in response.text.split("&")}
+        if data["is_correct"] == "0":
+            return Exception("Data Sent is not correct!")
+        
+        return self.waitSolution(data["captcha"],timeout=timeout)
+        
+   
+    def waitSolution(self,captcha,timeout=30):
+        start = time.time()
+        response = requests.request("GET", f"{self.URL}/{captcha}")
+        data = {x.split('=')[0]:x.split('=')[1] for x in response.text.split("&")}
+        if data["is_correct"] == "0":
+            return Exception("Data received is not correct!")
+        if timeout <= 0:
+            return Exception("Timeout solving captcha")
+        if data["text"] == "":
+            count = time.time()- start
+            return self.waitSolution(captcha,timeout-count)
+        
         return data["text"]
```

### Comparing `PrimeBotFramework-0.0.9/PrimeBot/Documents/__init__.py` & `PrimeBotFramework-1.0.12/PrimeBot/Documents/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-from ast import Raise
-import re
-
-def verifica_digito_cnpj(cnpj):
-
-    cnpj = re.sub(r'[#*-.,/!]', '', cnpj)
-    
-    tamanho_cnpj = (len(cnpj))
-
-    if tamanho_cnpj < 14:
-        ultimos_quatro_numeros= cnpj[-4:]
-        validar_matriz= ultimos_quatro_numeros[0:3]
-        if  validar_matriz != '000':
-            cnpj = cnpj + '0001'
-
-        cnpj= cnpj[-12:]
-        
-        calc_num = [6,7,8,9,2,3,4,5,6,7,8,9]
-
-        if len(cnpj) != 12:
-            Raise("Por favor insira os 12 digitos do cnpj!")
-
-        cgcPriDig = sum([n*int(v) for n,v in zip(calc_num,cnpj)])%11
-
-        if(cgcPriDig==10):cgcPriDig=0
-
-        cnpj2 = cnpj + str(cgcPriDig)
-
-        cgcSegDig = sum([n*int(v) for n,v in zip([5] + calc_num,cnpj2)])%11
-        if(cgcPriDig==10):cgcPriDig=0
-        if(cgcSegDig==10):cgcSegDig=0
-
-        cgcDV=cgcPriDig*10+cgcSegDig
-        cgcDV=f"{cgcDV:02d}"
-
-        cnpj=cnpj+cgcDV
-    else:
-        ultimos_seis_numeros= cnpj[-6:]
-        validar_matriz= ultimos_seis_numeros[0:3]
-        if  validar_matriz != '000':
-            cnpj = ''
-
+from ast import Raise
+import re
+
+def verifica_digito_cnpj(cnpj):
+
+    cnpj = re.sub(r'[#*-.,/!]', '', cnpj)
+    
+    tamanho_cnpj = (len(cnpj))
+
+    if tamanho_cnpj < 14:
+        ultimos_quatro_numeros= cnpj[-4:]
+        validar_matriz= ultimos_quatro_numeros[0:3]
+        if  validar_matriz != '000':
+            cnpj = cnpj + '0001'
+
+        cnpj= cnpj[-12:]
+        
+        calc_num = [6,7,8,9,2,3,4,5,6,7,8,9]
+
+        if len(cnpj) != 12:
+            Raise("Por favor insira os 12 digitos do cnpj!")
+
+        cgcPriDig = sum([n*int(v) for n,v in zip(calc_num,cnpj)])%11
+
+        if(cgcPriDig==10):cgcPriDig=0
+
+        cnpj2 = cnpj + str(cgcPriDig)
+
+        cgcSegDig = sum([n*int(v) for n,v in zip([5] + calc_num,cnpj2)])%11
+        if(cgcPriDig==10):cgcPriDig=0
+        if(cgcSegDig==10):cgcSegDig=0
+
+        cgcDV=cgcPriDig*10+cgcSegDig
+        cgcDV=f"{cgcDV:02d}"
+
+        cnpj=cnpj+cgcDV
+    else:
+        cnpj= cnpj[-14:]
+        ultimos_seis_numeros= cnpj[-6:]
+        validar_matriz= ultimos_seis_numeros[0:3]
+        if  validar_matriz != '000':
+            cnpj = ''
+
     return cnpj
```

### Comparing `PrimeBotFramework-0.0.9/PrimeBot/Elastic/__init__.py` & `PrimeBotFramework-1.0.12/PrimeBot/Elastic/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from datetime import datetime
-from elasticsearch_dsl import Document, Date, Keyword, connections, \
-    Integer
-
-
-class BaseDocument(Document):
-    timestamp = Date(default_timezone='Brazil/East')
-    robot_name = Keyword()
-
-    @classmethod
-    def connect(cls, host, user, pwd):
-        connections.create_connection(hosts=[host], http_auth=f'{user}:{pwd}')
-
-
-class RobotLog(BaseDocument):
-    message = Keyword()
-    level = Keyword()
-
-    class Index:
-        name = 'robot-logs'
-        settings = {
-            "number_of_shards": 1
-        }
-
-    def save(self, **kwargs):
-        if not self.timestamp:
-            self.timestamp = datetime.now()
-
-        kwargs['index'] = self.timestamp.strftime(
-            f'robot-logs-{self.robot_name}-%Y.%m')
-        return super().save(**kwargs)
-
-
-class SuiteLog(BaseDocument):
-    status = Keyword()
-    duration = Integer()
-
-    class Index:
-        name = 'robot-suite'
-        settings = {
-            "number_of_shards": 1
-        }
-
-    def save(self, **kwargs):
-        if not self.timestamp:
-            self.timestamp = datetime.now()
-
-        kwargs['index'] = self.timestamp.strftime(
-            f'robot-suite-{self.robot_name}-%Y.%m')
-        return super().save(**kwargs)
-
-
-
+from datetime import datetime
+from elasticsearch_dsl import Document, Date, Keyword, connections, \
+    Integer
+
+
+class BaseDocument(Document):
+    timestamp = Date(default_timezone='Brazil/East')
+    robot_name = Keyword()
+
+    @classmethod
+    def connect(cls, host, user, pwd):
+        connections.create_connection(hosts=[host], http_auth=f'{user}:{pwd}')
+
+
+class RobotLog(BaseDocument):
+    message = Keyword()
+    level = Keyword()
+
+    class Index:
+        name = 'robot-logs'
+        settings = {
+            "number_of_shards": 1
+        }
+
+    def save(self, **kwargs):
+        if not self.timestamp:
+            self.timestamp = datetime.now()
+
+        kwargs['index'] = self.timestamp.strftime(
+            f'robot-logs-{self.robot_name}-%Y.%m')
+        return super().save(**kwargs)
+
+
+class SuiteLog(BaseDocument):
+    status = Keyword()
+    duration = Integer()
+
+    class Index:
+        name = 'robot-suite'
+        settings = {
+            "number_of_shards": 1
+        }
+
+    def save(self, **kwargs):
+        if not self.timestamp:
+            self.timestamp = datetime.now()
+
+        kwargs['index'] = self.timestamp.strftime(
+            f'robot-suite-{self.robot_name}-%Y.%m')
+        return super().save(**kwargs)
+
+
+
```

### Comparing `PrimeBotFramework-0.0.9/PrimeBot/ExchangeGraph/__init__.py` & `PrimeBotFramework-1.0.12/PrimeBot/ExchangeGraph/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,274 +1,274 @@
-from ast import Raise
-import base64
-from dataclasses import Field, dataclass, field
-from email.policy import default
-from functools import wraps
-import msal
-import requests
-import json
-from dateUts import *
-import os
-
-
-@dataclass
-class OauthParams:
-    username     : str
-    password     : str
-    client_id    : str
-    client_secret: str
-    tenant_id    : str
-    user_id      : str
-    base_url     : str = field(default='')
-    authority    : str = field(default='')
-
-class ExchangeAuth:
-    last_token_key_at = None
-    token_code        = None
-    exp_secs          = None
-
-    def __init__(self, config: OauthParams):
-    
-        self.config = config
-        self.config.authority = f"https://login.microsoftonline.com/{self.config.tenant_id}"
-        self.config.base_url = f"https://graph.microsoft.com/v1.0/users/{self.config.user_id}"
-        self.app = msal.ConfidentialClientApplication(
-            client_id=config.client_id,
-            client_credential=config.client_secret,
-            authority=config.authority)
-
-    def update_token(self):
-        # TODO Avaliar se pode vir como parametro
-        scopes = ["https://graph.microsoft.com/.default"]
-        result = None
-        result = self.app.acquire_token_by_username_password(
-            username=self.config.username,
-            password=self.config.password,
-            scopes=scopes
-        )
-        if not result:
-            print(
-                "Não existe um token em cache. Criando um novo do Azure Active Directory.")
-        result = self.app.acquire_token_for_client(scopes=scopes)
-        if "access_token" in result:
-            print(result)
-            #print("Access token - " + result["access_token"])
-            self.token_code = result["access_token"]
-            self.last_token_key_at = today()
-            self.exp_secs = result["expires_in"]
-            return (True, '')
-        else:
-            return (False, result)
-
-    def validate_token(self):
-        expired = False
-        if self.last_token_key_at:
-            expired = today() >= dateAdd(self.last_token_key_at, self.exp_secs-10*60, 'seconds')
-
-        if not self.last_token_key_at or expired:
-            resp = self.update_token()
-            if not resp[0]:
-                raise Exception(f"Error generating new Token:{resp[1]}")
-            else:
-                print("New token generated!")
-
-    @property
-    def headers(self):
-        self.validate_token()
-        return {"Authorization": f"Bearer {self.token_code}"}
-
-    @property
-    def token(self):
-        self.validate_token()
-        self.token_code
-
-class OFolder:
-    def __init__(self,jsonObj:dict,cnt:ExchangeAuth):
-        self.__dict__ = jsonObj
-        self.exgAuth = cnt
-
-    def childFolders(self):
-        
-        endpoint = f"{self.exgAuth.config.base_url}/mailFolders/{self.id}/childFolders"
-        r = requests.get(url=endpoint, headers=self.exgAuth.headers)
-        if r.status_code != 200: raise Exception("Error:" + r.text)
-        fdrs = [OFolder(x,self.exgAuth) for x in r.json()["value"]]
-        return fdrs
-
-    def get_mails(self,**kargs):
-        params = "&".join([f"{k}={v}" for k,v in kargs.items() if v is not None])
-        endpoint = f"{self.exgAuth.config.base_url}/mailFolders/{self.id}/messages?{params}"
-        emailList = []
-        data = None
-
-        while True:
-            url = endpoint if not data else data["@odata.nextLink"]
-            r = requests.get(url, headers=self.exgAuth.headers)
-            if r.status_code != 200:
-                raise Exception("Error:" + r.text)
-            data = r.json()
-            emailList += data["value"]
-            if not "@odata.nextLink" in data: break
-
-        return [OMail(x,self.exgAuth) for x in emailList]
-
-    def __repr__(self):
-        return f"<OFolder {self.displayName}>"
-
-class OMail:
-    exgAuth = None
-
-    def __init__(self,jsonObj:dict,cnt:ExchangeAuth):
-        self.create(jsonObj)
-        self.exgAuth = cnt
-
-    def create(self,jsonObj):
-        jsonObj["_from"] = jsonObj["from"]
-        exgAuth = self.exgAuth
-        self.__dict__ = jsonObj
-        self.exgAuth = exgAuth
-
-    def set_read(self,isRead:bool):
-        endpoint = f"{self.exgAuth.config.base_url}/messages/{self.id}"
-        body = {"isRead": isRead}
-        r = requests.patch(url=endpoint, headers=self.exgAuth.headers, json=body)
-        if r.status_code != 200:
-            raise Exception("Error:" + r.text)
-        self.create(r.json())
-        
-
-
-    def __repr__(self):
-        return f"<Omail {self._from['emailAddress']['name']}>"
-
-class OMessage:
-    subject = None
-    body = None
-    def __init__(self,cnt:ExchangeAuth):
-        self.exgAuth = cnt
-    
-    def set_subject(self,subject):
-        self.subject = subject
-    
-    def set_body(self,contentType,content):
-        self.body = {
-            "contentType": contentType,
-            "content"    : content
-        }
-    
-    def set_toRecipients(self,address:list):
-        self.toRecipients = [
-            {"emailAddress":{"address":x}} for x in address
-        ]
-    
-    def set_attachments(self,attachments:list):
-        atts = []
-        for att in attachments:
-            fl_binary = open(att,"rb").read()
-            encoded_file = base64.b64encode(fl_binary)
-            data = {
-                    "@odata.type": "#microsoft.graph.fileAttachment",
-                    "name": os.path.basename(att),
-                    #"contentType": "reference",
-                    "contentBytes": encoded_file.decode("utf-8")
-                }
-            atts.append(data)
-        self.attachments = atts
-    
-    def send(self):
-        payload = {
-            "message":{
-                "subject"     : self.subject,
-                "body"        : self.body,
-                "toRecipients": self.toRecipients,
-                "attachments" : self.attachments
-            }
-
-        }
-        endpoint = f"{self.exgAuth.config.base_url}/sendMail"
-        r = requests.post(url=endpoint, headers=self.exgAuth.headers, json=payload)
-        if r.status_code not in [200,202]:
-            raise Exception("Error:" + r.text)
-            
-        return True
-
-class ExchangeGraph:
-
-    def __init__(self,username,password,client_id,client_secret,tenant_id,user_id):
-        config = OauthParams(
-            username      = username,     
-            password      = password,     
-            client_id     = client_id,    
-            client_secret = client_secret,
-            tenant_id     = tenant_id,    
-            user_id       = user_id    
-        )
-        
-        self.exgAuth = ExchangeAuth(config=config)
-    
-    def get_folders(self):
-        endpoint = f"{self.exgAuth.config.base_url}/mailFolders"
-        r = requests.get(url=endpoint, headers=self.exgAuth.headers)
-        if r.status_code != 200:
-            raise Exception("Error:" + r.text)
-
-        return [OFolder(x,self.exgAuth) for x in r.json()["value"]]
-    
-    def get_folder_by_path(self,path,current_folder=None):
-        dirs = os.path.normpath(path).split(os.sep)
-        if not dirs: raise Exception("Please insert a valid path")
-
-        fdr = None
-        if not current_folder:
-            main_folders = self.get_folders()
-            fdr = [x for x in main_folders if x.displayName == dirs[0]]
-        else:
-            chlds = current_folder.childFolders()
-            fdr = [x for x in chlds if x.displayName == dirs[0]]
-        
-        if len(dirs) == 1: return fdr[0]
-        return self.get_folder_by_path("/".join(dirs[1:]),fdr[0])
-
-    def newMessage(self):
-        return OMessage(self.exgAuth)
-        
-
-# import glob
-
-# if __name__ == "__main__":
-
-#     username      = "rpa.cotacaoautomatica@primecontrol.com.br",
-#     password      = "Cpfl@2022*",
-#     client_id     = "ef15e8b4-6087-491c-a939-97e985f36ddf",
-#     client_secret = "~m08Q~y5QAd6M3fD~SZRoalE2WCrAplofO9Kncox",
-#     tenant_id     = "3c924ffe-f013-49fb-ab9c-abc7152969ad",
-#     user_id       = "8d9a5d16-12ca-40a7-96f0-82266fde95d0"
-
-#     exchange_client = ExchangeGraph(username=username,password=password,client_id=client_id,client_secret=client_secret,tenant_id=tenant_id,user_id=user_id)
-
-#     #ENVIANDO EMAIL
-#     msg = exchange_client.newMessage()
-#     msg.set_subject("test Subject")
-#     msg.set_body("Text","Esse e um email de teste!")
-#     msg.set_toRecipients(["melque_ex@yahoo.com.br"])
-#     msg.set_attachments(glob.glob(r"C:\Users\melque\Documents\test\*.*"))
-#     msg.send()
- 
-#     #RETORNANDO PASTAS
-#     folders = exchange_client.get_folders()
-
-#     #RETORNANDO PASTA ESPECIFICA
-#     subf = exchange_client.get_folder_by_path("Teste/subfolder1")
-
-#     #LENDO EMAILS DE UMA PASTA
-#     mails = subf.get_mails()
-
-#     #LENDO EMAILS NAO LIDOS
-#     mails = subf.get_mails(filter="isRead eq true") #PODE ADCIONAR O PARAMETRO -> top=1 PRA TRAZER SO 1 ITEM
-
-#     # MARCANDO O EMAIL COMO LIDO
-#     mails[0].set_read(False)
-
-#     # MARCANDO O EMAIL COMO NAO LIDO
-#     mails[0].set_read(True)
-
-
+from ast import Raise
+import base64
+from dataclasses import Field, dataclass, field
+from email.policy import default
+from functools import wraps
+import msal
+import requests
+import json
+from dateUts import *
+import os
+
+
+@dataclass
+class OauthParams:
+    username     : str
+    password     : str
+    client_id    : str
+    client_secret: str
+    tenant_id    : str
+    user_id      : str
+    base_url     : str = field(default='')
+    authority    : str = field(default='')
+
+class ExchangeAuth:
+    last_token_key_at = None
+    token_code        = None
+    exp_secs          = None
+
+    def __init__(self, config: OauthParams):
+    
+        self.config = config
+        self.config.authority = f"https://login.microsoftonline.com/{self.config.tenant_id}"
+        self.config.base_url = f"https://graph.microsoft.com/v1.0/users/{self.config.user_id}"
+        self.app = msal.ConfidentialClientApplication(
+            client_id=config.client_id,
+            client_credential=config.client_secret,
+            authority=config.authority)
+
+    def update_token(self):
+        # TODO Avaliar se pode vir como parametro
+        scopes = ["https://graph.microsoft.com/.default"]
+        result = None
+        result = self.app.acquire_token_by_username_password(
+            username=self.config.username,
+            password=self.config.password,
+            scopes=scopes
+        )
+        if not result:
+            print(
+                "Não existe um token em cache. Criando um novo do Azure Active Directory.")
+        result = self.app.acquire_token_for_client(scopes=scopes)
+        if "access_token" in result:
+            print(result)
+            #print("Access token - " + result["access_token"])
+            self.token_code = result["access_token"]
+            self.last_token_key_at = today()
+            self.exp_secs = result["expires_in"]
+            return (True, '')
+        else:
+            return (False, result)
+
+    def validate_token(self):
+        expired = False
+        if self.last_token_key_at:
+            expired = today() >= dateAdd(self.last_token_key_at, self.exp_secs-10*60, 'seconds')
+
+        if not self.last_token_key_at or expired:
+            resp = self.update_token()
+            if not resp[0]:
+                raise Exception(f"Error generating new Token:{resp[1]}")
+            else:
+                print("New token generated!")
+
+    @property
+    def headers(self):
+        self.validate_token()
+        return {"Authorization": f"Bearer {self.token_code}"}
+
+    @property
+    def token(self):
+        self.validate_token()
+        self.token_code
+
+class OFolder:
+    def __init__(self,jsonObj:dict,cnt:ExchangeAuth):
+        self.__dict__ = jsonObj
+        self.exgAuth = cnt
+
+    def childFolders(self):
+        
+        endpoint = f"{self.exgAuth.config.base_url}/mailFolders/{self.id}/childFolders"
+        r = requests.get(url=endpoint, headers=self.exgAuth.headers)
+        if r.status_code != 200: raise Exception("Error:" + r.text)
+        fdrs = [OFolder(x,self.exgAuth) for x in r.json()["value"]]
+        return fdrs
+
+    def get_mails(self,**kargs):
+        params = "&".join([f"{k}={v}" for k,v in kargs.items() if v is not None])
+        endpoint = f"{self.exgAuth.config.base_url}/mailFolders/{self.id}/messages?{params}"
+        emailList = []
+        data = None
+
+        while True:
+            url = endpoint if not data else data["@odata.nextLink"]
+            r = requests.get(url, headers=self.exgAuth.headers)
+            if r.status_code != 200:
+                raise Exception("Error:" + r.text)
+            data = r.json()
+            emailList += data["value"]
+            if not "@odata.nextLink" in data: break
+
+        return [OMail(x,self.exgAuth) for x in emailList]
+
+    def __repr__(self):
+        return f"<OFolder {self.displayName}>"
+
+class OMail:
+    exgAuth = None
+
+    def __init__(self,jsonObj:dict,cnt:ExchangeAuth):
+        self.create(jsonObj)
+        self.exgAuth = cnt
+
+    def create(self,jsonObj):
+        jsonObj["_from"] = jsonObj["from"]
+        exgAuth = self.exgAuth
+        self.__dict__ = jsonObj
+        self.exgAuth = exgAuth
+
+    def set_read(self,isRead:bool):
+        endpoint = f"{self.exgAuth.config.base_url}/messages/{self.id}"
+        body = {"isRead": isRead}
+        r = requests.patch(url=endpoint, headers=self.exgAuth.headers, json=body)
+        if r.status_code != 200:
+            raise Exception("Error:" + r.text)
+        self.create(r.json())
+        
+
+
+    def __repr__(self):
+        return f"<Omail {self._from['emailAddress']['name']}>"
+
+class OMessage:
+    subject = None
+    body = None
+    def __init__(self,cnt:ExchangeAuth):
+        self.exgAuth = cnt
+    
+    def set_subject(self,subject):
+        self.subject = subject
+    
+    def set_body(self,contentType,content):
+        self.body = {
+            "contentType": contentType,
+            "content"    : content
+        }
+    
+    def set_toRecipients(self,address:list):
+        self.toRecipients = [
+            {"emailAddress":{"address":x}} for x in address
+        ]
+    
+    def set_attachments(self,attachments:list):
+        atts = []
+        for att in attachments:
+            fl_binary = open(att,"rb").read()
+            encoded_file = base64.b64encode(fl_binary)
+            data = {
+                    "@odata.type": "#microsoft.graph.fileAttachment",
+                    "name": os.path.basename(att),
+                    #"contentType": "reference",
+                    "contentBytes": encoded_file.decode("utf-8")
+                }
+            atts.append(data)
+        self.attachments = atts
+    
+    def send(self):
+        payload = {
+            "message":{
+                "subject"     : self.subject,
+                "body"        : self.body,
+                "toRecipients": self.toRecipients,
+                "attachments" : self.attachments
+            }
+
+        }
+        endpoint = f"{self.exgAuth.config.base_url}/sendMail"
+        r = requests.post(url=endpoint, headers=self.exgAuth.headers, json=payload)
+        if r.status_code not in [200,202]:
+            raise Exception("Error:" + r.text)
+            
+        return True
+
+class ExchangeGraph:
+
+    def __init__(self,username,password,client_id,client_secret,tenant_id,user_id):
+        config = OauthParams(
+            username      = username,     
+            password      = password,     
+            client_id     = client_id,    
+            client_secret = client_secret,
+            tenant_id     = tenant_id,    
+            user_id       = user_id    
+        )
+        
+        self.exgAuth = ExchangeAuth(config=config)
+    
+    def get_folders(self):
+        endpoint = f"{self.exgAuth.config.base_url}/mailFolders"
+        r = requests.get(url=endpoint, headers=self.exgAuth.headers)
+        if r.status_code != 200:
+            raise Exception("Error:" + r.text)
+
+        return [OFolder(x,self.exgAuth) for x in r.json()["value"]]
+    
+    def get_folder_by_path(self,path,current_folder=None):
+        dirs = os.path.normpath(path).split(os.sep)
+        if not dirs: raise Exception("Please insert a valid path")
+
+        fdr = None
+        if not current_folder:
+            main_folders = self.get_folders()
+            fdr = [x for x in main_folders if x.displayName == dirs[0]]
+        else:
+            chlds = current_folder.childFolders()
+            fdr = [x for x in chlds if x.displayName == dirs[0]]
+        
+        if len(dirs) == 1: return fdr[0]
+        return self.get_folder_by_path("/".join(dirs[1:]),fdr[0])
+
+    def newMessage(self):
+        return OMessage(self.exgAuth)
+        
+
+# import glob
+
+# if __name__ == "__main__":
+
+#     username      = "rpa.cotacaoautomatica@primecontrol.com.br",
+#     password      = "Cpfl@2022*",
+#     client_id     = "ef15e8b4-6087-491c-a939-97e985f36ddf",
+#     client_secret = "~m08Q~y5QAd6M3fD~SZRoalE2WCrAplofO9Kncox",
+#     tenant_id     = "3c924ffe-f013-49fb-ab9c-abc7152969ad",
+#     user_id       = "8d9a5d16-12ca-40a7-96f0-82266fde95d0"
+
+#     exchange_client = ExchangeGraph(username=username,password=password,client_id=client_id,client_secret=client_secret,tenant_id=tenant_id,user_id=user_id)
+
+#     #ENVIANDO EMAIL
+#     msg = exchange_client.newMessage()
+#     msg.set_subject("test Subject")
+#     msg.set_body("Text","Esse e um email de teste!")
+#     msg.set_toRecipients(["melque_ex@yahoo.com.br"])
+#     msg.set_attachments(glob.glob(r"C:\Users\melque\Documents\test\*.*"))
+#     msg.send()
+ 
+#     #RETORNANDO PASTAS
+#     folders = exchange_client.get_folders()
+
+#     #RETORNANDO PASTA ESPECIFICA
+#     subf = exchange_client.get_folder_by_path("Teste/subfolder1")
+
+#     #LENDO EMAILS DE UMA PASTA
+#     mails = subf.get_mails()
+
+#     #LENDO EMAILS NAO LIDOS
+#     mails = subf.get_mails(filter="isRead eq true") #PODE ADCIONAR O PARAMETRO -> top=1 PRA TRAZER SO 1 ITEM
+
+#     # MARCANDO O EMAIL COMO LIDO
+#     mails[0].set_read(False)
+
+#     # MARCANDO O EMAIL COMO NAO LIDO
+#     mails[0].set_read(True)
+
+
```

### Comparing `PrimeBotFramework-0.0.9/PrimeBot/Vault/__init__.py` & `PrimeBotFramework-1.0.12/PrimeBot/Vault/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from requests.exceptions import ConnectionError
-from hvac.exceptions import InvalidPath
-from dataclasses import dataclass
-import traceback
-import hvac
-import os
-
-""" 
-    ============== DESCRICAO GERAL ============
-        Classe para conectar o Vault e obter os dados
-        para execução do robô
-
-    ================= CLIENT =================
-        Obtem o cliente conectado no Vault
-
-        OUTPUT:
-            type:<TODO>
-            Obs:Retorna os vault object
-
-    ============= GET_CREDENTIALS ============
-        Obtem as credenciais do Vault
-
-        INPUT:
-            - secrets_path: str =  Especifica os dados do vault que serão utilizados
-        OUTPUT:
-            type:<Dict>
-            Obs:Retorna os dados da secrets
-        RAISES:
-            - Exception : Path ou chave inválida        
-"""
-
-@dataclass
-class Messages:
-    conError :str = """
-                        Verifique se o Vault está em execução e se as variáveis de
-                        ambiente, descritas na documentação dessa
-                        Lib, estão configuradas
-                    """
-    authError :str = "Verifique o token configurado na variável de ambiente"
-
-
-class Vault:
-    
-    def __init__(self,token):
-        self.client = self.__client(token)
-
-    def __client(self,token):
-        try:
-            client = hvac.Client(token=token)
-            
-            if not client.is_authenticated():
-                raise Exception(Messages.authError)
-
-            return client
-        except ConnectionError:
-            raise Exception(f'{traceback.format_exc()} \n\n{Messages.conError}')
-
-    def get_credentials(self,path, mount_point=None):
-        secret = os.path.basename(os.path.normpath(path))
-        val = self.verify_secret(mount_point=mount_point,secret=secret)
-        if not val:
-            raise Exception("Secret '{secret}' not found!")
-
-        try:
-            hvreponse = self.client.secrets.kv.v2.read_secret_version(mount_point=mount_point,path=path)
-            return hvreponse['data']['data']
-        except InvalidPath:
-            raise Exception(f'{traceback.format_exc()}')
-        except KeyError:
-            raise Exception(f'{traceback.format_exc()}')
-    def verify_secret(self,mount_point,secret,path=""):
-        try:
-            hvreponse = self.client.secrets.kv.v2.list_secrets(mount_point=mount_point,path=path)
-            keys = hvreponse['data']["keys"]
-            return secret in keys
-        except InvalidPath:
-            raise Exception(f'{traceback.format_exc()}')
-        except KeyError:
-            raise Exception(f'{traceback.format_exc()}')
-
-
-# token = "s.WrhdYlmstBXsdNIL2ztsccPF"
-# a = VaultClient(token)
-# cred = a.get_credentials("juju","kv")
-# a=1
-
-
-
+from requests.exceptions import ConnectionError
+from hvac.exceptions import InvalidPath
+from dataclasses import dataclass
+import traceback
+import hvac
+import os
+
+""" 
+    ============== DESCRICAO GERAL ============
+        Classe para conectar o Vault e obter os dados
+        para execução do robô
+
+    ================= CLIENT =================
+        Obtem o cliente conectado no Vault
+
+        OUTPUT:
+            type:<TODO>
+            Obs:Retorna os vault object
+
+    ============= GET_CREDENTIALS ============
+        Obtem as credenciais do Vault
+
+        INPUT:
+            - secrets_path: str =  Especifica os dados do vault que serão utilizados
+        OUTPUT:
+            type:<Dict>
+            Obs:Retorna os dados da secrets
+        RAISES:
+            - Exception : Path ou chave inválida        
+"""
+
+@dataclass
+class Messages:
+    conError :str = """
+                        Verifique se o Vault está em execução e se as variáveis de
+                        ambiente, descritas na documentação dessa
+                        Lib, estão configuradas
+                    """
+    authError :str = "Verifique o token configurado na variável de ambiente"
+
+
+class Vault:
+    
+    def __init__(self,token):
+        self.client = self.__client(token)
+
+    def __client(self,token):
+        try:
+            client = hvac.Client(token=token)
+            
+            if not client.is_authenticated():
+                raise Exception(Messages.authError)
+
+            return client
+        except ConnectionError:
+            raise Exception(f'{traceback.format_exc()} \n\n{Messages.conError}')
+
+    def get_credentials(self,path, mount_point=None):
+        secret = os.path.basename(os.path.normpath(path))
+        val = self.verify_secret(mount_point=mount_point,secret=secret)
+        if not val:
+            raise Exception("Secret '{secret}' not found!")
+
+        try:
+            hvreponse = self.client.secrets.kv.v2.read_secret_version(mount_point=mount_point,path=path)
+            return hvreponse['data']['data']
+        except InvalidPath:
+            raise Exception(f'{traceback.format_exc()}')
+        except KeyError:
+            raise Exception(f'{traceback.format_exc()}')
+    def verify_secret(self,mount_point,secret,path=""):
+        try:
+            hvreponse = self.client.secrets.kv.v2.list_secrets(mount_point=mount_point,path=path)
+            keys = hvreponse['data']["keys"]
+            return secret in keys
+        except InvalidPath:
+            raise Exception(f'{traceback.format_exc()}')
+        except KeyError:
+            raise Exception(f'{traceback.format_exc()}')
+
+
+# token = "s.WrhdYlmstBXsdNIL2ztsccPF"
+# a = VaultClient(token)
+# cred = a.get_credentials("juju","kv")
+# a=1
+
+
+
```

### Comparing `PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/SOURCES.txt` & `PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,33 @@
+.gitignore
+.pypirc
 CHANGELOG.txt
 MANIFEST.in
+PKG-INFO
+Pipfile
+Pipfile.lock
 README.md
+bitbucket-pipelines.yml
 requirements.txt
+setup.cfg
 setup.py
+.vscode/settings.json
 PrimeBot/__init__.py
-PrimeBotFramework.egg-info/PKG-INFO
-PrimeBotFramework.egg-info/SOURCES.txt
-PrimeBotFramework.egg-info/dependency_links.txt
-PrimeBotFramework.egg-info/requires.txt
-PrimeBotFramework.egg-info/top_level.txt
+PrimeBot/B2E/__init__.py
 PrimeBot/CpfCnpj/__init__.py
 PrimeBot/CpfCnpj/api_codes.py
 PrimeBot/CpfCnpj/model.py
+PrimeBot/D4Sign/__init__.py
 PrimeBot/DeathByCaptcha/__init__.py
 PrimeBot/Documents/__init__.py
 PrimeBot/Elastic/__init__.py
 PrimeBot/ExchangeGraph/__init__.py
+PrimeBot/IntegracaoSendGrid/__init__.py
+PrimeBot/ListenerECS/__init__.py
 PrimeBot/Mongo/__init__.py
-PrimeBot/Vault/__init__.py
+PrimeBot/OracleDB/__init__.py
+PrimeBot/Vault/__init__.py
+PrimeBotFramework.egg-info/PKG-INFO
+PrimeBotFramework.egg-info/SOURCES.txt
+PrimeBotFramework.egg-info/dependency_links.txt
+PrimeBotFramework.egg-info/requires.txt
+PrimeBotFramework.egg-info/top_level.txt
```

### Comparing `PrimeBotFramework-0.0.9/setup.py` & `PrimeBotFramework-1.0.12/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from setuptools import setup, find_packages, Extension
- 
-classifiers = [
-  'Development Status :: 5 - Production/Stable',
-  'Intended Audience :: Education',
-  'Operating System :: Microsoft :: Windows :: Windows 10',
-  'License :: OSI Approved :: MIT License',
-  'Programming Language :: Python :: 3'
-]
-
-setup(
-  name='PrimeBotFramework',
-  version='0.0.9',
-  description='Um pacote de padronizacao de pacotes a serem utilizados pela Prime',
-  long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
-  long_description_content_type='text/markdown',
-  url='',  
-  author='Melque Lima',
-  author_email='',
-  license='MIT', 
-  classifiers=classifiers,
-  keywords='PrimeBotFramework', 
-  packages=find_packages(),
-  install_requires=['hvac==1.0.2','mongoengine==0.22.1','elasticsearch-dsl==7.3.0','dateUts==0.1.0', 'datetime',
-'requests>=2.28.1', 'pyaml>=21.10.1', 'pydantic>=1.10.2'],
-  python_requires='~=3.8'
-)
-
-
-
+from setuptools import setup, find_packages, Extension
+ 
+classifiers = [
+  'Development Status :: 5 - Production/Stable',
+  'Intended Audience :: Education',
+  'Operating System :: Microsoft :: Windows :: Windows 10',
+  'License :: OSI Approved :: MIT License',
+  'Programming Language :: Python :: 3'
+]
+
+setup(
+  name='PrimeBotFramework',
+  use_scm_version=True,
+  description='Um pacote de padronizacao de pacotes a serem utilizados pela Prime',
+  long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
+  long_description_content_type='text/markdown',
+  url='',  
+  author='Prime Control',
+  author_email='',
+  license='MIT', 
+  classifiers=classifiers,
+  keywords='PrimeBotFramework', 
+  packages=find_packages(),
+  setup_requires=['setuptools_scm'],
+  install_requires=['hvac==1.0.2','mongoengine==0.22.1','elasticsearch-dsl==7.3.0','dateUts==0.1.0', 'ecs-logging', 'datetime',
+'requests>=2.28.1', 'pyaml>=21.10.1', 'pydantic>=1.10.2', 'cx-Oracle==8.3.0', 'sendgrid==6.10.0', 'certifi==2022.12.7'],
+  python_requires='~=3.8'
+)
+
+
+
```

