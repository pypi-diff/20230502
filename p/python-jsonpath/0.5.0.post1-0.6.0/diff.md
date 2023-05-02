# Comparing `tmp/python_jsonpath-0.5.0.post1.tar.gz` & `tmp/python_jsonpath-0.6.0.tar.gz`

## Comparing `python_jsonpath-0.5.0.post1.tar` & `python_jsonpath-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/__about__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/__init__.py
--rw-r--r--   0        0        0    14434 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/env.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/exceptions.py
--rw-r--r--   0        0        0    12325 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/filter.py
--rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/lex.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/match.py
--rw-r--r--   0        0        0    19148 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/parse.py
--rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/py.typed
--rw-r--r--   0        0        0    22016 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/selectors.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/stream.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/token.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/function_extensions/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/function_extensions/arguments.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/function_extensions/keys.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/function_extensions/length.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/function_extensions/match.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/function_extensions/search.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/jsonpath/function_extensions/value.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/LICENSE.txt
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/README.md
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/pyproject.toml
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 python_jsonpath-0.5.0.post1/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/__about__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/__init__.py
+-rw-r--r--   0        0        0    15062 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/env.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/exceptions.py
+-rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/filter.py
+-rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/lex.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/match.py
+-rw-r--r--   0        0        0    20411 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/parse.py
+-rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/py.typed
+-rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/selectors.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/stream.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/token.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/arguments.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/count.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/is_instance.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/keys.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/length.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/match.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/search.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/typeof.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/value.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/README.md
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/PKG-INFO
```

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/__init__.py` & `python_jsonpath-0.6.0/jsonpath/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/env.py` & `python_jsonpath-0.6.0/jsonpath/env.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,54 +51,60 @@
 
     ## Environment customization
 
     Environment customization is achieved by subclassing `JSONPathEnvironment`
     and overriding class attributes and/or methods. Some of these
     customizations include:
 
-    - Changing the root (`$`), self (`@`) or filter context (`#`) token with
+    - Changing the root (`$`), self (`@`) or filter context (`_`) token with
       class attributes `root_token`, `self_token` and `filter_context_token`.
     - Registering a custom lexer or parser with the class attributes
       `lexer_class` or `parser_class`. `lexer_class` must be a subclass of
       [`Lexer`]() and `parser_class` must be a subclass of [`Parser`]().
     - Setup built-in function extensions by overriding
       `setup_function_extensions()`
     - Hook in to mapping and sequence item getting by overriding `getitem()`.
     - Change filter comparison operator behavior by overriding `compare()`.
 
     ## Class attributes
 
     Attributes:
-        filter_context_token: The pattern used to select extra filter context data.
-            Defaults to `"#"`.
-        intersection_token: The pattern used as the intersection operator. Defaults
-            to `"$"`.
+        filter_context_token (str): The pattern used to select extra filter context
+            data. Defaults to `"_"`.
+        intersection_token (str): The pattern used as the intersection operator.
+            Defaults to `"$"`.
+        key_token (str): The pattern used to identify the current key or index when
+            filtering a, mapping or sequence. Defaults to `"#"`.
+        keys_selector_token (str): The pattern used as the "keys" selector. Defaults to
+            `"~"`.
         lexer_class: The lexer to use when tokenizing path strings.
-        max_int_index: The maximum integer allowed when selecting array items by index.
-            Defaults to `(2**53) - 1`.
-        min_int_index: The minimum integer allowed when selecting array items by index.
-            Defaults to `-(2**53) + 1`.
+        max_int_index (int): The maximum integer allowed when selecting array items by
+            index. Defaults to `(2**53) - 1`.
+        min_int_index (int): The minimum integer allowed when selecting array items by
+            index. Defaults to `-(2**53) + 1`.
         parser_class: The parser to use when parsing tokens from the lexer.
-        root_token: The pattern used to select the root node in a JSON document.
+        root_token (str): The pattern used to select the root node in a JSON document.
             Defaults to `"$"`.
