# Comparing `tmp/typedllm-0.1.4.tar.gz` & `tmp/typedllm-0.2.1.tar.gz`

## Comparing `typedllm-0.1.4.tar` & `typedllm-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.4/HISTORY.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/test_client.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/test_interop.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/test_tool.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.1.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.1.4/LICENSE
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.1.4/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 typedllm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 typedllm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.1/HISTORY.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 typedllm-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 typedllm-0.2.1/tests/test_client.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.2.1/tests/test_interop.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 typedllm-0.2.1/tests/test_tool.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.2.1/LICENSE
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.2.1/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 typedllm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 typedllm-0.2.1/PKG-INFO
```

### Comparing `typedllm-0.1.4/tests/conftest.py` & `typedllm-0.2.1/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pytest
 
-from typedllm import LLMModel, TypedPrompt, LLMSession, LLMRequest, Tool
+from typedllm import LLMModel, TypedPrompt, LLMSession, LLMRequest, Tool, create_tool_from_function
 from typedtemplate import JinjaTemplateEngine
 from pydantic import Field
 
 
 @pytest.fixture(name="openai_key")
 def get_openai_key() -> str:
     return os.getenv("OPENAI_API_KEY")
@@ -63,7 +63,21 @@
 @pytest.fixture(name="llmtool")
 def get_tool():
     class CityFoundingTool(Tool):
         """A tool to collect a city and its founding year."""
         city_name: str = Field(description="The name of the city")
         founded_year: int = Field(description="The year a city was founded")
     return CityFoundingTool
+
+
+@pytest.fixture(name="FuncTool")
+def get_function_tool():
+    def TestTool(value: int) -> str:
+        return str(value)
+    return create_tool_from_function(TestTool)
+
+
+@pytest.fixture(name="ClassTool")
+def get_class_tool():
+    class TestTool(Tool):
+        value: int
+    return TestTool
```

### Comparing `typedllm-0.1.4/tests/test_client.py` & `typedllm-0.2.1/tests/test_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from pydantic import BaseModel, Field
 
 from typedllm import (
     LLMModel,
     LLMSession,
     LLMRequest,
     LLMUserMessage,
-    llm_request,
-    async_llm_request,
+    request,
+    async_request,
     create_tool_from_function,
     Tool
 )
+from typedllm.client import typed_request
 
 
 @pytest.mark.asyncio
 async def test_basic_request(openai_key: str):
     model = LLMModel(
         name="gpt-4-0125-preview",
         api_key=openai_key,
@@ -27,34 +28,34 @@
     )
     request = LLMRequest(
         message=LLMUserMessage(
             content="What year was New York City founded?",
         ),
         force_text_response=True
     )
-    session, response = await async_llm_request(session, request)
+    session, response = await async_request(session, request)
     assert response.message.content.index("1624") > -1
 
 
-class FoundingYear(BaseModel):
+class CityFoundingInfo(Tool):
     """This represents a city and includes the year the city was founded."""
     year: int = Field(description="The year the city was founded.")
     city: str = Field(description="The name of the city.")
 
 
-def get_city_founding_history(city: FoundingYear) -> str:
-    return (f"Historical weather for {city.city} since its founding in {city.year}. "
+def get_city_founding_history(city_info: CityFoundingInfo) -> str:
+    return (f"Historical weather for {city_info.city} since its founding in {city_info.year}. "
             f"The weather is very nice. Average 80 degrees F.")
 
 
 def test_make_tool_from_function():
     Tool = create_tool_from_function(get_city_founding_history)
     assert Tool.__name__ == "get_city_founding_history"
-    assert "city" in Tool.model_fields
-    assert Tool.model_fields["city"].annotation == FoundingYear
+    assert "city_info" in Tool.model_fields
+    assert Tool.model_fields["city_info"].annotation == CityFoundingInfo
 
 
 @pytest.mark.asyncio
 async def test_basic_tools_request(openai_key: str):
     model = LLMModel(
         name="gpt-4",
         api_key=openai_key,
@@ -66,18 +67,28 @@
     )
     request = LLMRequest(
         message=LLMUserMessage(
             content="What is the founding story of New York City?",
         ),
         required_tool=tool,
     )
-    session, response = await async_llm_request(session, request)
+    session, response = await async_request(session, request)
     assert session
     assert response
     assert response.tool_calls[0].tool.__class__.__name__ == "get_city_founding_history"
-    assert response.tool_calls[0].tool.city.city.index("New York") > -1
-    assert response.tool_calls[0].tool.city.year == 1624
+    assert response.tool_calls[0].tool.city_info.city.index("New York") > -1
+    assert response.tool_calls[0].tool.city_info.year == 1624
 
 
 @pytest.mark.asyncio
-async def test_basic_lvm_request(openai_key: str):
-    pass
+async def test_basic_lvm_request(openai_key: str, llmprompt):
+    class Year(Tool):
+        year: int = Field(description="The year of the city's founding")
+
+    model = LLMModel(
+        name="gpt-4",
+        api_key=openai_key,
+    )
+    response = typed_request(model, llmprompt, Year, city="New York")
+    assert response
+    assert response.tool_calls[0].tool.__class__.__name__ == "Year"
+    assert response.tool_calls[0].tool.year == 1624
```

### Comparing `typedllm-0.1.4/tests/test_interop.py` & `typedllm-0.2.1/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.4/tests/test_tool.py` & `typedllm-0.2.1/tests/test_tool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 from pydantic import BaseModel
 from typedllm.tool import Tool, create_tool_from_function
 
 
-class TestTool(Tool):
-    value: int
-
-
-def test_basic_tool_creation():
-    result = TestTool.openapi_json()
+def test_basic_tool_creation(ClassTool):
+    result = ClassTool.openapi_json()
 
     assert result == {
         "type": "function",
         "function": {
             "name": "TestTool",
             "description": "Tool called TestTool",
             "parameters": {
                 "type": "object",
+                "title": "TestTool",
+                "description": "Tool called TestTool",
                 "properties": {
                     "value": {
                         "title": "Value",
                         "type": "integer"
                     }
                 },
                 "required": ["value"]
             }
         }
     }
 
 
-def test_tool_creation_from_function():
-    def test_function(value: int) -> str:
-        return str(value)
+def test_func_versus_class_tool_creation(FuncTool, ClassTool):
+    """
+    This test should show that you can create a tool from a function or class and they are equivalent.
+    """
+    f = FuncTool.openapi_json()
+    c = ClassTool.openapi_json()
+    assert f == c
 
-    FuncTool = create_tool_from_function(test_function)
 
+def test_tool_creation_from_function(FuncTool):
     result = FuncTool.openapi_json()
 
-    assert FuncTool.__name__ == "test_function"
-    assert FuncTool.__doc__ == "Tool called test_function"
+    assert FuncTool.__name__ == "TestTool"
+    assert FuncTool.__doc__ == "Tool called TestTool"
 
     assert result == {
         "type": "function",
         "function": {
-            "name": "test_function",
-            "description": "Tool called test_function",
+            "name": "TestTool",
+            "description": "Tool called TestTool",
             "parameters": {
                 "type": "object",
+                "title": "TestTool",
+                "description": "Tool called TestTool",
                 "properties": {
                     "value": {
                         "title": "Value",
                         "type": "integer"
                     }
                 },
                 "required": ["value"]
```

### Comparing `typedllm-0.1.4/.gitignore` & `typedllm-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.4/LICENSE` & `typedllm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.4/pyproject.toml` & `typedllm-0.2.1/pyproject.toml`

 * *Files identical despite different names*

