# Comparing `tmp/fastapi_async_langchain-0.3.3.tar.gz` & `tmp/fastapi_async_langchain-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.3.3.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.4.0.tar", max compression
```

## Comparing `fastapi_async_langchain-0.3.3.tar` & `fastapi_async_langchain-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-04-27 08:16:52.334951 fastapi_async_langchain-0.3.3/LICENSE
--rw-r--r--   0        0        0     1574 2023-04-27 08:16:52.334951 fastapi_async_langchain-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0      194 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      648 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/callbacks/base.py
--rw-r--r--   0        0        0      733 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0      171 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/__init__.py
--rw-r--r--   0        0        0     1839 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/base.py
--rw-r--r--   0        0        0     1183 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/llm.py
--rw-r--r--   0        0        0     1512 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/retrieval_qa.py
--rw-r--r--   0        0        0      481 2023-04-27 08:16:52.506951 fastapi_async_langchain-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-02 17:40:12.617572 fastapi_async_langchain-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1713 2023-05-02 17:40:12.617572 fastapi_async_langchain-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 17:40:12.821570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-02 17:40:12.821570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      273 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/streaming/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/streaming/base.py
+-rw-r--r--   0        0        0      906 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/streaming/retrieval_qa.py
+-rw-r--r--   0        0        0      257 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/websocket/__init__.py
+-rw-r--r--   0        0        0      971 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/websocket/base.py
+-rw-r--r--   0        0        0     1172 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/websocket/retrieval_qa.py
+-rw-r--r--   0        0        0      171 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/__init__.py
+-rw-r--r--   0        0        0     2502 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/base.py
+-rw-r--r--   0        0        0     1295 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/llm.py
+-rw-r--r--   0        0        0     2225 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/retrieval_qa.py
+-rw-r--r--   0        0        0      536 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/testing/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/testing/settings.py
+-rw-r--r--   0        0        0      281 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/__init__.py
+-rw-r--r--   0        0        0     2907 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/base.py
+-rw-r--r--   0        0        0     1379 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/llm.py
+-rw-r--r--   0        0        0     2370 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/retrieval_qa.py
+-rw-r--r--   0        0        0      481 2023-05-02 17:40:12.825570 fastapi_async_langchain-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.4.0/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.3.3/LICENSE` & `fastapi_async_langchain-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.3.3/README.md` & `fastapi_async_langchain-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
 
