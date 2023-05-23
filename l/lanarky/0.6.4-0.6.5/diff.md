# Comparing `tmp/lanarky-0.6.4.tar.gz` & `tmp/lanarky-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.6.4.tar", max compression
+gzip compressed data, was "lanarky-0.6.5.tar", max compression
```

## Comparing `lanarky-0.6.4.tar` & `lanarky-0.6.5.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1073 2023-05-22 14:41:40.512310 lanarky-0.6.4/LICENSE
--rw-r--r--   0        0        0     3991 2023-05-22 14:41:40.512310 lanarky-0.6.4/README.md
--rw-r--r--   0        0        0        0 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/__init__.py
--rw-r--r--   0        0        0     3018 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     1586 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1421 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     2675 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/callbacks/qa_with_sources.py
--rw-r--r--   0        0        0     2801 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0     1352 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/register.py
--rw-r--r--   0        0        0       74 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     2676 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/responses/streaming.py
--rw-r--r--   0        0        0      536 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-22 14:41:40.716309 lanarky-0.6.4/lanarky/websockets/base.py
--rw-r--r--   0        0        0      918 2023-05-22 14:41:40.716309 lanarky-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     4769 1970-01-01 00:00:00.000000 lanarky-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-23 17:13:55.227473 lanarky-0.6.5/LICENSE
+-rw-r--r--   0        0        0     3991 2023-05-23 17:13:55.227473 lanarky-0.6.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/__init__.py
+-rw-r--r--   0        0        0     2500 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3023 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2216 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3461 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0     2004 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/register.py
+-rw-r--r--   0        0        0       74 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     2926 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      715 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1093 2023-05-23 17:13:55.443477 lanarky-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 lanarky-0.6.5/PKG-INFO
```

### Comparing `lanarky-0.6.4/LICENSE` & `lanarky-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.4/README.md` & `lanarky-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.4/lanarky/callbacks/agents.py` & `lanarky-0.6.5/lanarky/callbacks/agents.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,36 @@
-from typing import Any, Dict, List
+from typing import Any
 
-from lanarky.register import register_streaming_callback, register_websocket_callback
+from lanarky.register import (
+    register_streaming_callback,
+    register_streaming_json_callback,
+    register_websocket_callback,
+)
+from lanarky.schemas import StreamingJSONResponse
 
 from .base import AsyncLanarkyCallback
-from .llm import AsyncLLMChainStreamingCallback, AsyncLLMChainWebsocketCallback
+from .llm import (
+    AsyncLLMChainStreamingCallback,
+    AsyncLLMChainStreamingJSONCallback,
+    AsyncLLMChainWebsocketCallback,
+)
 
 
 class AsyncAgentsLanarkyCallback(AsyncLanarkyCallback):
     """Base AsyncCallback handler for AgentExecutor.
 
     Adapted from `langchain/callbacks/streaming_stdout_final_only.py <https://github.com/hwchase17/langchain/blob/master/langchain/callbacks/streaming_stdout_final_only.py>`_
     """
 
-    answer_prefix_tokens: List[str] = ["Final", " Answer", ":"]
-    last_tokens: List[str] = [""] * len(answer_prefix_tokens)
+    answer_prefix_tokens: list[str] = ["Final", " Answer", ":"]
+    last_tokens: list[str] = [""] * len(answer_prefix_tokens)
     answer_reached: bool = False
 
     async def on_llm_start(
-        self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
+        self, serialized: dict[str, Any], prompts: list[str], **kwargs: Any
     ) -> None:
         """Run when LLM starts running."""
         self.last_tokens = [""] * len(self.answer_prefix_tokens)
         self.answer_reached = False
 
     def _check_if_answer_reached(self, token: str):
         self.last_tokens.append(token)
@@ -55,7 +64,20 @@
     """AsyncWebsocketCallback handler for AgentExecutor."""
 
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         """Run on new LLM token. Only available when streaming is enabled."""
         if self._check_if_answer_reached(token):
             message = self._construct_message(token)
             await self.websocket.send_json(message)
+
+
+@register_streaming_json_callback("AgentExecutor")
+class AsyncAgentsStreamingJSONCallback(
+    AsyncAgentsLanarkyCallback, AsyncLLMChainStreamingJSONCallback
+):
+    """AsyncStreamingJSONCallback handler for AgentExecutor."""
+
+    async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
+        """Run on new LLM token. Only available when streaming is enabled."""
+        if self._check_if_answer_reached(token):
+            message = self._construct_message(StreamingJSONResponse(token=token))
+            await self.send(message)
```

### Comparing `lanarky-0.6.4/lanarky/callbacks/base.py` & `lanarky-0.6.5/lanarky/callbacks/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,72 @@
+import json
 from abc import abstractmethod
 from typing import Any
 
 from fastapi import WebSocket
 from langchain.callbacks.base import AsyncCallbackHandler
 from pydantic import BaseModel, Field
 from starlette.types import Message, Send
 