-        self_token: The pattern used to select the current node in a JSON document.
-            Defaults to `"@"`
-        union_token: The pattern used as the union operator. Defaults to `"|"`.
+        self_token (str): The pattern used to select the current node in a JSON
+            document. Defaults to `"@"`
+        union_token (str): The pattern used as the union operator. Defaults to `"|"`.
     """
 
     # These should be unescaped strings. `re.escape` will be called
     # on them automatically when compiling lexer rules.
-    intersection_token: str = "&"
-    root_token: str = "$"
-    self_token: str = "@"
-    union_token: str = "|"
-    filter_context_token: str = "#"
+    filter_context_token = "_"
+    intersection_token = "&"
+    key_token = "#"
+    keys_selector_token = "~"
+    root_token = "$"
+    self_token = "@"
+    union_token = "|"
 
-    max_int_index: int = (2**53) - 1
-    min_int_index: int = -(2**53) + 1
+    max_int_index = (2**53) - 1
+    min_int_index = -(2**53) + 1
 
     # Override these to customize path tokenization and parsing.
     lexer_class: Type[Lexer] = Lexer
     parser_class: Type[Parser] = Parser
 
     def __init__(self) -> None:  # noqa: D107
         self.lexer: Lexer = self.lexer_class(env=self)
@@ -242,18 +248,22 @@
             data, filter_context=filter_context
         )
 
     def setup_function_extensions(self) -> None:
         """Initialize function extensions."""
         self.function_extensions["keys"] = function_extensions.keys
         self.function_extensions["length"] = function_extensions.length
-        self.function_extensions["count"] = function_extensions.length
+        self.function_extensions["count"] = function_extensions.Count()
         self.function_extensions["match"] = function_extensions.Match()
         self.function_extensions["search"] = function_extensions.Search()
         self.function_extensions["value"] = function_extensions.value
+        self.function_extensions["isinstance"] = function_extensions.IsInstance()
+        self.function_extensions["is"] = self.function_extensions["isinstance"]
+        self.function_extensions["typeof"] = function_extensions.TypeOf()
+        self.function_extensions["type"] = self.function_extensions["typeof"]
 
     def validate_function_extension_signature(
         self, token: Token, args: List[Any]
     ) -> List[Any]:
         """Compile-time validation of function extension arguments.
 
         The IETF JSONPath draft requires us to reject paths that use filter
```

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/exceptions.py` & `python_jsonpath-0.6.0/jsonpath/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/filter.py` & `python_jsonpath-0.6.0/jsonpath/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,15 @@
 
 
 class FilterContextPath(Path):
     """A JSONPath starting at the root of any extra context data."""
 
     def __str__(self) -> str:
         path_repr = str(self.path)
-        return "#" + path_repr[1:]
+        return "_" + path_repr[1:]
 
     def evaluate(self, context: FilterContext) -> object:
         matches = self.path.findall(context.extra_context)
         if not matches:
             return UNDEFINED
         if len(matches) == 1:
             return matches[0]
@@ -445,7 +445,24 @@
     async def evaluate_async(self, context: FilterContext) -> object:
         try:
             func = context.env.function_extensions[self.name]
         except KeyError:
             return UNDEFINED
         args = [await arg.evaluate_async(context) for arg in self.args]
         return func(*args)
+
+
+class CurrentKey(FilterExpression):
+    """The key/property or index associated with the current object."""
+
+    __slots__ = ()
+
+    def evaluate(self, context: FilterContext) -> object:
+        if context.current_key is None:
+            return UNDEFINED
+        return context.current_key
+
+    async def evaluate_async(self, context: FilterContext) -> object:
+        return self.evaluate(context)
+
+
+CURRENT_KEY = CurrentKey()
```

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/lex.py` & `python_jsonpath-0.6.0/jsonpath/lex.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 from .token import TOKEN_GE
 from .token import TOKEN_GT
 from .token import TOKEN_ILLEGAL
 from .token import TOKEN_IN
 from .token import TOKEN_INDEX
 from .token import TOKEN_INT
 from .token import TOKEN_INTERSECTION
+from .token import TOKEN_KEY
+from .token import TOKEN_KEYS
 from .token import TOKEN_LE
 from .token import TOKEN_LG
 from .token import TOKEN_LIST_SLICE
 from .token import TOKEN_LIST_START
 from .token import TOKEN_LPAREN
 from .token import TOKEN_LT
 from .token import TOKEN_MISSING
