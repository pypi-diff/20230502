# Comparing `tmp/promptwatch-0.0.2.tar.gz` & `tmp/promptwatch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.0.2.tar", last modified: Mon Apr 24 20:11:04 2023, max compression
+gzip compressed data, was "promptwatch-0.0.3.tar", last modified: Tue May  2 18:40:25 2023, max compression
```

## Comparing `promptwatch-0.0.2.tar` & `promptwatch-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 20:11:04.342497 promptwatch-0.0.2/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-04-24 20:11:04.342336 promptwatch-0.0.2/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3781 2023-04-21 05:55:12.000000 promptwatch-0.0.2/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.2/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-04-24 20:11:04.342541 promptwatch-0.0.2/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1137 2023-04-24 13:18:48.000000 promptwatch-0.0.2/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 20:11:04.338345 promptwatch-0.0.2/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 20:11:04.340617 promptwatch-0.0.2/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      206 2023-04-24 20:10:51.000000 promptwatch-0.0.2/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2284 2023-04-22 17:25:04.000000 promptwatch-0.0.2/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.2/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1506 2023-04-22 10:56:22.000000 promptwatch-0.0.2/src/promptwatch/decorators.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16765 2023-04-22 20:40:51.000000 promptwatch-0.0.2/src/promptwatch/langchain_handler.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15224 2023-04-24 20:09:25.000000 promptwatch-0.0.2/src/promptwatch/promptwatch_context.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      559 2023-04-22 10:49:03.000000 promptwatch-0.0.2/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 20:11:04.342121 promptwatch-0.0.2/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      480 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.2/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       19 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.639824 promptwatch-0.0.3/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-05-02 18:40:25.639650 promptwatch-0.0.3/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3781 2023-04-21 05:55:12.000000 promptwatch-0.0.3/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.3/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-02 18:40:25.639868 promptwatch-0.0.3/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 11:55:00.000000 promptwatch-0.0.3/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.632914 promptwatch-0.0.3/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.637036 promptwatch-0.0.3/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-02 18:40:10.000000 promptwatch-0.0.3/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11830 2023-05-02 08:57:06.000000 promptwatch-0.0.3/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 11:55:00.000000 promptwatch-0.0.3/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.3/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1912 2023-05-02 11:55:00.000000 promptwatch-0.0.3/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.638902 promptwatch-0.0.3/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-02 10:03:23.000000 promptwatch-0.0.3/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    34206 2023-05-02 18:26:30.000000 promptwatch-0.0.3/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13397 2023-05-02 11:55:00.000000 promptwatch-0.0.3/src/promptwatch/promptwatch_context.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 17:20:28.000000 promptwatch-0.0.3/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-02 18:40:25.638362 promptwatch-0.0.3/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.3/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-02 18:40:25.000000 promptwatch-0.0.3/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.0.2/PKG-INFO` & `promptwatch-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.2
+Version: 0.0.3
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.2/README.md` & `promptwatch-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.2/setup.py` & `promptwatch-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,10 +20,11 @@
                 keywords='promptwatch prompt monitoring',
 
                 classifiers=[
                 ],
                 python_requires='>=3.8',
                 install_requires=[
                     "langchain",
-                    "pydantic"
+                    "pydantic",
+                    "tiktoken"
                 ]
                 )
```

### Comparing `promptwatch-0.0.2/src/promptwatch/data_model.py` & `promptwatch-0.0.3/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.2/src/promptwatch/decorators.py` & `promptwatch-0.0.3/src/promptwatch/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 from promptwatch import PromptWatch
 from promptwatch import ChainSequence
-from .utils import _find_the_caller_in_the_stack
-
+from .utils import find_the_caller_in_the_stack
+from typing import Callable
 from langchain.chains import LLMChain
 
 
 FORMATTED_PROMPT_CONTEXT_KEY = "formatted_prompt"
 TEMPLATE_NAME_CONTEXT_KEY = "template_name"
 
 def format_prompt_decorator(template_name:str):
     def decorator_function(func):
         def wrapper(*args, **kwargs):
             
 
             #skipping the first argument because it is self
-            result = func(*args[1:], **kwargs)
+            result = func(*args, **kwargs)
             pw = PromptWatch.get_active_instance()
             if pw is not None:
                 _self=args[0]
                 pw.add_context(FORMATTED_PROMPT_CONTEXT_KEY, result)
                 pw.add_context(TEMPLATE_NAME_CONTEXT_KEY, template_name)
                 if pw.current_activity and hasattr(pw, "langchain_callback_handler")and isinstance(pw.current_activity,ChainSequence) and pw.current_activity.sequence_type=="LLMChain":
                     # if current_llm_chain is None, we want to fill it in. Probably running in async mode, so it was not accessible from the callback handler
-                    if pw.langchain_callback_handler.current_llm_chain is None:
-                        llm_chain = _find_the_caller_in_the_stack(type=LLMChain)
+                    if pw.langchain.langchain_callback_handler.current_llm_chain is None:
+                        llm_chain = find_the_caller_in_the_stack(type=LLMChain)
                         if llm_chain:
-                            pw.langchain_callback_handler.current_llm_chain =  llm_chain
+                            pw.langchain.langchain_callback_handler.current_llm_chain =  llm_chain
                         
 
                 
             return result
         return wrapper
