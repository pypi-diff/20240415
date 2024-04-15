# Comparing `tmp/macal-5.0rc9.tar.gz` & `tmp/macal-5.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macal-5.0rc9.tar", last modified: Mon Nov 13 20:39:07 2023, max compression
+gzip compressed data, was "macal-5.5.0a1.tar", last modified: Mon Apr 15 15:30:14 2024, max compression
```

## Comparing `macal-5.0rc9.tar` & `macal-5.5.0a1.tar`

### file list

```diff
@@ -1,190 +1,49 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/
--rw-r--r--   0 marco     (1000) marco     (1000)     1121 2023-03-07 14:15:31.000000 macal-5.0rc9/LICENSE.txt
--rw-r--r--   0 marco     (1000) marco     (1000)      153 2023-11-13 19:19:23.000000 macal-5.0rc9/MANIFEST.in
--rw-r--r--   0 marco     (1000) marco     (1000)    32449 2023-11-13 20:39:07.615218 macal-5.0rc9/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)    31916 2023-11-13 19:19:23.000000 macal-5.0rc9/README.md
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.605218 macal-5.0rc9/documentation/
--rw-r--r--   0 marco     (1000) marco     (1000)     4950 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/General_Design_Interpreter_VM_Instructions_Opcodes_Etc.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     5119 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/ascii_art.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     3159 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/fib.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     2380 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/foreach.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     2121 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/function6_lex.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     7076 2023-10-24 20:15:07.000000 macal-5.0rc9/documentation/history.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       42 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     1994 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/performance_bottlenecks.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     3385 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/register_flags.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     1320 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/tests.md
--rw-r--r--   0 marco     (1000) marco     (1000)    10194 2023-11-13 19:19:23.000000 macal-5.0rc9/documentation/variables_and_scope.md
--rw-r--r--   0 marco     (1000) marco     (1000)      750 2023-11-13 20:37:36.000000 macal-5.0rc9/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-11-13 20:39:07.615218 macal-5.0rc9/setup.cfg
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.605218 macal-5.0rc9/src/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/src/macal/
--rw-r--r--   0 marco     (1000) marco     (1000)      345 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/__about__.py
--rw-r--r--   0 marco     (1000) marco     (1000)      170 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)      629 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2148 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_assignment.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1193 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_binary_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)      919 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_block.py
--rw-r--r--   0 marco     (1000) marco     (1000)      790 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_break_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      922 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_case_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      807 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_continue_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      700 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_default_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1148 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_elif_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      828 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_else_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1013 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1132 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_foreach_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1157 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_function_call_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1653 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_function_call_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2061 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_function_definition.py
--rw-r--r--   0 marco     (1000) marco     (1000)      915 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_function_parameter.py
--rw-r--r--   0 marco     (1000) marco     (1000)      969 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_halt_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1518 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_if_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1091 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_include_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1066 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_indexed_variable_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1000 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_istype.py
--rw-r--r--   0 marco     (1000) marco     (1000)      908 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_library_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1109 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_literal_array_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1628 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_literal_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1144 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_literal_record_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1025 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_print_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      943 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_program.py
--rw-r--r--   0 marco     (1000) marco     (1000)      981 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_return_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1694 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_select_field.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1763 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_select_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1012 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      968 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_switch_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)      872 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_type_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1107 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_unary_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1026 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_variable.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1059 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_variable_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1272 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_variable_function_call_expression.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1219 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_node_while_statement.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4528 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ast_nodetype.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1078 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_address.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4789 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_debugger.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3805 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_flags_register.py
--rw-r--r--   0 marco     (1000) marco     (1000)      449 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_function.py
--rw-r--r--   0 marco     (1000) marco     (1000)      648 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_jump.py
--rw-r--r--   0 marco     (1000) marco     (1000)      687 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_label.py
--rw-r--r--   0 marco     (1000) marco     (1000)      656 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_library.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3320 2023-11-13 19:57:56.000000 macal-5.0rc9/src/macal/bytecode_optimizer.py
--rw-r--r--   0 marco     (1000) marco     (1000)     7852 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_register.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5500 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/bytecode_variable.py
--rw-r--r--   0 marco     (1000) marco     (1000)    36802 2023-11-13 20:06:30.000000 macal-5.0rc9/src/macal/cmacal_vm.pyx
--rw-r--r--   0 marco     (1000) marco     (1000)     7203 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/compiler_scope.py
--rw-r--r--   0 marco     (1000) marco     (1000)      401 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/config.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5037 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/conversion.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1341 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ct_function.py
--rw-r--r--   0 marco     (1000) marco     (1000)      971 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/ct_variable.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1186 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lex_token.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/src/macal/lib/
--rw-r--r--   0 marco     (1000) marco     (1000)      284 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/csv.mcl
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/src/macal/lib/ext/
--rw-r--r--   0 marco     (1000) marco     (1000)      682 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_csv.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1723 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_io.py
--rw-r--r--   0 marco     (1000) marco     (1000)      504 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_keyring.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1880 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_math.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2044 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_strings.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3723 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_syslog.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2429 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_system.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1617 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/ext_time.py
--rw-r--r--   0 marco     (1000) marco     (1000)    30467 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/ext/meraki_api_library_v1.py
--rw-r--r--   0 marco     (1000) marco     (1000)      544 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/io.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      383 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/keyring.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      916 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/math.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     4241 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/meraki_v1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1023 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/strings.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      302 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/syslog.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1116 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/system.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      620 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/lib/time.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)    51453 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_compiler.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3248 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_decompiler.py
--rw-r--r--   0 marco     (1000) marco     (1000)    14642 2023-11-13 19:37:29.000000 macal-5.0rc9/src/macal/macal_instruction_emitter.py
--rw-r--r--   0 marco     (1000) marco     (1000)    12185 2023-11-13 19:34:40.000000 macal-5.0rc9/src/macal/macal_instructions.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2729 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_interactive.py
--rw-r--r--   0 marco     (1000) marco     (1000)    15971 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_lexer.py
--rw-r--r--   0 marco     (1000) marco     (1000)    35358 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/macal_parser.py
--rw-r--r--   0 marco     (1000) marco     (1000)    32749 2023-11-13 20:15:04.000000 macal-5.0rc9/src/macal/macal_select_compiler.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3343 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/mc.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2324 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/md.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4927 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/mi.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1984 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/mr.py
--rw-r--r--   0 marco     (1000) marco     (1000)      781 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/python_module_info.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1394 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/runtime_scope.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2316 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/statement_type_table.py
--rw-r--r--   0 marco     (1000) marco     (1000)      394 2023-11-13 19:19:23.000000 macal-5.0rc9/src/macal/switch_case_table.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/src/macal.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)    32449 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     4832 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       90 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/entry_points.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       17 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/requires.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        6 2023-11-13 20:39:07.000000 macal-5.0rc9/src/macal.egg-info/top_level.txt
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-11-13 20:39:07.615218 macal-5.0rc9/tests/
--rw-r--r--   0 marco     (1000) marco     (1000)      529 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/aor.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1486 2023-11-09 20:38:02.000000 macal-5.0rc9/tests/args.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)       32 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/args.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      442 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/artest.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      255 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/bleed_test.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      116 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/continue.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      334 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/fetest.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      172 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/fn_def.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      121 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/fnfnt.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      385 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       94 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      228 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function3.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      287 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function4.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     3559 2023-11-11 21:51:37.000000 macal-5.0rc9/tests/function5.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      541 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function5.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      357 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/function6.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       51 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/halt_test.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      475 2023-11-13 00:12:46.000000 macal-5.0rc9/tests/if.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      124 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/if.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      155 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/if2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      938 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/iftest.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      159 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/include_1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      112 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/include_2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       96 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       89 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      133 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_3.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       54 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_4.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      172 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_5.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      550 2023-11-13 11:08:02.000000 macal-5.0rc9/tests/indexed_6.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      101 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/indexed_6.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       27 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/interpolation_shorts.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1245 2023-11-09 20:24:45.000000 macal-5.0rc9/tests/libvar.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)       40 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/libvar.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)    46965 2023-11-13 14:46:31.000000 macal-5.0rc9/tests/mdi.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)     5722 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/mdi.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     3827 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/meraki_firewall_dc.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     3001 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/meraki_firewall_sh.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     7301 2023-10-25 01:39:02.000000 macal-5.0rc9/tests/meraki_test.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      613 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/meraki_test.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     6804 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/mt.py
--rw-r--r--   0 marco     (1000) marco     (1000)      374 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/nested.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2198 2023-11-13 01:31:23.000000 macal-5.0rc9/tests/select_1.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      689 2023-11-13 10:01:28.000000 macal-5.0rc9/tests/select_2.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      160 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2365 2023-11-13 10:01:37.000000 macal-5.0rc9/tests/select_3.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      557 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_3.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      607 2023-11-13 10:01:40.000000 macal-5.0rc9/tests/select_4.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      264 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_4.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     4328 2023-11-13 20:08:24.000000 macal-5.0rc9/tests/select_5.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      583 2023-11-13 20:11:27.000000 macal-5.0rc9/tests/select_5.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     4586 2023-11-13 20:15:11.000000 macal-5.0rc9/tests/select_6.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      486 2023-11-13 20:14:09.000000 macal-5.0rc9/tests/select_6.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      955 2023-11-13 19:50:16.000000 macal-5.0rc9/tests/select_7.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      196 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_7.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1437 2023-11-13 18:03:42.000000 macal-5.0rc9/tests/select_8.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      611 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/select_8.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2956 2023-11-13 20:17:34.000000 macal-5.0rc9/tests/select_9.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      190 2023-11-13 20:17:18.000000 macal-5.0rc9/tests/select_9.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      213 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/switch_1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1011 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/test.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)       96 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/test2.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      139 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/test3.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1052 2023-11-10 00:25:51.000000 macal-5.0rc9/tests/usereserved.mbc
--rw-r--r--   0 marco     (1000) marco     (1000)      798 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/usereserved.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      131 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/variable.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      176 2023-11-13 19:19:23.000000 macal-5.0rc9/tests/whiletest.mcl
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1184 2024-03-22 12:04:18.000000 macal-5.5.0a1/LICENSE.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     1878 2024-04-15 15:30:14.522592 macal-5.5.0a1/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     1228 2024-04-08 15:14:58.000000 macal-5.5.0a1/README.md
+-rw-r--r--   0 marco     (1000) marco     (1000)      848 2024-04-04 14:03:06.000000 macal-5.5.0a1/pyproject.toml
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-15 15:30:14.522592 macal-5.5.0a1/setup.cfg
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1474 2024-04-07 01:56:29.000000 macal-5.5.0a1/src/macal/__about__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:11:34.000000 macal-5.5.0a1/src/macal/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/frontend/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:27.000000 macal-5.5.0a1/src/macal/frontend/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/frontend/ast/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:13:42.000000 macal-5.5.0a1/src/macal/frontend/ast/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2568 2024-04-08 13:40:36.000000 macal-5.5.0a1/src/macal/frontend/ast/kind.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1892 2024-04-08 20:08:54.000000 macal-5.5.0a1/src/macal/frontend/ast/metadata.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    32164 2024-04-09 13:34:29.000000 macal-5.5.0a1/src/macal/frontend/ast/node.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 23:39:28.000000 macal-5.5.0a1/src/macal/frontend/ast/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)    20787 2024-04-15 14:41:47.000000 macal-5.5.0a1/src/macal/frontend/mlexer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    49158 2024-04-15 14:43:00.000000 macal-5.5.0a1/src/macal/frontend/mparser.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4851 2024-04-09 09:41:36.000000 macal-5.5.0a1/src/macal/frontend/mparserstate.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:45.000000 macal-5.5.0a1/src/macal/frontend/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     5713 2024-04-10 21:36:36.000000 macal-5.5.0a1/src/macal/macal.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2172 2024-04-08 15:16:25.000000 macal-5.5.0a1/src/macal/mexceptions.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3570 2024-04-10 14:47:02.000000 macal-5.5.0a1/src/macal/mrepl.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     7519 2024-04-15 14:32:17.000000 macal-5.5.0a1/src/macal/mrun.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:34.000000 macal-5.5.0a1/src/macal/py.typed
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/runtime/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:21.000000 macal-5.5.0a1/src/macal/runtime/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal/runtime/library/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-23 23:21:40.000000 macal-5.5.0a1/src/macal/runtime/library/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-24 20:22:17.000000 macal-5.5.0a1/src/macal/runtime/library/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     2129 2024-04-15 14:35:04.000000 macal-5.5.0a1/src/macal/runtime/library/system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1618 2024-03-24 06:01:49.000000 macal-5.5.0a1/src/macal/runtime/library/time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     8922 2024-04-09 13:03:11.000000 macal-5.5.0a1/src/macal/runtime/menvironment.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4011 2024-04-10 20:55:22.000000 macal-5.5.0a1/src/macal/runtime/mimporter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    77580 2024-04-15 14:47:24.000000 macal-5.5.0a1/src/macal/runtime/minterpreter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-23 18:22:52.000000 macal-5.5.0a1/src/macal/runtime/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     1705 2024-04-08 15:40:52.000000 macal-5.5.0a1/src/macal/runtime/value_type.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    17433 2024-04-11 16:42:19.000000 macal-5.5.0a1/src/macal/runtime/values.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/src/macal.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1878 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     1071 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)      117 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       73 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        6 2024-04-15 15:30:14.000000 macal-5.5.0a1/src/macal.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 15:30:14.522592 macal-5.5.0a1/tests/
+-rw-r--r--   0 marco     (1000) marco     (1000)     5867 2024-04-09 23:07:14.000000 macal-5.5.0a1/tests/test.py
```

### Comparing `macal-5.0rc9/LICENSE.txt` & `macal-5.5.0a1/src/macal/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,30 @@
-MIT License
-
-Copyright (c) 2019-present Westcon Security Netherlands <marco.caspers@westcon.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+# -*- coding: utf-8 -*-
+#
+# Product:   Macal
+# Author:    Marco Caspers
+# Email:     SamaDevTeam@westcon.com
+# License:   MIT License
+# Date:      2024-03-22
+#
+# Copyright 2024 Westcon-Comstor
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+# IN THE SOFTWARE.
+#
+# SPDX-License-Identifier: MIT
+#
```

### Comparing `macal-5.0rc9/pyproject.toml` & `macal-5.5.0a1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 [build-system]
-requires = ["Cython >= 0.29", "setuptools >= 67", "wheel >= 0.40"]
+requires = ["setuptools >= 67", "wheel >= 0.40"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macal"
-version = "5.0.rc9"
+version = "5.5.0.alpha.1"
 authors = [
   { name="Marco Caspers", email="SamaDevTeam@westcon.com" },
 ]
 description = "Macal is a DSL for collecting and transforming data from various sources."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "unidecode",
-    "Cython",
+    "keyring",
+    "keyrings.alt",
+    "meraki",
+    "pydantic",
+    "python-jose[cryptography]"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Sama-Developer/macal"
 
 [project.scripts]
-mi = "macal.mi:Run"
-md = "macal.md:Run"
-mc = "macal.mc:Run"
-mr = "macal.mr:Run"
+mrepl = "macal.mrepl:main"
+mdeco = "macal.mdeco:main"
+mcomp = "macal.mccomp:main"
+mrun = "macal.mrun:main"
```

