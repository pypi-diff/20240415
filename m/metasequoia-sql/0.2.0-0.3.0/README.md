# Comparing `tmp/metasequoia-sql-0.2.0.tar.gz` & `tmp/metasequoia-sql-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasequoia-sql-0.2.0.tar", last modified: Thu Apr 11 23:37:26 2024, max compression
+gzip compressed data, was "metasequoia-sql-0.3.0.tar", last modified: Mon Apr 15 01:03:43 2024, max compression
```

## Comparing `metasequoia-sql-0.2.0.tar` & `metasequoia-sql-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.256211 metasequoia-sql-0.2.0/
--rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     6477 2024-04-11 23:37:26.256211 metasequoia-sql-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5808 2024-04-11 23:36:28.000000 metasequoia-sql-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.246211 metasequoia-sql-0.2.0/metasequoia_sql/
--rw-rw-rw-   0        0        0      150 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.248211 metasequoia-sql-0.2.0/metasequoia_sql/analyzer/
--rw-rw-rw-   0        0        0        0 2024-04-09 23:10:25.000000 metasequoia-sql-0.2.0/metasequoia_sql/analyzer/__init__.py
--rw-rw-rw-   0        0        0     1523 2024-04-09 23:10:25.000000 metasequoia-sql-0.2.0/metasequoia_sql/analyzer/consanguinity.py
-drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.251211 metasequoia-sql-0.2.0/metasequoia_sql/ast/
--rw-rw-rw-   0        0        0       86 2024-04-07 00:08:43.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/__init__.py
--rw-rw-rw-   0        0        0     8647 2024-04-07 00:08:43.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/functions.py
--rw-rw-rw-   0        0        0    17097 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/nodes.py
--rw-rw-rw-   0        0        0     8463 2024-04-09 23:15:51.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/parser.py
--rw-rw-rw-   0        0        0     5581 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/static.py
-drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.253211 metasequoia-sql-0.2.0/metasequoia_sql/common/
--rw-rw-rw-   0        0        0      145 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/__init__.py
--rw-rw-rw-   0        0        0     3617 2024-04-09 23:15:51.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/base_scanner.py
--rw-rw-rw-   0        0        0      325 2024-04-07 00:08:43.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/basic.py
--rw-rw-rw-   0        0        0      150 2024-04-09 23:15:51.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/text_scanner.py
--rw-rw-rw-   0        0        0     6279 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/token_scanner.py
-drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.255211 metasequoia-sql-0.2.0/metasequoia_sql/core/
--rw-rw-rw-   0        0        0      144 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/__init__.py
--rw-rw-rw-   0        0        0      341 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/data_source.py
--rw-rw-rw-   0        0        0    85050 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/objects.py
--rw-rw-rw-   0        0        0    80134 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/parser.py
--rw-rw-rw-   0        0        0      271 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/static.py
--rw-rw-rw-   0        0        0      592 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/errors.py
--rw-rw-rw-   0        0        0     1041 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/static.py
-drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.255211 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/
--rw-rw-rw-   0        0        0     6477 2024-04-11 23:37:26.000000 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      843 2024-04-11 23:37:26.000000 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 23:37:26.000000 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-11 23:37:26.000000 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 23:37:26.256211 metasequoia-sql-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1042 2024-04-11 23:36:52.000000 metasequoia-sql-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.089912 metasequoia-sql-0.3.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     7222 2024-04-15 01:03:43.089912 metasequoia-sql-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6553 2024-04-15 01:00:03.000000 metasequoia-sql-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.081409 metasequoia-sql-0.3.0/metasequoia_sql/
+-rw-rw-rw-   0        0        0      183 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.083408 metasequoia-sql-0.3.0/metasequoia_sql/analyzer/
+-rw-rw-rw-   0        0        0        0 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     1009 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/analyzer/data_lineage.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.085409 metasequoia-sql-0.3.0/metasequoia_sql/ast/
+-rw-rw-rw-   0        0        0      136 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/ast/__init__.py
+-rw-rw-rw-   0        0        0     8793 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/ast/nodes.py
+-rw-rw-rw-   0        0        0    15035 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/ast/parser.py
+-rw-rw-rw-   0        0        0     5622 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/ast/static.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.087409 metasequoia-sql-0.3.0/metasequoia_sql/common/
+-rw-rw-rw-   0        0        0      209 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/__init__.py
+-rw-rw-rw-   0        0        0     3937 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/base_scanner.py
+-rw-rw-rw-   0        0        0      601 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/basic.py
+-rw-rw-rw-   0        0        0      226 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/text_scanner.py
+-rw-rw-rw-   0        0        0     5612 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/common/token_scanner.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.088409 metasequoia-sql-0.3.0/metasequoia_sql/core/
+-rw-rw-rw-   0        0        0      116 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/core/__init__.py
+-rw-rw-rw-   0        0        0    84297 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/core/objects.py
+-rw-rw-rw-   0        0        0    69929 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/core/parser.py
+-rw-rw-rw-   0        0        0      405 2024-04-15 00:51:46.000000 metasequoia-sql-0.3.0/metasequoia_sql/core/static.py
+-rw-rw-rw-   0        0        0      592 2024-04-11 15:14:53.000000 metasequoia-sql-0.3.0/metasequoia_sql/errors.py
+-rw-rw-rw-   0        0        0     1041 2024-04-11 15:14:53.000000 metasequoia-sql-0.3.0/metasequoia_sql/static.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:03:43.088409 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/
+-rw-rw-rw-   0        0        0     7222 2024-04-15 01:03:43.000000 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-15 01:03:43.000000 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 01:03:43.000000 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 01:03:43.000000 metasequoia-sql-0.3.0/metasequoia_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 01:03:43.089912 metasequoia-sql-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2024-04-15 00:52:01.000000 metasequoia-sql-0.3.0/setup.py
```

### Comparing `metasequoia-sql-0.2.0/LICENSE` & `metasequoia-sql-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.2.0/PKG-INFO` & `metasequoia-sql-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,45 @@
-Metadata-Version: 2.1
-Name: metasequoia-sql
-Version: 0.2.0
-Summary: SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能
-Home-page: https://github.com/ChangxingJiang/metasequoia-sql
-Author: changxing
-Author-email: 1278729001@qq.com
-License: MIT License
-Platform: all
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sql-tree：SQL 解析器
 
 ## 安装方法
 
 ```bash
 pip install metasequoia-sql
 ```
 
 ## 使用方法
 
 ### 词法分析
 
-对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象语法树节点（详见 demo_1）：
-
-```python
-from metasequoia_sql.ast.functions import parse_as_statements
-
-root = parse_as_statements("your sql")
-```
+对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象语法树节点：
 
 ### 句法分析
 
 对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
 
 ```python
 from metasequoia_sql import *
 
-statement = parse_create_table_statement(build_token_scanner("your sql"))
+statement = SQLParser.parse_create_table_statement("your sql")
 ```
 
 ### 翻译工具
 
 将 MySQL 的 CREATE TABLE 语句转换为 Hive 的 CREATE TABLE 语句：
 
 ```python
 from metasequoia_sql import *
 
-statement = parse_create_table_statement(build_token_scanner("your sql"))
+statement = SQLParser.parse_create_table_statement("your sql")
+```
+
+### pylint 自检
+
+```bash
+pylint --max-line-length=120 metasequoia_sql
 ```
 
 ## 实现原理
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
@@ -129,16 +111,38 @@
 - `SQLUnionClause`：UNION 语句。包含多个 SELECT 语句。
 - `SQLUnionALLClause`：UNION ALL 语句。包含多个 SELECT 语句。
 
 ## 已知的不兼容
 
 - DB2 的 `CURRENT DATE` 的语法
 
+参考文档：https://www.alibabacloud.com/help/zh/maxcompute/user-guide/insert-or-update-data-into-a-table-or-a-static-partition?spm=a2c63.p38356.0.0.637d7109wr3nC3
+
 ## 修改记录
 
+#### 0.2.0 > 0.3.0
+
+新增：
+
+- 重构词法解析和语法解析以支持插件开发
+- SET 语句的解析逻辑
+- LATERAL VIEW 子句的解析逻辑
+
+优化：
+
+- core.objects 将语法节点重构为 dataclasses 类型
+- 含 WITH 表达式的上游表解析逻辑
+- core.parser 中的方法兼容字符串类型的 TokenScanner 类型
+- 整理单元测试逻辑
+- 代码质量提升
+- core.objects 中将 get_used_column_list 和 get_used_table_list 改为抽象方法
+- 支持 DB2 的 CURRENT DATE、CURRENT TIME、CURRENT TIMESTAMP 语法
+- 增加 TokenScanner 未解析完成的发现机制
+- 支持窗口函数的 ROWS 子句
+
 #### 0.1.0 > 0.2.0
 
 新增：
 - `INSERT` 语句解析逻辑
 - 一次性解析多条 SQL 语句
 
 优化：
@@ -153,8 +157,8 @@
 ##### 0.1.0
 
 - 新增 SELECT 语句解析逻辑
 - Bug 修复：移除在 Hive 建表语句末尾的分号
 
 ##### 0.0.1
 
-- 新增 CREATE TABLE 语句解析逻辑
+- 新增 CREATE TABLE 语句解析逻辑
```

### Comparing `metasequoia-sql-0.2.0/metasequoia_sql/ast/static.py` & `metasequoia-sql-0.3.0/metasequoia_sql/ast/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+词法分析的静态常量
+"""
+
 # 十六机制的字符集
 HEXADECIMAL_CHARACTER_SET = {"0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "a", "B", "b", "C", "c", "D", "d",
                              "E", "e", "F", "f"}
 
 # 二级制的字符集
 BINARY_CHARACTER_SET = {"0", "1"}
```

### Comparing `metasequoia-sql-0.2.0/metasequoia_sql/common/base_scanner.py` & `metasequoia-sql-0.3.0/metasequoia_sql/common/base_scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,20 @@
         self._pos = pos
         self._len = len(elements)
 
         self._last = elements[pos - 1] if pos > 0 else None  # 上一个元素
 
     @property
     def elements(self) -> List[T]:
+        """返回扫描器中的所有元素"""
         return self._elements
 
     @property
     def pos(self) -> int:
+        """返回当前扫描指针"""
         return self._pos
 
     @property
     def last(self) -> Optional[T]:
         """当前指针位置的上一个字符"""
         return self._last
 
@@ -104,9 +106,14 @@
         return self._elements[self.pos + idx]
 
     @property
     def is_finish(self) -> bool:
         """返回当前是否已匹配结束"""
         return self.pos == self._len
 
+    def close(self) -> None:
+        """关闭扫描器，如果扫描器没有遍历完成则抛出异常"""
+        if not self.is_finish:
+            raise ScannerError(f"关闭了没有遍历完成的扫描器 {self}")
+
     def __repr__(self):
-        return f"<{self.__class__.__name__} tokens={self.elements[self.pos:]}, pos={self.pos}>"
+        return f"<{self.__class__.__name__} tokens={self.elements[self.pos:]}, pos={self.pos}>"
```

### Comparing `metasequoia-sql-0.2.0/metasequoia_sql/common/token_scanner.py` & `metasequoia-sql-0.3.0/metasequoia_sql/common/token_scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 """
-TODO 多语句解析支持
-TODO 支持匹配各种特殊要求，例如：
-    return not scanner.is_finish and (
-            scanner.now.is_maybe_name and scanner.now.source.upper() in WINDOW_FUNCTION_NAME_SET and
-            scanner.next1 is not None and scanner.next1.is_parenthesis and
-            scanner.next2 is not None and scanner.next2.equals("OVER") and
-            scanner.next3 is not None and scanner.next3.is_parenthesis)
+抽象语法树扫描器
 """
 
-from typing import List
+from typing import List, Union
 
-from metasequoia_sql import ast
+from metasequoia_sql.ast import AST, ASTParser, ASTMark
 from metasequoia_sql.common.base_scanner import BaseScanner
 from metasequoia_sql.errors import ScannerError
 
 
 class TokenScanner(BaseScanner):
     """Token 扫描器"""
 
-    def __init__(self, elements: List[ast.AST],
+    def __init__(self, elements: List[AST],
                  pos: int = 0,
                  ignore_space: bool = False,
                  ignore_comment: bool = False):
         """
 
         Parameters
         ----------
@@ -30,57 +24,52 @@
             当前层级的抽象语法树节点列表
         pos : int, default = 0
             当前正在处理的抽象语法树节点下标
         """
         # 根据要求筛选输入元素
         filtered_elements = []
         for element in elements:
-            if element.is_space:
+            if element.equals(ASTMark.SPACE):
                 if ignore_space is False:  # 关闭忽略空白字符的模式
                     filtered_elements.append(element)
-            elif element.is_comment:
+            elif element.equals(ASTMark.COMMENT):
                 if ignore_comment is False:  # 关闭忽略注释的模式
                     filtered_elements.append(element)
             else:
                 filtered_elements.append(element)
 
         super().__init__(filtered_elements, pos)
 
-    @property
-    def now_is_parenthesis(self):
-        return self.now.is_parenthesis
-
-    def search(self, *tokens: str) -> bool:
+    def search(self, *tokens: Union[str, ASTMark]) -> bool:
         """从当前配置开始匹配 tokens
 
         - 如果匹配成功，则返回 True
         - 如果匹配失败，则返回 False
         """
         for idx, token in enumerate(tokens):
             refer = self._get_by_offset(idx)
             if refer is None or not refer.equals(token):
                 return False
         return True
 
-    def search_and_move(self, *tokens: str) -> bool:
+    def search_and_move(self, *tokens: Union[str, ASTMark]) -> bool:
         """从当前配置开始匹配 tokens
 
         - 如果匹配成功，则将指针移动到 tokens 后的下一个元素并返回 True
         - 如果匹配失败，则不移动指针并返回 False
         """
         for idx, token in enumerate(tokens):
             refer = self._get_by_offset(idx)
             if refer is None or not refer.equals(token):
                 return False
-        else:
-            for _ in range(len(tokens)):
-                self.pop()
-            return True
+        for _ in range(len(tokens)):
+            self.pop()
+        return True
 
-    def match(self, *tokens: str) -> None:
+    def match(self, *tokens: Union[str, ASTMark]) -> None:
         """从当前配置开始匹配 tokens
 
         - 如果匹配成功，则将指针移动到 tokens 后的下一个元素
         - 如果匹配失败，则抛出异常
         """
         for word in tokens:
             if not self.pop().equals(word):
@@ -92,29 +81,29 @@
 
     def pop_as_source(self) -> str:
         """将指针向后移动 1 个元素并返回当前元素的 source"""
         return self.pop().source
 
     def get_as_children_scanner(self, ignore_space: bool = True, ignore_comment: bool = True) -> "TokenScanner":
         """【不移动指针】返回当前指针位置的插入语节点的子节点的扫描器"""
-        return TokenScanner(self.now.children, ignore_space=ignore_space, ignore_comment=ignore_comment)
+        return TokenScanner(self.now.children(), ignore_space=ignore_space, ignore_comment=ignore_comment)
 
     def pop_as_children_scanner(self, ignore_space: bool = True, ignore_comment: bool = True) -> "TokenScanner":
         """【移动指针】返回当前指针位置的插入语节点的子节点的扫描器"""
-        return TokenScanner(self.pop().children, ignore_space=ignore_space, ignore_comment=ignore_comment)
+        return TokenScanner(self.pop().children(), ignore_space=ignore_space, ignore_comment=ignore_comment)
 
     def split_by(self,
                  source: str,
                  ignore_space: bool = True,
                  ignore_comment: bool = True) -> List["TokenScanner"]:
         """【移动指针（到末尾）】将后续元素拆分为使用 source 分隔的扫描器列表"""
         result = []
         tokens = []
         while not self.is_finish:
-            token: ast.AST = self.pop()
+            token: AST = self.pop()
             if token.equals(source):
                 if len(tokens) > 0:
                     result.append(TokenScanner(tokens, ignore_space=ignore_space, ignore_comment=ignore_comment))
                     tokens = []
             else:
                 tokens.append(token)
         if len(tokens) > 0:
@@ -124,27 +113,22 @@
     def pop_as_children_scanner_list_split_by(self,
                                               source: str,
                                               ignore_space: bool = True,
                                               ignore_comment: bool = True) -> List["TokenScanner"]:
         """【移动指针】返回当前指针位置的插入语结点的子节点使用 source 分隔的扫描器列表"""
         result = []
         tokens = []
-        for token in self.pop().children:
+        for token in self.pop().children():
             if token.equals(source):
                 if len(tokens) > 0:
                     result.append(TokenScanner(tokens, ignore_space=ignore_space, ignore_comment=ignore_comment))
                     tokens = []
             else:
                 tokens.append(token)
         if len(tokens) > 0:
             result.append(TokenScanner(tokens, ignore_space=ignore_space, ignore_comment=ignore_comment))
         return result
 
     @property
     def is_finish(self) -> bool:
         """返回是否已匹配结束"""
         return not self._pos < self._len
-
-
-def build_token_scanner(sql: str, ignore_space=True, ignore_comment=True):
-    """根据 sql 语句构造扫描器"""
-    return TokenScanner(ast.parse_as_tokens(sql), ignore_space=ignore_space, ignore_comment=ignore_comment)
```

### Comparing `metasequoia-sql-0.2.0/metasequoia_sql/core/parser.py` & `metasequoia-sql-0.3.0/metasequoia_sql/core/parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,1729 +1,1380 @@
+# pylint: disable=C0302
+
 """
 基础元素的解析逻辑
 
+因为不同解析函数之间需要相互调用，所以脚本文件不可避免地需要超过 1000 行，故忽略 pylint C0302。
+
 TODO 使用 search 替代直接使用 now 判断
