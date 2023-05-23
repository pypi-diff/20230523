# Comparing `tmp/llmspec-0.2.0.tar.gz` & `tmp/llmspec-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmspec-0.2.0.tar", last modified: Fri May 19 04:35:47 2023, max compression
+gzip compressed data, was "llmspec-0.3.0.tar", last modified: Tue May 23 03:18:41 2023, max compression
```

## Comparing `llmspec-0.2.0.tar` & `llmspec-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11098 2023-05-19 04:35:37.579458 llmspec-0.2.0/LICENSE
--rw-r--r--   0        0        0       33 2023-05-19 04:35:37.579458 llmspec-0.2.0/README.md
--rw-r--r--   0        0        0      461 2023-05-19 04:35:37.579458 llmspec-0.2.0/llmspec/__init__.py
--rw-r--r--   0        0        0     8693 2023-05-19 04:35:37.579458 llmspec-0.2.0/llmspec/llmspec.py
--rw-r--r--   0        0        0     1056 2023-05-19 04:35:47.575492 llmspec-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-19 04:35:37.579458 llmspec-0.2.0/tests/dummy_test.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11098 2023-05-23 03:18:29.120567 llmspec-0.3.0/LICENSE
+-rw-r--r--   0        0        0       33 2023-05-23 03:18:29.120567 llmspec-0.3.0/README.md
+-rw-r--r--   0        0        0      503 2023-05-23 03:18:29.120567 llmspec-0.3.0/llmspec/__init__.py
+-rw-r--r--   0        0        0     8553 2023-05-23 03:18:29.120567 llmspec-0.3.0/llmspec/llmspec.py
+-rw-r--r--   0        0        0     1056 2023-05-23 03:18:41.428842 llmspec-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-23 03:18:29.120567 llmspec-0.3.0/tests/dummy_test.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.0/PKG-INFO
```

### Comparing `llmspec-0.2.0/LICENSE` & `llmspec-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmspec-0.2.0/llmspec/llmspec.py` & `llmspec-0.3.0/llmspec/llmspec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import json
 from typing import Union, Optional, Dict, List
 from datetime import datetime
 from enum import Enum
 
 import msgspec
 
@@ -22,71 +23,65 @@
     """Unified chat message interface."""
 
     content: str
     role: Role = Role.USER
     name: str = ""
 
 
-class RoleTokenMap(msgspec.Struct, kw_only=True):
+class LanguageModelInfo(msgspec.Struct):
+    """Language model information."""
+
+    # token
     user_token: str = ""
     assistant_token: str = ""
     system_token: str = ""
+    append_assistant_token: bool = False
 
+    # model class name in `transformers`
+    transformer_model_cls: str = "AutoModelForCausalLM"
 
-class ChatGLMRoleTokenMap(RoleTokenMap):
-    """
-    ChatGLM role token map.
-    Currently not used because standard ChatGLM prompt
-    requires the inclusion of a dynamic round number.
-    """
-
-    user_token: str = "问："
-    assistant_token: str = "答："
-    system_token: str = ""
-
-
-class MOSSRoleTokenMap(RoleTokenMap):
-    """
-    MOSS role token map.
-    """
-
-    user_token: str = "<|USER|>"
-    assistant_token: str = "<|ASSISTANT|>"
-    system_token: str = "<|SYSTEM|>"
-
-
-class StableLMRoleTokenMap(RoleTokenMap):
-    """
-    StableLM role token map.
-    """
-
-    user_token: str = "<|Human|>"
-    assistant_token: str = "<|StableLM|>"
-    system_token: str = ""
-
-
-def get_standard_conversation_prompt(
-    messages: List[ChatMessage],
-    role_token_map: RoleTokenMap,
-    append_assistant_token: bool = True,
-) -> str:
-    """Get a prompt for a conversation using the commonly used format in chat models."""
-    formatted_messages = []
-    for message in messages:
-        if message.role == Role.USER:
-            message_prefix = role_token_map.user_token
-        elif message.role == Role.ASSISTANT:
-            message_prefix = role_token_map.assistant_token
-        else:
-            message_prefix = role_token_map.system_token
-        formatted_messages.append(f"{message_prefix}{message.content}")
-    prompt_suffix = (
-        f"\n{role_token_map.assistant_token}" if append_assistant_token else ""
-    )
-    return "\n".join(formatted_messages) + prompt_suffix
+    def get_conversation_prompt(self, messages: List[ChatMessage]) -> str:
+        """Get the prompt for a conversation using the specific tokens of the model."""
+        formatted_messages = []
+        for message in messages:
+            if message.role == Role.USER:
+                message_prefix = self.user_token
+            elif message.role == Role.ASSISTANT:
+                message_prefix = self.assistant_token
+            else:
+                message_prefix = self.system_token
+            formatted_messages.append(f"{message_prefix}{message.content}")
+        conversation = "\n".join(formatted_messages)
+        if self.append_assistant_token:
+            conversation += f"\n{self.assistant_token}"
+        return conversation
+
+
+ChatGLM = LanguageModelInfo(
+    user_token="问：",
+    assistant_token="答：",
+    system_token="",
+    transformer_model_cls="AutoModel",
+)
+MOSS = LanguageModelInfo(
+    user_token="<|USER|>",
+    assistant_token="<|ASSISTANT|>",
+    system_token="<|SYSTEM|>",
+    transformer_model_cls="AutoModelForCausalLM",
+    append_assistant_token=True,
+)
+StableLM = LanguageModelInfo(
+    user_token="<|Human|>",
+    assistant_token="<|StableLM|>",
+    system_token="",
+    append_assistant_token=True,
+)
+BloomZ = LanguageModelInfo()
+LLaMA = LanguageModelInfo()
+Unknown = LanguageModelInfo()
 
 
 class CompletionRequest(msgspec.Struct, kw_only=True):
     suffix: Optional[str] = None
     max_tokens: int = 16
     temperature: float = 1.0
     top_p: float = 1.0
