# Comparing `tmp/llmspec-0.3.0.tar.gz` & `tmp/llmspec-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmspec-0.3.0.tar", last modified: Tue May 23 03:18:41 2023, max compression
+gzip compressed data, was "llmspec-0.3.1.tar", last modified: Tue May 23 09:33:17 2023, max compression
```

## Comparing `llmspec-0.3.0.tar` & `llmspec-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11098 2023-05-23 03:18:29.120567 llmspec-0.3.0/LICENSE
--rw-r--r--   0        0        0       33 2023-05-23 03:18:29.120567 llmspec-0.3.0/README.md
--rw-r--r--   0        0        0      503 2023-05-23 03:18:29.120567 llmspec-0.3.0/llmspec/__init__.py
--rw-r--r--   0        0        0     8553 2023-05-23 03:18:29.120567 llmspec-0.3.0/llmspec/llmspec.py
--rw-r--r--   0        0        0     1056 2023-05-23 03:18:41.428842 llmspec-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-23 03:18:29.120567 llmspec-0.3.0/tests/dummy_test.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11098 2023-05-23 09:33:03.150615 llmspec-0.3.1/LICENSE
+-rw-r--r--   0        0        0       33 2023-05-23 09:33:03.150615 llmspec-0.3.1/README.md
+-rw-r--r--   0        0        0      609 2023-05-23 09:33:03.150615 llmspec-0.3.1/llmspec/__init__.py
+-rw-r--r--   0        0        0     9569 2023-05-23 09:33:03.150615 llmspec-0.3.1/llmspec/llmspec.py
+-rw-r--r--   0        0        0     1056 2023-05-23 09:33:17.610716 llmspec-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-23 09:33:03.150615 llmspec-0.3.1/tests/dummy_test.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.1/PKG-INFO
```

### Comparing `llmspec-0.3.0/LICENSE` & `llmspec-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.0/llmspec/llmspec.py` & `llmspec-0.3.1/llmspec/llmspec.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,19 +98,24 @@
     @classmethod
     def from_bytes(cls, buf: bytes):
         return msgspec.json.decode(buf, type=cls)
 
 
 class PromptCompletionRequest(CompletionRequest):
     model: str
-    prompt: str = "<|endoftext|>"
+    prompt: Union[str, List[str]] = "<|endoftext|>"
     echo: bool = False
     logprobs: Optional[int] = None
     best_of: int = 1
 
+    def get_prompt(self):
+        if isinstance(self.prompt, list):
+            return "\n".join(self.prompt)
+        return self.prompt
+
 
 class LanguageModels(Enum):
     CHAT_GLM = ChatGLM
     MOSS = MOSS
     STABLE_LM = StableLM
     BLOOM_Z = BloomZ
 
@@ -134,31 +139,31 @@
 
 
 class ChatCompletionRequest(CompletionRequest):
     model: str
     messages: List[ChatMessage]
 
     def get_prompt(self, model: str):
-        model = LanguageModels.find(model)
-        if model is LanguageModels.CHAT_GLM:
+        language_model = LanguageModels.find(model)
+        if language_model is LanguageModels.CHAT_GLM:
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
-        return model.value.get_conversation_prompt(self.messages)
+        return language_model.value.get_conversation_prompt(self.messages)
 
     def get_inference_args(self, model: str):
         if LanguageModels.find(model) == LanguageModels.CHAT_GLM:
             return dict(
                 max_length=self.max_tokens,
                 top_p=self.top_p,
                 temperature=self.temperature,
@@ -186,25 +191,40 @@
 
 class TokenUsage(msgspec.Struct):
     prompt_tokens: int
     completion_tokens: int
     total_tokens: int
 
 
-class CompletionResponse(msgspec.Struct):
+class CompletionChoice(msgspec.Struct):
+    text: str
+    index: int = 0
+    logprobs: Optional[int] = None
+    finish_reason: str = "length"
+
+
+class LMResponse(msgspec.Struct):
     id: str
     object: str
     created: datetime
-    choices: List[ChatChoice]
+    model: str
     usage: TokenUsage
 
     def to_json(self):
         return msgspec.json.encode(self)
 
 
+class CompletionResponse(LMResponse):
+    choices: List[CompletionChoice]
+
+
+class ChatResponse(LMResponse):
+    choices: List[ChatChoice]
+
+
 class EmbeddingRequest(msgspec.Struct):
     model: str
     input: Union[str, List[str]]
     user: str = ""
 
 
 class EmbeddingData(msgspec.Struct):
@@ -216,14 +236,41 @@
 class EmbeddingResponse(msgspec.Struct):
     data: EmbeddingData
     model: str
     usage: TokenUsage
     object: str = "list"
 
 
+class ErrorMessage(msgspec.Struct):
+    code: int
+    type: str
+    message: str
+    param: str
+
+
+class ErrorResponse(msgspec.Struct):
+    error: ErrorMessage
+
+    @classmethod
+    def from_validation_err(
+        cls, err: msgspec.ValidationError, param: str = ""
+    ) -> ErrorResponse:
+        return ErrorResponse(
+            error=ErrorMessage(
+                code=400,
+                type="validation_error",
+                message=str(err),
+                param=param,
+            )
+        )
+
+    def to_json(self):
+        return msgspec.json.encode(self)
+
+
 class LLMSpec:
     """
     Represents an LLMSpec object.
 
     Args:
         text (str): The text content of the LLMSpec.
```

### Comparing `llmspec-0.3.0/pyproject.toml` & `llmspec-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "msgspec>=0.15.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.0"
+version = "0.3.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
```