-FastAPI async components for streaming LLM chains.
+Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with [FastAPI](https://github.com/tiangolo/fastapi).
 
-## Installation
+## :rocket: Features
+
+- supports token streaming over HTTP and Websocket
+- supports multiple langchain `Chain` types (ongoing...)
+- simple gradio chatbot UI for fast prototyping
+
+## 💾 Installation
 
 The library is available on PyPI and can be installed via `pip`.
 
 ```bash
 pip install fastapi-async-langchain
 ```
 
-## Demo Example
+## 🎯 Demo Examples
+
+See [`examples/`](examples/README.md) for list of available demo examples.
 
-See [Demo](demo/README.md) for setup instructions and usage of the demo FastAPI application.
+![demo](assets/demo.gif)
 
-## Contributing
+## 🤝 Contributing
 
 [![Code check](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/code-check.yaml/badge.svg)](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/code-check.yaml)
 [![Publish](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/publish.yaml/badge.svg)](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/publish.yaml)
 
 Contributions are more than welcome! If you have an idea for a new feature or want to help improve fastapi-async-langchain, please create an issue or submit a pull request
 on [GitHub](https://github.com/ajndkr/fastapi-async-langchain).
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md) for more information.
 
-## License
+## ⚖️ License
 
 The library is released under the [MIT License](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE).
-
-## Credits:
-
-- [ninely/main.py](https://gist.github.com/ninely/88485b2e265d852d3feb8bd115065b1a)
-- https://github.com/hwchase17/langchain/discussions/1706
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fastapi_async_langchain-0.3.3/fastapi_async_langchain/callbacks/base.py` & `fastapi_async_langchain-0.4.0/fastapi_async_langchain/callbacks/streaming/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from typing import Any
 
 from langchain.callbacks.base import AsyncCallbackHandler
 from pydantic import BaseModel, Field
 from starlette.types import Send
 
 
-class AsyncFastApiStreamingCallback(AsyncCallbackHandler, BaseModel):
+class AsyncStreamingResponseCallback(AsyncCallbackHandler, BaseModel):
     """Async Callback handler for FastAPI StreamingResponse."""
 
     send: Send = Field(...)
 
     @property
     def always_verbose(self) -> bool:
         """Whether to call verbose callbacks even if verbose is False."""
         return True
 
+
+class AsyncLLMChainStreamingCallback(AsyncStreamingResponseCallback):
+    """AsyncStreamingResponseCallback handler for LLMChain."""
+
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         """Run on new LLM token. Only available when streaming is enabled."""
         await self.send(token)
```

### Comparing `fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/llm.py` & `fastapi_async_langchain-0.4.0/fastapi_async_langchain/responses/llm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from typing import Any, Dict, Union
+from typing import Any, Awaitable, Callable, Dict, Union
 
 from langchain import LLMChain
 from langchain.callbacks import AsyncCallbackManager
 from starlette.types import Send
 
-from ..callbacks import AsyncFastApiStreamingCallback
+from ..callbacks import AsyncLLMChainStreamingCallback, AsyncStreamingResponseCallback
 from .base import BaseLangchainStreamingResponse
 
 
 class LLMChainStreamingResponse(BaseLangchainStreamingResponse):
     """BaseLangchainStreamingResponse class wrapper for LLMChain instances."""
 
     @staticmethod
-    def chain_wrapper_fn(chain: LLMChain, inputs: Union[Dict[str, Any], Any]):
+    def _create_chain_executor(
+        chain: LLMChain, inputs: Union[Dict[str, Any], Any]
+    ) -> Callable[[Send], Awaitable[Any]]:
         async def wrapper(send: Send):
             if not isinstance(chain.llm.callback_manager, AsyncCallbackManager):
                 raise TypeError(
                     "llm.callback_manager must be an instance of AsyncCallbackManager"
                 )
             for handler in chain.llm.callback_manager.handlers:
-                if isinstance(handler, AsyncFastApiStreamingCallback):
+                if isinstance(handler, AsyncStreamingResponseCallback):
                     chain.llm.callback_manager.remove_handler(handler)
                     break
             chain.llm.callback_manager.add_handler(
-                AsyncFastApiStreamingCallback(send=send)
+                AsyncLLMChainStreamingCallback(send=send)
             )
             return await chain.arun(inputs)
 
         return wrapper
```

### Comparing `fastapi_async_langchain-0.3.3/fastapi_async_langchain/responses/retrieval_qa.py` & `fastapi_async_langchain-0.4.0/fastapi_async_langchain/websockets/retrieval_qa.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,61 @@
-from typing import Any, Dict, Union
+from typing import Any, Awaitable, Callable
 
+from fastapi import WebSocket
 from langchain.callbacks import AsyncCallbackManager
 from langchain.chains.retrieval_qa.base import BaseRetrievalQA
-from starlette.types import Send
 
-from ..callbacks import RetrievalQAFastApiStreamingCallback
-from .base import BaseLangchainStreamingResponse
+from ..callbacks import (
+    AsyncLLMChainWebsocketCallback,
+    AsyncRetrievalQAWebsocketCallback,
+    AsyncWebsocketCallback,
+)
+from ..schemas import WebsocketResponse
+from .base import BaseLangchainWebsocketConnection
 
 
-class RetrievalQAStreamingResponse(BaseLangchainStreamingResponse):
-    """BaseLangchainStreamingResponse class wrapper for BaseRetrievalQA instances."""
+class RetrievalQAWebsocketConnection(BaseLangchainWebsocketConnection):
+    """BaseLangchainWebsocketConnection class wrapper for BaseRetrievalQA instances."""
 
     @staticmethod
-    def chain_wrapper_fn(chain: BaseRetrievalQA, inputs: Union[Dict[str, Any], Any]):
-        async def wrapper(send: Send):
+    def _create_chain_executor(
+        chain: BaseRetrievalQA,
+        websocket: WebSocket,
+        response: WebsocketResponse,
+    ) -> Callable[[], Awaitable[Any]]:
+        async def wrapper(user_message: str):
             if not isinstance(
                 chain.combine_documents_chain.llm_chain.llm.callback_manager,
                 AsyncCallbackManager,
             ):
                 raise TypeError(
                     "llm.callback_manager must be an instance of AsyncCallbackManager"
                 )
             for (
                 handler
             ) in chain.combine_documents_chain.llm_chain.llm.callback_manager.handlers:
-                if isinstance(handler, RetrievalQAFastApiStreamingCallback):
+                if isinstance(handler, AsyncWebsocketCallback):
                     chain.combine_documents_chain.llm_chain.llm.callback_manager.remove_handler(
                         handler
                     )
                     break
             chain.combine_documents_chain.llm_chain.llm.callback_manager.add_handler(
-                RetrievalQAFastApiStreamingCallback(send=send)
+                AsyncLLMChainWebsocketCallback(websocket=websocket, response=response)
             )
-            return await chain.acall(inputs)
+
+            if not isinstance(chain.callback_manager, AsyncCallbackManager):
+                raise TypeError(
+                    "chain.callback_manager must be an instance of AsyncCallbackManager"
+                )
+            for handler in chain.callback_manager.handlers:
+                if isinstance(handler, AsyncWebsocketCallback):
+                    chain.callback_manager.remove_handler(handler)
+                    break
+            chain.callback_manager.add_handler(
+                AsyncRetrievalQAWebsocketCallback(
+                    websocket=websocket, response=response
+                )
+            )
+
+            return await chain.acall(user_message)
 
         return wrapper
```

### Comparing `fastapi_async_langchain-0.3.3/PKG-INFO` & `fastapi_async_langchain-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.3.3
+Version: 0.4.0
 Summary: FastAPI async components for streaming LLM chains.
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,40 +14,43 @@
 Description-Content-Type: text/markdown
 
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
 
-FastAPI async components for streaming LLM chains.
+Ship production-ready [LangChain](https://github.com/hwchase17/langchain) projects with [FastAPI](https://github.com/tiangolo/fastapi).
 
-## Installation
+## :rocket: Features
+
+- supports token streaming over HTTP and Websocket
+- supports multiple langchain `Chain` types (ongoing...)
+- simple gradio chatbot UI for fast prototyping
+
+## 💾 Installation
 
 The library is available on PyPI and can be installed via `pip`.
 
 ```bash
 pip install fastapi-async-langchain
 ```
 
-## Demo Example
+## 🎯 Demo Examples
+
+See [`examples/`](examples/README.md) for list of available demo examples.
 
-See [Demo](demo/README.md) for setup instructions and usage of the demo FastAPI application.
+![demo](assets/demo.gif)
 
-## Contributing
+## 🤝 Contributing
 
 [![Code check](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/code-check.yaml/badge.svg)](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/code-check.yaml)
 [![Publish](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/publish.yaml/badge.svg)](https://github.com/ajndkr/fastapi-async-langchain/actions/workflows/publish.yaml)
 
 Contributions are more than welcome! If you have an idea for a new feature or want to help improve fastapi-async-langchain, please create an issue or submit a pull request
 on [GitHub](https://github.com/ajndkr/fastapi-async-langchain).
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md) for more information.
 
-## License
+## ⚖️ License
 
 The library is released under the [MIT License](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE).
 
-## Credits:
-
-- [ninely/main.py](https://gist.github.com/ninely/88485b2e265d852d3feb8bd115065b1a)
-- https://github.com/hwchase17/langchain/discussions/1706
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