-    return decorator_function
+    return decorator_function
+
+
+def cached_call(cache_handler:Callable):
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            cached_response = cache_handler(*args, **kwargs)
+            if cached_response is not None:
+                return cached_response
+            else:        
+                return func(*args, **kwargs)
+        return wrapper
+    return decorator
```

### Comparing `promptwatch-0.0.2/src/promptwatch/promptwatch_context.py` & `promptwatch-0.0.3/src/promptwatch/promptwatch_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 import re
 from .data_model import (ActivityBase, Log, Session)
 import logging
 from .data_model import Session, ActivityBase,  ChainSequence, Log, Answer, Action, Question, RetrievedDocuments, DocumentSnippet
 from .client import Client
 from uuid import uuid4
 import types
-
+from .utils import wrap_a_method, classproperty
+from .caching import PromptWatchCacheManager
 
 
 
 
 class PromptWatch():
     _thread_local = threading.local()
+    prompt_template_register_cache={}
 
     def __init__(self, session_id: Optional[str] = None, tracking_project: Optional[str] = None, tracking_tenant: Optional[str] = None, api_key: Optional[str] = None):
         """
         PromptWatch context to track all the activities inside your LLM chain
 
         ## Parameters:
 
@@ -56,55 +58,47 @@
                 GREEN = '\033[32m'
                 RESET = '\033[0m'
                 print(f"{GREEN}You are using a temporary API key. Do not use in production.")
                 print(f"Visit the the detail of this session at https://www.promptwatch.io/sessions?temp-api-key={api_key} {RESET}")
                 
 
 
-
         self.client = Client(api_key=api_key)
         
         
         self.chain_hierarchy:List[ChainSequence]=[]
         self.pending_session_save=True
         self.pending_stack:List[ActivityBase]=[]
-        self.prompt_template_register_cache={}
+        
         self.current_session=None
         self.context={}
+        self._cache_manager = PromptWatchCacheManager(self)
+        self.tracing_handlers={}
 
+    @property
+    def caching(self):
+        return self._cache_manager
 
-    def use_langchain_tracing(self, langchain_callback_manager=None)->PromptWatch:
-        """ Enable langchain tracing
-
-        Args:
-            langchain_callback_manager (langchain.callbacks.base.BaseCallbackManager, optional):  If using custom callback manager, pass it here. Otherwise, default callback manager will be used. Defaults to None.
-
-        """
-
-        from langchain.callbacks import get_callback_manager
-        from promptwatch.langchain_handler import LangChainCallbackHandler
-
-        self.langchain_callback_handler = LangChainCallbackHandler(self)
-        langchain_callback_manager = langchain_callback_manager or get_callback_manager()
-        langchain_callback_manager.add_handler(self.langchain_callback_handler)
-
-        return self
+    @property
+    def langchain(self):
+        if not hasattr(self,"_langchain"):
+            from .langchain.langchain_support import LangChainSupport
+            self._langchain = LangChainSupport(self)
+            
+        
+        return self._langchain
+    
 
-    def get_langchain_callback_handler(self):
-        if not ( hasattr(self, "langchain_callback_handler") and self.langchain_callback_handler ):
-            from promptwatch.langchain_handler import LangChainCallbackHandler
-            self.langchain_callback_handler = LangChainCallbackHandler(self)
-        return self.langchain_callback_handler
 
     def __enter__(self):
         self._thread_local.active_instance = self
 
-        if not ( hasattr(self, "langchain_callback_handler") and self.langchain_callback_handler ):
+        if not self.tracing_handlers:
             # lets enable tracing by default
-            self.use_langchain_tracing()
+            self.langchain.init_tracing()
             #raise Exception("PromptWatch: LangChain callback handler is not set. Please call langchain_tracing() before entering the context.")
 
         if not self.current_session:
             self.start_session()
         
         
 
@@ -209,32 +203,18 @@
             my_chain("The quick brown fox jumped over")
         ```
 
         ### Registering chat messages template (completion)
         ...
 
         """
-        if not template_name:
-            raise Exception("template_name can't be empty")
-        if re.search(r"\s", template_name):
-            raise Exception("template_name can't contain white spaces")
-        if len(template_name)>126:
-            raise Exception("template_name must be less than 126 characters")
-        
-        converted_template =  self.langchain_callback_handler.create_prompt_template_description(prompt_template, template_name=template_name, template_version=version)
-        from .decorators import format_prompt_decorator
-        decorator_func = format_prompt_decorator(template_name)
-        
-        # need to go around pydantic restrictions on __setattr__  by using __dict__ directly
-        prompt_template.__dict__["format_prompt"] =  types.MethodType(decorator_func(prompt_template.format_prompt), prompt_template)
-        # we need to mark the prompt template somehow... keeping just the reference doesn't work since pydantic is creating copy of it when passed to the constructor
-        # that is why we add special field __template_name__ into it... also skipping setattr() since that might be blocked by pydantic as well (depending on the configuration)
-        prompt_template.__dict__["__template_name__"]=template_name
-
-        self.prompt_template_register_cache[template_name] = converted_template
+        
+        from .langchain.langchain_support import register_prompt_template
+        register_prompt_template(template_name,prompt_template, version=version)
+        
 
 
     def add_context(self, key:str, value:Any):
         self.context[key]=(self.current_activity ,value)
     
     def get_context(self, key:str) -> Any:
         if key in self.context:
```

### Comparing `promptwatch-0.0.2/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.0.3/src/promptwatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.2
+Version: 0.0.3
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