@@ -140,17 +142,19 @@
             (TOKEN_FLOAT, r"-?\d+\.\d*(?:e[+-]?\d+)?"),
             (TOKEN_INT, r"-?\d+(?:e[+\-]?\d+)?\b"),
             (TOKEN_DDOT, r"\.\."),
             (TOKEN_AND, self.bool_and_pattern),
             (TOKEN_OR, self.bool_or_pattern),
             (TOKEN_ROOT, re.escape(self.env.root_token)),
             (TOKEN_SELF, re.escape(self.env.self_token)),
+            (TOKEN_KEY, re.escape(self.env.key_token)),
             (TOKEN_UNION, re.escape(self.env.union_token)),
             (TOKEN_INTERSECTION, re.escape(self.env.intersection_token)),
             (TOKEN_FILTER_CONTEXT, re.escape(self.env.filter_context_token)),
+            (TOKEN_KEYS, re.escape(self.env.keys_selector_token)),
             (TOKEN_IN, r"in"),
             (TOKEN_TRUE, r"[Tt]rue"),
             (TOKEN_FALSE, r"[Ff]alse"),
             (TOKEN_NIL, r"[Nn]il"),
             (TOKEN_NULL, r"[Nn]ull"),
             (TOKEN_NONE, r"[Nn]one"),
             (TOKEN_CONTAINS, r"contains"),
