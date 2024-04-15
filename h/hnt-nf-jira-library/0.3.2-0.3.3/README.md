# Comparing `tmp/hnt_nf_jira_library-0.3.2.tar.gz` & `tmp/hnt_nf_jira_library-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.3.2.tar", last modified: Sat Apr 13 16:41:15 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.3.3.tar", last modified: Mon Apr 15 14:05:07 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.3.2.tar` & `hnt_nf_jira_library-0.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 16:41:15.701021 hnt_nf_jira_library-0.3.2/
--rw-rw-rw-   0        0        0      286 2024-04-13 16:41:15.698027 hnt_nf_jira_library-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 16:41:15.693587 hnt_nf_jira_library-0.3.2/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-13 16:41:15.000000 hnt_nf_jira_library-0.3.2/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-04-13 16:41:15.000000 hnt_nf_jira_library-0.3.2/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 16:41:15.000000 hnt_nf_jira_library-0.3.2/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-13 16:41:15.000000 hnt_nf_jira_library-0.3.2/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 16:41:15.000000 hnt_nf_jira_library-0.3.2/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 16:41:15.602211 hnt_nf_jira_library-0.3.2/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.2/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 16:41:15.673034 hnt_nf_jira_library-0.3.2/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-13 16:41:15.689586 hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-13 15:41:39.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     2162 2024-04-13 16:37:44.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     3874 2024-04-13 15:58:32.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     2956 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      259 2024-04-12 21:48:41.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      448 2024-04-13 15:45:00.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      379 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.2/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    18639 2024-04-13 16:01:45.000000 hnt_nf_jira_library-0.3.2/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-13 16:41:15.701021 hnt_nf_jira_library-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-13 16:41:05.000000 hnt_nf_jira_library-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:05:07.003652 hnt_nf_jira_library-0.3.3/
+-rw-rw-rw-   0        0        0      286 2024-04-15 14:05:06.999652 hnt_nf_jira_library-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 14:05:06.996651 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 14:05:06.000000 hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 14:05:06.862644 hnt_nf_jira_library-0.3.3/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.3/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:05:06.942647 hnt_nf_jira_library-0.3.3/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:05:06.991651 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4893 2024-04-15 12:56:23.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     2162 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     3874 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     2956 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      234 2024-04-15 13:00:20.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      448 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      354 2024-04-15 13:00:14.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.3/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    14426 2024-04-15 13:20:15.000000 hnt_nf_jira_library-0.3.3/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:05:07.003652 hnt_nf_jira_library-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-15 14:04:48.000000 hnt_nf_jira_library-0.3.3/setup.py
```

### Comparing `hnt_nf_jira_library-0.3.2/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.3.3/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/helper.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.2/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.3.3/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.2/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.3.3/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.2/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.3.3/nf_jira/wrapper_nf_jira.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,14 +52,16 @@
                 issue_sap_json["miro"] = miro_model
 
         elif issue_transition == 'FV60':
             fatura_factory = self._fatura_factory(issue)
             fatura_model   = Fatura(**fatura_factory).model_dump()
             issue_sap_json["fatura"] = fatura_model
 
+        issue_sap_json["jira_info"] = issue["jira_info"]
+
         if self._test_mode:
             for json in issue_sap_json:
                 self.JsonHelper.save_json(f'{json}_{issue_key}', issue_sap_json[json])
             
         return issue_sap_json
 
     def _get_issue_by_key(self, issue_key):
@@ -163,15 +165,14 @@
             "tipo": "ZCOR",
             "org_compras": issue["domain_data"]["centro"]["org_compras"],
             "grp_compradores": issue['json_data']['grupo_compradores'][0],
             "empresa": "HFNT",
             "cod_fornecedor": issue["domain_data"]["fornecedor"]["codigo_sap"],
             "sintese_itens": sintese_itens,
             "anexo": anexo,
-            "jira_info": issue["jira_info"],
         }
 
         return nota_pedido
 
     def _miro_factory(self, issue: dict):
 
         texto = self._prepare_ref(issue)
@@ -240,148 +241,18 @@
             "data_basica": datetime.now().strftime("%d.%m.%Y"),
             "cond_pgto": "0000" #CONSTANTE 
         }
 
         fatura_model = {
             "dados_basicos": dados_basicos,
             "pagamento":pagamento,
-            "jira_info": issue["jira_info"],
         }
 
         return fatura_model
 