-TODO 整理各种函数的共同规律
-TODO 将 doctest 转化为单元测试
+TODO 将 CAST_DATA_TYPE 提出作为一个基础类型节点
+TODO 将 function_name 提出作为一个专有表达式
 """
 
 from typing import Optional, Tuple, List, Union
 
-from metasequoia_sql import ast
-from metasequoia_sql.common import TokenScanner, build_token_scanner
+from metasequoia_sql.ast import (AST, ASTMark, ASTSingle, ASTLiteralInteger, ASTLiteralFloat, ASTLiteralString,
+                                 ASTLiteralHex, ASTLiteralBool, ASTLiteralBit, ASTLiteralNull, ASTParser)
+from metasequoia_sql.common import TokenScanner
 from metasequoia_sql.core.objects import *
-from metasequoia_sql.core.static import *
+from metasequoia_sql.core.static import AGGREGATION_FUNCTION_NAME_SET, WINDOW_FUNCTION_NAME_SET
 from metasequoia_sql.errors import SqlParseError
 
-__all__ = [
-    # ------------------------------ 基础元素解析 ------------------------------
-    # 判断、解析插入类型
-    "check_insert_type", "parse_insert_type",
-
-    # 判断、解析关联类型
-    "check_join_type", "parse_join_type",
-
-    # 判断、解析排序类型
-    "check_order_type", "parse_order_type",
-
-    # 判断、解析组合类型
-    "check_union_type", "parse_union_type",
-
-    # 判断、解析比较运算符
-    "check_compare_operator", "parse_compare_operator",
-
-    # 判断、解析计算运算符
-    "check_compute_operator", "parse_compute_operator",
-
-    # 判断、解析逻辑运算符
-    "check_logical_operator", "parse_logical_operator",
-
-    # ------------------------------ 一般表达式解析 ------------------------------
-    # 判断、解析字面值表达式
-    "check_literal_expression", "parse_literal_expression",
-
-    # 判断、解析列名表达式
-    "check_column_name_expression", "parse_column_name_expression",
-
-    # 判断、解析函数表达式
-    # TODO 将 CAST_DATA_TYPE 提出作为一个基础类型节点
-    # TODO 将 function_name 提出作为一个专有表达式
-    "check_function_expression", "parse_cast_data_type", "parse_cast_function_expression",
-    "parse_extract_function_expression", "parse_if_function_expression", "parse_function_name",
-    "parse_function_expression",
-
-    # 解析布尔值表达式
-    "parse_bool_expression",
-
-    # 判断、解析窗口表达式
-    "check_window_expression", "parse_window_expression",
-
-    # 判断、解析通配符表达式
-    "check_wildcard_expression", "parse_wildcard_expression",
-
-    # 解析条件表达式
-    "parse_condition_expression",
-
-    # 判断、解析 CASE 表达式
-    "check_case_expression", "parse_case_expression",
-
-    # 解析值表达式
-    "parse_value_expression",
-
-    # 判断、解析子查询表达式
-    "check_sub_query_parenthesis", "parse_sub_query_expression",
-
-    # 解析一般表达式
-    "parse_general_expression",
-
-    # ------------------------------ 专有表达式解析 ------------------------------
-    # 解析表名表达式
-    "parse_table_name_expression",
-
-    # 判断、解析表名表达式
-    "check_alias_expression", "parse_alias_expression",
-
-    # 判断、解析关联表达式
-    "check_join_expression", "parse_join_on_expression", "parse_join_using_expression", "parse_join_expression",
-
-    # 解析字段类型表达式
-    "parse_column_type_expression",
-
-    # 解析表表达式
-    "parse_table_expression",
-
-    # 解析列表达式
-    "parse_column_expression",
-
-    # 解析等式表达式
-    "parse_equal_expression",
-
-    # 判断、解析分区表达式
-    "check_partition_expression", "parse_partition_expression",
-
-    # 判断、解析声明外键表达式
-    "check_foreign_key_expression", "parse_foreign_key_expression",
-
-    # 判断、解析声明索引表达式
-    "check_primary_index_expression", "parse_primary_index_expression", "check_unique_index_expression",
-    "parse_unique_index_expression", "check_normal_index_expression", "parse_normal_index_expression",
-    "check_fulltext_expression", "parse_fulltext_expression",
-
-    # 解析声明字段表达式
-    "parse_define_column_expression",
-
-    # ------------------------------ 子句解析 ------------------------------
-    # 判断、解析 SELECT 子句
-    "check_select_clause", "parse_select_clause",
-
-    # 判断、解析 FROM 子句
-    "check_from_clause", "parse_from_clause",
-
-    # 判断、解析 JOIN 子句
-    "check_join_clause", "parse_join_clause",
-
-    # 判断、解析 WHERE 子句
-    "check_where_clause", "parse_where_clause",
-
-    # 判断、解析 GROUP BY 子句
-    "check_group_by_clause", "parse_group_by_clause",
-
-    # 判断、解析 HAVING 子句
-    "check_having_clause", "parse_having_clause",
-
-    # 判断、解析 ORDER BY 子句
-    "check_order_by_clause", "parse_order_by_clause",
-
-    # 判断、解析 LIMIT 子句
-    "check_limit_clause", "parse_limit_clause",
-
-    # 解析 WITH 子句
-    "parse_with_clause",
-
-    # ------------------------------ 语句解析 ------------------------------
-    # 判断、解析 SELECT 语句
-    "check_select_statement", "parse_single_select_statement", "parse_select_statement",
-
-    # 判断、解析 INSERT 语句
-    "check_insert_statement", "parse_insert_statement",
-
-    # 解析 CREATE TABLE 语句
-    "parse_create_table_statement",
-
-    # 通用表达式解析
-    "parse_statement"
-]
-
-
-def check_insert_type(scanner: TokenScanner) -> bool:
-    """判断是否为插入类型"""
-    return scanner.search_and_move("INSERT", "INTO") or scanner.search_and_move("INSERT", "OVERWRITE")
-
-
-def parse_insert_type(scanner: TokenScanner) -> SQLInsertType:
-    """解析插入类型"""
-    if scanner.search_and_move("INSERT", "INTO"):
-        return SQLInsertType(insert_type=EnumInsertType.INSERT_INTO)
-    if scanner.search_and_move("INSERT", "OVERWRITE"):
-        return SQLInsertType(insert_type=EnumInsertType.INSERT_OVERWRITE)
-    raise SqlParseError(f"未知的 INSERT 类型: {scanner}")
-
-
-def check_join_type(scanner: TokenScanner) -> bool:
-    for join_type in EnumJoinType:
-        if scanner.search(*join_type.value):
-            return True
-    return False
-
-
-def parse_join_type(scanner: TokenScanner) -> SQLJoinType:
-    for join_type in EnumJoinType:
-        if scanner.search_and_move(*join_type.value):
-            return SQLJoinType(join_type=join_type)
-    raise SqlParseError(f"无法解析的关联类型: {scanner}")
-
-
-def check_order_type() -> bool:
-    """任何元素都可以是排序类型（省略升序），所以均返回 True"""
-    return True
-
-
-def parse_order_type(scanner: TokenScanner) -> SQLOrderType:
-    if scanner.search_and_move("DESC"):
-        return SQLOrderType(order_type=EnumOrderType.DESC)
-    return SQLOrderType(order_type=EnumOrderType.ASC)
-
-
-def check_union_type(scanner: TokenScanner) -> bool:
-    for union_type in EnumUnionType:
-        if scanner.search(*union_type.value):
-            return True
-    return False
-
-
-def parse_union_type(scanner: TokenScanner) -> SQLUnionType:
-    for union_type in EnumUnionType:
-        if scanner.search_and_move(*union_type.value):
-            return SQLUnionType(union_type=union_type)
-    raise SqlParseError(f"无法解析的组合类型: {scanner}")
-
-
-def check_compare_operator(scanner: TokenScanner) -> bool:
-    return scanner.get_as_source() in {"=", "!=", "<>", "<", "<=", ">", ">="}
-
-
-def parse_compare_operator(scanner: TokenScanner) -> SQLCompareOperator:
-    compare_operator_hash = {
-        "=": EnumCompareOperator.EQUAL_TO,
-        "<": EnumCompareOperator.LESS_THAN,
-        "<=": EnumCompareOperator.LESS_THAN_OR_EQUAL,
-        ">": EnumCompareOperator.GREATER_THAN,
-        ">=": EnumCompareOperator.GREATER_THAN_OR_EQUAL,
-        "!=": EnumCompareOperator.NOT_EQUAL_TO,
-        "<>": EnumCompareOperator.NOT_EQUAL_TO
-    }
-    compare_operator = compare_operator_hash.get(scanner.pop_as_source())
-    if compare_operator is not None:
-        return SQLCompareOperator(compare_operator=compare_operator)
-    raise SqlParseError(f"无法解析的比较运算符: {scanner}")
-
-
-def check_compute_operator(scanner: TokenScanner) -> bool:
-    for compute_operator in EnumComputeOperator:
-        if scanner.search(compute_operator.value):
-            return True
-    return False
-
-
-def parse_compute_operator(scanner: TokenScanner) -> SQLComputeOperator:
-    for compute_operator in EnumComputeOperator:
-        if scanner.search_and_move(compute_operator.value):
-            return SQLComputeOperator(compute_operator=compute_operator)
-    raise SqlParseError(f"无法解析的计算运算符: {scanner}")
+__all__ = ["SQLParser"]
 
 
-def check_logical_operator(scanner: TokenScanner) -> bool:
-    return scanner.get_as_source() in {"AND", "OR", "NOT"}
+class SQLParser:
+    # pylint: disable=R0904 忽略类中包含过多共有方法的问题
 
+    """SQL语法解析器
 