@@ -110,62 +105,60 @@
     prompt: str = "<|endoftext|>"
     echo: bool = False
     logprobs: Optional[int] = None
     best_of: int = 1
 
 
 class LanguageModels(Enum):
-    CHAT_GLM = "ChatGLM"
-    MOSS = "MOSS"
-    STABLE_LM = "StableLM"
+    CHAT_GLM = ChatGLM
+    MOSS = MOSS
+    STABLE_LM = StableLM
+    BLOOM_Z = BloomZ
 
-    UNKNOWN = "unknown"
+    UNKNOWN = Unknown
 
     @classmethod
-    def find(cls, name: str) -> "LanguageModels":
+    def find(cls, name: str) -> LanguageModels:
         if name.lower().startswith("thudm/chatglm"):
             return cls.CHAT_GLM
         if name.lower().startswith("fnlp/moss-moon"):
             return cls.MOSS
         if name.lower().startswith("stabilityai/stablelm"):
             return cls.STABLE_LM
+        if name.lower().startswith("bigscience/bloomz"):
+            return cls.BLOOM_Z
         return cls.UNKNOWN
 
+    @classmethod
+    def transformer_cls(cls, name: str) -> str:
+        return cls.find(name).value.transformer_model_cls
+
 
 class ChatCompletionRequest(CompletionRequest):
     model: str
     messages: List[ChatMessage]
 
     def get_prompt(self, model: str):
-        if LanguageModels.find(model) == LanguageModels.CHAT_GLM:
+        model = LanguageModels.find(model)
+        if model is LanguageModels.CHAT_GLM:
             # ref to https://huggingface.co/THUDM/chatglm-6b/blob/main/modeling_chatglm.py#L1267
             if len(self.messages) == 1:
                 return self.messages[0].content
             round = -1
             prompt = ""
             for message in self.messages:
                 if message.role == Role.USER:
                     round += 1
                     prompt += f"[Round {round}]\n问：{message.content}\n"
                 elif message.role == Role.ASSISTANT:
                     prompt += f"答：{message.content}\n"
                 else:
                     prompt += f"{message.content}\n"
             return prompt
-        elif LanguageModels.find(model) == LanguageModels.MOSS:
-            return get_standard_conversation_prompt(
-                self.messages, MOSSRoleTokenMap(), True
-            )
-        elif LanguageModels.find(model) == LanguageModels.STABLE_LM:
-            return get_standard_conversation_prompt(
-                self.messages, StableLMRoleTokenMap(), True
-            )
-
-        # return all the content by default
-        return get_standard_conversation_prompt(self.messages, RoleTokenMap(), False)
+        return model.value.get_conversation_prompt(self.messages)
 
     def get_inference_args(self, model: str):
         if LanguageModels.find(model) == LanguageModels.CHAT_GLM:
             return dict(
                 max_length=self.max_tokens,
                 top_p=self.top_p,
                 temperature=self.temperature,
```

### Comparing `llmspec-0.2.0/pyproject.toml` & `llmspec-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "msgspec>=0.15.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.2.0"
+version = "0.3.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
```