```

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/match.py` & `python_jsonpath-0.6.0/jsonpath/match.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/parse.py` & `python_jsonpath-0.6.0/jsonpath/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Union
 
 from .exceptions import JSONPathSyntaxError
+from .filter import CURRENT_KEY
 from .filter import FALSE
 from .filter import NIL
 from .filter import TRUE
 from .filter import UNDEFINED_LITERAL
 from .filter import BooleanExpression
 from .filter import FilterContextPath
 from .filter import FilterExpression
@@ -29,14 +30,15 @@
 from .filter import RootPath
 from .filter import SelfPath
 from .filter import StringLiteral
 from .path import JSONPath
 from .selectors import Filter
 from .selectors import IndexSelector
 from .selectors import JSONPathSelector
+from .selectors import KeysSelector
 from .selectors import ListSelector
 from .selectors import PropertySelector
 from .selectors import RecursiveDescentSelector
 from .selectors import SliceSelector
 from .selectors import WildSelector
 from .token import TOKEN_AND
 from .token import TOKEN_BARE_PROPERTY
@@ -53,14 +55,16 @@
 from .token import TOKEN_FUNCTION
 from .token import TOKEN_GE
 from .token import TOKEN_GT
 from .token import TOKEN_IN
 from .token import TOKEN_INDEX
 from .token import TOKEN_INT
 from .token import TOKEN_INTERSECTION
+from .token import TOKEN_KEY
+from .token import TOKEN_KEYS
 from .token import TOKEN_LE
 from .token import TOKEN_LG
 from .token import TOKEN_LIST_START
 from .token import TOKEN_LPAREN
 from .token import TOKEN_LT
 from .token import TOKEN_MISSING
 from .token import TOKEN_NE
@@ -192,14 +196,15 @@
     def __init__(self, *, env: JSONPathEnvironment) -> None:
         self.env = env
 
         self.token_map: Dict[str, Callable[[TokenStream], FilterExpression]] = {
             TOKEN_FALSE: self.parse_boolean,
             TOKEN_FLOAT: self.parse_float_literal,
             TOKEN_INT: self.parse_integer_literal,
+            TOKEN_KEY: self.parse_current_key,
             TOKEN_LIST_START: self.parse_list_literal,
             TOKEN_LPAREN: self.parse_grouped_expression,
             TOKEN_MISSING: self.parse_undefined,
             TOKEN_NIL: self.parse_nil,
             TOKEN_NONE: self.parse_nil,
             TOKEN_NOT: self.parse_prefix_expression,
             TOKEN_NULL: self.parse_nil,
@@ -226,14 +231,15 @@
 
         self.function_argument_map: Dict[
             str, Callable[[TokenStream], FilterExpression]
         ] = {
             TOKEN_FALSE: self.parse_boolean,
             TOKEN_FLOAT: self.parse_float_literal,
             TOKEN_INT: self.parse_integer_literal,
+            TOKEN_KEY: self.parse_current_key,
             TOKEN_NIL: self.parse_nil,
             TOKEN_NONE: self.parse_nil,
             TOKEN_NULL: self.parse_nil,
             TOKEN_STRING: self.parse_string_literal,
             TOKEN_TRUE: self.parse_boolean,
             TOKEN_ROOT: self.parse_root_path,
             TOKEN_SELF: self.parse_self_path,
@@ -262,26 +268,27 @@
             if stream.current.kind in (TOKEN_PROPERTY, TOKEN_BARE_PROPERTY):
                 yield PropertySelector(
                     env=self.env,
                     token=stream.current,
                     name=stream.current.value,
                 )
             elif stream.current.kind == TOKEN_INDEX:
-                yield IndexSelector(
-                    env=self.env,
-                    token=stream.current,
-                    index=int(stream.current.value),
-                )
+                yield self.parse_index(stream)
             elif stream.current.kind == TOKEN_SLICE_START:
                 yield self.parse_slice(stream)
             elif stream.current.kind == TOKEN_WILD:
                 yield WildSelector(
                     env=self.env,
                     token=stream.current,
                 )
+            elif stream.current.kind == TOKEN_KEYS:
+                yield KeysSelector(
+                    env=self.env,
+                    token=stream.current,
+                )
             elif stream.current.kind == TOKEN_DDOT:
                 yield RecursiveDescentSelector(
                     env=self.env,
                     token=stream.current,
                 )
             elif stream.current.kind == TOKEN_LIST_START:
                 yield self.parse_selector_list(stream)
@@ -290,14 +297,28 @@
             else:
                 if in_filter:
                     stream.push(stream.current)
                 break
 
             stream.next_token()
 
+    def parse_index(self, stream: TokenStream) -> IndexSelector:
+        """Parse an index selector from a stream of tokens."""
+        if (
+            len(stream.current.value) > 1 and stream.current.value.startswith("0")
+        ) or stream.current.value.startswith("-0"):
+            raise JSONPathSyntaxError(
+                "leading zero in index selector", token=stream.current
+            )
+        return IndexSelector(
+            env=self.env,
+            token=stream.current,
+            index=int(stream.current.value),
+        )
+
     def parse_slice(self, stream: TokenStream) -> SliceSelector:
         """Parse a slice JSONPath expression from a stream of tokens."""
         start_token = stream.next_token()
         stream.expect(TOKEN_SLICE_STOP)
         stop_token = stream.next_token()
         stream.expect(TOKEN_SLICE_STEP)
         step_token = stream.current
@@ -325,15 +346,21 @@
             step=step,
         )
 
     def parse_selector_list(self, stream: TokenStream) -> ListSelector:
         """Parse a comma separated list JSONPath selectors from a stream of tokens."""
         tok = stream.next_token()
         list_items: List[
-            Union[IndexSelector, PropertySelector, SliceSelector, WildSelector]
+            Union[
+                IndexSelector,
+                KeysSelector,
+                PropertySelector,
+                SliceSelector,
+                WildSelector,
+            ]
         ] = []
 
         while stream.current.kind != TOKEN_RBRACKET:
             if stream.current.kind == TOKEN_INT:
                 list_items.append(
                     IndexSelector(
                         env=self.env,
@@ -345,14 +372,21 @@
                 list_items.append(
                     PropertySelector(
                         env=self.env,
                         token=stream.current,
                         name=stream.current.value,
                     ),
                 )
+            elif stream.current.kind == TOKEN_KEYS:
+                list_items.append(
+                    KeysSelector(
+                        env=self.env,
+                        token=stream.current,
+                    )
+                )
             elif stream.current.kind == TOKEN_STRING:
                 if self.RE_INVALID_NAME_SELECTOR.search(stream.current.value):
                     raise JSONPathSyntaxError(
                         f"invalid name selector {stream.current.value!r}",
                         token=stream.current,
                     )
 
@@ -473,14 +507,17 @@
 
     def parse_self_path(self, stream: TokenStream) -> FilterExpression:
         stream.next_token()
         return SelfPath(
             JSONPath(env=self.env, selectors=self.parse_path(stream, in_filter=True))
         )
 
+    def parse_current_key(self, _: TokenStream) -> FilterExpression:
+        return CURRENT_KEY
+
     def parse_filter_context_path(self, stream: TokenStream) -> FilterExpression:
         stream.next_token()
         return FilterContextPath(
             JSONPath(env=self.env, selectors=self.parse_path(stream, in_filter=True))
         )
 
     def parse_regex(self, stream: TokenStream) -> FilterExpression:
```

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/path.py` & `python_jsonpath-0.6.0/jsonpath/path.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/selectors.py` & `python_jsonpath-0.6.0/jsonpath/selectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,48 @@
                         path=match.path + f"[{norm_index}]",
                         root=match.root,
                     )
                     match.add_child(_match)
                     yield _match
 
 
