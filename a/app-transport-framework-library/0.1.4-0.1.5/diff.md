# Comparing `tmp/app_transport_framework_library-0.1.4.tar.gz` & `tmp/app_transport_framework_library-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_transport_framework_library-0.1.4.tar", max compression
+gzip compressed data, was "app_transport_framework_library-0.1.5.tar", max compression
```

## Comparing `app_transport_framework_library-0.1.4.tar` & `app_transport_framework_library-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3846 2023-05-16 22:12:18.801764 app_transport_framework_library-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-16 20:50:56.861597 app_transport_framework_library-0.1.4/app_transport_framework_library/__init__.py
--rw-r--r--   0        0        0     6549 2023-05-22 21:59:08.700521 app_transport_framework_library-0.1.4/app_transport_framework_library/atf_bundle_processor.py
--rw-r--r--   0        0        0      824 2023-05-16 21:36:51.746182 app_transport_framework_library-0.1.4/app_transport_framework_library/base_use_case_handler.py
--rw-r--r--   0        0        0      279 2023-05-16 21:02:55.215837 app_transport_framework_library-0.1.4/app_transport_framework_library/models/bundle_focus_content.py
--rw-r--r--   0        0        0      393 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.4/app_transport_framework_library/models/empfangsbestaetigung.py
--rw-r--r--   0        0        0      350 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.4/app_transport_framework_library/models/event.py
--rw-r--r--   0        0        0      295 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.4/app_transport_framework_library/models/message_to_send.py
--rw-r--r--   0        0        0     1138 2023-05-16 21:02:46.011962 app_transport_framework_library-0.1.4/app_transport_framework_library/ressource_creators/message_bundle_creator.py
--rw-r--r--   0        0        0     1197 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.4/app_transport_framework_library/ressource_creators/message_header_creator.py
--rw-r--r--   0        0        0     1780 2023-05-16 21:03:31.391345 app_transport_framework_library-0.1.4/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py
--rw-r--r--   0        0        0      838 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.4/app_transport_framework_library/ressource_creators/operation_outcome_creator.py
--rw-r--r--   0        0        0     3902 2023-05-22 21:58:54.574818 app_transport_framework_library-0.1.4/app_transport_framework_library/ressource_creators/test_message_creator.py
--rw-r--r--   0        0        0     1613 2023-05-16 21:38:28.224802 app_transport_framework_library-0.1.4/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py
--rw-r--r--   0        0        0     1931 2023-05-16 21:39:27.990263 app_transport_framework_library-0.1.4/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py
--rw-r--r--   0        0        0      375 2023-05-22 22:00:27.020144 app_transport_framework_library-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 app_transport_framework_library-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-22 22:04:58.127954 app_transport_framework_library-0.1.5/app_transport_framework_library/__init__.py
+-rw-r--r--   0        0        0     6427 2023-05-23 19:52:56.836795 app_transport_framework_library-0.1.5/app_transport_framework_library/atf_bundle_processor.py
+-rw-r--r--   0        0        0      848 2023-05-22 22:04:58.129954 app_transport_framework_library-0.1.5/app_transport_framework_library/base_use_case_handler.py
+-rw-r--r--   0        0        0      287 2023-05-22 22:04:58.131960 app_transport_framework_library-0.1.5/app_transport_framework_library/models/bundle_focus_content.py
+-rw-r--r--   0        0        0      452 2023-05-23 19:53:32.165799 app_transport_framework_library-0.1.5/app_transport_framework_library/models/empfangsbestaetigung.py
+-rw-r--r--   0        0        0      363 2023-05-22 22:04:58.132952 app_transport_framework_library-0.1.5/app_transport_framework_library/models/event.py
+-rw-r--r--   0        0        0      261 2023-05-23 18:58:39.501228 app_transport_framework_library-0.1.5/app_transport_framework_library/models/message_to_send.py
+-rw-r--r--   0        0        0     1172 2023-05-22 22:04:58.137428 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/message_bundle_creator.py
+-rw-r--r--   0        0        0     1232 2023-05-22 22:04:58.138443 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/message_header_creator.py
+-rw-r--r--   0        0        0     1757 2023-05-23 19:52:55.631553 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py
+-rw-r--r--   0        0        0      859 2023-05-22 22:04:58.140443 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/operation_outcome_creator.py
+-rw-r--r--   0        0        0     3930 2023-05-23 19:52:55.631553 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/test_message_creator.py
+-rw-r--r--   0        0        0     1706 2023-05-23 19:06:28.832327 app_transport_framework_library-0.1.5/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py
+-rw-r--r--   0        0        0     1977 2023-05-22 22:04:58.143445 app_transport_framework_library-0.1.5/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py
+-rw-r--r--   0        0        0      390 2023-05-23 19:58:06.639312 app_transport_framework_library-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3943 2023-05-22 22:04:58.126959 app_transport_framework_library-0.1.5/README.md
+-rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 app_transport_framework_library-0.1.5/PKG-INFO
```

### Comparing `app_transport_framework_library-0.1.4/README.md` & `app_transport_framework_library-0.1.5/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-# ATF Library
-
-Die App-Transport-Framework (ATF) Library ist eine Python-Bibliothek zur Verarbeitung und Handhabung von ATF-Nachrichten (<https://simplifier.net/app-transport-framework>) im FHIR-Format. Die Bibliothek bietet eine einfache Möglichkeit, verschiedene Anwendungsfälle und ihre zugehörigen Handler zu registrieren und zu verwalten.
-
-## Installation
-
-Installieren Sie diese Bibliothek mit dem folgenden Befehl:
-
-```
-pip install app-transport-framework-library
-```
-
-## Verwendung
-
-1. Importieren Sie die benötigten Klassen und Funktionen aus der Bibliothek:
-
-```python
-from app_transport_framework_library.atf_bundle_processor import ATF_BundleProcessor
-```
-
-2. Erstellen Sie eine Instanz des ATF_BundleProcessor und registrieren Sie die Handler für die Anwendungsfälle, die Sie erweitern möchten:
-
-```python
-atf_processor = ATF_BundleProcessor(sender, source)
-
-atf_processor.register_use_case_handler(
-    "https://gematik.de/fhir/atf/CodeSystem/operation-identifier-cs",
-    "eRezept_Rezeptanforderung;Rezeptanfrage",
-    eRezept_Rezeptanforderung_RezeptanfrageHandler()
-)
-
-atf_processor.register_use_case_handler(
-    "https://gematik.de/fhir/atf/CodeSystem/service-identifier-cs",
-    "eRezept_Rezeptanforderung;Rezeptanfrage_Storno",
-    eRezept_Rezeptanforderung_Rezeptanfrage_StornoHandler()
-)
-
-```
-
-3. Events
-
-Abonnieren Sie das 'message_to_send_event', um die generierten ausgehenden Eingangsbestätigungen zu erhalten und weiterzuleiten:
-
-```python
-from app_transport_framework_library.models.message_to_send import MessageToSend
-
-def on_message_to_send_triggered(message_to_send: MessageToSend):
-    # Senden der Empfangsbestätigung an den ursprünglichen Absender
-    pass
-
-
-atf_processor.message_to_send_event.subscribe(on_message_to_send_triggered)
-
-```
-
-Abonnieren Sie das 'received_Empfangsbestaetigung_event', um die eingehenden Eingangsbestätigungen des belieferten Adressaten zu erhalten und die Message-ID der gesendeten Nachricht auszuwerten:
-
-```python
-from app_transport_framework_library.models.empfangsbestaetigung import Empfangsbestaetigung
-
-def on_received_Empfangsbestaetigung(empfangsbestaetigung: Empfangsbestaetigung):
-    print(f"'{receiver_address}' hat Empfangsbestätigung für '{empfangsbestaetigung.message_id}' von '{empfangsbestaetigung.sender}' erhalten")
-
-atf_processor.received_Empfangsbestaetigung_event.subscribe(on_received_Empfangsbestaetigung)
-```
-
-Abonnieren Sie das 'focus_Ressource_to_process_event', um die inhaltlichen Ressourcen des Anwendungsfalls zu erhalten und auswerten zu können:
-
-```python
-from app_transport_framework_library.models.bundle_focus_content import BundleFocusContent
-from fhir.resources.communication import Communication
-
-def on_focus_Ressource_to_process(bundle_content: BundleFocusContent):
-    from app_transport_framework_library.models.bundle_focus_content import BundleFocusContent
-from fhir.resources.communication import Communication
-
-def on_focus_Ressource_to_process(bundle_content: BundleFocusContent):
-    print(f"Verarbeitung des Bundles mit Fokus auf '{bundle_content.code}'")
-    if bundle_content.code == "Selbsttest;Lieferung":
-        com_parsed = Communication.parse_raw(bundle_content.bundle_entries[0].json())
-        decoded_message = base64.b64decode(com_parsed.payload[0].contentAttachment.data)
-
-        print(f"Das Bundle enthält {len(bundle_content.bundle_entries)} Einträge")
-        print(f"Die Kommunikation enthält die Payload '{decoded_message.decode('utf-8')}'")
-
-atf_processor.focus_Ressource_to_process_event.subscribe(on_focus_Ressource_to_process)
-
-```
-
-## Beispielimplementierung
-
-Eine Beispielimplementierung kann hier eingesehen werden:
-<https://github.com/gematik/api-app-transport-framework/tree/main/src/poc>
-
-## Lizenz
-
-Dieses Projekt steht unter der MIT-Lizenz - siehe die LICENSE-Datei für Details.
+# ATF Library
+
+Die App-Transport-Framework (ATF) Library ist eine Python-Bibliothek zur Verarbeitung und Handhabung von ATF-Nachrichten (<https://simplifier.net/app-transport-framework>) im FHIR-Format. Die Bibliothek bietet eine einfache Möglichkeit, verschiedene Anwendungsfälle und ihre zugehörigen Handler zu registrieren und zu verwalten.
+
+## Installation
+
+Installieren Sie diese Bibliothek mit dem folgenden Befehl:
+
+```
+pip install app-transport-framework-library
+```
+
+## Verwendung
+
+1. Importieren Sie die benötigten Klassen und Funktionen aus der Bibliothek:
+
+```python
+from app_transport_framework_library.atf_bundle_processor import ATF_BundleProcessor
+```
+
+2. Erstellen Sie eine Instanz des ATF_BundleProcessor und registrieren Sie die Handler für die Anwendungsfälle, die Sie erweitern möchten:
+
+```python
+atf_processor = ATF_BundleProcessor(sender, source)
+
+atf_processor.register_use_case_handler(
+    "https://gematik.de/fhir/atf/CodeSystem/operation-identifier-cs",
+    "eRezept_Rezeptanforderung;Rezeptanfrage",
+    eRezept_Rezeptanforderung_RezeptanfrageHandler()
+)
+
+atf_processor.register_use_case_handler(
+    "https://gematik.de/fhir/atf/CodeSystem/service-identifier-cs",
+    "eRezept_Rezeptanforderung;Rezeptanfrage_Storno",
+    eRezept_Rezeptanforderung_Rezeptanfrage_StornoHandler()
+)
+
+```
+
+3. Events
+
+Abonnieren Sie das 'message_to_send_event', um die generierten ausgehenden Eingangsbestätigungen zu erhalten und weiterzuleiten:
+
+```python
+from app_transport_framework_library.models.message_to_send import MessageToSend
+
+def on_message_to_send_triggered(message_to_send: MessageToSend):
+    # Senden der Empfangsbestätigung an den ursprünglichen Absender
+    pass
+
+
+atf_processor.message_to_send_event.subscribe(on_message_to_send_triggered)
+
+```
+
+Abonnieren Sie das 'received_Empfangsbestaetigung_event', um die eingehenden Eingangsbestätigungen des belieferten Adressaten zu erhalten und die Message-ID der gesendeten Nachricht auszuwerten:
+
+```python
+from app_transport_framework_library.models.empfangsbestaetigung import Empfangsbestaetigung
+
+def on_received_Empfangsbestaetigung(empfangsbestaetigung: Empfangsbestaetigung):
+    print(f"'{receiver_address}' hat Empfangsbestätigung für '{empfangsbestaetigung.message_id}' von '{empfangsbestaetigung.sender}' erhalten")
+
+atf_processor.received_Empfangsbestaetigung_event.subscribe(on_received_Empfangsbestaetigung)
+```
+
+Abonnieren Sie das 'focus_Ressource_to_process_event', um die inhaltlichen Ressourcen des Anwendungsfalls zu erhalten und auswerten zu können:
+
+```python
+from app_transport_framework_library.models.bundle_focus_content import BundleFocusContent
+from fhir.resources.communication import Communication
+
+def on_focus_Ressource_to_process(bundle_content: BundleFocusContent):
+    from app_transport_framework_library.models.bundle_focus_content import BundleFocusContent
+from fhir.resources.communication import Communication
+
+def on_focus_Ressource_to_process(bundle_content: BundleFocusContent):
+    print(f"Verarbeitung des Bundles mit Fokus auf '{bundle_content.code}'")
+    if bundle_content.code == "Selbsttest;Lieferung":
+        com_parsed = Communication.parse_raw(bundle_content.bundle_entries[0].json())
+        decoded_message = base64.b64decode(com_parsed.payload[0].contentAttachment.data)
+
+        print(f"Das Bundle enthält {len(bundle_content.bundle_entries)} Einträge")
+        print(f"Die Kommunikation enthält die Payload '{decoded_message.decode('utf-8')}'")
+
+atf_processor.focus_Ressource_to_process_event.subscribe(on_focus_Ressource_to_process)
+
+```
+
+## Beispielimplementierung
+
+Eine Beispielimplementierung kann hier eingesehen werden:
+<https://github.com/gematik/api-app-transport-framework/tree/main/src/poc>
+
+## Lizenz
+
+Dieses Projekt steht unter der MIT-Lizenz - siehe die LICENSE-Datei für Details.
```

### Comparing `app_transport_framework_library-0.1.4/app_transport_framework_library/atf_bundle_processor.py` & `app_transport_framework_library-0.1.5/app_transport_framework_library/atf_bundle_processor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-import logging
-from json import JSONDecodeError
-from fhir.resources.bundle import Bundle
-from fhir.resources.messageheader import MessageHeader, MessageHeaderSource, MessageHeaderDestination
-from fhir.resources.operationoutcome import OperationOutcomeIssue
-from fhir.resources.fhirtypes import ReferenceType
-from app_transport_framework_library.app_transport_framework_library.base_use_case_handler import BaseUseCaseHandler
-from app_transport_framework_library.app_transport_framework_library.models.bundle_focus_content import BundleFocusContent
-from app_transport_framework_library.app_transport_framework_library.models.event import Event
-from app_transport_framework_library.app_transport_framework_library.models.message_to_send import MessageToSend
-from app_transport_framework_library.app_transport_framework_library.ressource_creators.operation_outcome_bundle_creator import OperationOutcomeBundleCreator
-from app_transport_framework_library.app_transport_framework_library.ressource_creators.operation_outcome_creator import OperationOutcomeCreator
-from app_transport_framework_library.app_transport_framework_library.use_cases.empfangsbestaetigung_handler import EmpfangsbestaetigungHandler
-from app_transport_framework_library.app_transport_framework_library.use_cases.selbsttest_lieferung_handler import SelbsttestLieferungHandler
-
-
-
-
-
-
-# Configure logging
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger(__name__)
-
-
-class ATF_BundleProcessor:
-    def __init__(self, sender: ReferenceType, source: MessageHeaderSource):
-        self.sender = sender
-        self.source = source
-        self.use_case_handlers = {}
-        self.message_to_send_event = Event()
-        self.received_Empfangsbestaetigung_event = Event()
-        self.focus_Ressource_to_process_event = Event()
-        self.empfangsbestaetigungs_handler = EmpfangsbestaetigungHandler(
-            self.sender, self.source)
-        self.register_standard_use_case_handlers()
-        self.empfangsbestaetigungs_handler.received_Empfangsbestaetigung_event.subscribe(
-            self.on_empfangsbestaetigung_to_forwarded)
-
-    def on_empfangsbestaetigung_to_forwarded(self, empfangsbestaetigung):
-        self.received_Empfangsbestaetigung_event.trigger(empfangsbestaetigung)
-
-    def register_standard_use_case_handlers(self):
-        self.register_use_case_handler(
-            "https://gematik.de/fhir/atf/CodeSystem/operation-identifier-cs",
-            "atf;Empfangsbestaetigung",
-            self.empfangsbestaetigungs_handler
-        )
-
-        self.register_use_case_handler(
-            "https://gematik.de/fhir/atf/CodeSystem/service-identifier-cs",
-            "Selbsttest;Lieferung",
-            SelbsttestLieferungHandler(self.sender, self.source)
-        )
-
-    def register_use_case_handler(self, system: str, code: str, handler: BaseUseCaseHandler):
-        self.use_case_handlers[(system, code)] = handler
-
-    def process_bundle(self, bundle: Bundle) -> BundleFocusContent:
-        parsed_bundle = self.parse_bundle(bundle)
-
-        if parsed_bundle is None:
-            return
-
-        if not self.is_valid_atf_message(parsed_bundle):
-            return
-
-        message_header = self.get_message_header(parsed_bundle)
-
-        if message_header is None:
-            logger.error(
-                "Die empfangene Nachricht ist keine gültige ATF-Nachricht. Ein MessageHeader fehlt.")
-            return
-
-        handler_key = (message_header.eventCoding.system,
-                       message_header.eventCoding.code)
-
-        if handler_key in self.use_case_handlers:
-            handler = self.use_case_handlers[handler_key]
-            ressources, issues = handler.handle(message_header, parsed_bundle)
-
-            if issues:
-                self.send_empfangsbestätigung(message_header, issues)
-
-            if ressources:
-                focusRessource = BundleFocusContent(
-                    message_header.eventCoding.system, message_header.eventCoding.code, ressources)
-                self.focus_Ressource_to_process_event.trigger(focusRessource)
-
-        else:
-            issues = self.create_unsupported_use_case_issues(
-                message_header.eventCoding.code)
-            self.send_empfangsbestätigung(message_header, issues)
-            return
-
-    def parse_bundle(self, bundle: Bundle):
-        try:
-            return Bundle.parse_raw(bundle.json())
-        except JSONDecodeError:
-            logger.error(
-                "Die empfangene Nachricht ist keine gültige FHIR-Nachricht.")
-            return None
-
-    def is_valid_atf_message(self, parsed_bundle: Bundle):
-        bundle_codesystem = parsed_bundle.meta.profile[0]
-        if bundle_codesystem != "https://gematik.de/fhir/atf/StructureDefinition/bundle-app-transport-framework":
-            logger.error(
-                "Die empfangene Nachricht ist keine gültige ATF-Nachricht.")
-            return False
-
-        return True
-
-    def get_message_header(self, parsed_bundle: Bundle):
-        return next((entry.resource for entry in parsed_bundle.entry if isinstance(
-            entry.resource, MessageHeader)), None)
-
-    def create_unsupported_use_case_issues(self, event_code: str):
-        return [
-            OperationOutcomeIssue(
-                severity="error",
-                code="processing",
-                diagnostics=f"Die empfangene Nachricht mit dem {event_code} kann nicht verarbeitet werden, da der Use-Case nicht unterstützt wird."
-            )
-        ]
-
-    def send_empfangsbestätigung(self, message_header, issues):
-        operation_outcome = OperationOutcomeCreator.create_operation_outcome_ressource(
-            message_id=message_header.id,
-            issues=issues)
-
-        message_to_send = self.create_MessageToSend(
-            message_header, operation_outcome)
-
-        self.message_to_send_event.trigger(message_to_send)
-
-    def create_MessageToSend(self, message_header, operation_outcome):
-        destination = [MessageHeaderDestination(endpoint=message_header.source.endpoint,
-                                                receiver=message_header.sender)]
-
-        operationOutcomeBundle = OperationOutcomeBundleCreator.create_operation_outcome_receipt_bundle(
-            self.sender, self.source, destination, operation_outcome)
-        message_to_send = MessageToSend(
-            operation_outcome_bundle=operationOutcomeBundle,
-            receiver=message_header.sender.identifier.value,
-            message_type="atf;Empfangsbestaetigung"
-        )
-
-        return message_to_send
+import logging
+from json import JSONDecodeError
+from fhir.resources.bundle import Bundle
+from fhir.resources.messageheader import MessageHeader, MessageHeaderSource, MessageHeaderDestination
+from fhir.resources.operationoutcome import OperationOutcomeIssue
+from fhir.resources.fhirtypes import ReferenceType
+from app_transport_framework_library.base_use_case_handler import BaseUseCaseHandler
+from app_transport_framework_library.models.bundle_focus_content import BundleFocusContent
+from app_transport_framework_library.models.event import Event
+from app_transport_framework_library.models.message_to_send import MessageToSend
+from app_transport_framework_library.ressource_creators.operation_outcome_bundle_creator import OperationOutcomeBundleCreator
+from app_transport_framework_library.ressource_creators.operation_outcome_creator import OperationOutcomeCreator
+from app_transport_framework_library.use_cases.empfangsbestaetigung_handler import EmpfangsbestaetigungHandler
+from app_transport_framework_library.use_cases.selbsttest_lieferung_handler import SelbsttestLieferungHandler
+
+
+
+
+
+
+# Configure logging
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
+
+
+class ATF_BundleProcessor:
+    def __init__(self, sender: ReferenceType, source: MessageHeaderSource):
+        self.sender = sender
+        self.source = source
+        self.use_case_handlers = {}
+        self.message_to_send_event = Event()
+        self.received_Empfangsbestaetigung_event = Event()
+        self.focus_Ressource_to_process_event = Event()
+        self.empfangsbestaetigungs_handler = EmpfangsbestaetigungHandler(
+            self.sender, self.source)
+        self.register_standard_use_case_handlers()
+        self.empfangsbestaetigungs_handler.received_Empfangsbestaetigung_event.subscribe(
+            self.on_empfangsbestaetigung_to_forwarded)
+
+    def on_empfangsbestaetigung_to_forwarded(self, empfangsbestaetigung):
+        self.received_Empfangsbestaetigung_event.trigger(empfangsbestaetigung)
+
+    def register_standard_use_case_handlers(self):
+        self.register_use_case_handler(
+            "https://gematik.de/fhir/atf/CodeSystem/operation-identifier-cs",
+            "atf;Empfangsbestaetigung",
+            self.empfangsbestaetigungs_handler
+        )
+
+        self.register_use_case_handler(
+            "https://gematik.de/fhir/atf/CodeSystem/service-identifier-cs",
+            "Selbsttest;Lieferung",
+            SelbsttestLieferungHandler(self.sender, self.source)
+        )
+
+    def register_use_case_handler(self, system: str, code: str, handler: BaseUseCaseHandler):
+        self.use_case_handlers[(system, code)] = handler
+
+    def process_bundle(self, bundle: Bundle) -> BundleFocusContent:
+        parsed_bundle = self.parse_bundle(bundle)
+
+        if parsed_bundle is None:
+            return
+
+        if not self.is_valid_atf_message(parsed_bundle):
+            return
+
+        message_header = self.get_message_header(parsed_bundle)
+
+        if message_header is None:
+            logger.error(
+                "Die empfangene Nachricht ist keine gültige ATF-Nachricht. Ein MessageHeader fehlt.")
+            return
+
+        handler_key = (message_header.eventCoding.system,
+                       message_header.eventCoding.code)
+
+        if handler_key in self.use_case_handlers:
+            handler = self.use_case_handlers[handler_key]
+            ressources, issues = handler.handle(message_header, parsed_bundle)
+
+            if issues:
+                self.send_empfangsbestätigung(message_header, issues)
+
+            if ressources:
+                focusRessource = BundleFocusContent(
+                    message_header.eventCoding.system, message_header.eventCoding.code, ressources)
+                self.focus_Ressource_to_process_event.trigger(focusRessource)
+
+        else:
+            issues = self.create_unsupported_use_case_issues(
+                message_header.eventCoding.code)
+            self.send_empfangsbestätigung(message_header, issues)
+            return
+
+    def parse_bundle(self, bundle: Bundle):
+        try:
+            return Bundle.parse_raw(bundle.json())
+        except JSONDecodeError:
+            logger.error(
+                "Die empfangene Nachricht ist keine gültige FHIR-Nachricht.")
+            return None
+
+    def is_valid_atf_message(self, parsed_bundle: Bundle):
+        bundle_codesystem = parsed_bundle.meta.profile[0]
+        if bundle_codesystem != "https://gematik.de/fhir/atf/StructureDefinition/bundle-app-transport-framework":
+            logger.error(
+                "Die empfangene Nachricht ist keine gültige ATF-Nachricht.")
+            return False
+
+        return True
+
+    def get_message_header(self, parsed_bundle: Bundle):
+        return next((entry.resource for entry in parsed_bundle.entry if isinstance(
+            entry.resource, MessageHeader)), None)
+
+    def create_unsupported_use_case_issues(self, event_code: str):
+        return [
+            OperationOutcomeIssue(
+                severity="error",
+                code="processing",
+                diagnostics=f"Die empfangene Nachricht mit dem {event_code} kann nicht verarbeitet werden, da der Use-Case nicht unterstützt wird."
+            )
+        ]
+
+    def send_empfangsbestätigung(self, message_header, issues):
+        operation_outcome = OperationOutcomeCreator.create_operation_outcome_ressource(
+            message_id=message_header.id,
+            issues=issues)
+
+        message_to_send = self.create_MessageToSend(
+            message_header, operation_outcome)
+
+        self.message_to_send_event.trigger(message_to_send)
+
+    def create_MessageToSend(self, message_header, operation_outcome):
+        destination = [MessageHeaderDestination(endpoint=message_header.source.endpoint,
+                                                receiver=message_header.sender)]
+
+        operationOutcomeBundle = OperationOutcomeBundleCreator.create_operation_outcome_receipt_bundle(
+            self.sender, self.source, destination, operation_outcome)
+        message_to_send = MessageToSend(
+            atf_bundle=operationOutcomeBundle,
+            receiver=message_header.sender.identifier.value,
+            message_type="atf;Empfangsbestaetigung"
+        )
+
+        return message_to_send
```

### Comparing `app_transport_framework_library-0.1.4/app_transport_framework_library/ressource_creators/message_header_creator.py` & `app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/message_header_creator.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from fhir.resources.meta import Meta
-from fhir.resources.messageheader import MessageHeader, MessageHeaderDestination, MessageHeaderSource
-from fhir.resources.fhirtypes import ReferenceType
-from fhir.resources.coding import Coding
-from typing import List
-
-
-class MessageHeaderCreator:
-    @staticmethod
-    def create_message_header(
-        id: str,
-        message_sender: ReferenceType,
-        source: MessageHeaderSource,
-        destinations: List[MessageHeaderDestination],
-        code_system: str,
-        use_case: str,
-        use_case_display: str,
-        focus_reference: str,
-    ) -> MessageHeader:
-        message_header = MessageHeader(
-            id=id,
-            meta=Meta.construct(profile=[
-                "https://gematik.de/fhir/atf/StructureDefinition/message-header-app-transport"
-            ]),
-            eventCoding=Coding(
-                system=code_system,
-                code=use_case,
-                display=use_case_display
-            ),
-            source=source,
-            destination=destinations,
-            sender=message_sender,
-            focus=[ReferenceType(reference=f"urn:uuid:{focus_reference}")]
-        )
-        return message_header
+from fhir.resources.meta import Meta
+from fhir.resources.messageheader import MessageHeader, MessageHeaderDestination, MessageHeaderSource
+from fhir.resources.fhirtypes import ReferenceType
+from fhir.resources.coding import Coding
+from typing import List
+
+
+class MessageHeaderCreator:
+    @staticmethod
+    def create_message_header(
+        id: str,
+        message_sender: ReferenceType,
+        source: MessageHeaderSource,
+        destinations: List[MessageHeaderDestination],
+        code_system: str,
+        use_case: str,
+        use_case_display: str,
+        focus_reference: str,
+    ) -> MessageHeader:
+        message_header = MessageHeader(
+            id=id,
+            meta=Meta.construct(profile=[
+                "https://gematik.de/fhir/atf/StructureDefinition/message-header-app-transport"
+            ]),
+            eventCoding=Coding(
+                system=code_system,
+                code=use_case,
+                display=use_case_display
+            ),
+            source=source,
+            destination=destinations,
+            sender=message_sender,
+            focus=[ReferenceType(reference=f"urn:uuid:{focus_reference}")]
+        )
+        return message_header
```

### Comparing `app_transport_framework_library-0.1.4/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py` & `app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from fhir.resources.bundle import Bundle, BundleEntry
-from fhir.resources.messageheader import MessageHeaderDestination, MessageHeaderSource
-from fhir.resources.fhirtypes import ReferenceType
-from fhir.resources.operationoutcome import OperationOutcome
-from typing import List
-from uuid import uuid4
-
-from app_transport_framework_library.app_transport_framework_library.ressource_creators.message_bundle_creator import MessageBundleCreator
-from app_transport_framework_library.app_transport_framework_library.ressource_creators.message_header_creator import MessageHeaderCreator
-
-
-
-class OperationOutcomeBundleCreator:
-    def create_operation_outcome_receipt_bundle(message_sender: ReferenceType,
-                                                source: MessageHeaderSource,
-                                                destinations: List[MessageHeaderDestination],
-                                                operation_outcome: OperationOutcome) -> Bundle:
-
-        message_header = MessageHeaderCreator.create_message_header(
-            str(uuid4()),
-            message_sender,
-            source,
-            destinations,
-            code_system="https://gematik.de/fhir/atf/CodeSystem/operation-identifier-cs",
-            use_case="atf;Empfangsbestaetigung",
-            use_case_display="Empfangsbestätigung und Auskunft über FHIR Interpretierbarkeit der Nachricht",
-            focus_reference=operation_outcome.id)
-
-        resources = [
-            BundleEntry(
-                fullUrl=f"urn:uuid:{operation_outcome.id}",
-                resource=operation_outcome
-            )
-        ]
-
-        bundle = MessageBundleCreator.create_message_bundle(
-            message_header=message_header,
-            resources=resources
-        )
-
-        return bundle
+from fhir.resources.bundle import Bundle, BundleEntry
+from fhir.resources.messageheader import MessageHeaderDestination, MessageHeaderSource
+from fhir.resources.fhirtypes import ReferenceType
+from fhir.resources.operationoutcome import OperationOutcome
+from typing import List
+from uuid import uuid4
+
+from app_transport_framework_library.ressource_creators.message_bundle_creator import MessageBundleCreator
+from app_transport_framework_library.ressource_creators.message_header_creator import MessageHeaderCreator
+
+
+
+class OperationOutcomeBundleCreator:
+    def create_operation_outcome_receipt_bundle(message_sender: ReferenceType,
+                                                source: MessageHeaderSource,
+                                                destinations: List[MessageHeaderDestination],
+                                                operation_outcome: OperationOutcome) -> Bundle:
+
+        message_header = MessageHeaderCreator.create_message_header(
+            str(uuid4()),
+            message_sender,
+            source,
+            destinations,
+            code_system="https://gematik.de/fhir/atf/CodeSystem/operation-identifier-cs",
+            use_case="atf;Empfangsbestaetigung",
+            use_case_display="Empfangsbestätigung und Auskunft über FHIR Interpretierbarkeit der Nachricht",
+            focus_reference=operation_outcome.id)
+
+        resources = [
+            BundleEntry(
+                fullUrl=f"urn:uuid:{operation_outcome.id}",
+                resource=operation_outcome
+            )
+        ]
+
+        bundle = MessageBundleCreator.create_message_bundle(
+            message_header=message_header,
+            resources=resources
+        )
+
+        return bundle
```

### Comparing `app_transport_framework_library-0.1.4/app_transport_framework_library/ressource_creators/operation_outcome_creator.py` & `app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/operation_outcome_creator.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from fhir.resources.operationoutcome import OperationOutcome, OperationOutcomeIssue
-from fhir.resources.meta import Meta
-from fhir.resources.extension import Extension
-from uuid import uuid4
-
-
-class OperationOutcomeCreator:
-    def create_operation_outcome_ressource(message_id: str, issues: list[OperationOutcomeIssue]) -> OperationOutcome:
-        operation_outcome = OperationOutcome(
-            id=str(uuid4()),
-            meta=Meta.construct(
-                profile=["https://gematik.de/fhir/atf/StructureDefinition/atf-operation-outcome"]),
-            extension=[
-                Extension(
-                    url="https://gematik.de/fhir/atf/StructureDefinition/atf-message-id-ex",
-                    valueString=message_id
-                )
-            ],
-            issue=issues
-        )
-        return operation_outcome
+from fhir.resources.operationoutcome import OperationOutcome, OperationOutcomeIssue
+from fhir.resources.meta import Meta
+from fhir.resources.extension import Extension
+from uuid import uuid4
+
+
+class OperationOutcomeCreator:
+    def create_operation_outcome_ressource(message_id: str, issues: list[OperationOutcomeIssue]) -> OperationOutcome:
+        operation_outcome = OperationOutcome(
+            id=str(uuid4()),
+            meta=Meta.construct(
+                profile=["https://gematik.de/fhir/atf/StructureDefinition/atf-operation-outcome"]),
+            extension=[
+                Extension(
+                    url="https://gematik.de/fhir/atf/StructureDefinition/atf-message-id-ex",
+                    valueString=message_id
+                )
+            ],
+            issue=issues
+        )
+        return operation_outcome
```

### Comparing `app_transport_framework_library-0.1.4/app_transport_framework_library/ressource_creators/test_message_creator.py` & `app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/test_message_creator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from uuid import uuid4
-from fhir.resources.messageheader import MessageHeaderDestination, MessageHeaderSource
-from fhir.resources.bundle import BundleEntry
-from fhir.resources.communication import Communication, CommunicationPayload
-from fhir.resources.fhirtypes import ReferenceType, CodeableConceptType
-from fhir.resources.attachment import Attachment
-from app_transport_framework_library.app_transport_framework_library.ressource_creators.message_bundle_creator import MessageBundleCreator
-
-from app_transport_framework_library.app_transport_framework_library.ressource_creators.message_header_creator import MessageHeaderCreator
-
-
-
-class CommunicationCreator:
-    def __init__(self):
-        pass
-
-    def create(id: str, status: str, priority: str, subject_display: str, sender_display: str,
-               content_attachment_title: str, content_attachment_content_type: str,
-               content_attachment_data: str, sent: str, received: str) -> Communication:
-        communication = Communication(
-            id=id,
-            status=status,
-            priority=priority,
-            subject=ReferenceType(display=subject_display),
-            sender=ReferenceType(display=sender_display),
-            payload=[
-                CommunicationPayload(
-                    contentAttachment=Attachment(
-                        title=content_attachment_title,
-                        contentType=content_attachment_content_type,
-                        data=content_attachment_data
-                    )
-                )
-            ],
-            sent=sent,
-            received=received
-        )
-        category_coding = CodeableConceptType(
-            system="http://loinc.org",
-            code="45012-6",
-            display="Communication regarding test results"
-        )
-        communication.category = [
-            CodeableConceptType(coding=[category_coding])]
-        return communication
-
-
-class TestMessageCreator:
-    def create_test_bundle(sender: ReferenceType, source: MessageHeaderSource,   receiver: ReferenceType, message_id: str):
-        communication_id = str(uuid4())
-
-        source = source
-        message_receiver = receiver
-        destination = [MessageHeaderDestination(endpoint="https://receiver.example.com/endpoint",
-                                                receiver=message_receiver)]
-
-        message_header = MessageHeaderCreator.create_message_header(
-            message_id,
-            sender,
-            source,
-            destination,
-            code_system="https://gematik.de/fhir/atf/CodeSystem/service-identifier-cs",
-            use_case="Selbsttest;Lieferung",
-            use_case_display="Diese Dienstkennung dient ausschließlich der Einrichtung des Kontos innerhalb eines PVS und des Testes, ob Nachrichten versendet und empfangen werden können. Diese Dienstkennung wird im PVS bei der normalen Abholung von Nachrichten ignoriert.",
-            focus_reference=communication_id)
-
-        communication = CommunicationCreator.create(
-            id=communication_id,
-            status="completed",
-            priority="routine",
-            subject_display="Max Mustermann",
-            sender_display="Dr. Anna Schmidt",
-            content_attachment_title="Selbsttest Bestätigung",
-            content_attachment_content_type="text/plain",
-            content_attachment_data="U2VsYnN0dGVzdCBhYnNjaGxpZXNzZW4uIEJpdHRlIGtsYXJlbiBTaWUgZGllIFRlc3RlcmdlYm5pc3NlIGFiLg==",
-            sent="2023-03-29T13:28:17.239+02:00",
-            received="2023-03-29T13:30:00.000+02:00"
-        )
-
-        resources = [
-            BundleEntry(
-                fullUrl=f"urn:uuid:{communication_id}",
-                resource=communication
-            )
-        ]
-
-        bundle = MessageBundleCreator.create_message_bundle(
-            message_header=message_header,
-            resources=resources
-        )
-
-        return bundle
+from uuid import uuid4
+from fhir.resources.messageheader import MessageHeaderDestination, MessageHeaderSource
+from fhir.resources.bundle import BundleEntry
+from fhir.resources.communication import Communication, CommunicationPayload
+from fhir.resources.fhirtypes import ReferenceType, CodeableConceptType
+from fhir.resources.attachment import Attachment
+from app_transport_framework_library.ressource_creators.message_bundle_creator import MessageBundleCreator
+
+from app_transport_framework_library.ressource_creators.message_header_creator import MessageHeaderCreator
+
+
+
+class CommunicationCreator:
+    def __init__(self):
+        pass
+
+    def create(id: str, status: str, priority: str, subject_display: str, sender_display: str,
+               content_attachment_title: str, content_attachment_content_type: str,
+               content_attachment_data: str, sent: str, received: str) -> Communication:
+        communication = Communication(
+            id=id,
+            status=status,
+            priority=priority,
+            subject=ReferenceType(display=subject_display),
+            sender=ReferenceType(display=sender_display),
+            payload=[
+                CommunicationPayload(
+                    contentAttachment=Attachment(
+                        title=content_attachment_title,
+                        contentType=content_attachment_content_type,
+                        data=content_attachment_data
+                    )
+                )
+            ],
+            sent=sent,
+            received=received
+        )
+        category_coding = CodeableConceptType(
+            system="http://loinc.org",
+            code="45012-6",
+            display="Communication regarding test results"
+        )
+        communication.category = [
+            CodeableConceptType(coding=[category_coding])]
+        return communication
+
+
+class TestMessageCreator:
+    def create_test_bundle(sender: ReferenceType, source: MessageHeaderSource,   receiver: ReferenceType, message_id: str):
+        communication_id = str(uuid4())
+
+        source = source
+        message_receiver = receiver
+        destination = [MessageHeaderDestination(endpoint="https://receiver.example.com/endpoint",
+                                                receiver=message_receiver)]
+
+        message_header = MessageHeaderCreator.create_message_header(
+            message_id,
+            sender,
+            source,
+            destination,
+            code_system="https://gematik.de/fhir/atf/CodeSystem/service-identifier-cs",
+            use_case="Selbsttest;Lieferung",
+            use_case_display="Diese Dienstkennung dient ausschließlich der Einrichtung des Kontos innerhalb eines PVS und des Testes, ob Nachrichten versendet und empfangen werden können. Diese Dienstkennung wird im PVS bei der normalen Abholung von Nachrichten ignoriert.",
+            focus_reference=communication_id)
+
+        communication = CommunicationCreator.create(
+            id=communication_id,
+            status="completed",
+            priority="routine",
+            subject_display="Max Mustermann",
+            sender_display="Dr. Anna Schmidt",
+            content_attachment_title="Selbsttest Bestätigung",
+            content_attachment_content_type="text/plain",
+            content_attachment_data="U2VsYnN0dGVzdCBhYnNjaGxpZXNzZW4uIEJpdHRlIGtsYXJlbiBTaWUgZGllIFRlc3RlcmdlYm5pc3NlIGFiLg==",
+            sent="2023-03-29T13:28:17.239+02:00",
+            received="2023-03-29T13:30:00.000+02:00"
+        )
+
+        resources = [
+            BundleEntry(
+                fullUrl=f"urn:uuid:{communication_id}",
+                resource=communication
+            )
+        ]
+
+        bundle = MessageBundleCreator.create_message_bundle(
+            message_header=message_header,
+            resources=resources
+        )
+
+        return bundle
```

### Comparing `app_transport_framework_library-0.1.4/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py` & `app_transport_framework_library-0.1.5/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from typing import List, Tuple
-from fhir.resources.bundle import Bundle
-from fhir.resources.operationoutcome import OperationOutcome, OperationOutcomeIssue
-from fhir.resources.messageheader import MessageHeader
-from fhir.resources.bundle import BundleEntry
-
-from app_transport_framework_library.base_use_case_handler import BaseUseCaseHandler
-from app_transport_framework_library.models.empfangsbestaetigung import Empfangsbestaetigung
-
-
-
-
-class EmpfangsbestaetigungHandler(BaseUseCaseHandler):
-
-    def resolve_reference(self, reference_str: str, bundle: Bundle):
-        for entry in bundle.entry:
-            if entry.resource.id == reference_str.split('urn:uuid:')[-1]:
-                return entry.resource
-        return None
-
-    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[List[BundleEntry], List[OperationOutcomeIssue]]:
-        self.bundleEntries = []
-        self.issues = []
-        message_header = self.get_ressource_by_type(bundle, MessageHeader)
-        outcome = self.get_ressource_by_type(bundle, OperationOutcome)
-        message_id = outcome.extension[0].valueString.split(
-            'urn:uuid:')[-1]
-        empfangsbestaetigung = Empfangsbestaetigung(
-            message_id, True, message_header.sender.identifier.value, outcome.issue[0])
-
-        self.received_Empfangsbestaetigung_event.trigger(empfangsbestaetigung)
-        return self.bundleEntries, self.issues
-
-    def get_ressource_by_type(self, parsed_bundle: Bundle, type):
-        return next((entry.resource for entry in parsed_bundle.entry if isinstance(
-            entry.resource, type)), None)
+from typing import List, Tuple
+from fhir.resources.bundle import Bundle
+from fhir.resources.operationoutcome import OperationOutcome, OperationOutcomeIssue
+from fhir.resources.messageheader import MessageHeader
+from fhir.resources.bundle import BundleEntry
+
+from app_transport_framework_library.base_use_case_handler import BaseUseCaseHandler
+from app_transport_framework_library.models.empfangsbestaetigung import Empfangsbestaetigung
+
+
+
+
+class EmpfangsbestaetigungHandler(BaseUseCaseHandler):
+
+    def resolve_reference(self, reference_str: str, bundle: Bundle):
+        for entry in bundle.entry:
+            if entry.resource.id == reference_str.split('urn:uuid:')[-1]:
+                return entry.resource
+        return None
+
+    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[List[BundleEntry], List[OperationOutcomeIssue]]:
+        self.bundleEntries = []
+        self.issues = []
+        message_header = self.get_ressource_by_type(bundle, MessageHeader)
+        outcome = self.get_ressource_by_type(bundle, OperationOutcome)
+        message_id = outcome.extension[0].valueString.split(
+            'urn:uuid:')[-1]
+        empfangsbestaetigung = Empfangsbestaetigung(
+            message_id, True, message_header.sender.identifier.value, message_header.destination[0].receiver.identifier.value, outcome.issue[0])
+
+        self.received_Empfangsbestaetigung_event.trigger(empfangsbestaetigung)
+        return self.bundleEntries, self.issues
+
+    def get_ressource_by_type(self, parsed_bundle: Bundle, type):
+        return next((entry.resource for entry in parsed_bundle.entry if isinstance(
+            entry.resource, type)), None)
```

### Comparing `app_transport_framework_library-0.1.4/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py` & `app_transport_framework_library-0.1.5/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from typing import List, Tuple
-from fhir.resources.messageheader import MessageHeader
-from fhir.resources.bundle import Bundle
-from fhir.resources.bundle import Bundle
-from fhir.resources.operationoutcome import OperationOutcome, OperationOutcomeIssue
-from fhir.resources.messageheader import MessageHeader
-from fhir.resources.communication import Communication
-from fhir.resources.bundle import BundleEntry
-
-from app_transport_framework_library.base_use_case_handler import BaseUseCaseHandler
-
-
-
-
-class SelbsttestLieferungHandler(BaseUseCaseHandler):
-    def resolve_reference(self, reference_str: str, bundle: Bundle):
-        for entry in bundle.entry:
-            if entry.resource.id == reference_str.split('urn:uuid:')[-1]:
-                return entry.resource
-        return None
-
-    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[List[BundleEntry], List[OperationOutcomeIssue]]:
-        self.bundleEntries = []
-        self.issues = []
-        if not any([isinstance(self.resolve_reference(focus_ref.reference, Bundle.parse_raw(bundle.json())), Communication) for focus_ref in message_header.focus]):
-            self.issues.append(
-                OperationOutcomeIssue(
-                    severity="fatal",
-                    code="invalid",
-                    diagnostics="Eine Communication-Ressource wurde im MessageHeader.focus nicht gefunden"
-                )
-            )
-        else:
-            self.issues.append(
-                OperationOutcomeIssue(
-                    severity="information",
-                    code="informational",
-                    diagnostics="Anfrage erfolgreich entgegengenommen"
-                )
-            )
-
-            for entry in bundle.entry:
-                if not isinstance(entry.resource, (MessageHeader, OperationOutcome)):
-                    self.bundleEntries.append(entry.resource)
-
-        return self.bundleEntries, self.issues
+from typing import List, Tuple
+from fhir.resources.messageheader import MessageHeader
+from fhir.resources.bundle import Bundle
+from fhir.resources.bundle import Bundle
+from fhir.resources.operationoutcome import OperationOutcome, OperationOutcomeIssue
+from fhir.resources.messageheader import MessageHeader
+from fhir.resources.communication import Communication
+from fhir.resources.bundle import BundleEntry
+
+from app_transport_framework_library.base_use_case_handler import BaseUseCaseHandler
+
+
+
+
+class SelbsttestLieferungHandler(BaseUseCaseHandler):
+    def resolve_reference(self, reference_str: str, bundle: Bundle):
+        for entry in bundle.entry:
+            if entry.resource.id == reference_str.split('urn:uuid:')[-1]:
+                return entry.resource
+        return None
+
+    def handle(self, message_header: MessageHeader, bundle: Bundle) -> Tuple[List[BundleEntry], List[OperationOutcomeIssue]]:
+        self.bundleEntries = []
+        self.issues = []
+        if not any([isinstance(self.resolve_reference(focus_ref.reference, Bundle.parse_raw(bundle.json())), Communication) for focus_ref in message_header.focus]):
+            self.issues.append(
+                OperationOutcomeIssue(
+                    severity="fatal",
+                    code="invalid",
+                    diagnostics="Eine Communication-Ressource wurde im MessageHeader.focus nicht gefunden"
+                )
+            )
+        else:
+            self.issues.append(
+                OperationOutcomeIssue(
+                    severity="information",
+                    code="informational",
+                    diagnostics="Anfrage erfolgreich entgegengenommen"
+                )
+            )
+
+            for entry in bundle.entry:
+                if not isinstance(entry.resource, (MessageHeader, OperationOutcome)):
+                    self.bundleEntries.append(entry.resource)
+
+        return self.bundleEntries, self.issues
```

### Comparing `app_transport_framework_library-0.1.4/PKG-INFO` & `app_transport_framework_library-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-transport-framework-library
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Sven Sommer
 Author-email: rob.hoffmann@posteo.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