-from lanarky.schemas import WebsocketResponse
+from lanarky.schemas import StreamingJSONResponse, WebsocketResponse
 
 
 class AsyncLanarkyCallback(AsyncCallbackHandler, BaseModel):
     """Async Callback handler for FastAPI StreamingResponse."""
 
     @property
     def always_verbose(self) -> bool:
         """Whether to call verbose callbacks even if verbose is False."""
         return True
 
     class Config:
         arbitrary_types_allowed = True
 
     @abstractmethod
-    def _construct_message(self, message: str) -> Any:  # pragma: no cover
+    def _construct_message(self, content: Any) -> Any:  # pragma: no cover
         """Construct a Message from a string."""
         pass
 
 
 class AsyncStreamingResponseCallback(AsyncLanarkyCallback):
-    """Async Callback handler for FastAPI StreamingResponse."""
+    """Async Callback handler for StreamingResponse."""
 
     send: Send = Field(...)
 
-    def _construct_message(self, message_str: str) -> Message:
+    def _construct_message(self, content: str) -> Message:
         """Construct a Message from a string."""
         return {
             "type": "http.response.body",
-            "body": message_str.encode("utf-8"),
+            "body": content.encode("utf-8"),
             "more_body": True,
         }
 
 
 class AsyncWebsocketCallback(AsyncLanarkyCallback):
-    """Async Callback handler for FastAPI websocket connection."""
+    """Async Callback handler for WebsocketConnection."""
 
     websocket: WebSocket = Field(...)
     response: WebsocketResponse = Field(...)
 
-    def _construct_message(self, message_str: str) -> dict:
+    def _construct_message(self, content: str) -> dict:
         """Construct a WebsocketResponse from a string."""
-        return {**self.response.dict(), **{"message": message_str.encode("utf-8")}}
+        return {**self.response.dict(), **{"message": content.encode("utf-8")}}
+
+
+class AsyncStreamingJSONResponseCallback(AsyncStreamingResponseCallback):
+    """Async Callback handler for StreamingJSONResponse."""
+
+    send: Send = Field(...)
+
+    def _construct_message(self, content: StreamingJSONResponse) -> Message:
+        """Construct a Message from a dictionary."""
+        return {
+            "type": "http.response.body",
+            "body": json.dumps(
+                content.dict(),
+                ensure_ascii=False,
+                allow_nan=False,
+                indent=None,
+                separators=(",", ":"),
+            ).encode("utf-8"),
+            "more_body": True,
+        }
```

### Comparing `lanarky-0.6.4/lanarky/callbacks/llm.py` & `lanarky-0.6.5/lanarky/callbacks/llm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 from typing import Any
 
-from lanarky.register import register_streaming_callback, register_websocket_callback
+from lanarky.register import (
+    register_streaming_callback,
+    register_streaming_json_callback,
+    register_websocket_callback,
+)
+from lanarky.schemas import StreamingJSONResponse
+
+from .base import (
+    AsyncStreamingJSONResponseCallback,
+    AsyncStreamingResponseCallback,
+    AsyncWebsocketCallback,
+)
 
-from .base import AsyncStreamingResponseCallback, AsyncWebsocketCallback
+SUPPORTED_CHAINS = ["LLMChain", "ConversationChain"]
 
 
-@register_streaming_callback("LLMChain")
+@register_streaming_callback(SUPPORTED_CHAINS)
 class AsyncLLMChainStreamingCallback(AsyncStreamingResponseCallback):
     """AsyncStreamingResponseCallback handler for LLMChain."""
 
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         """Run on new LLM token. Only available when streaming is enabled."""
         message = self._construct_message(token)
         await self.send(message)
 
 
-@register_websocket_callback("LLMChain")
+@register_websocket_callback(SUPPORTED_CHAINS)
 class AsyncLLMChainWebsocketCallback(AsyncWebsocketCallback):
     """AsyncWebsocketCallback handler for LLMChain."""
 
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         """Run on new LLM token. Only available when streaming is enabled."""
         message = self._construct_message(token)
         await self.websocket.send_json(message)
 
 
-@register_streaming_callback("ConversationChain")
-class AsyncConversationChainStreamingCallback(AsyncLLMChainStreamingCallback):
-    """AsyncStreamingResponseCallback handler for ConversationChain."""
+@register_streaming_json_callback(SUPPORTED_CHAINS)
+class AsyncLLMChainStreamingJSONCallback(AsyncStreamingJSONResponseCallback):
+    """AsyncStreamingJSONResponseCallback handler for LLMChain."""
 