+class KeysSelector(JSONPathSelector):
+    """Select an mapping's keys/properties."""
+
+    __slots__ = ()
+
+    def __str__(self) -> str:
+        return f"[{self.env.keys_selector_token}]"
+
+    def _keys(self, match: JSONPathMatch) -> Iterable[JSONPathMatch]:
+        if isinstance(match.obj, Mapping):
+            for i, key in enumerate(match.obj.keys()):
+                _match = JSONPathMatch(
+                    filter_context=match.filter_context(),
+                    obj=key,
+                    parent=match,
+                    parts=match.parts + (self.env.keys_selector_token, i),
+                    path=f"{match.path}[{self.env.keys_selector_token}][{i}]",
+                    root=match.root,
+                )
+                match.add_child(_match)
+                yield _match
+
+    def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
+        for match in matches:
+            yield from self._keys(match)
+
+    async def resolve_async(
+        self, matches: AsyncIterable[JSONPathMatch]
+    ) -> AsyncIterable[JSONPathMatch]:
+        async for match in matches:
+            for _match in self._keys(match):
+                yield _match
+
+
 class SliceSelector(JSONPathSelector):
     """Sequence slicing selector."""
 
     __slots__ = ("slice",)
 
     def __init__(
         self,
@@ -405,15 +439,21 @@
 
     def __init__(
         self,
         *,
         env: JSONPathEnvironment,
         token: Token,
         items: List[
-            Union[SliceSelector, IndexSelector, PropertySelector, WildSelector]
+            Union[
+                SliceSelector,
+                KeysSelector,
+                IndexSelector,
+                PropertySelector,
+                WildSelector,
+            ]
         ],
     ) -> None:
         super().__init__(env=env, token=token)
         self.items = items
 
     def __str__(self) -> str:
         buf: List[str] = []
@@ -423,14 +463,16 @@
                 start = item.slice.start if item.slice.start is not None else ""
                 step = item.slice.step if item.slice.step is not None else "1"
                 buf.append(f"{start}:{stop}:{step}")
             elif isinstance(item, PropertySelector):
                 buf.append(f"'{item.name}'")
             elif isinstance(item, WildSelector):
                 buf.append("*")
+            elif isinstance(item, KeysSelector):
+                buf.append(self.env.keys_selector_token)
             else:
                 buf.append(str(item.index))
         return f"[{', '.join(buf)}]"
 
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
         _matches = list(matches)
         for item in self.items:
@@ -470,14 +512,15 @@
             if isinstance(match.obj, Mapping):
                 for key, val in match.obj.items():
                     context = FilterContext(
                         env=self.env,
                         current=val,
                         root=match.root,
                         extra_context=match.filter_context(),
+                        current_key=key,
                     )
                     try:
                         if self.expression.evaluate(context):
                             _match = JSONPathMatch(
                                 filter_context=match.filter_context(),
                                 obj=val,
                                 parent=match,
@@ -495,14 +538,15 @@
             elif isinstance(match.obj, Sequence) and not isinstance(match.obj, str):
                 for i, obj in enumerate(match.obj):
                     context = FilterContext(
                         env=self.env,
                         current=obj,
                         root=match.root,
                         extra_context=match.filter_context(),
+                        current_key=i,
                     )
                     try:
                         if self.expression.evaluate(context):
                             _match = JSONPathMatch(
                                 filter_context=match.filter_context(),
                                 obj=obj,
                                 parent=match,
@@ -524,14 +568,15 @@
             if isinstance(match.obj, Mapping):
                 for key, val in match.obj.items():
                     context = FilterContext(
                         env=self.env,
                         current=val,
                         root=match.root,
                         extra_context=match.filter_context(),
+                        current_key=key,
                     )
 
                     try:
                         result = await self.expression.evaluate_async(context)
                     except JSONPathTypeError as err:
                         if not err.token:
                             err.token = self.token
@@ -552,14 +597,15 @@
             elif isinstance(match.obj, Sequence) and not isinstance(match.obj, str):
                 for i, obj in enumerate(match.obj):
                     context = FilterContext(
                         env=self.env,
                         current=obj,
                         root=match.root,
                         extra_context=match.filter_context(),
+                        current_key=i,
                     )
 
                     try:
                         result = await self.expression.evaluate_async(context)
                     except JSONPathTypeError as err:
                         if not err.token:
                             err.token = self.token
@@ -576,27 +622,29 @@
                         match.add_child(_match)
                         yield _match
 
 
 class FilterContext:
     """A filter expression context."""
 
-    __slots__ = ("current", "env", "root", "extra_context")
+    __slots__ = ("current", "current_key", "env", "root", "extra_context")
 
     def __init__(
         self,
         *,
         env: JSONPathEnvironment,
         current: object,
         root: Union[Sequence[Any], Mapping[str, Any]],
         extra_context: Optional[Mapping[str, Any]] = None,
+        current_key: Union[str, int, None] = None,
     ) -> None:
         self.env = env
         self.current = current
         self.root = root
         self.extra_context = extra_context or {}
+        self.current_key = current_key
 
     def __str__(self) -> str:
         return (
             f"FilterContext(current={self.current}, "
             f"extra_context={self.extra_context!r})"
         )
```

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/stream.py` & `python_jsonpath-0.6.0/jsonpath/stream.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/token.py` & `python_jsonpath-0.6.0/jsonpath/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 TOKEN_DOT = sys.intern("DOT")
 TOKEN_DOT_INDEX = sys.intern("DINDEX")
 TOKEN_DOT_PROPERTY = sys.intern("DOT_PROPERTY")
 TOKEN_FILTER_END = sys.intern("FILTER_END")
 TOKEN_FILTER_START = sys.intern("FILTER_START")
 TOKEN_IDENT = sys.intern("IDENT")
 TOKEN_INDEX = sys.intern("IDX")
+TOKEN_KEY = sys.intern("KEY")
+TOKEN_KEYS = sys.intern("KEYS")
 TOKEN_RBRACKET = sys.intern("RBRACKET")
 TOKEN_BARE_PROPERTY = sys.intern("BARE_PROPERTY")
 TOKEN_LIST_SLICE = sys.intern("LSLICE")
 TOKEN_LIST_START = sys.intern("LBRACKET")
 TOKEN_PROPERTY = sys.intern("PROP")
 TOKEN_QUESTION = sys.intern("QUESTION")
 TOKEN_QUOTE_PROPERTY = sys.intern("QUOTE_PROPERTY")
```

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/function_extensions/arguments.py` & `python_jsonpath-0.6.0/jsonpath/function_extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/function_extensions/match.py` & `python_jsonpath-0.6.0/jsonpath/function_extensions/match.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/jsonpath/function_extensions/search.py` & `python_jsonpath-0.6.0/jsonpath/function_extensions/search.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/.gitignore` & `python_jsonpath-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/LICENSE.txt` & `python_jsonpath-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.5.0.post1/pyproject.toml` & `python_jsonpath-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
   "types-pyyaml",
   "twine",
   "ruff",
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=jsonpath --cov=tests {args}"
+cov-html = "pytest --cov-report=html --cov-config=pyproject.toml --cov=jsonpath --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 test = "pytest {args}"
 lint = "ruff check ."
 typing = "mypy"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311", "pypy38", "pypy39"]
```