-    def _get_nf_issue_context(self, issue_id: str):
-        try:
-
-            issue_json = self._get_nf_jira(issue_id)
-
-            attachment = issue_json["attachment"]
-            jira_info = issue_json["jira_info"]
-
-            ##### GET DOMAIN #####
-            ## FORNECEDOR
-            cnpj_fornecedor = attachment.get(CNPJ_DO_FORNECEDOR)
-            fornecedor = self._get_nf_domain("fornecedor", cnpj_fornecedor)
-
-            ## CENTRO
-            cnpj_centro = attachment.get(CNPJ_DO_CLIENTE)
-            centro = self._get_nf_domain("centro", cnpj_centro)
-
-            domain = {"fornecedor": fornecedor, "centro": centro}
-
-            ##### GET PDF #####
-            pdf_data = self._download_pdf(attachment[ARQUIVOS_DA_FATURA][0])
-
-            ##### GET ALLOCATION #####
-            allocation = self._get_allocation(
-                attachment[CNPJ_DO_FORNECEDOR],
-                attachment[CNPJ_DO_CLIENTE],
-                attachment[NÚMERO_DO_CONTRATO],
-            )
-
-            ##### FORMAT JSON #####
-
-
-            ##### PARSE JSON #####
-            # issue_model = self._issue_factory(issue)
-
-            ##### CREATE MODEL #####
-            # nota_pedido = NotaPedido(**issue_model).model_dump()
-
-            #### SAVE JSON ####
-
-
-            # return nota_pedido
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-
-        except Exception as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-
-    def _get_nf_miro_context(self, issue_id: str, cod_sap: str):
-        try:
-
-            issue_data = self._get_nf_jira(issue_id)
-
-            clean_fields = self._remove_null_fields(
-                issue_data["issue_data"].get("fields")
-            )
-            issue_data["issue_data"]["fields"] = clean_fields
-
-            attachment = issue_data["attachment"]
-            attachment["cod_sap"] = cod_sap
-
-            ##### GET DOMAIN #####
-            ## FORNECEDOR
-            cnpj_fornecedor = attachment.get(CNPJ_DO_FORNECEDOR)
-            fornecedor = self._get_nf_domain("fornecedor", cnpj_fornecedor)
-
-            ## CENTRO
-            cnpj_centro = attachment.get(CNPJ_DO_CLIENTE)
-            centro = self._get_nf_domain("centro", cnpj_centro)
-
-            attachment["domain_data"] = {"fornecedor": fornecedor, "centro": centro}
-
-            miro_model = self._miro_factory(attachment)
-
-            miro = Miro(**miro_model).model_dump()
-
-            if self._test_mode:
-                self.JsonHelper.save_json(f'Miro_{issue_id}', miro)
-
-            return miro
-
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-
-        except Exception as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-
-    def _get_nf_fatura_context(self, issue_id):
-        try:
-
-            issue_data = self._get_nf_jira(issue_id)
-
-            attachment = issue_data['attachment']
-
-            # não esta vindo no json guiando, não há como validar sem isso no momento
-            # if not attachment['invoiceNumber']:
-            #     return {}
-
-            cnpj_fornecedor = attachment.get(CNPJ_DO_FORNECEDOR)
-            fornecedor = self._get_nf_domain('fornecedor', cnpj_fornecedor)
-
-            cnpj_centro = attachment.get(CNPJ_DO_CLIENTE)
-            centro = self._get_nf_domain('centro', cnpj_centro)
-
-            domain_data = {
-                "fornecedor": fornecedor,
-                "centro": centro
-            }
-
-            issue = {
-                'json_data': attachment,
-                'domain_data': domain_data
-            }
-
-            fatura_model = self._fatura_factory(issue)
-
-            fatura = Fatura(**fatura_model).model_dump()
-
-            if self._test_mode:
-                self.JsonHelper.save_json(f'Fatura_{issue_id}', fatura)
-
-            return fatura
-    
-        except requests.exceptions.HTTPError as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-
-        except Exception as e:
-            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
-        
     def _get_nf_jira(self, issue_id):
         try:
 
             issue_data = self.IssueJira.get_issue(issue_id)
             complement_form = self._get_issue_fields_by_keys( issue_id, FORM_TEMPLATE_COMPLEMENTO )
 
             issue_data["fields"] = self.JiraFieldsHelper.remove_null_fields(issue_data.get("fields"))
@@ -420,17 +291,17 @@
             attachment["data_procmto"] = complement_form['data_autorizacao']
             attachment["hora_procmto"] = complement_form['hora_autorizacao']
             attachment[nf_type]["DataLeituraAnterior"] = complement_form['data_leitura_anterior']
             attachment[nf_type]["DataLeituraAtual"] = complement_form['data_leitura_atual']
             attachment["grupo_compradores"] = complement_form['grupo_compradores']
 
             #Validação de Valor Liquido da Fatura
-            if complement_form['valor_liquido'] != "":
+            if complement_form['valor_liquido'] != "" and complement_form['valor_liquido'] != None:
                 attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_liquido']
-            elif complement_form['valor_nota'] != None:
+            elif complement_form['valor_nota'] != None and complement_form['valor_nota'] != "":
                 attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_nota']
             else:
                 attachment[VALOR_TOTAL_DA_FATURA] = attachment.get(
                     VALOR_TOTAL_DA_FATURA
                 )
 
             automation_form_id = self.FormJira.get_form_id(issue_id, FORM_TEMPLATE_AUTOMACAO)
@@ -470,10 +341,8 @@
     def _get_issue_fields_by_keys(self, issue_key, form_template):
 
         form_jira_keys = self.FormJira.get_form_jira_keys(issue_key, form_template)
         form_fields    = self.FormJira.get_form_fields(issue_key, form_template)
         jira_fields    = self.IssueJira.get_issue_fields_data(issue_key)
         fields_by_jira_and_form = self.IssueFields.get_fields_by_form_and_jira(form_jira_keys, form_fields, jira_fields)
 
-        return fields_by_jira_and_form
-    
-
+        return fields_by_jira_and_form
```