-    pass
-
-
-@register_websocket_callback("ConversationChain")
-class AsyncConversationChainWebsocketCallback(AsyncLLMChainWebsocketCallback):
-    """AsyncWebsocketCallback handler for ConversationChain."""
-
-    pass
+    async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
+        """Run on new LLM token. Only available when streaming is enabled."""
+        message = self._construct_message(StreamingJSONResponse(token=token))
+        await self.send(message)
```

### Comparing `lanarky-0.6.4/lanarky/responses/streaming.py` & `lanarky-0.6.5/lanarky/responses/streaming.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Awaitable, Callable, Optional, Union
 
 from fastapi.responses import StreamingResponse as _StreamingResponse
 from langchain.chains.base import Chain
 from starlette.background import BackgroundTask
 from starlette.types import Send
 
-from lanarky.callbacks import get_streaming_callback
+from lanarky.callbacks import get_streaming_callback, get_streaming_json_callback
 
 
 class StreamingResponse(_StreamingResponse):
     """StreamingResponse class wrapper for langchain chains."""
 
     def __init__(
         self,
@@ -52,33 +52,43 @@
             )
             return
 
         await send({"type": "http.response.body", "body": b"", "more_body": False})
 
     @staticmethod
     def _create_chain_executor(
-        chain: Chain, inputs: Union[dict[str, Any], Any], **callback_kwargs
+        chain: Chain,
+        inputs: Union[dict[str, Any], Any],
+        as_json: bool = False,
+        **callback_kwargs,
     ) -> Callable[[Send], Awaitable[Any]]:
+        get_callback_fn = (
+            get_streaming_json_callback if as_json else get_streaming_callback
+        )
+
         async def wrapper(send: Send):
             return await chain.acall(
                 inputs=inputs,
-                callbacks=[get_streaming_callback(chain, send=send, **callback_kwargs)],
+                callbacks=[get_callback_fn(chain, send=send, **callback_kwargs)],
             )
 
         return wrapper
 
     @classmethod
     def from_chain(
         cls,
         chain: Chain,
         inputs: Union[dict[str, Any], Any],
+        as_json: bool = False,
         background: Optional[BackgroundTask] = None,
         callback_kwargs: dict[str, Any] = {},
         **kwargs: Any,
     ) -> "StreamingResponse":
-        chain_executor = cls._create_chain_executor(chain, inputs, **callback_kwargs)
+        chain_executor = cls._create_chain_executor(
+            chain, inputs, as_json, **callback_kwargs
+        )
 
         return cls(
             chain_executor=chain_executor,
             background=background,
             **kwargs,
         )
```

### Comparing `lanarky-0.6.4/lanarky/schemas.py` & `lanarky-0.6.5/lanarky/schemas.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Union
+from typing import Any, Union
 
 from pydantic import BaseModel
 
 
 class Sender(str, Enum):
     BOT = "bot"
     HUMAN = "human"
@@ -25,7 +25,15 @@
 class WebsocketResponse(BaseModel):
     sender: Sender
     message: Union[Message, str]
     message_type: MessageType
 
     class Config:
         use_enum_values = True
+
+
+class StreamingJSONResponse(BaseModel):
+    token: str = ""
+
+
+class BaseRetrievalQAStreamingJSONResponse(StreamingJSONResponse):
+    source_documents: list[dict[str, Any]]
```

### Comparing `lanarky-0.6.4/lanarky/testing/gradio.py` & `lanarky-0.6.5/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.4/lanarky/websockets/base.py` & `lanarky-0.6.5/lanarky/websockets/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.4/pyproject.toml` & `lanarky-0.6.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.6.4"
+version = "0.6.5"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = ">=0.95.2"
-langchain = ">=0.0.175"
+langchain = ">=0.0.178"
 urllib3 = "<=1.26.15"  # added due to poetry errors
 python-dotenv = "^1.0.0"
+typing-extensions = "4.5.0"  # added due to https://github.com/hwchase17/langchain/issues/5113
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2023.3.27"
 sphinx-autobuild = "^2021.3.14"
+myst-parser = "^1.0.0"
+sphinx-copybutton = "^0.5.2"
+autodoc-pydantic = "^1.8.0"
 
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.21.0"
 coveralls = "^3.3.1"
```

### Comparing `lanarky-0.6.4/PKG-INFO` & `lanarky-0.6.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.6.4
+Version: 0.6.5
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.2)
-Requires-Dist: langchain (>=0.0.175)
+Requires-Dist: langchain (>=0.0.178)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: typing-extensions (==4.5.0)
 Requires-Dist: urllib3 (<=1.26.15)
 Project-URL: Repository, https://github.com/ajndkr/lanarky
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/ajndkr/lanarky/main/assets/logo.png" alt="lanarky-logo" width="150">
```