-def parse_logical_operator(scanner: TokenScanner) -> SQLLogicalOperator:
-    for logical_operator in EnumLogicalOperator:
-        if scanner.search_and_move(logical_operator.value):
-            return SQLLogicalOperator(logical_operator=logical_operator)
-    raise SqlParseError(f"无法解析的逻辑运算符: {scanner}")
-
-
-def check_literal_expression(scanner: TokenScanner) -> bool:
-    """判断是否为字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值
-
-    Examples
-    --------
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("1 WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("'a' WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("x'3f' WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("TRUE WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("true WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("False WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("b'1' WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("null WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("NULL WHERE"), ignore_space=True))
-    True
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("cnt WHERE"), ignore_space=True))
-    False
-    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("table_name.column_name WHERE"), ignore_space=True))
-    False
-    """
-    return not scanner.is_finish and scanner.now.is_literal
-
-
-def parse_literal_expression(scanner: TokenScanner) -> SQLLiteralExpression:
-    """解析字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值
-
-    Examples
-    --------
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("1 WHERE"), ignore_space=True))
-    <SQLLiteralInteger source=1>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
-    <SQLLiteralFloat source=2.5>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("'a' WHERE"), ignore_space=True))
-    <SQLLiteralString source='a'>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("x'3f' WHERE"), ignore_space=True))
-    <SQLLiteralHex source=x'3F'>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("TRUE WHERE"), ignore_space=True))
-    <SQLLiteralBool source=TRUE>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("true WHERE"), ignore_space=True))
-    <SQLLiteralBool source=TRUE>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("False WHERE"), ignore_space=True))
-    <SQLLiteralBool source=FALSE>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("b'1' WHERE"), ignore_space=True))
-    <SQLLiteralBit source=b'1'>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("null WHERE"), ignore_space=True))
-    <SQLLiteralNull source=NULL>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("NULL WHERE"), ignore_space=True))
-    <SQLLiteralNull source=NULL>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("cnt WHERE"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 未知的字面值: <ASTOther source=cnt>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("table_name.column_name WHERE"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 未知的字面值: <ASTOther source=table_name>
-    """
-    token: ast.AST = scanner.pop()
-    if isinstance(token, ast.ASTLiteralInteger):
-        return SQLLiteralIntegerExpression(token.literal_value)
-    if isinstance(token, ast.ASTLiteralFloat):
-        return SQLLiteralFloatExpression(token.literal_value)
-    if isinstance(token, ast.ASTLiteralString):
-        return SQLLiteralStringExpression(token.literal_value)
-    if isinstance(token, ast.ASTLiteralHex):
-        return SQLLiteralHexExpression(token.literal_value)
-    if isinstance(token, ast.ASTLiteralBool):
-        return SQLLiteralBoolExpression(token.literal_value)
-    if isinstance(token, ast.ASTLiteralBit):
-        return SQLLiteralBitExpression(token.literal_value)
-    if isinstance(token, ast.ASTLiteralNull):
-        return SQLLiteralNullExpression()
-    raise SqlParseError(f"未知的字面值: {token}")
-
-
-def check_column_name_expression(scanner: TokenScanner) -> bool:
-    """是否可能为列名表达式
-
-    Examples
-    --------
-    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
-    False
-    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
-    False
-    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.column AND"), ignore_space=True))
-    True
-    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`column` AND"), ignore_space=True))
-    True
-    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
-    False
-    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
-    False
-    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("column_name WHERE"), ignore_space=True))
-    True
-    """
-    return not scanner.is_finish and (
-            (scanner.now.is_maybe_name and
-             (scanner.next1 is None or (not scanner.next1.is_dot and not scanner.next1.is_parenthesis))) or
-            (scanner.now.is_maybe_name and
-             scanner.next1 is not None and scanner.next1.is_dot and
-             scanner.next2 is not None and scanner.next2.is_maybe_name and
-             (scanner.next3 is None or not scanner.next3.is_parenthesis))
-    )
-
-
-def parse_column_name_expression(scanner: TokenScanner) -> SQLColumnNameExpression:
-    """解析列名表达式
-
-    Examples
-    --------
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTOther source=schema>, <ASTCommon source=.>, <ASTOther source=function>, <ASTParenthesis children=[<ASTOther source=param>]>, <ASTCommon source=AND>], pos=0>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTIdentifier source=`schema`>, <ASTCommon source=.>, <ASTIdentifier source=`function`>, <ASTParenthesis children=[<ASTOther source=param>]>, <ASTCommon source=AND>], pos=0>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.column AND"), ignore_space=True))
-    <SQLColumnNameExpression source=schema.column>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`column` AND"), ignore_space=True))
-    <SQLColumnNameExpression source=`schema`.`column`>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTOther source=trim>, <ASTParenthesis children=[<ASTOther source=column_name>]>, <ASTCommon source=AND>], pos=0>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTLiteralFloat source=2.5>, <ASTOther source=WHERE>], pos=0>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("column_name WHERE"), ignore_space=True))
-    <SQLColumnNameExpression source=coumn_name>
-    """
-    if (scanner.now.is_maybe_name and
-            (scanner.next1 is None or (not scanner.next1.is_dot and not scanner.next1.is_parenthesis))):
-        return SQLColumnNameExpression(None, scanner.pop_as_source())
-    if (scanner.now.is_maybe_name and
-            scanner.next1 is not None and scanner.next1.is_dot and
-            scanner.next2 is not None and scanner.next2.is_maybe_name and
-            (scanner.next3 is None or not scanner.next3.is_parenthesis)):
-        table_name = scanner.pop_as_source()
-        scanner.pop()
-        column_name = scanner.pop_as_source()
-        return SQLColumnNameExpression(table_name, column_name)
-    raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+    如需替换词法解析器，重写 build_token_scanner 方法即可
+    """
+
+    @classmethod
+    def build_token_scanner(cls, string: str) -> TokenScanner:
+        """构造词法扫描器"""
+        context_automaton = ASTParser(string)
+        context_automaton.parse()
+        return TokenScanner(context_automaton.result(), ignore_space=True, ignore_comment=True)
+
+    @classmethod
+    def _unify_input_scanner(cls, scanner_or_string: Union[TokenScanner, str]) -> TokenScanner:
+        """格式化输入的参数，将字符串格式的 SQL 语句统一为词法扫描器 TokenScanner"""
+        if isinstance(scanner_or_string, TokenScanner):
+            return scanner_or_string
+        if isinstance(scanner_or_string, str):
+            # 兼容 DB2 的 CURRENT DATE、CURRENT TIME、CURRENT TIMESTAMP 语法
+            scanner_or_string = scanner_or_string.replace("CURRENT DATE", "CURRENT_DATE")
+            scanner_or_string = scanner_or_string.replace("CURRENT TIME", "CURRENT_TIME")
+            scanner_or_string = scanner_or_string.replace("CURRENT TIMESTAMP", "CURRENT_TIMESTAMP")
+            return cls.build_token_scanner(scanner_or_string)
+        raise SqlParseError(f"未知的参数类型: {scanner_or_string} (type={type(scanner_or_string)})")
+
+    @classmethod
+    def check_insert_type(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为插入类型"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search_and_move("INSERT", "INTO") or scanner.search_and_move("INSERT", "OVERWRITE")
+
+    @classmethod
+    def parse_insert_type(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLInsertType:
+        """解析插入类型"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if scanner.search_and_move("INSERT", "INTO"):
+            return SQLInsertType(insert_type=EnumInsertType.INSERT_INTO)
+        if scanner.search_and_move("INSERT", "OVERWRITE"):
+            return SQLInsertType(insert_type=EnumInsertType.INSERT_OVERWRITE)
+        raise SqlParseError(f"未知的 INSERT 类型: {scanner}")
+
+    @classmethod
+    def check_join_type(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为关联类型"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        for join_type in EnumJoinType:
+            if scanner.search(*join_type.value):
+                return True
+        return False
+
+    @classmethod
+    def parse_join_type(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinType:
+        """解析关联类型"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        for join_type in EnumJoinType:
+            if scanner.search_and_move(*join_type.value):
+                return SQLJoinType(join_type=join_type)
+        raise SqlParseError(f"无法解析的关联类型: {scanner}")
+
+    @classmethod
+    def check_order_type(cls) -> bool:
+        """判断是否为排序类型：任何元素都可以是排序类型（省略升序），所以均返回 True"""
+        return True
+
+    @classmethod
+    def parse_order_type(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLOrderType:
+        """解析排序类型"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if scanner.search_and_move("DESC"):
+            return SQLOrderType(order_type=EnumOrderType.DESC)
+        if scanner.search_and_move("ASC"):
+            return SQLOrderType(order_type=EnumOrderType.ASC)
+        return SQLOrderType(order_type=EnumOrderType.ASC)
+
+    @classmethod
+    def check_union_type(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为组合类型"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        for union_type in EnumUnionType:
+            if scanner.search(*union_type.value):
+                return True
+        return False
+
+    @classmethod
+    def parse_union_type(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLUnionType:
+        """解析组合类型"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        for union_type in EnumUnionType:
+            if scanner.search_and_move(*union_type.value):
+                return SQLUnionType(union_type=union_type)
+        raise SqlParseError(f"无法解析的组合类型: {scanner}")
+
+    @classmethod
+    def check_compare_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为比较运算符"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.get_as_source() in {"=", "!=", "<>", "<", "<=", ">", ">="}
+
+    @classmethod
+    def parse_compare_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLCompareOperator:
+        """解析比较运算符"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        compare_operator_hash = {
+            "=": EnumCompareOperator.EQUAL_TO,
+            "<": EnumCompareOperator.LESS_THAN,
+            "<=": EnumCompareOperator.LESS_THAN_OR_EQUAL,
+            ">": EnumCompareOperator.GREATER_THAN,
+            ">=": EnumCompareOperator.GREATER_THAN_OR_EQUAL,
+            "!=": EnumCompareOperator.NOT_EQUAL_TO,
+            "<>": EnumCompareOperator.NOT_EQUAL_TO
+        }
+        compare_operator = compare_operator_hash.get(scanner.pop_as_source())
+        if compare_operator is not None:
+            return SQLCompareOperator(compare_operator=compare_operator)
+        raise SqlParseError(f"无法解析的比较运算符: {scanner}")
+
+    @classmethod
+    def check_compute_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为计算运算符"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        for compute_operator in EnumComputeOperator:
+            if scanner.search(compute_operator.value):
+                return True
+        return False
+
+    @classmethod
+    def parse_compute_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLComputeOperator:
+        """解析计算运算符"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        for compute_operator in EnumComputeOperator:
+            if scanner.search_and_move(compute_operator.value):
+                return SQLComputeOperator(compute_operator=compute_operator)
+        raise SqlParseError(f"无法解析的计算运算符: {scanner}")
+
+    @classmethod
+    def check_logical_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为逻辑运算符"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.get_as_source() in {"AND", "OR"}
+
+    @classmethod
+    def parse_logical_operator(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLLogicalOperator:
+        """解析逻辑运算符"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        for logical_operator in EnumLogicalOperator:
+            if scanner.search_and_move(logical_operator.value):
+                return SQLLogicalOperator(logical_operator=logical_operator)
+        raise SqlParseError(f"无法解析的逻辑运算符: {scanner}")
+
+    @classmethod
+    def check_literal_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search(ASTMark.LITERAL) or scanner.search("-")
+
+    @classmethod
+    def parse_literal_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLLiteralExpression:
+        """解析字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        token: AST = scanner.pop()
+        if isinstance(token, ASTLiteralInteger):
+            return SQLLiteralIntegerExpression(value=token.literal_value)
+        if isinstance(token, ASTLiteralFloat):
+            return SQLLiteralFloatExpression(value=token.literal_value)
+        if isinstance(token, ASTLiteralString):
+            return SQLLiteralStringExpression(value=token.literal_value)
+        if isinstance(token, ASTLiteralHex):
+            return SQLLiteralHexExpression(value=token.literal_value)
+        if isinstance(token, ASTLiteralBool):
+            return SQLLiteralBoolExpression(value=token.literal_value)
+        if isinstance(token, ASTLiteralBit):
+            return SQLLiteralBitExpression(value=token.literal_value)
+        if isinstance(token, ASTLiteralNull):
+            return SQLLiteralNullExpression()
+        if token.equals("-") and isinstance(scanner.now, ASTLiteralInteger):
+            next_token = scanner.pop()
+            return SQLLiteralIntegerExpression(value=-next_token.literal_value)
+        if token.equals("-") and isinstance(scanner.now, ASTLiteralFloat):
+            next_token = scanner.pop()
+            return SQLLiteralFloatExpression(value=-next_token.literal_value)
+        raise SqlParseError(f"未知的字面值: {token}")
+
+    @classmethod
+    def check_column_name_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """是否可能为列名表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return not scanner.is_finish and (
+                (scanner.now.equals(ASTMark.NAME) and
+                 (scanner.next1 is None or (
+                         not scanner.next1.equals(".") and not scanner.next1.equals(ASTMark.PARENTHESIS)))) or
+                (scanner.now.equals(ASTMark.NAME) and
+                 scanner.next1 is not None and scanner.next1.equals(".") and
+                 scanner.next2 is not None and scanner.next2.equals(ASTMark.NAME) and
+                 (scanner.next3 is None or not scanner.next3.equals(ASTMark.PARENTHESIS)))
+        )
 
+    @classmethod
+    def parse_column_name_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLColumnNameExpression:
+        """解析列名表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if (scanner.search(ASTMark.NAME, ".", ASTMark.NAME) and
+                not scanner.search(ASTMark.NAME, ".", ASTMark.NAME, ASTMark.PARENTHESIS)):
+            table_name = scanner.pop_as_source()
+            scanner.pop()
+            column_name = scanner.pop_as_source()
+            return SQLColumnNameExpression(table=table_name, column=column_name)
+        if scanner.search(ASTMark.NAME) and not scanner.search(ASTMark.NAME, ASTMark.PARENTHESIS):
+            return SQLColumnNameExpression(column=scanner.pop_as_source())
+        raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+
+    @classmethod
+    def check_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """是否可能为函数表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return (scanner.search(ASTMark.NAME, ASTMark.PARENTHESIS) or
+                scanner.search(ASTMark.NAME, ".", ASTMark.NAME, ASTMark.PARENTHESIS))
+
+    @classmethod
+    def parse_cast_data_type(cls, scanner_or_string: Union[TokenScanner, str]) -> EnumCastDataType:
+        """解析 CAST 函数表达式中的类型"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        for cast_type in EnumCastDataType:
+            if scanner.search_and_move(cast_type.value):
+                return cast_type
+        raise SqlParseError(f"无法解析的 CAST 函数表达式中的类型: {scanner}")
+
+    @classmethod
+    def parse_cast_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLCastFunctionExpression:
+        """解析 CAST 函数表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        column_expression = cls.parse_general_expression(scanner)
+        scanner.match("AS")
+        signed = scanner.search_and_move("SIGNED")
+        cast_type = cls.parse_cast_data_type(scanner)
+        if scanner.search(ASTMark.PARENTHESIS):
+            parenthesis_scanner = scanner.pop_as_children_scanner()
+            cast_params: Optional[List[SQLGeneralExpression]] = []
+            for param_scanner in parenthesis_scanner.split_by(","):
+                cast_params.append(cls.parse_general_expression(param_scanner))
+                param_scanner.close()
+        else:
+            cast_params = None
+        scanner.close()
+        cast_data_type = SQLCastDataType(signed=signed, data_type=cast_type, params=cast_params)
+        return SQLCastFunctionExpression(column_expression=column_expression, cast_type=cast_data_type)
+
+    @classmethod
+    def parse_extract_function_expression(cls,
+                                          scanner_or_string: Union[TokenScanner, str]) -> SQLExtractFunctionExpression:
+        """解析 EXTRACT 函数表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        extract_name = cls.parse_general_expression(scanner)
+        scanner.match("FROM")
+        column_expression = cls.parse_general_expression(scanner)
+        scanner.close()
+        return SQLExtractFunctionExpression(extract_name=extract_name, column_expression=column_expression)
+
+    @classmethod
+    def parse_if_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLNormalFunctionExpression:
+        """解析 IF 函数表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        function_params: List[SQLGeneralExpression] = []
+        first_param = True
+        for param_scanner in scanner.split_by(","):
+            if first_param is True:
+                function_params.append(cls.parse_condition_expression(param_scanner))
+                first_param = False
+            else:
+                function_params.append(cls.parse_general_expression(param_scanner))
+            param_scanner.close()
+        return SQLNormalFunctionExpression(function_name="IF", function_params=function_params)
+
+    @classmethod
+    def parse_function_name(cls, scanner_or_string: Union[TokenScanner, str]) -> Tuple[Optional[str], str]:
+        """解析函数表达式函数的 schema 名和 function 名"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if scanner.search(ASTMark.NAME, ASTMark.PARENTHESIS):
+            return None, scanner.pop_as_source()
+        if scanner.search(ASTMark.NAME, ".", ASTMark.NAME, ASTMark.PARENTHESIS):
+            schema_name = scanner.pop_as_source()
+            scanner.pop()
+            return schema_name, scanner.pop_as_source()
+        raise SqlParseError(f"无法解析为函数表达式: {scanner}")
 
-def check_function_expression(scanner: TokenScanner) -> bool:
-    """是否可能为函数表达式
+    @classmethod
+    def parse_function_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> Union[SQLFunctionExpression]:
+        """解析函数表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        schema_name, function_name = cls.parse_function_name(scanner)
+
+        if function_name.upper() == "CAST":
+            return cls.parse_cast_function_expression(scanner.pop_as_children_scanner())
+        if function_name.upper() == "EXTRACT":
+            return cls.parse_extract_function_expression(scanner.pop_as_children_scanner())
+        if function_name.upper() == "IF":
+            return cls.parse_if_function_expression(scanner.pop_as_children_scanner())
 
-    Examples
-    --------
-    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
-    True
-    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
-    True
-    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
-    True
-    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
-    False
-    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("column_name WHERE"), ignore_space=True))
-    False
-    """
-    return not scanner.is_finish and (
-            (scanner.now.is_maybe_name and
-             scanner.next1 is not None and scanner.next1.is_parenthesis) or
-            (scanner.now.is_maybe_name and
-             scanner.next1 is not None and scanner.next1.is_dot and
-             scanner.next2 is not None and scanner.next2.is_maybe_name and
-             scanner.next3 is not None and scanner.next3.is_parenthesis
-             ))
-
-
-def parse_cast_data_type(scanner: TokenScanner) -> EnumCastDataType:
-    """解析 CAST 函数表达式中的类型"""
-    for cast_type in EnumCastDataType:
-        if scanner.search_and_move(cast_type.value):
-            return cast_type
-    raise SqlParseError(f"无法解析的 CAST 函数表达式中的类型: {scanner}")
-
-
-def parse_cast_function_expression(scanner: TokenScanner) -> SQLCastFunctionExpression:
-    """解析 CAST 函数表达式"""
-    column_expression = parse_general_expression(scanner)
-    scanner.match("AS")
-    signed = scanner.search_and_move("SIGNED")
-    cast_type = parse_cast_data_type(scanner)
-    if not scanner.is_finish and scanner.now_is_parenthesis:
         parenthesis_scanner = scanner.pop_as_children_scanner()
-        cast_params: Optional[List[SQLGeneralExpression]] = []
+        if function_name.upper() == "SUBSTRING":
+            # 将 MySQL 和 PostgreSQL 中的 "SUBSTRING(str1 FROM 3 FOR 2)" 格式化为 "SUBSTRING(str1, 3, 2)"
+            parenthesis_scanner = TokenScanner([
+                element if not element.equals("FROM") and not element.equals("FOR") else ASTSingle(",")
+                for element in parenthesis_scanner.elements])
+
+        is_distinct = False
+        if function_name.upper() in AGGREGATION_FUNCTION_NAME_SET and parenthesis_scanner.search_and_move("DISTINCT"):
+            is_distinct = True
+
+        function_params: List[SQLGeneralExpression] = []
         for param_scanner in parenthesis_scanner.split_by(","):
-            cast_params.append(parse_general_expression(param_scanner))
+            function_params.append(cls.parse_general_expression(param_scanner))
             if not param_scanner.is_finish:
                 raise SqlParseError(f"无法解析函数参数: {param_scanner}")
-    else:
-        cast_params = None
-    if not scanner.is_finish:
-        raise SqlParseError(f"无法解析CAST函数参数: {scanner}")
-    cast_data_type = SQLCastDataType(signed=signed, data_type=cast_type, params=cast_params)
-    return SQLCastFunctionExpression(column_expression=column_expression, cast_type=cast_data_type)
-
-
-def parse_extract_function_expression(parenthesis_scanner: TokenScanner) -> SQLExtractFunctionExpression:
-    """解析 EXTRACT 函数表达式"""
-    extract_name = parse_general_expression(parenthesis_scanner)
-    parenthesis_scanner.match("FROM")
-    column_expression = parse_general_expression(parenthesis_scanner)
-    if not parenthesis_scanner.is_finish:
-        raise SqlParseError(f"无法解析EXTRACT函数参数: {parenthesis_scanner}")
-    return SQLExtractFunctionExpression(extract_name=extract_name, column_expression=column_expression)
-
-
-def parse_if_function_expression(parenthesis_scanner: TokenScanner) -> SQLFunctionExpression:
-    """解析 IF 函数表达式"""
-    function_params: List[SQLGeneralExpression] = []
-    first_param = True
-    for param_scanner in parenthesis_scanner.split_by(","):
-        if first_param is True:
-            function_params.append(parse_condition_expression(param_scanner))
-            first_param = False
-        else:
-            function_params.append(parse_general_expression(param_scanner))
-        if not param_scanner.is_finish:
-            raise SqlParseError(f"无法解析函数参数: {param_scanner}")
-    return SQLFunctionExpression(schema_name=None, function_name="IF", function_params=function_params)
-
-
-def parse_function_name(scanner: TokenScanner) -> Tuple[Optional[str], str]:
-    """解析函数表达式函数的 schema 名和 function 名"""
-    if (scanner.now.is_maybe_name and
-            scanner.next1 is not None and scanner.next1.is_parenthesis):
-        return None, scanner.pop_as_source()
-    if (scanner.now.is_maybe_name and
-            scanner.next1 is not None and scanner.next1.is_dot and
-            scanner.next2 is not None and scanner.next2.is_maybe_name and
-            scanner.next3 is not None and scanner.next3.is_parenthesis):
-        schema_name = scanner.pop_as_source()
-        scanner.pop()
-        return schema_name, scanner.pop_as_source()
-    raise SqlParseError(f"无法解析为函数表达式: {scanner}")
-
-
-def parse_function_expression(scanner: TokenScanner) -> SQLFunctionExpression:
-    """解析函数表达式
-
-    Examples
-    --------
-    >>> parse_function_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
-    <SQLFunctionExpression source=schema.function(<SQLColumnNameExpression source=param>)>
-    >>> parse_function_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
-    <SQLFunctionExpression source=`schema`.`function`(<SQLColumnNameExpression source=param>)>
-    >>> parse_function_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
-    <SQLFunctionExpression source=trim(<SQLColumnNameExpression source=column_name>)>
-    >>> parse_function_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为函数表达式: <TokenScanner tokens=[<ASTLiteralFloat source=2.5>, <ASTOther source=WHERE>], pos=0>
-    >>> parse_function_expression(TokenScanner(ast.parse_as_tokens("column_name WHERE"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为函数表达式: <TokenScanner tokens=[<ASTOther source=coumn_name>, <ASTOther source=WHERE>], pos=0>
-    """
-    schema_name, function_name = parse_function_name(scanner)
 
-    if function_name.upper() == "CAST":
-        return parse_cast_function_expression(scanner.pop_as_children_scanner())
-    if function_name.upper() == "EXTRACT":
-        return parse_extract_function_expression(scanner.pop_as_children_scanner())
-    if function_name.upper() == "IF":
-        return parse_if_function_expression(scanner.pop_as_children_scanner())
-
-    parenthesis_scanner = scanner.pop_as_children_scanner()
-    if function_name.upper() == "SUBSTRING":
-        # 将 MySQL 和 PostgreSQL 中的 "SUBSTRING(str1 FROM 3 FOR 2)" 格式化为 "SUBSTRING(str1, 3, 2)"
-        parenthesis_scanner = TokenScanner([
-            element if not element.equals("FROM") and not element.equals("FOR") else ast.ASTComma()
-            for element in parenthesis_scanner.elements])
-
-    is_distinct = False
-    if function_name.upper() in {"COUNT", "SUM", "MIN", "MAX", "AVG"} and parenthesis_scanner.now.equals("DISTINCT"):
-        parenthesis_scanner.pop()
-        is_distinct = True
-
-    function_params: List[SQLGeneralExpression] = []
-    for param_scanner in parenthesis_scanner.split_by(","):
-        function_params.append(parse_general_expression(param_scanner))
-        if not param_scanner.is_finish:
-            raise SqlParseError(f"无法解析函数参数: {param_scanner}")
-
-    if schema_name is None and function_name.upper() in {"COUNT", "SUM", "MIN", "MAX", "AVG"}:
-        return SQLAggregationFunctionExpression(function_name=function_name,
-                                                function_params=function_params,
-                                                is_distinct=is_distinct)
-    else:
-        return SQLFunctionExpression(schema_name=schema_name,
-                                     function_name=function_name,
-                                     function_params=function_params)
-
-
-def parse_bool_expression(scanner: TokenScanner) -> SQLBoolExpression:
-    """解析布尔值表达式
-
-    Examples
-    --------
-    >>> parse_bool_expression(build_token_scanner("column1 > 3"))
-    <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>>
-    >>> parse_bool_expression(build_token_scanner("t2.column1 > 3"))
-    <SQLBoolCompareExpression source=<SQLColumnNameExpression source=t2.column1> <SQLGreaterThan> <SQLLiteralExpression source=3>>
-    >>> parse_bool_expression(build_token_scanner("t2.column1 + 3 > 3"))
-    <SQLBoolCompareExpression source=<SQLComputeExpression source=<SQLColumnNameExpression source=t2.column1> <SQLPlus> <SQLLiteralExpression source=3>> <SQLGreaterThan> <SQLLiteralExpression source=3>>
-    >>> parse_bool_expression(build_token_scanner("column1 BETWEEN 3 AND 4"))
-    <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column1> BETWEEN <SQLLiteralExpression source=3> TO <SQLLiteralExpression source=4>>
-    >>> parse_bool_expression(build_token_scanner("column1 + 3 BETWEEN 3 AND 4"))
-    <SQLBoolBetweenExpression source=<SQLComputeExpression source=<SQLColumnNameExpression source=column1> <SQLPlus> <SQLLiteralExpression source=3>> BETWEEN <SQLLiteralExpression source=3> TO <SQLLiteralExpression source=4>>
-    """
-    if scanner.search_and_move("EXISTS"):
-        after_value = parse_sub_query_expression(scanner)
-        return SQLBoolExistsExpression(is_not=False, after_value=after_value)
-    if scanner.search_and_move("NOT", "EXISTS"):
-        after_value = parse_sub_query_expression(scanner)
-        return SQLBoolExistsExpression(is_not=True, after_value=after_value)
-    before_value = parse_general_expression(scanner)
-    if scanner.search_and_move("BETWEEN"):
-        # "... BETWEEN ... AND ..."
-        from_value = parse_general_expression(scanner)
-        if not scanner.search_and_move("AND"):
-            raise SqlParseError(f"无法解析为 BETWEEN 布尔值表达式: {scanner}")
-        to_value = parse_general_expression(scanner)
-        return SQLBoolBetweenExpression(before_value=before_value, from_value=from_value, to_value=to_value)
-    if scanner.search_and_move("IS"):
-        # ".... IS ...." 或 "... IS NOT ..."
-        if scanner.search_and_move("NOT"):
-            is_not = True
-        else:
-            is_not = False
-        after_value = parse_general_expression(scanner)
-        return SQLBoolIsExpression(is_not=is_not, before_value=before_value, after_value=after_value)
-    if scanner.search_and_move("IN"):
-        # "... IN (1, 2, 3)" 或 "... IN (SELECT ... )"
-        after_value = _parse_in_parenthesis(scanner)
-        return SQLBoolInExpression(is_not=False, before_value=before_value, after_value=after_value)
-    if scanner.search_and_move("NOT", "IN"):
-        after_value = _parse_in_parenthesis(scanner)
-        return SQLBoolInExpression(is_not=True, before_value=before_value, after_value=after_value)
-    if scanner.search_and_move("LIKE"):
-        after_value = parse_general_expression(scanner)
-        return SQLBoolLikeExpression(is_not=False, before_value=before_value, after_value=after_value)
-    if scanner.search_and_move("NOT LIKE"):
-        after_value = parse_general_expression(scanner)
-        return SQLBoolLikeExpression(is_not=True, before_value=before_value, after_value=after_value)
-    if check_compare_operator(scanner):
-        # "... > ..."
-        compare_operator = parse_compare_operator(scanner)
-        after_value = parse_general_expression(scanner)
-        return SQLBoolCompareExpression(operator=compare_operator, before_value=before_value, after_value=after_value)
-    raise SqlParseError(f"无法解析为布尔值表达式: {scanner}")
-
-
-def check_window_expression(scanner: TokenScanner) -> bool:
-    """判断是否可能为窗口函数
-
-    Examples
-    --------
-    >>> check_window_expression(build_token_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
-    True
-    >>> check_window_expression(build_token_scanner("3 + 5"))
-    False
-    """
-    return not scanner.is_finish and (
-            scanner.now.is_maybe_name and scanner.now.source.upper() in WINDOW_FUNCTION_NAME_SET and
-            scanner.next1 is not None and scanner.next1.is_parenthesis and
-            scanner.next2 is not None and scanner.next2.equals("OVER") and
-            scanner.next3 is not None and scanner.next3.is_parenthesis)
-
-
-def parse_window_expression(scanner: TokenScanner) -> SQLWindowExpression:
-    """解析窗口函数
-
-    TODO 支持 ROW BETWEEN 的语法
-
-    Examples
-    --------
-    >>> parse_window_expression(build_token_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
-    <SQLWindowExpression source=<SQLFunctionExpression source=ROW_NUMBER()> OVER (PARTITION BY <SQLColumnNameExpression source=column1>ORDER BY <SQLColumnNameExpression source=column2>)>
-    >>> parse_window_expression(build_token_scanner("3 + 5"))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为函数表达式: <TokenScanner tokens=[<ASTLiteralInteger source=3>, <ASTCommon source=+>, <ASTLiteralInteger source=5>], pos=0>
-    """
-    window_function = parse_function_expression(scanner)
-    partition_by = None
-    order_by = None
-    if not scanner.pop().equals("OVER"):
-        raise SqlParseError(f"无法解析为窗口表达式: {scanner}")
-    parenthesis_scanner = scanner.pop_as_children_scanner()
-    if parenthesis_scanner.search_and_move("PARTITION", "BY"):
-        partition_by = parse_general_expression(parenthesis_scanner, maybe_window=False)
-    if parenthesis_scanner.search_and_move("ORDER", "BY"):
-        order_by = parse_general_expression(parenthesis_scanner, maybe_window=False)
-    return SQLWindowExpression(window_function=window_function, partition_by=partition_by, order_by=order_by)
-
-
-def check_wildcard_expression(scanner: TokenScanner) -> bool:
-    """判断是否可能为通配符表达式
-
-    Examples
-    --------
-    >>> check_wildcard_expression(build_token_scanner("*"))
-    True
-    >>> check_wildcard_expression(build_token_scanner("t1.*"))
-    True
-    """
-    return not scanner.is_finish and (scanner.now.is_maybe_wildcard or
-                                      (scanner.now.is_maybe_name and
-                                       scanner.next1 is not None and scanner.next1.is_dot and
-                                       scanner.next2 is not None and scanner.next2.is_maybe_wildcard))
-
-
-def parse_wildcard_expression(scanner: TokenScanner) -> SQLWildcardExpression:
-    """解析通配符表达式
-
-    Examples
-    --------
-    >>> parse_wildcard_expression(build_token_scanner("*"))
-    <SQLWildcardExpression source=*>
-    >>> parse_wildcard_expression(build_token_scanner("t1.*"))
-    <SQLWildcardExpression source=t1.*>
-    """
-    if scanner.now.is_maybe_wildcard:
-        scanner.pop()
-        return SQLWildcardExpression(schema=None)
-    if (scanner.now.is_maybe_name and
-            scanner.next1 is not None and scanner.next1.is_dot and
-            scanner.next2 is not None and scanner.next2.is_maybe_wildcard):
-        schema_name = scanner.pop_as_source()
-        scanner.pop()
-        scanner.pop()
-        return SQLWildcardExpression(schema=schema_name)
-    raise SqlParseError("无法解析为通配符表达式")
-
-
-def parse_condition_expression(scanner: TokenScanner) -> SQLConditionExpression:
-    """解析条件表达式
-
-    Examples
-    --------
-    >>> parse_condition_expression(build_token_scanner("column1 > 3 AND column2 > 2 WHERE"))
-    <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>
-    >>> parse_condition_expression(build_token_scanner("column1 > 3 OR column2 > 2 WHERE"))
-    <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>
-    >>> parse_condition_expression(build_token_scanner("column1 > 3 OR column2 BETWEEN 2 AND 4 WHERE"))
-    <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>
-    """
-
-    def parse_single():
-        if scanner.search("NOT"):
-            elements.append(parse_logical_operator(scanner))
-        if scanner.now_is_parenthesis:
-            elements.append(parse_condition_expression(scanner.pop_as_children_scanner()))  # 插入语，子句也应该是一个条件表达式
-        else:
-            elements.append(parse_bool_expression(scanner))
-
-    elements: List[Union["SQLConditionExpression", SQLBoolExpression, SQLLogicalOperator]] = []
-    parse_single()  # 解析第 1 个表达式元素
-    while not scanner.is_finish and scanner.now.source.upper() in {"AND", "OR"}:  # 如果是用 AND 和 OR 连接的多个表达式，则继续解析
-        elements.append(parse_logical_operator(scanner))
-        parse_single()
-
-    return SQLConditionExpression(elements=elements)
-
-
-def check_case_expression(scanner: TokenScanner) -> bool:
-    """判断是否可能为 CASE 表达式
-
-    Examples
-    --------
-    >>> check_case_expression(TokenScanner(ast.parse_as_tokens("CASE WHEN 2 THEN 3 ELSE 4 END"), ignore_space=True))
-    True
-    >>> check_case_expression(TokenScanner(ast.parse_as_tokens("3 + 5"), ignore_space=True))
-    False
-    """
-    return not scanner.is_finish and scanner.now.equals("CASE")
+        parenthesis_scanner.close()
 
+        if schema_name is None and function_name.upper() in AGGREGATION_FUNCTION_NAME_SET:
+            return SQLAggregationFunctionExpression(function_name=function_name,
+                                                    function_params=function_params,
+                                                    is_distinct=is_distinct)
+        return SQLNormalFunctionExpression(schema_name=schema_name, function_name=function_name,
+                                           function_params=function_params)
+
+    @classmethod
+    def parse_function_expression_maybe_with_array_index(
+            cls, scanner_or_string: Union[TokenScanner, str]
+    ) -> Union[SQLFunctionExpression, SQLArrayIndexExpression]:
+        """解析函数表达式，并解析函数表达式后可能包含的数组下标"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        array_expression = cls.parse_function_expression(scanner)
+        if scanner.is_finish or not scanner.search(ASTMark.ARRAY_INDEX):
+            return array_expression
+        idx = int(scanner.pop_as_source().lstrip("[").rstrip("]"))
+        return SQLArrayIndexExpression(array_expression=array_expression, idx=idx)
+
+    @classmethod
+    def parse_bool_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLBoolExpression:
+        """解析布尔值表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        is_not = scanner.search_and_move("NOT")
+        if scanner.search_and_move("EXISTS"):
+            after_value = cls.parse_sub_query_expression(scanner)
+            return SQLBoolExistsExpression(is_not=is_not, after_value=after_value)
+        before_value = cls.parse_general_expression(scanner)
+        is_not = is_not or scanner.search_and_move("NOT")
+        if scanner.search_and_move("BETWEEN"):  # "... BETWEEN ... AND ..."
+            from_value = cls.parse_general_expression(scanner)
+            scanner.match("AND")
+            to_value = cls.parse_general_expression(scanner)
+            return SQLBoolBetweenExpression(is_not=is_not, before_value=before_value, from_value=from_value,
+                                            to_value=to_value)
+        if scanner.search_and_move("IS"):  # ".... IS ...." 或 "... IS NOT ..."
+            is_not = is_not or scanner.search_and_move("NOT")
+            after_value = cls.parse_general_expression(scanner)
+            return SQLBoolIsExpression(is_not=is_not, before_value=before_value, after_value=after_value)
+        if scanner.search_and_move("IN"):  # "... IN (1, 2, 3)" 或 "... IN (SELECT ... )"
+            after_value = cls._parse_in_parenthesis(scanner)
+            return SQLBoolInExpression(is_not=is_not, before_value=before_value, after_value=after_value)
+        if scanner.search_and_move("LIKE"):
+            after_value = cls.parse_general_expression(scanner)
+            return SQLBoolLikeExpression(is_not=is_not, before_value=before_value, after_value=after_value)
+        if cls.check_compare_operator(scanner):  # "... > ..."
+            compare_operator = cls.parse_compare_operator(scanner)
+            after_value = cls.parse_general_expression(scanner)
+            return SQLBoolCompareExpression(is_not=is_not, operator=compare_operator, before_value=before_value,
+                                            after_value=after_value)
+        raise SqlParseError(f"无法解析为布尔值表达式: {scanner}")
+
+    @classmethod
+    def check_window_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否可能为窗口函数"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return not scanner.is_finish and (
+                scanner.now.equals(ASTMark.NAME) and scanner.now.source.upper() in WINDOW_FUNCTION_NAME_SET and
+                scanner.next1 is not None and scanner.next1.equals(ASTMark.PARENTHESIS) and
+                scanner.next2 is not None and scanner.next2.equals("OVER") and
+                scanner.next3 is not None and scanner.next3.equals(ASTMark.PARENTHESIS))
+
+    @classmethod
+    def parse_window_row(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWindowRow:
+        """解析窗口函数行限制中的行"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if scanner.search_and_move("CURRENT", "ROW"):
+            return SQLWindowRow(row_type=EnumWindowRowType.CURRENT_ROW)
+        if scanner.search_and_move("UNBOUNDED"):
+            if scanner.search_and_move("PRECEDING"):
+                return SQLWindowRow(row_type=EnumWindowRowType.PRECEDING, is_unbounded=True)
+            if scanner.search_and_move("FOLLOWING"):
+                return SQLWindowRow(row_type=EnumWindowRowType.FOLLOWING, is_unbounded=True)
+            raise SqlParseError(f"无法解析的窗口函数限制行: {scanner}")
+        row_num = int(scanner.pop_as_source())
+        if scanner.search_and_move("PRECEDING"):
+            return SQLWindowRow(row_type=EnumWindowRowType.PRECEDING, row_num=row_num)
+        if scanner.search_and_move("FOLLOWING"):
+            return SQLWindowRow(row_type=EnumWindowRowType.FOLLOWING, row_num=row_num)
+        raise SqlParseError(f"无法解析的窗口函数限制行: {scanner}")
+
+    @classmethod
+    def parse_window_row_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWindowRowExpression:
+        """解析窗口语句限制行的表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("ROWS", "BETWEEN")
+        from_row = cls.parse_window_row(scanner)
+        scanner.match("AND")
+        to_row = cls.parse_window_row(scanner)
+        return SQLWindowRowExpression(from_row=from_row, to_row=to_row)
+
+    @classmethod
+    def parse_window_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWindowExpression:
+        """解析窗口函数"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        window_function = cls.parse_function_expression_maybe_with_array_index(scanner)
+        partition_by = None
+        order_by = None
+        row_expression = None
+        scanner.match("OVER")
+        parenthesis_scanner = scanner.pop_as_children_scanner()
+        if parenthesis_scanner.search_and_move("PARTITION", "BY"):
+            partition_by = cls.parse_general_expression(parenthesis_scanner, maybe_window=False)
+        if parenthesis_scanner.search_and_move("ORDER", "BY"):
+            order_by = cls.parse_general_expression(parenthesis_scanner, maybe_window=False)
+        if parenthesis_scanner.search("ROWS", "BETWEEN"):
+            row_expression = cls.parse_window_row_expression(parenthesis_scanner)
+        parenthesis_scanner.close()
+        return SQLWindowExpression(window_function=window_function,
+                                   partition_by=partition_by,
+                                   order_by=order_by,
+                                   row_expression=row_expression)
+
+    @classmethod
+    def check_wildcard_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否可能为通配符表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("*") or scanner.search(ASTMark.NAME, ".", "*")
+
+    @classmethod
+    def parse_wildcard_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWildcardExpression:
+        """解析通配符表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if scanner.search_and_move("*"):
+            return SQLWildcardExpression()
+        if scanner.search(ASTMark.NAME, ".", "*"):
+            schema_name = scanner.pop_as_source()
+            scanner.pop()
+            scanner.pop()
+            return SQLWildcardExpression(schema=schema_name)
+        raise SqlParseError("无法解析为通配符表达式")
 
-def parse_case_expression(scanner: TokenScanner) -> Union[SQLCaseExpression, SQLCaseValueExpression]:
-    """解析 CASE 表达式
+    @classmethod
+    def parse_condition_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLConditionExpression:
+        """解析条件表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+
+        def parse_single():
+            if scanner.search(ASTMark.PARENTHESIS):
+                parenthesis_scanner = scanner.pop_as_children_scanner()
+                elements.append(cls.parse_condition_expression(parenthesis_scanner))  # 插入语，子句也应该是一个条件表达式
+                parenthesis_scanner.close()
+            else:
+                elements.append(cls.parse_bool_expression(scanner))
 
-    Examples
-    --------
-    >>> parse_case_expression(build_token_scanner("CASE WHEN 2 THEN 3 ELSE 4 END"))
-    <SQLCaseExpression source=CASE
-        WHEN <SQLLiteralExpression source=2> THEN <SQLLiteralExpression source=3>
-        ELSE <SQLLiteralExpression source=4>
-    END>
-    >>> parse_case_expression(build_token_scanner("3 + 5"))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为CASE表达式: <TokenScanner tokens=[<ASTLiteralInteger source=3>, <ASTCommon source=+>, <ASTLiteralInteger source=5>], pos=1>
-    """
-    scanner.match("CASE")
-    if scanner.search("WHEN"):
-        # 第 1 种格式的 CASE 表达式
-        cases = []
-        else_value = None
-        while scanner.search_and_move("WHEN"):
-            when_expression = parse_condition_expression(scanner)
-            scanner.match("THEN")
-            case_expression = parse_general_expression(scanner)
-            cases.append((when_expression, case_expression))
-        if scanner.search_and_move("ELSE"):
-            else_value = parse_general_expression(scanner)
-        scanner.match("END")
-        return SQLCaseExpression(cases=cases, else_value=else_value)
-    else:
+        elements: List[Union["SQLConditionExpression", SQLBoolExpression, SQLLogicalOperator]] = []
+        parse_single()  # 解析第 1 个表达式元素
+        while not scanner.is_finish and scanner.now.source.upper() in {"AND", "OR"}:  # 如果是用 AND 和 OR 连接的多个表达式，则继续解析
+            elements.append(cls.parse_logical_operator(scanner))
+            parse_single()
+
+        return SQLConditionExpression(elements=elements)
+
+    @classmethod
+    def check_case_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否可能为 CASE 表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("CASE")
+
+    @classmethod
+    def parse_case_expression(cls, scanner_or_string: Union[TokenScanner, str]
+                              ) -> Union[SQLCaseExpression, SQLCaseValueExpression]:
+        """解析 CASE 表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("CASE")
+        if scanner.search("WHEN"):
+            # 第 1 种格式的 CASE 表达式
+            cases = []
+            else_value = None
+            while scanner.search_and_move("WHEN"):
+                when_expression = cls.parse_condition_expression(scanner)
+                scanner.match("THEN")
+                case_expression = cls.parse_general_expression(scanner)
+                cases.append((when_expression, case_expression))
+            if scanner.search_and_move("ELSE"):
+                else_value = cls.parse_general_expression(scanner)
+            scanner.match("END")
+            return SQLCaseExpression(cases=cases, else_value=else_value)
         # 第 2 种格式的 CASE 表达式
-        case_value = parse_general_expression(scanner)
+        case_value = cls.parse_general_expression(scanner)
         cases = []
         else_value = None
         while scanner.search_and_move("WHEN"):
-            when_expression = parse_general_expression(scanner)
+            when_expression = cls.parse_general_expression(scanner)
             scanner.match("THEN")
-            case_expression = parse_general_expression(scanner)
+            case_expression = cls.parse_general_expression(scanner)
             cases.append((when_expression, case_expression))
         if scanner.search_and_move("ELSE"):
-            else_value = parse_general_expression(scanner)
+            else_value = cls.parse_general_expression(scanner)
         scanner.match("END")
         return SQLCaseValueExpression(case_value=case_value, cases=cases, else_value=else_value)
 
-
-def parse_value_expression(scanner: TokenScanner) -> SQLValueExpression:
-    """解析值表达式"""
-    values = []
-    for value_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-        values.append(parse_general_expression(value_scanner))
-    return SQLValueExpression(values=values)
-
-
-def check_sub_query_parenthesis(scanner: TokenScanner) -> bool:
-    """判断是否为子查询的插入语"""
-    parenthesis_scanner: TokenScanner = scanner.get_as_children_scanner()
-    return check_select_statement(parenthesis_scanner)
-
-
-def parse_sub_query_expression(scanner: TokenScanner) -> SQLSubQueryExpression:
-    """解析子查询表达式"""
-    return SQLSubQueryExpression(select_statement=parse_select_statement(scanner.pop_as_children_scanner()))
-
-
-def _parse_in_parenthesis(scanner: TokenScanner) -> SQLGeneralExpression:
-    """解析 IN 关键字后的插入语：插入语可能为子查询或值表达式"""
-    if check_sub_query_parenthesis(scanner):
-        return parse_sub_query_expression(scanner)
-    return parse_value_expression(scanner)
-
-
-def _parse_general_parenthesis(scanner: TokenScanner) -> SQLGeneralExpression:
-    """解析一般表达式中的插入语：插入语可能为一般表达式或子查询"""
-    if check_sub_query_parenthesis(scanner):
-        return parse_sub_query_expression(scanner)
-    return parse_general_expression(scanner.pop_as_children_scanner())
-
-
-def _parse_general_expression_element(scanner: TokenScanner, maybe_window: bool) -> SQLGeneralExpression:
-    """解析一般表达式中的一个元素
-
-    # TODO 将非一般表达式的子类移出一般表达式
-    """
-    if check_case_expression(scanner):
-        return parse_case_expression(scanner)
-    if maybe_window is True and check_window_expression(scanner):
-        return parse_window_expression(scanner)
-    if check_function_expression(scanner):
-        return parse_function_expression(scanner)
-    if check_literal_expression(scanner):
-        return parse_literal_expression(scanner)
-    if check_column_name_expression(scanner):
-        return parse_column_name_expression(scanner)
-    if scanner.now_is_parenthesis:
-        return _parse_general_parenthesis(scanner)
-    if check_wildcard_expression(scanner):
-        return parse_wildcard_expression(scanner)
-    raise SqlParseError(f"未知的一般表达式元素: {scanner}")
-
-
-def parse_general_expression(scanner: TokenScanner, maybe_window: bool = True) -> SQLGeneralExpression:
-    """解析一般表达式"""
-    elements = [_parse_general_expression_element(scanner, maybe_window)]
-    while check_compute_operator(scanner):
-        elements.append(parse_compute_operator(scanner))
-        elements.append(_parse_general_expression_element(scanner, maybe_window))
-    if len(elements) > 1:
+    @classmethod
+    def parse_value_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLValueExpression:
+        """解析值表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        values = []
+        for value_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            values.append(cls.parse_general_expression(value_scanner))
+            value_scanner.close()
+        return SQLValueExpression(values=values)
+
+    @classmethod
+    def check_sub_query_parenthesis(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为子查询的插入语"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return cls.check_select_statement(scanner.get_as_children_scanner())
+
+    @classmethod
+    def parse_sub_query_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLSubQueryExpression:
+        """解析子查询表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        parenthesis_scanner = scanner.pop_as_children_scanner()
+        result = SQLSubQueryExpression(select_statement=cls.parse_select_statement(parenthesis_scanner))
+        parenthesis_scanner.close()
+        return result
+
+    @classmethod
+    def _parse_in_parenthesis(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLGeneralExpression:
+        """解析 IN 关键字后的插入语：插入语可能为子查询或值表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if cls.check_sub_query_parenthesis(scanner):
+            return cls.parse_sub_query_expression(scanner)
+        return cls.parse_value_expression(scanner)
+
+    @classmethod
+    def _parse_general_parenthesis(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLGeneralExpression:
+        """解析一般表达式中的插入语：插入语可能为一般表达式或子查询"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if cls.check_sub_query_parenthesis(scanner):
+            return cls.parse_sub_query_expression(scanner)
+        parenthesis_scanner = scanner.pop_as_children_scanner()
+        result = cls.parse_general_expression(parenthesis_scanner)
+        parenthesis_scanner.close()
+        return result
+
+    @classmethod
+    def parse_general_expression_element(cls, scanner_or_string: Union[TokenScanner, str],
+                                         maybe_window: bool) -> SQLGeneralExpression:
+        """解析一般表达式中的一个元素"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if cls.check_case_expression(scanner):
+            return cls.parse_case_expression(scanner)
+        if maybe_window is True and cls.check_window_expression(scanner):
+            return cls.parse_window_expression(scanner)
+        if cls.check_function_expression(scanner):
+            return cls.parse_function_expression_maybe_with_array_index(scanner)
+        if cls.check_literal_expression(scanner):
+            return cls.parse_literal_expression(scanner)
+        if cls.check_column_name_expression(scanner):
+            return cls.parse_column_name_expression(scanner)
+        if scanner.search(ASTMark.PARENTHESIS):
+            return cls._parse_general_parenthesis(scanner)
+        if cls.check_wildcard_expression(scanner):
+            return cls.parse_wildcard_expression(scanner)
+        raise SqlParseError(f"未知的一般表达式元素: {scanner}")
+
+    @classmethod
+    def parse_general_expression(cls, scanner_or_string: Union[TokenScanner, str],
+                                 maybe_window: bool = True) -> SQLGeneralExpression:
+        """解析一般表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        elements = [cls.parse_general_expression_element(scanner, maybe_window)]
+        while cls.check_compute_operator(scanner):
+            elements.append(cls.parse_compute_operator(scanner))
+            elements.append(cls.parse_general_expression_element(scanner, maybe_window))
+        if len(elements) == 1:
+            return elements[0]  # 如果只有 1 个元素，则返回该元素的表达式
         return SQLComputeExpression(elements=elements)  # 如果超过 1 个元素，则返回计算表达式（多项式）
-    else:
-        return elements[0]  # 如果只有 1 个元素，则返回该元素的表达式
-
-
-def parse_table_name_expression(scanner: TokenScanner) -> Union[SQLTableNameExpression, SQLSubQueryExpression]:
-    """解析表名表达式或子查询表达式
-
-    Examples
-    --------
-    >>> parse_table_name_expression(build_token_scanner("table1.column1 AS t1"))
-    <SQLTableNameExpression source=table1.column1>
-    """
-    if (scanner.now.is_maybe_name and
-            (scanner.next1 is None or (not scanner.next1.is_dot and not scanner.next1.is_parenthesis))):
-        return SQLTableNameExpression(None, scanner.pop_as_source())
-    if (scanner.now.is_maybe_name and
-            scanner.next1 is not None and scanner.next1.is_dot and
-            scanner.next2 is not None and scanner.next2.is_maybe_name and
-            (scanner.next3 is None or not scanner.next3.is_parenthesis)):
-        schema_name = scanner.pop_as_source()
-        scanner.pop()
-        table_name = scanner.pop_as_source()
-        return SQLTableNameExpression(schema_name, table_name)
-    if check_sub_query_parenthesis(scanner):
-        return parse_sub_query_expression(scanner)
-    raise SqlParseError(f"无法解析为表名表达式: {scanner}")
-
-
-def check_alias_expression(scanner: TokenScanner) -> bool:
-    """判断是否可能为别名表达式
-
-    Examples
-    --------
-    >>> check_alias_expression(build_token_scanner("t1"))
-    True
-    >>> check_alias_expression(build_token_scanner("AS t1"))
-    True
-    >>> check_alias_expression(build_token_scanner("WHERE"))
-    False
-    """
-    return not scanner.is_finish and (scanner.now.equals("AS") or scanner.now.is_maybe_name)
-
-
-def parse_alias_expression(scanner: TokenScanner) -> SQLAlisaExpression:
-    """解析别名表达式
-
-    Examples
-    --------
-    >>> parse_alias_expression(build_token_scanner("t1"))
-    <SQLAlisaExpression source=AS t1>
-    >>> parse_alias_expression(build_token_scanner("AS t1"))
-    <SQLAlisaExpression source=AS t1>
-    >>> parse_alias_expression(build_token_scanner("WHERE"))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为别名表达式: <TokenScanner tokens=[<ASTCommon source=WHERE>], pos=0>
-    """
-    scanner.search_and_move("AS")
-    if not scanner.now.is_maybe_name:
-        raise SqlParseError(f"无法解析为别名表达式: {scanner}")
-    return SQLAlisaExpression(alias_name=scanner.pop_as_source())
-
-
-def check_join_expression(scanner: TokenScanner) -> bool:
-    """判断是否为关联表达式"""
-    return scanner.search("ON") or scanner.search("USING")
-
-
-def parse_join_on_expression(scanner: TokenScanner) -> SQLJoinOnExpression:
-    """解析 ON 关联表达式
-
-    Examples
-    --------
-    >>> parse_join_on_expression(build_token_scanner("ON t1.column1 = t2.column2"))
-    <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column2>>>>
-    """
-    if not scanner.search_and_move("ON"):
-        raise SqlParseError(f"无法解析为 ON 关联表达式: {scanner}")
-    return SQLJoinOnExpression(condition=parse_condition_expression(scanner))
-
-
-def parse_join_using_expression(scanner: TokenScanner) -> SQLJoinUsingExpression:
-    """解析 USING 关联表达式
-
-    Examples
-    --------
-    >>> parse_join_using_expression(build_token_scanner("USING(column1, column2)"))
-    <SQLJoinUsingExpression source=<SQLFunctionExpression source=USING(<SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>)>>
-    >>> parse_join_using_expression(build_token_scanner("using(column1, column2)"))
-    <SQLJoinUsingExpression source=<SQLFunctionExpression source=using(<SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>)>>
-    """
-    if not scanner.now.equals("USING"):
-        raise SqlParseError(f"无法解析为 USING 关联表达式: {scanner}")
-    return SQLJoinUsingExpression(using_function=parse_function_expression(scanner))
-
-
-def parse_join_expression(scanner: TokenScanner) -> SQLJoinExpression:
-    """解析关联表达式
-
-    Examples
-    --------
-    >>> parse_join_on_expression(build_token_scanner("ON t1.column1 = t2.column2"))
-    <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column2>>>>
-    >>> parse_join_using_expression(build_token_scanner("USING(column1, column2)"))
-    <SQLJoinUsingExpression source=<SQLFunctionExpression source=USING(<SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>)>>
-    >>> parse_join_using_expression(build_token_scanner("using(column1, column2)"))
-    <SQLJoinUsingExpression source=<SQLFunctionExpression source=using(<SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>)>>
-    """
-    if scanner.search("ON"):
-        return parse_join_on_expression(scanner)
-    if scanner.search("USING"):
-        return parse_join_using_expression(scanner)
-    raise SqlParseError(f"无法解析为关联表达式: {scanner}")
-
-
-def parse_column_type_expression(scanner: TokenScanner) -> SQLColumnTypeExpression:
-    """解析 DDL 的字段类型：要求当前指针位置节点为函数名，下一个节点可能为函数参数也可能不是，解析为 SQLColumnType 对象"""
-    # 解析字段类型名称
-    function_name: str = scanner.pop_as_source()
-
-    # 解析字段类型参数
-    if not scanner.is_finish and scanner.now_is_parenthesis:
-        function_params: List[SQLGeneralExpression] = []
-        for param_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            function_params.append(parse_general_expression(param_scanner))
-        return SQLColumnTypeExpression(function_name, function_params)
-    else:
-        return SQLColumnTypeExpression(function_name, [])
 
-
-def parse_table_expression(scanner: TokenScanner) -> SQLTableExpression:
-    """解析表名表达式
-
-    Examples
-    --------
-    >>> parse_table_expression(build_token_scanner("schema1.table1 AS t1"))
-    <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>
-    """
-    table_name_expression = parse_table_name_expression(scanner)
-    alias_expression = parse_alias_expression(scanner) if check_alias_expression(scanner) else None
-    return SQLTableExpression(table=table_name_expression, alias=alias_expression)
-
-
-def parse_column_expression(scanner: TokenScanner) -> SQLColumnExpression:
-    """解析列名表达式
-
-    Examples
-    --------
-    >>> parse_column_expression(build_token_scanner("table1.column1 AS t1"))
-    <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column1>)> AS <SQLAlisaExpression source=AS t1>>
-    >>> parse_column_expression(build_token_scanner("3 + 5 AS t1"))
-    <SQLColumnExpression source=<SQLComputeExpression source=<SQLLiteralExpression source=3> <SQLPlus> <SQLLiteralExpression source=5>> AS <SQLAlisaExpression source=AS t1>>
-    >>> parse_column_expression(build_token_scanner("TRIM(column1) AS t1"))
-    <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column1>)> AS <SQLAlisaExpression source=AS t1>>
-    """
-    general_expression = parse_general_expression(scanner)
-    alias_expression = parse_alias_expression(scanner) if check_alias_expression(scanner) else None
-    return SQLColumnExpression(column=general_expression, alias=alias_expression)
-
-
-def parse_equal_expression(scanner: TokenScanner) -> SQLEqualExpression:
-    """解析等式表达式"""
-    before_value = parse_general_expression(scanner)
-    scanner.match("=")
-    after_value = parse_general_expression(scanner)
-    return SQLEqualExpression(before_value=before_value, after_value=after_value)
-
-
-def check_partition_expression(scanner: TokenScanner) -> bool:
-    """判断是否可能为分区表达式"""
-    return scanner.search("PARTITION")
-
-
-def parse_partition_expression(scanner: TokenScanner) -> SQLPartitionExpression:
-    """解析分区表达式"""
-    scanner.match("PARTITION")
-    partition_list = []
-    for partition_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-        partition_list.append(parse_equal_expression(partition_scanner))
-    return SQLPartitionExpression(partition_list=partition_list)
-
-
-def check_foreign_key_expression(scanner: TokenScanner) -> bool:
-    """判断是否为外键表达式"""
-    return scanner.search("CONSTRAINT")
-
-
-def parse_foreign_key_expression(scanner: TokenScanner) -> SQLForeignKeyExpression:
-    """解析外键表达式"""
-    scanner.match("CONSTRAINT")
-    constraint_name = scanner.pop_as_source()
-    scanner.match("FOREIGN", "KEY")
-    slave_columns = [column_scanner.pop_as_source()
-                     for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    scanner.match("REFERENCES")
-    master_table_name = scanner.pop_as_source()
-    master_columns = [column_scanner.pop_as_source()
-                      for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return SQLForeignKeyExpression(
-        constraint_name=constraint_name,
-        slave_columns=slave_columns,
-        master_table_name=master_table_name,
-        master_columns=master_columns
-    )
-
-
-def check_primary_index_expression(scanner: TokenScanner) -> bool:
-    """判断是否为主键表达式"""
-    return scanner.search("PRIMARY", "KEY")
-
-
-def parse_primary_index_expression(scanner: TokenScanner) -> SQLPrimaryIndexExpression:
-    """解析主键表达式"""
-    scanner.match("PRIMARY", "KEY")
-    columns = [column_scanner.pop_as_source()
-               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return SQLPrimaryIndexExpression(columns=columns)
-
-
-def check_unique_index_expression(scanner: TokenScanner) -> bool:
-    """判断是否为唯一键表达式"""
-    return scanner.search("UNIQUE", "KEY")
-
-
-def parse_unique_index_expression(scanner: TokenScanner) -> SQLUniqueIndexExpression:
-    """解析唯一键表达式"""
-    scanner.match("UNIQUE", "KEY")
-    name = scanner.pop_as_source()
-    columns = [column_scanner.pop_as_source()
-               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return SQLUniqueIndexExpression(name=name, columns=columns)
-
-
-def check_normal_index_expression(scanner: TokenScanner) -> bool:
-    """判断是否为一般索引表达式"""
-    return scanner.search("KEY")
-
-
-def parse_normal_index_expression(scanner: TokenScanner) -> SQLNormalIndexExpression:
-    """解析一般索引表达式"""
-    scanner.match("KEY")
-    name = scanner.pop_as_source()
-    columns = [column_scanner.pop_as_source()
-               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return SQLNormalIndexExpression(name=name, columns=columns)
-
-
-def check_fulltext_expression(scanner: TokenScanner) -> bool:
-    """判断是否为全文索引表达式"""
-    return scanner.search("FULLTEXT", "KEY")
-
-
-def parse_fulltext_expression(scanner: TokenScanner) -> SQLFulltextIndexExpression:
-    """解析全文索引表达式"""
-    scanner.match("FULLTEXT", "KEY")
-    name = scanner.pop_as_source()
-    columns = [column_scanner.pop_as_source()
-               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return SQLFulltextIndexExpression(name=name, columns=columns)
-
-
-def parse_define_column_expression(scanner: TokenScanner) -> SQLDefineColumnExpression:
-    """解析 DDL 的字段表达式"""
-    # 解析顺序固定的信息
-    column_name = scanner.pop_as_source()
-    column_type = parse_column_type_expression(scanner)
-
-    # 解析顺序可能不定的字段信息
-    comment: Optional[str] = None
-    is_unsigned: bool = False
-    is_zerofill: bool = False
-    character_set: Optional[str] = None
-    collate: Optional[str] = None
-    is_allow_null: bool = False
-    is_not_null: bool = False
-    is_auto_increment: bool = False
-    default: Optional[SQLGeneralExpression] = None
-    on_update: Optional[SQLGeneralExpression] = None
-    while not scanner.is_finish:
-        if scanner.search_and_move("NOT", "NULL"):
-            is_not_null = True
-        elif scanner.search_and_move("NULL"):
-            is_allow_null = True
-        elif scanner.search_and_move("CHARACTER", "SET"):
-            character_set = scanner.pop_as_source()
-        elif scanner.search_and_move("COLLATE"):
-            collate = scanner.pop_as_source()
-        elif scanner.search_and_move("DEFAULT"):
-            default = parse_general_expression(scanner)
-        elif scanner.search_and_move("COMMENT"):
-            comment = scanner.pop_as_source()
-        elif scanner.search_and_move("ON", "UPDATE"):  # ON UPDATE
-            on_update = parse_general_expression(scanner)
-        elif scanner.search_and_move("AUTO_INCREMENT"):
-            is_auto_increment = True
-        elif scanner.search_and_move("UNSIGNED"):
-            is_unsigned = True
-        elif scanner.search_and_move("ZEROFILL"):
-            is_zerofill = True
+    @classmethod
+    def parse_config_name_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLConfigNameExpression:
+        """解析配置名称表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        config_name_list = [scanner.pop_as_source()]
+        while scanner.search_and_move("."):
+            config_name_list.append(scanner.pop_as_source())
+        return SQLConfigNameExpression(config_name=".".join(config_name_list))
+
+    @classmethod
+    def parse_config_value_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLConfigValueExpression:
+        """解析配置值表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return SQLConfigValueExpression(config_value=scanner.pop_as_source())
+
+    @classmethod
+    def parse_table_name_expression(cls, scanner_or_string: Union[TokenScanner, str]
+                                    ) -> Union[SQLTableNameExpression, SQLSubQueryExpression]:
+        """解析表名表达式或子查询表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if (scanner.search(ASTMark.NAME, ".", ASTMark.NAME) and
+                not scanner.search(ASTMark.NAME, ".", ASTMark.NAME, ASTMark.PARENTHESIS)):
+            schema_name = scanner.pop_as_source()
+            scanner.pop()
+            table_name = scanner.pop_as_source()
+            return SQLTableNameExpression(schema=schema_name, table=table_name)
+        if scanner.search(ASTMark.NAME) and not scanner.search(ASTMark.NAME, ASTMark.PARENTHESIS):
+            return SQLTableNameExpression(table=scanner.pop_as_source())
+        if cls.check_sub_query_parenthesis(scanner):
+            return cls.parse_sub_query_expression(scanner)
+        raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+
+    @classmethod
+    def check_alias_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否可能为别名表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return not scanner.is_finish and (scanner.search("AS") or scanner.search(ASTMark.NAME))
+
+    @classmethod
+    def parse_alias_expression(cls, scanner_or_string: Union[TokenScanner, str],
+                               must_has_as_keyword: bool = False) -> SQLAlisaExpression:
+        """解析别名表达式
+
+        Parameters
+        ----------
+        scanner_or_string : str
+            词法扫描器或 SQL 字符串语句
+        must_has_as_keyword : bool, default = False
+            是否必须包含 AS 关键字
+        """
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if must_has_as_keyword is True:
+            scanner.match("AS")
         else:
-            raise SqlParseError(f"无法解析的 DDL 字段表达式的字段属性: {scanner}")
-
-    # 构造 DDL 字段表达式对象
-    return SQLDefineColumnExpression(
-        column_name=column_name,
-        column_type=column_type,
-        comment=comment,
-        is_unsigned=is_unsigned,
-        is_zerofill=is_zerofill,
-        character_set=character_set,
-        collate=collate,
-        is_allow_null=is_allow_null,
-        is_not_null=is_not_null,
-        is_auto_increment=is_auto_increment,
-        default=default,
-        on_update=on_update
-    )
-
-
-def check_select_clause(scanner: TokenScanner) -> bool:
-    """判断是否为 SELECT 子句
-
-    Examples
-    --------
-    >>> check_from_clause(build_token_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
-    True
-    >>> check_from_clause(build_token_scanner("SELECT column1 AS c1"))
-    True
-    >>> check_from_clause(build_token_scanner("FROM table1"))
-    False
-    """
-    return scanner.search("SELECT")
-
-
-def parse_select_clause(scanner: TokenScanner) -> SQLSelectClause:
-    """解析 SELECT 子句
-
-    Examples
-    --------
-    >>> parse_select_clause(build_token_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
-    <SQLSelectClause source=SELECT <SQLColumnExpression source=<SQLColumnNameExpression source=column1> AS <SQLAlisaExpression source=AS c1>>,
-    <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column2>)> AS <SQLAlisaExpression source=AS c2>>>
-    >>> parse_select_clause(build_token_scanner("SELECT DISTINCT column1 AS c1"))
-    <SQLSelectClause source=SELECT DISTINCT <SQLColumnExpression source=<SQLColumnNameExpression source=column1> AS <SQLAlisaExpression source=AS c1>>>
-    """
-
-    scanner.match("SELECT")
-    distinct = scanner.search_and_move("DISTINCT")
-    columns = [parse_column_expression(scanner)]
-    while not scanner.is_finish and scanner.now.is_comma:
-        scanner.pop()
-        columns.append(parse_column_expression(scanner))
-    return SQLSelectClause(distinct=distinct, columns=columns)
-
-
-def check_from_clause(scanner: TokenScanner) -> bool:
-    """判断是否为 FROM 子句
-
-    Examples
-    --------
-    >>> check_from_clause(build_token_scanner("FROM schema1.table1 AS t1"))
-    True
-    >>> check_from_clause(build_token_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
-    True
-    >>> check_from_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
-    False
-    """
-    return scanner.search("FROM")
-
-
-def parse_from_clause(scanner: TokenScanner) -> SQLFromClause:
-    """解析 FROM 子句
-
-    Examples
-    --------
-    >>> parse_from_clause(build_token_scanner("FROM schema1.table1 AS t1"))
-    <SQLFromClause source=FROM <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>>
-    >>> parse_from_clause(build_token_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
-    <SQLFromClause source=FROM <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>, <SQLTableExpression source=<SQLTableNameExpression source=schema2.table2> AS <SQLAlisaExpression source=AS t2>>>
-    """
-    scanner.match("FROM")
-    tables = [parse_table_expression(scanner)]
-    while not scanner.is_finish and scanner.now.is_comma:
-        scanner.pop()
-        tables.append(parse_table_expression(scanner))
-    return SQLFromClause(tables=tables)
-
-
-def check_join_clause(scanner: TokenScanner) -> bool:
-    """判断是否为 JOIN 子句
-
-    Examples
-    --------
-    >>> check_join_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
-    True
-    >>> check_join_clause(build_token_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
-    True
-    >>> check_join_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
-    False
-    """
-    return check_join_type(scanner)
-
-
-def parse_join_clause(scanner: TokenScanner) -> SQLJoinClause:
-    """解析 JOIN 子句
-
-    Examples
-    --------
-    >>> parse_join_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
-    <SQLJoinClause source=LEFT JOIN <SQLTableExpression source=<SQLTableNameExpression source=table2> AS <SQLAlisaExpression source=AS t2>> <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column1>>>>>
-    >>> parse_join_clause(build_token_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
-    <SQLJoinClause source=LEFT JOIN <SQLTableExpression source=<SQLTableNameExpression source=schema2.table2> AS <SQLAlisaExpression source=AS t2>> <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column1>>>>>
-    """
-    join_type = parse_join_type(scanner)
-    table_expression = parse_table_expression(scanner)
-    if check_join_expression(scanner):
-        join_rule = parse_join_expression(scanner)
-    else:
-        join_rule = None
-    return SQLJoinClause(join_type=join_type, table=table_expression, join_rule=join_rule)
-
-
-def check_where_clause(scanner: TokenScanner) -> bool:
-    """判断是否可能为 WHERE 子句
-
-    Examples
-    --------
-    >>> check_where_clause(build_token_scanner("WHERE column1 > 3 AND column2 > 2"))
-    True
-    >>> check_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 > 2"))
-    True
-    >>> check_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
-    True
-    >>> check_where_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
-    False
-    """
-    return scanner.search("WHERE")
-
+            scanner.search_and_move("AS")
+        if not scanner.search(ASTMark.NAME):
+            raise SqlParseError(f"无法解析为别名表达式: {scanner}")
+        return SQLAlisaExpression(name=scanner.pop_as_source())
+
+    @classmethod
+    def check_join_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为关联表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("ON") or scanner.search("USING")
+
+    @classmethod
+    def parse_join_on_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinOnExpression:
+        """解析 ON 关联表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if not scanner.search_and_move("ON"):
+            raise SqlParseError(f"无法解析为 ON 关联表达式: {scanner}")
+        return SQLJoinOnExpression(condition=cls.parse_condition_expression(scanner))
+
+    @classmethod
+    def parse_join_using_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinUsingExpression:
+        """解析 USING 关联表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if not scanner.search("USING"):
+            raise SqlParseError(f"无法解析为 USING 关联表达式: {scanner}")
+        return SQLJoinUsingExpression(using_function=cls.parse_function_expression(scanner))
+
+    @classmethod
+    def parse_join_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinExpression:
+        """解析关联表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if scanner.search("ON"):
+            return cls.parse_join_on_expression(scanner)
+        if scanner.search("USING"):
+            return cls.parse_join_using_expression(scanner)
+        raise SqlParseError(f"无法解析为关联表达式: {scanner}")
+
+    @classmethod
+    def parse_column_type_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLColumnTypeExpression:
+        """解析 DDL 的字段类型：要求当前指针位置节点为函数名，下一个节点可能为函数参数也可能不是，解析为 SQLColumnType 对象"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+
+        # 解析字段类型名称
+        function_name: str = scanner.pop_as_source()
+
+        # 解析字段类型参数
+        if scanner.search(ASTMark.PARENTHESIS):
+            function_params: List[SQLGeneralExpression] = []
+            for param_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+                function_params.append(cls.parse_general_expression(param_scanner))
+                param_scanner.close()
+            return SQLColumnTypeExpression(name=function_name, params=function_params)
+        return SQLColumnTypeExpression(name=function_name)
+
+    @classmethod
+    def parse_table_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLTableExpression:
+        """解析表名表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        table_name_expression = cls.parse_table_name_expression(scanner)
+        alias_expression = cls.parse_alias_expression(scanner) if cls.check_alias_expression(scanner) else None
+        return SQLTableExpression(table=table_name_expression, alias=alias_expression)
+
+    @classmethod
+    def parse_column_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLColumnExpression:
+        """解析列名表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        general_expression = cls.parse_general_expression(scanner)
+        alias_expression = cls.parse_alias_expression(scanner) if cls.check_alias_expression(scanner) else None
+        return SQLColumnExpression(column=general_expression, alias=alias_expression)
+
+    @classmethod
+    def parse_equal_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLEqualExpression:
+        """解析等式表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        before_value = cls.parse_general_expression(scanner)
+        scanner.match("=")
+        after_value = cls.parse_general_expression(scanner)
+        return SQLEqualExpression(before_value=before_value, after_value=after_value)
+
+    @classmethod
+    def check_partition_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否可能为分区表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("PARTITION")
+
+    @classmethod
+    def parse_partition_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLPartitionExpression:
+        """解析分区表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("PARTITION")
+        partition_list = []
+        for partition_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            partition_list.append(cls.parse_equal_expression(partition_scanner))
+            partition_scanner.close()
+        return SQLPartitionExpression(partition_list=partition_list)
+
+    @classmethod
+    def check_foreign_key_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为外键表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("CONSTRAINT")
+
+    @classmethod
+    def parse_foreign_key_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLForeignKeyExpression:
+        """解析外键表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("CONSTRAINT")
+        constraint_name = scanner.pop_as_source()
+        scanner.match("FOREIGN", "KEY")
+        slave_columns = []
+        for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            column_scanner.pop_as_source()
+            column_scanner.close()
+        scanner.match("REFERENCES")
+        master_table_name = scanner.pop_as_source()
+        master_columns = []
+        for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            column_scanner.pop_as_source()
+            column_scanner.close()
+        return SQLForeignKeyExpression(
+            constraint_name=constraint_name,
+            slave_columns=slave_columns,
+            master_table_name=master_table_name,
+            master_columns=master_columns
+        )
 
-def parse_where_clause(scanner: TokenScanner) -> SQLWhereClause:
-    """解析 WHERE 子句
+    @classmethod
+    def check_primary_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为主键表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("PRIMARY", "KEY")
+
+    @classmethod
+    def parse_primary_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLPrimaryIndexExpression:
+        """解析主键表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("PRIMARY", "KEY")
+        columns = []
+        for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            column_scanner.pop_as_source()
+            column_scanner.close()
+        return SQLPrimaryIndexExpression(columns=columns)
+
+    @classmethod
+    def check_unique_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为唯一键表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("UNIQUE", "KEY")
+
+    @classmethod
+    def parse_unique_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLUniqueIndexExpression:
+        """解析唯一键表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("UNIQUE", "KEY")
+        name = scanner.pop_as_source()
+        columns = []
+        for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            column_scanner.pop_as_source()
+            column_scanner.close()
+        return SQLUniqueIndexExpression(name=name, columns=columns)
+
+    @classmethod
+    def check_normal_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为一般索引表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("KEY")
+
+    @classmethod
+    def parse_normal_index_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLNormalIndexExpression:
+        """解析一般索引表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("KEY")
+        name = scanner.pop_as_source()
+        columns = []
+        for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            column_scanner.pop_as_source()
+            column_scanner.close()
+        return SQLNormalIndexExpression(name=name, columns=columns)
+
+    @classmethod
+    def check_fulltext_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为全文索引表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("FULLTEXT", "KEY")
+
+    @classmethod
+    def parse_fulltext_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLFulltextIndexExpression:
+        """解析全文索引表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("FULLTEXT", "KEY")
+        name = scanner.pop_as_source()
+        columns = []
+        for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            column_scanner.pop_as_source()
+            column_scanner.close()
+        return SQLFulltextIndexExpression(name=name, columns=columns)
+
+    @classmethod
+    def parse_define_column_expression(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLDefineColumnExpression:
+        """解析 DDL 的字段表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        # 解析顺序固定的信息
+        column_name = scanner.pop_as_source()
+        column_type = cls.parse_column_type_expression(scanner)
 
-    Examples
-    --------
-    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 AND column2 > 2"))
-    <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 > 2"))
-    <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
-    <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>>
-    """
-    scanner.match("WHERE")
-    return SQLWhereClause(condition=parse_condition_expression(scanner))
+        # 解析顺序可能不定的字段信息
+        comment: Optional[str] = None
+        is_unsigned: bool = False
+        is_zerofill: bool = False
+        character_set: Optional[str] = None
+        collate: Optional[str] = None
+        is_allow_null: bool = False
+        is_not_null: bool = False
+        is_auto_increment: bool = False
+        default: Optional[SQLGeneralExpression] = None
+        on_update: Optional[SQLGeneralExpression] = None
+        while not scanner.is_finish:
+            if scanner.search_and_move("NOT", "NULL"):
+                is_not_null = True
+            elif scanner.search_and_move("NULL"):
+                is_allow_null = True
+            elif scanner.search_and_move("CHARACTER", "SET"):
+                character_set = scanner.pop_as_source()
+            elif scanner.search_and_move("COLLATE"):
+                collate = scanner.pop_as_source()
+            elif scanner.search_and_move("DEFAULT"):
+                default = cls.parse_general_expression(scanner)
+            elif scanner.search_and_move("COMMENT"):
+                comment = scanner.pop_as_source()
+            elif scanner.search_and_move("ON", "UPDATE"):  # ON UPDATE
+                on_update = cls.parse_general_expression(scanner)
+            elif scanner.search_and_move("AUTO_INCREMENT"):
+                is_auto_increment = True
+            elif scanner.search_and_move("UNSIGNED"):
+                is_unsigned = True
+            elif scanner.search_and_move("ZEROFILL"):
+                is_zerofill = True
+            else:
+                raise SqlParseError(f"无法解析的 DDL 字段表达式的字段属性: {scanner}")
 
+        # 构造 DDL 字段表达式对象
+        return SQLDefineColumnExpression(
+            column_name=column_name,
+            column_type=column_type,
+            comment=comment,
+            is_unsigned=is_unsigned,
+            is_zerofill=is_zerofill,
+            character_set=character_set,
+            collate=collate,
+            is_allow_null=is_allow_null,
+            is_not_null=is_not_null,
+            is_auto_increment=is_auto_increment,
+            default=default,
+            on_update=on_update
+        )
 
-def check_group_by_clause(scanner: TokenScanner) -> bool:
-    """判断是否可能为 GROUP BY 子句
+    @classmethod
+    def check_select_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为 SELECT 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("SELECT")
+
+    @classmethod
+    def parse_select_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLSelectClause:
+        """解析 SELECT 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("SELECT")
+        distinct = scanner.search_and_move("DISTINCT")
+        columns = [cls.parse_column_expression(scanner)]
+        while scanner.search_and_move(","):
+            columns.append(cls.parse_column_expression(scanner))
+        return SQLSelectClause(distinct=distinct, columns=columns)
 
-    Examples
-    --------
-    >>> check_group_by_clause(build_token_scanner("GROUP BY column1, column2"))
-    True
-    >>> check_group_by_clause(build_token_scanner("GROUP BY column1, column2 DESC"))
-    True
-    >>> check_group_by_clause(build_token_scanner("GROUP BY trim(column1) ASC, column2"))
-    True
-    >>> check_group_by_clause(build_token_scanner("WHERE trim(column1) IS NOT NULL"))
-    False
-    """
-    return scanner.search("GROUP", "BY")
+    @classmethod
+    def check_from_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为 FROM 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("FROM")
+
+    @classmethod
+    def parse_from_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLFromClause:
+        """解析 FROM 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("FROM")
+        tables = [cls.parse_table_expression(scanner)]
+        while scanner.search_and_move(","):
+            tables.append(cls.parse_table_expression(scanner))
+        return SQLFromClause(tables=tables)
 
+    @classmethod
+    def check_lateral_view_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为 LATERAL VIEW 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("LATERAL", "VIEW")
+
+    @classmethod
+    def parse_lateral_view_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLLateralViewClause:
+        """解析 LATERAL VIEW 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("LATERAL", "VIEW")
+        function = cls.parse_function_expression(scanner)
+        view_name = scanner.pop_as_source()
+        alias = cls.parse_alias_expression(scanner, must_has_as_keyword=True)
+        return SQLLateralViewClause(function=function, view_name=view_name, alias=alias)
+
+    @classmethod
+    def check_join_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为 JOIN 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return cls.check_join_type(scanner)
+
+    @classmethod
+    def parse_join_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLJoinClause:
+        """解析 JOIN 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        join_type = cls.parse_join_type(scanner)
+        table_expression = cls.parse_table_expression(scanner)
+        if cls.check_join_expression(scanner):
+            join_rule = cls.parse_join_expression(scanner)
+        else:
+            join_rule = None
+        return SQLJoinClause(join_type=join_type, table=table_expression, join_rule=join_rule)
 
-def parse_group_by_clause(scanner: TokenScanner) -> SQLGroupByClause:
-    """解析 GROUP BY 子句
+    @classmethod
+    def check_where_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否可能为 WHERE 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("WHERE")
+
+    @classmethod
+    def parse_where_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLWhereClause:
+        """解析 WHERE 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("WHERE")
+        return SQLWhereClause(condition=cls.parse_condition_expression(scanner))
+
+    @classmethod
+    def check_group_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否可能为 GROUP BY 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("GROUP", "BY")
+
+    @classmethod
+    def parse_group_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLGroupByClause:
+        """解析 GROUP BY 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("GROUP", "BY")
+        if scanner.search_and_move("GROUPING", "SETS"):
+            # 处理 GROUPING SETS 的语法
+            grouping_list = []
+            for grouping_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+                if grouping_scanner.search(ASTMark.PARENTHESIS):
+                    parenthesis_scanner_list = grouping_scanner.pop_as_children_scanner_list_split_by(",")
+                    columns_list = []
+                    for parenthesis_scanner in parenthesis_scanner_list:
+                        cls.parse_general_expression(parenthesis_scanner)
+                        parenthesis_scanner.close()
+                    grouping_list.append(columns_list)
+                else:
+                    grouping_list.append([cls.parse_general_expression(grouping_scanner)])
+                grouping_scanner.close()
+            return SQLGroupingSetsGroupByClause(grouping_list=grouping_list)
 
-    Examples
-    --------
-    >>> parse_group_by_clause(build_token_scanner("GROUP BY column1, column2"))
-    <SQLGroupByClause source=GROUP BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>>
-    >>> parse_group_by_clause(build_token_scanner("GROUP BY column1, column2 DESC"))
-    <SQLGroupByClause source=GROUP BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>>
-    >>> parse_group_by_clause(build_token_scanner("GROUP BY trim(column1) ASC, column2"))
-    <SQLGroupByClause source=GROUP BY <SQLFunctionExpression source=trim(<SQLColumnNameExpression source=column1>)>>
-    """
-    scanner.match("GROUP", "BY")
-    if scanner.search_and_move("GROUPING", "SETS"):
-        grouping_list = []
-        for grouping_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            if grouping_scanner.now_is_parenthesis:
-                parenthesis_scanner_list = grouping_scanner.pop_as_children_scanner_list_split_by(",")
-                columns_list = [parse_general_expression(parenthesis_scanner)
-                                for parenthesis_scanner in parenthesis_scanner_list]
-                grouping_list.append(columns_list)
-            else:
-                grouping_list.append([parse_general_expression(grouping_scanner)])
-        return SQLGroupingSetsGroupByClause(grouping_list=grouping_list)
-    else:
-        columns = [parse_general_expression(scanner)]
-        while not scanner.is_finish and scanner.now.is_comma:
-            scanner.pop()
-            columns.append(parse_general_expression(scanner))
+        # 处理一般的 GROUP BY 的语法
+        columns = [cls.parse_general_expression(scanner)]
+        while scanner.search_and_move(","):
+            columns.append(cls.parse_general_expression(scanner))
         with_rollup = False
         if scanner.search_and_move("WITH", "ROLLUP"):
             with_rollup = True
         return SQLNormalGroupByClause(columns=columns, with_rollup=with_rollup)
 
+    @classmethod
+    def check_having_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """是否可能为 HAVING 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("HAVING")
+
+    @classmethod
+    def parse_having_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLHavingClause:
+        """解析 HAVING 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("HAVING")
+        return SQLHavingClause(condition=cls.parse_condition_expression(scanner))
+
+    @classmethod
+    def check_order_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """是否可能为 ORDER BY 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("ORDER", "BY")
+
+    @classmethod
+    def parse_order_by_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLOrderByClause:
+        """解析 ORDER BY 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+
+        def parse_single():
+            column = cls.parse_general_expression(scanner)
+            order = cls.parse_order_type(scanner)
+            columns.append((column, order))
 
-def check_having_clause(scanner: TokenScanner) -> bool:
-    """是否可能为 HAVING 子句
-
-    Examples
-    --------
-    >>> check_having_clause(build_token_scanner("HAVING column1 > 3 AND column2 > 2"))
-    True
-    >>> check_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 > 2"))
-    True
-    >>> check_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
-    True
-    >>> check_having_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
-    False
-    """
-    return scanner.search("HAVING")
-
-
-def parse_having_clause(scanner: TokenScanner) -> SQLHavingClause:
-    """解析 HAVING 子句
-
-    Examples
-    --------
-    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 AND column2 > 2"))
-    <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 > 2"))
-    <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
-    <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>>
-    """
-    scanner.match("HAVING")
-    return SQLHavingClause(condition=parse_condition_expression(scanner))
-
-
-def check_order_by_clause(scanner: TokenScanner) -> bool:
-    """是否可能为 ORDER BY 子句
-
-    Examples
-    --------
-    >>> check_order_by_clause(build_token_scanner("ORDER BY column1, column2"))
-    True
-    >>> check_order_by_clause(build_token_scanner("ORDER BY column1, column2 DESC"))
-    True
-    >>> check_order_by_clause(build_token_scanner("ORDER BY trim(column1) ASC, column2"))
-    True
-    >>> check_order_by_clause(build_token_scanner("WHERE trim(column1) IS NOT NULL"))
-    False
-    """
-    return scanner.search("ORDER", "BY")
-
-
-def parse_order_by_clause(scanner: TokenScanner) -> SQLOrderByClause:
-    """解析 ORDER BY 子句
-
-    Examples
-    --------
-    >>> parse_order_by_clause(build_token_scanner("ORDER BY column1, column2"))
-    <SQLOrderByClause source=ORDER BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>>
-    >>> parse_order_by_clause(build_token_scanner("ORDER BY column1, column2 DESC"))
-    <SQLOrderByClause source=ORDER BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2> DESC>
-    >>> parse_order_by_clause(build_token_scanner("ORDER BY trim(column1) ASC, column2"))
-    <SQLOrderByClause source=ORDER BY <SQLFunctionExpression source=trim(<SQLColumnNameExpression source=column1>)>>
-    """
-
-    def parse_single():
-        column = parse_general_expression(scanner)
-        order = parse_order_type(scanner)
-        columns.append((column, order))
-
-    scanner.match("ORDER", "BY")
-    columns = []
-    parse_single()
-    while not scanner.is_finish and scanner.now.is_comma:
-        scanner.pop()
+        scanner.match("ORDER", "BY")
+        columns = []
         parse_single()
-
-    return SQLOrderByClause(columns=columns)
-
-
-def check_limit_clause(scanner: TokenScanner) -> bool:
-    """是否可能为 LIMIT 子句
-
-    Examples
-    --------
-    >>> check_limit_clause(build_token_scanner("LIMIT 2, 5"))
-    True
-    >>> check_limit_clause(build_token_scanner("LIMIT 5 OFFSET 2"))
-    True
-    >>> check_limit_clause(build_token_scanner("ORDER BY column1"))
-    False
-    """
-    return scanner.search("LIMIT")
-
-
-def parse_limit_clause(scanner: TokenScanner) -> SQLLimitClause:
-    """解析 LIMIT 子句
-
-    Examples
-    --------
-    >>> parse_limit_clause(build_token_scanner("LIMIT 2, 5"))
-    <SQLLimitClause source=LIMIT 2, 5>
-    >>> parse_limit_clause(build_token_scanner("LIMIT 5 OFFSET 2"))
-    <SQLLimitClause source=LIMIT 2, 5>
-    """
-    if not scanner.search_and_move("LIMIT"):
-        raise SqlParseError("无法解析为 LIMIT 子句")
-    cnt_1 = parse_literal_expression(scanner).as_int()
-    mark = scanner.pop()
-    if mark.is_comma:
-        offset_int = cnt_1
-        limit_int = parse_literal_expression(scanner).as_int()
-    elif mark.equals("OFFSET"):
-        offset_int = parse_literal_expression(scanner).as_int()
-        limit_int = cnt_1
-    else:
-        raise SqlParseError("无法解析为 LIMIT 子句")
-
-    return SQLLimitClause(limit=limit_int, offset=offset_int)
-
-
-def _parse_single_with_table(scanner: TokenScanner) -> Tuple[str, SQLSelectStatement]:
-    """解析一个 WITH 临时表"""
-    table_name = scanner.pop_as_source()
-    scanner.match("AS")
-    table_statement = parse_select_statement(scanner.pop_as_children_scanner(), with_clause=SQLWithClause.empty())
-    return table_name, table_statement
-
-
-def parse_with_clause(scanner: TokenScanner) -> Optional[SQLWithClause]:
-    """解析 WITH 子句"""
-    if scanner.search_and_move("WITH"):
-        tables = [_parse_single_with_table(scanner)]
         while scanner.search_and_move(","):
-            table_statement = _parse_single_with_table(scanner)
-            tables.append(table_statement)  # 将前置的 WITH 作为当前解析临时表的 WITH 子句
-        return SQLWithClause(tables=tables)
-    else:
-        return SQLWithClause.empty()
-
-
-def check_select_statement(scanner: TokenScanner) -> bool:
-    """判断是否可能为 SELECT 语句"""
-    return scanner.search("SELECT")
+            parse_single()
 
+        return SQLOrderByClause(columns=columns)
 
-def parse_single_select_statement(scanner: TokenScanner,
-                                  with_clause: Optional[SQLWithClause] = None
-                                  ) -> SQLSingleSelectStatement:
-    """
+    @classmethod
+    def check_limit_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """是否可能为 LIMIT 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("LIMIT")
+
+    @classmethod
+    def parse_limit_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLLimitClause:
+        """解析 LIMIT 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if not scanner.search_and_move("LIMIT"):
+            raise SqlParseError("无法解析为 LIMIT 子句")
+        cnt_1 = cls.parse_literal_expression(scanner).as_int()
+        if scanner.search_and_move(","):
+            offset_int = cnt_1
+            limit_int = cls.parse_literal_expression(scanner).as_int()
+        elif scanner.search_and_move("OFFSET"):
+            offset_int = cls.parse_literal_expression(scanner).as_int()
+            limit_int = cnt_1
+        else:
+            raise SqlParseError("无法解析为 LIMIT 子句")
+        return SQLLimitClause(limit=limit_int, offset=offset_int)
 
-    Parameters
-    ----------
-    scanner : TokenScanner
-        扫描器
-    with_clause : Optional[SQLWithClause], default = None
-        前置 with 语句，如果该参数为 None 的话，则会尝试匹配 WITH 语句
+    @classmethod
+    def _parse_single_with_table(cls, scanner_or_string: Union[TokenScanner, str]) -> Tuple[str, SQLSelectStatement]:
+        """解析一个 WITH 临时表"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        table_name = scanner.pop_as_source()
+        scanner.match("AS")
+        parenthesis_scanner = scanner.pop_as_children_scanner()
+        table_statement = cls.parse_select_statement(parenthesis_scanner, with_clause=SQLWithClause.empty())
+        parenthesis_scanner.close()
+        return table_name, table_statement
+
+    @classmethod
+    def parse_with_clause(cls, scanner_or_string: Union[TokenScanner, str]) -> Optional[SQLWithClause]:
+        """解析 WITH 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if scanner.search_and_move("WITH"):
+            tables = [cls._parse_single_with_table(scanner)]
+            while scanner.search_and_move(","):
+                table_statement = cls._parse_single_with_table(scanner)
+                tables.append(table_statement)  # 将前置的 WITH 作为当前解析临时表的 WITH 子句
+            return SQLWithClause(tables=tables)
+        return SQLWithClause.empty()
 
-    Returns
-    -------
+    @classmethod
+    def check_select_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否可能为 SELECT 语句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("SELECT")
+
+    @classmethod
+    def parse_single_select_statement(cls, scanner_or_string: Union[TokenScanner, str],
+                                      with_clause: Optional[SQLWithClause] = None
+                                      ) -> SQLSingleSelectStatement:
+        """
+
+        Parameters
+        ----------
+        scanner_or_string : Union[TokenScanner, str]
+            扫描器
+        with_clause : Optional[SQLWithClause], default = None
+            前置 with 语句，如果该参数为 None 的话，则会尝试匹配 WITH 语句
+
+        Returns
+        -------
+
+        """
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if with_clause is None:
+            with_clause = cls.parse_with_clause(scanner)
+        select_clause = cls.parse_select_clause(scanner)
+        from_clause = cls.parse_from_clause(scanner) if cls.check_from_clause(scanner) else None
+        lateral_view_clauses = []
+        while cls.check_lateral_view_clause(scanner):
+            lateral_view_clauses.append(cls.parse_lateral_view_clause(scanner))
+        join_clause = []
+        while cls.check_join_clause(scanner):
+            join_clause.append(cls.parse_join_clause(scanner))
+        where_clause = cls.parse_where_clause(scanner) if cls.check_where_clause(scanner) else None
+        group_by_clause = cls.parse_group_by_clause(scanner) if cls.check_group_by_clause(scanner) else None
+        having_clause = cls.parse_having_clause(scanner) if cls.check_having_clause(scanner) else None
+        order_by_clause = cls.parse_order_by_clause(scanner) if cls.check_order_by_clause(scanner) else None
+        limit_clause = cls.parse_limit_clause(scanner) if cls.check_limit_clause(scanner) else None
+        return SQLSingleSelectStatement(
+            with_clause=with_clause,
+            select_clause=select_clause,
+            from_clause=from_clause,
+            lateral_view_clauses=lateral_view_clauses,
+            join_clauses=join_clause,
+            where_clause=where_clause,
+            group_by_clause=group_by_clause,
+            having_clause=having_clause,
+            order_by_clause=order_by_clause,
+            limit_clause=limit_clause
+        )
 
-    """
-    if with_clause is None:
-        with_clause = parse_with_clause(scanner)
-    select_clause = parse_select_clause(scanner)
-    from_clause = parse_from_clause(scanner) if check_from_clause(scanner) else None
-    join_clause = []
-    while check_join_clause(scanner):
-        join_clause.append(parse_join_clause(scanner))
-    where_clause = parse_where_clause(scanner) if check_where_clause(scanner) else None
-    group_by_clause = parse_group_by_clause(scanner) if check_group_by_clause(scanner) else None
-    having_clause = parse_having_clause(scanner) if check_having_clause(scanner) else None
-    order_by_clause = parse_order_by_clause(scanner) if check_order_by_clause(scanner) else None
-    limit_clause = parse_limit_clause(scanner) if check_limit_clause(scanner) else None
-    return SQLSingleSelectStatement(
-        with_clause=with_clause,
-        select_clause=select_clause,
-        from_clause=from_clause,
-        join_clauses=join_clause,
-        where_clause=where_clause,
-        group_by_clause=group_by_clause,
-        having_clause=having_clause,
-        order_by_clause=order_by_clause,
-        limit_clause=limit_clause
-    )
-
-
-def parse_select_statement(scanner: TokenScanner,
-                           with_clause: Optional[SQLWithClause] = None) -> SQLSelectStatement:
-    """解析 SELECT 语句"""
-    if with_clause is None:
-        with_clause = parse_with_clause(scanner)
-    result = [parse_single_select_statement(scanner, with_clause=with_clause)]
-    while not scanner.is_finish and check_union_type(scanner):
-        result.append(parse_union_type(scanner))
-        result.append(parse_single_select_statement(scanner, with_clause=with_clause))
-    scanner.search_and_move(";")
-    if not scanner.is_finish:
-        raise SqlParseError(f"没有解析完成: {scanner}")
+    @classmethod
+    def parse_select_statement(cls, scanner_or_string: Union[TokenScanner, str],
+                               with_clause: Optional[SQLWithClause] = None) -> SQLSelectStatement:
+        """解析 SELECT 语句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        if with_clause is None:
+            with_clause = cls.parse_with_clause(scanner)
+        result = [cls.parse_single_select_statement(scanner, with_clause=with_clause)]
+        while not scanner.is_finish and cls.check_union_type(scanner):
+            result.append(cls.parse_union_type(scanner))
+            result.append(cls.parse_single_select_statement(scanner, with_clause=with_clause))
+        scanner.search_and_move(";")
+        if not scanner.is_finish:
+            raise SqlParseError(f"没有解析完成: {scanner}")
 
-    if len(result) > 1:
+        if len(result) == 1:
+            return result[0]
         return SQLUnionSelectStatement(with_clause=with_clause, elements=result)
-    else:
-        return result[0]
-
 
-def check_insert_statement(scanner: TokenScanner) -> bool:
-    """判断是否为 INSERT 语句（已匹配过 WITH 语句才可以调用）"""
-    return scanner.search("INSERT")
-
-
-def parse_insert_statement(scanner: TokenScanner, with_clause: SQLWithClause) -> SQLInsertStatement:
-    """解析 INSERT 表达式"""
-    insert_type = parse_insert_type(scanner)
-
-    # 匹配可能包含的 TABLE 关键字
-    has_table_keyword = scanner.search_and_move("TABLE")
-
-    # 匹配表名
-    table_name = parse_table_name_expression(scanner)
-
-    # 匹配分区表达式
-    if check_partition_expression(scanner):
-        partition = parse_partition_expression(scanner)
-    else:
-        partition = None
+    @classmethod
+    def check_insert_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为 INSERT 语句（已匹配过 WITH 语句才可以调用）"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("INSERT")
+
+    @classmethod
+    def parse_insert_statement(cls, scanner_or_string: Union[TokenScanner, str],
+                               with_clause: SQLWithClause) -> SQLInsertStatement:
+        """解析 INSERT 表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        insert_type = cls.parse_insert_type(scanner)
+
+        # 匹配可能包含的 TABLE 关键字
+        scanner.search_and_move("TABLE")
+
+        # 匹配表名
+        table_name = cls.parse_table_name_expression(scanner)
+
+        # 匹配分区表达式
+        if cls.check_partition_expression(scanner):
+            partition = cls.parse_partition_expression(scanner)
+        else:
+            partition = None
 
-    # 匹配列名列表
-    if scanner.now_is_parenthesis:
-        columns = []
-        for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            columns.append(parse_column_name_expression(column_scanner))
-            if not column_scanner.is_finish:
-                raise SqlParseError(f"未解析完成的列名: {column_scanner}")
-    else:
-        columns = None
+        # 匹配列名列表
+        if scanner.search(ASTMark.PARENTHESIS):
+            columns = []
+            for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+                columns.append(cls.parse_column_name_expression(column_scanner))
+                column_scanner.close()
+        else:
+            columns = None
 
-    # 匹配 VALUES 类型
-    if scanner.search_and_move("VALUES"):
-        values = []
-        while scanner.now_is_parenthesis:
-            values.append(parse_value_expression(scanner))
-            scanner.search_and_move(",")
+        # 匹配 VALUES 类型
+        if scanner.search_and_move("VALUES"):
+            values = []
+            while scanner.search(ASTMark.PARENTHESIS):
+                values.append(cls.parse_value_expression(scanner))
+                scanner.search_and_move(",")
+
+            return SQLInsertValuesStatement(
+                with_clause=with_clause,
+                insert_type=insert_type,
+                table_name=table_name,
+                partition=partition,
+                columns=columns,
+                values=values
+            )
+
+        if scanner.search("SELECT"):
+            select_statement = cls.parse_select_statement(scanner, with_clause=SQLWithClause.empty())
+            return SQLInsertSelectStatement(
+                with_clause=with_clause,
+                insert_type=insert_type,
+                table_name=table_name,
+                partition=partition,
+                columns=columns,
+                select_statement=select_statement
+            )
+
+        raise SqlParseError(f"未知的 INSERT 语句类型 {scanner}")
+
+    @classmethod
+    def check_set_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> bool:
+        """判断是否为 SET 语句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        return scanner.search("SET")
+
+    @classmethod
+    def parse_set_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLSetStatement:
+        """解析 SET 语句"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("SET")
+        config_name = cls.parse_config_name_expression(scanner)
+        scanner.match("=")
+        config_value = cls.parse_config_value_expression(scanner)
+        return SQLSetStatement(config_name=config_name, config_value=config_value)
+
+    @classmethod
+    def parse_create_table_statement(cls, scanner_or_string: Union[TokenScanner, str]) -> SQLCreateTableStatement:
+        """解析 CREATE TABLE 语句"""
+        # 解析字段、索引括号前的部分
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        scanner.match("CREATE", "TABLE")
+        if_not_exists = scanner.search_and_move("IF", "NOT", "EXISTS")
+        table_name_expression = cls.parse_table_name_expression(scanner)
+
+        # 解析字段和索引
+        columns: List[SQLDefineColumnExpression] = []
+        primary_key: Optional[SQLPrimaryIndexExpression] = None
+        unique_key: List[SQLUniqueIndexExpression] = []
+        key: List[SQLNormalIndexExpression] = []
+        fulltext_key: List[SQLFulltextIndexExpression] = []
+        foreign_key: List[SQLForeignKeyExpression] = []
+        for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            if cls.check_primary_index_expression(group_scanner):
+                primary_key = cls.parse_primary_index_expression(group_scanner)
+            elif cls.check_unique_index_expression(group_scanner):
+                unique_key.append(cls.parse_unique_index_expression(group_scanner))
+            elif cls.check_normal_index_expression(group_scanner):
+                key.append(cls.parse_normal_index_expression(group_scanner))
+            elif cls.check_fulltext_expression(group_scanner):
+                fulltext_key.append(cls.parse_fulltext_expression(group_scanner))
+            elif cls.check_foreign_key_expression(group_scanner):
+                foreign_key.append(cls.parse_foreign_key_expression(group_scanner))
+            else:
+                columns.append(cls.parse_define_column_expression(group_scanner))
+            group_scanner.close()
 
-        return SQLInsertValuesStatement(
-            with_clause=with_clause,
-            insert_type=insert_type,
-            has_table_keyword=has_table_keyword,
-            table_name=table_name,
-            partition=partition,
-            columns=columns,
-            values=values
-        )
+        # 解析表属性
+        comment: Optional[str] = None
+        engine: Optional[str] = None
+        auto_increment: Optional[int] = None
+        default_charset: Optional[str] = None
+        collate: Optional[str] = None
+        row_format: Optional[str] = None
+        states_persistent: Optional[str] = None
+        while not scanner.is_finish:
+            if scanner.search_and_move("ENGINE"):
+                scanner.search_and_move("=")
+                engine = scanner.pop_as_source()
+            elif scanner.search_and_move("AUTO_INCREMENT"):
+                scanner.match("=")
+                auto_increment = int(scanner.pop_as_source())
+            elif scanner.search_and_move("DEFAULT", "CHARSET"):
+                scanner.match("=")
+                default_charset = scanner.pop_as_source()
+            elif scanner.search_and_move("ROW_FORMAT"):
+                scanner.match("=")
+                row_format = scanner.pop_as_source()
+            elif scanner.search_and_move("COLLATE"):
+                scanner.match("=")
+                collate = scanner.pop_as_source()
+            elif scanner.search_and_move("COMMENT"):
+                scanner.match("=")
+                comment = scanner.pop_as_source()
+            elif scanner.search_and_move("STATS_PERSISTENT"):
+                scanner.match("=")
+                states_persistent = scanner.pop_as_source()
+            else:
+                raise SqlParseError(f"未知的 DDL 表属性: {scanner}")
+        scanner.search_and_move(";")
 
-    if scanner.search("SELECT"):
-        select_statement = parse_select_statement(scanner, with_clause=SQLWithClause.empty())
-        return SQLInsertSelectStatement(
-            with_clause=with_clause,
-            insert_type=insert_type,
-            has_table_keyword=has_table_keyword,
-            table_name=table_name,
-            partition=partition,
+        return SQLCreateTableStatement(
+            table_name_expression=table_name_expression,
+            comment=comment,
+            if_not_exists=if_not_exists,
             columns=columns,
-            select_statement=select_statement
+            primary_key=primary_key,
+            unique_key=unique_key,
+            key=key,
+            fulltext_key=fulltext_key,
+            foreign_key=foreign_key,
+            engine=engine,
+            auto_increment=auto_increment,
+            default_charset=default_charset,
+            collate=collate,
+            row_format=row_format,
+            states_persistent=states_persistent,
+            partition_by=[]  # TODO 待支持 Hive 建表语句解析
         )
 
+    @classmethod
+    def parse_statements(cls, scanner_or_string: Union[TokenScanner, str]) -> List[SQLStatement]:
+        """解析一段 SQL 语句，返回表达式的列表"""
+        scanner = cls._unify_input_scanner(scanner_or_string)
+        statement_list = []
+        for statement_scanner in scanner.split_by(";"):
+            # 解析 SET 语句
+            if cls.check_set_statement(statement_scanner):
+                statement_list.append(cls.parse_set_statement(statement_scanner))
+                continue
+
+            # 先尝试解析 WITH 语句
+            with_clause = cls.parse_with_clause(statement_scanner)
+
+            if cls.check_select_statement(statement_scanner):
+                statement_list.append(cls.parse_select_statement(statement_scanner, with_clause=with_clause))
+            elif cls.check_insert_statement(statement_scanner):
+                statement_list.append(cls.parse_insert_statement(statement_scanner, with_clause=with_clause))
+            else:
+                raise SqlParseError(f"未知语句类型: {statement_scanner}")
 
-def parse_create_table_statement(scanner: TokenScanner) -> SQLCreateTableStatement:
-    # 解析字段、索引括号前的部分
-    scanner.match("CREATE", "TABLE")
-    if_not_exists = scanner.search_and_move("IF", "NOT", "EXISTS")
-    table_name = scanner.pop_as_source().strip("`")  # TODO 待改为 TableNameExpression，并支持 schema_name
-
-    # 解析字段和索引
-    columns: List[SQLDefineColumnExpression] = []
-    primary_key: Optional[SQLPrimaryIndexExpression] = None
-    unique_key: List[SQLUniqueIndexExpression] = []
-    key: List[SQLNormalIndexExpression] = []
-    fulltext_key: List[SQLFulltextIndexExpression] = []
-    foreign_key: List[SQLForeignKeyExpression] = []
-    for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-        if check_primary_index_expression(group_scanner):
-            primary_key = parse_primary_index_expression(group_scanner)
-        elif check_unique_index_expression(group_scanner):
-            unique_key.append(parse_unique_index_expression(group_scanner))
-        elif check_normal_index_expression(group_scanner):
-            key.append(parse_normal_index_expression(group_scanner))
-        elif check_fulltext_expression(group_scanner):
-            fulltext_key.append(parse_fulltext_expression(group_scanner))
-        elif check_foreign_key_expression(group_scanner):
-            foreign_key.append(parse_foreign_key_expression(group_scanner))
-        else:
-            columns.append(parse_define_column_expression(group_scanner))
-
-    # 解析表属性
-    comment: Optional[str] = None
-    engine: Optional[str] = None
-    auto_increment: Optional[int] = None
-    default_charset: Optional[str] = None
-    collate: Optional[str] = None
-    row_format: Optional[str] = None
-    states_persistent: Optional[str] = None
-    while not scanner.is_finish:
-        if scanner.search_and_move("ENGINE"):
-            scanner.search_and_move("=")
-            engine = scanner.pop_as_source()
-        elif scanner.search_and_move("AUTO_INCREMENT"):
-            scanner.match("=")
-            auto_increment = int(scanner.pop_as_source())
-        elif scanner.search_and_move("DEFAULT", "CHARSET"):
-            scanner.match("=")
-            default_charset = scanner.pop_as_source()
-        elif scanner.search_and_move("ROW_FORMAT"):
-            scanner.match("=")
-            row_format = scanner.pop_as_source()
-        elif scanner.search_and_move("COLLATE"):
-            scanner.match("=")
-            collate = scanner.pop_as_source()
-        elif scanner.search_and_move("COMMENT"):
-            scanner.match("=")
-            comment = scanner.pop_as_source()
-        elif scanner.search_and_move("STATS_PERSISTENT"):
-            scanner.match("=")
-            states_persistent = scanner.pop_as_source()
-        else:
-            raise SqlParseError(f"未知的 DDL 表属性: {scanner}")
-    scanner.search_and_move(";")
-
-    return SQLCreateTableStatement(
-        table_name=table_name,
-        comment=comment,
-        if_not_exists=if_not_exists,
-        columns=columns,
-        primary_key=primary_key,
-        unique_key=unique_key,
-        key=key,
-        fulltext_key=fulltext_key,
-        foreign_key=foreign_key,
-        engine=engine,
-        auto_increment=auto_increment,
-        default_charset=default_charset,
-        collate=collate,
-        row_format=row_format,
-        states_persistent=states_persistent
-    )
-
-
-def parse_statement(scanner: TokenScanner) -> List[SQLStatement]:
-    """解析一段 SQL 语句，返回表达式的列表
-
-    Examples
-    --------
-    >>> parse_statement(build_token_scanner("SELECT a FROM b; SELECT c FROM d"))
-    [<SQLSingleSelectStatement source=SELECT a
-    FROM b>, <SQLSingleSelectStatement source=SELECT c
-    FROM d>]
-    """
-    statement_list = []
-    for statement_scanner in scanner.split_by(";"):
-        # 先尝试解析 WITH 语句
-        with_clause = parse_with_clause(statement_scanner)
-
-        if check_select_statement(statement_scanner):
-            statement_list.append(parse_select_statement(statement_scanner, with_clause=with_clause))
-        else:
-            raise SqlParseError(f"未知语句类型: {statement_scanner}")
+            statement_scanner.close()
 
-    return statement_list
+        return statement_list
```

### Comparing `metasequoia-sql-0.2.0/metasequoia_sql/errors.py` & `metasequoia-sql-0.3.0/metasequoia_sql/errors.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.2.0/metasequoia_sql/static.py` & `metasequoia-sql-0.3.0/metasequoia_sql/static.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.2.0/metasequoia_sql.egg-info/PKG-INFO` & `metasequoia-sql-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasequoia-sql
-Version: 0.2.0
+Version: 0.3.0
 Summary: SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能
 Home-page: https://github.com/ChangxingJiang/metasequoia-sql
 Author: changxing
 Author-email: 1278729001@qq.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
@@ -24,40 +24,40 @@
 pip install metasequoia-sql
 ```
 
 ## 使用方法
 
 ### 词法分析
 
-对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象语法树节点（详见 demo_1）：
-
-```python
-from metasequoia_sql.ast.functions import parse_as_statements
-
-root = parse_as_statements("your sql")
-```
+对 SQL 语句进行句法分析，将 SQL 语句中的每个部分拆分为一个抽象语法树节点：
 
 ### 句法分析
 
 对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
 
 ```python
 from metasequoia_sql import *
 
-statement = parse_create_table_statement(build_token_scanner("your sql"))
+statement = SQLParser.parse_create_table_statement("your sql")
 ```
 
 ### 翻译工具
 
 将 MySQL 的 CREATE TABLE 语句转换为 Hive 的 CREATE TABLE 语句：
 
 ```python
 from metasequoia_sql import *
 
-statement = parse_create_table_statement(build_token_scanner("your sql"))
+statement = SQLParser.parse_create_table_statement("your sql")
+```
+
+### pylint 自检
+
+```bash
+pylint --max-line-length=120 metasequoia_sql
 ```
 
 ## 实现原理
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
@@ -129,16 +129,38 @@
 - `SQLUnionClause`：UNION 语句。包含多个 SELECT 语句。
 - `SQLUnionALLClause`：UNION ALL 语句。包含多个 SELECT 语句。
 
 ## 已知的不兼容
 
 - DB2 的 `CURRENT DATE` 的语法
 
+参考文档：https://www.alibabacloud.com/help/zh/maxcompute/user-guide/insert-or-update-data-into-a-table-or-a-static-partition?spm=a2c63.p38356.0.0.637d7109wr3nC3
+
 ## 修改记录
 
+#### 0.2.0 > 0.3.0
+
+新增：
+
+- 重构词法解析和语法解析以支持插件开发
+- SET 语句的解析逻辑
+- LATERAL VIEW 子句的解析逻辑
+
+优化：
+
+- core.objects 将语法节点重构为 dataclasses 类型
+- 含 WITH 表达式的上游表解析逻辑
+- core.parser 中的方法兼容字符串类型的 TokenScanner 类型
+- 整理单元测试逻辑
+- 代码质量提升
+- core.objects 中将 get_used_column_list 和 get_used_table_list 改为抽象方法
+- 支持 DB2 的 CURRENT DATE、CURRENT TIME、CURRENT TIMESTAMP 语法
+- 增加 TokenScanner 未解析完成的发现机制
+- 支持窗口函数的 ROWS 子句
+
 #### 0.1.0 > 0.2.0
 
 新增：
 - `INSERT` 语句解析逻辑
 - 一次性解析多条 SQL 语句
 
 优化：
```

### Comparing `metasequoia-sql-0.2.0/metasequoia_sql.egg-info/SOURCES.txt` & `metasequoia-sql-0.3.0/metasequoia_sql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 metasequoia_sql/errors.py
 metasequoia_sql/static.py
 metasequoia_sql.egg-info/PKG-INFO
 metasequoia_sql.egg-info/SOURCES.txt
 metasequoia_sql.egg-info/dependency_links.txt
 metasequoia_sql.egg-info/top_level.txt
 metasequoia_sql/analyzer/__init__.py
-metasequoia_sql/analyzer/consanguinity.py
+metasequoia_sql/analyzer/data_lineage.py
 metasequoia_sql/ast/__init__.py
-metasequoia_sql/ast/functions.py
 metasequoia_sql/ast/nodes.py
 metasequoia_sql/ast/parser.py
 metasequoia_sql/ast/static.py
 metasequoia_sql/common/__init__.py
 metasequoia_sql/common/base_scanner.py
 metasequoia_sql/common/basic.py
 metasequoia_sql/common/text_scanner.py
 metasequoia_sql/common/token_scanner.py
 metasequoia_sql/core/__init__.py
-metasequoia_sql/core/data_source.py
 metasequoia_sql/core/objects.py
 metasequoia_sql/core/parser.py
 metasequoia_sql/core/static.py
```

### Comparing `metasequoia-sql-0.2.0/setup.py` & `metasequoia-sql-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="metasequoia-sql",
-    version="0.2.0",
+    version="0.3.0",
     description="SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="changxing",
     author_email="1278729001@qq.com",
     url="https://github.com/ChangxingJiang/metasequoia-sql",
     install_requires=[],
```

