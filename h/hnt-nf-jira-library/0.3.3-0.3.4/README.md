# Comparing `tmp/hnt_nf_jira_library-0.3.3.tar.gz` & `tmp/hnt_nf_jira_library-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.3.3.tar", last modified: Mon Apr 15 14:05:07 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.3.4.tar", last modified: Mon Apr 15 14:36:36 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.3.3.tar` & `hnt_nf_jira_library-0.3.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:05:07.003652 hnt_nf_jira_library-0.3.3/
--rw-rw-rw-   0        0        0      286 2024-04-15 14:05:06.999652 hnt_nf_jira_library-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 14:05:06.996651 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 14:05:06.862644 hnt_nf_jira_library-0.3.3/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.3/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:05:06.942647 hnt_nf_jira_library-0.3.3/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:05:06.991651 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-15 12:56:23.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     2162 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     3874 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     2956 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      234 2024-04-15 13:00:20.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      448 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      354 2024-04-15 13:00:14.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    14426 2024-04-15 13:20:15.000000 hnt_nf_jira_library-0.3.3/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-15 14:05:07.003652 hnt_nf_jira_library-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-15 14:04:48.000000 hnt_nf_jira_library-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:36:36.558745 hnt_nf_jira_library-0.3.4/
+-rw-rw-rw-   0        0        0      286 2024-04-15 14:36:36.555745 hnt_nf_jira_library-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 14:36:36.552744 hnt_nf_jira_library-0.3.4/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-15 14:36:36.000000 hnt_nf_jira_library-0.3.4/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2024-04-15 14:36:36.000000 hnt_nf_jira_library-0.3.4/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:36:36.000000 hnt_nf_jira_library-0.3.4/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-15 14:36:36.000000 hnt_nf_jira_library-0.3.4/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 14:36:36.000000 hnt_nf_jira_library-0.3.4/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 14:36:36.483040 hnt_nf_jira_library-0.3.4/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.4/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:36:36.533743 hnt_nf_jira_library-0.3.4/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:36:36.548745 hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4893 2024-04-15 12:56:23.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     2162 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     5454 2024-04-15 14:35:02.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     2956 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      234 2024-04-15 13:00:20.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      448 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      354 2024-04-15 13:00:14.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.4/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    14486 2024-04-15 14:35:44.000000 hnt_nf_jira_library-0.3.4/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:36:36.558745 hnt_nf_jira_library-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-15 14:35:52.000000 hnt_nf_jira_library-0.3.4/setup.py
```

### Comparing `hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.3.4/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/helper.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.3.4/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.3/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.3.4/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.3/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.3.4/nf_jira/wrapper_nf_jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .entities.nota_pedido import NotaPedido
 from .entities.miro import Miro
 from .entities.fatura import Fatura
 from .entities.constants import *
 
 from .entities.classes.form_jira    import FormJira
-from .entities.classes.issue_jira   import IssueJira, AttachmentJira, TransitionJira
+from .entities.classes.issue_jira   import IssueJira, AttachmentJira, TransitionJira, CommentJira
 from .entities.classes.issue_fields import IssueFields
 from .entities.classes.helper       import JiraFieldsHelper, JsonHelper, GuiandoHelper
 from .entities.classes.n8n_domain   import N8NDomain
 class wrapper_jira:
 
     def __init__(self, miro_is_active=False ,debug=False):
         
@@ -24,14 +24,15 @@
         self._instance_class()
 
     def _instance_class(self):
         self.FormJira         = FormJira()
         self.IssueJira        = IssueJira()
         self.AttachmentJira   = AttachmentJira()
         self.TrasnsitionJira  = TransitionJira()
+        self.CommentJira      = CommentJira()
         self.JiraFieldsHelper = JiraFieldsHelper()
         self.GuiandoHelper    = GuiandoHelper()
         self.JsonHelper       = JsonHelper()
         self.IssueFields      = IssueFields()
         self.N8NDomain        = N8NDomain()
 
     def get_document_by_issue(self, issue_key):
```

