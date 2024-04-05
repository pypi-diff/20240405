# Comparing `tmp/hnt_nf_jira_library-0.2.4.tar.gz` & `tmp/hnt_nf_jira_library-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.2.4.tar", last modified: Wed Apr  3 19:16:52 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.2.5.tar", last modified: Fri Apr  5 13:33:44 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.2.4.tar` & `hnt_nf_jira_library-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:52.195120 hnt_nf_jira_library-0.2.4/
--rw-rw-rw-   0        0        0      286 2024-04-03 19:16:52.192119 hnt_nf_jira_library-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:52.190122 hnt_nf_jira_library-0.2.4/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-03 19:16:51.000000 hnt_nf_jira_library-0.2.4/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2024-04-03 19:16:51.000000 hnt_nf_jira_library-0.2.4/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 19:16:51.000000 hnt_nf_jira_library-0.2.4/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-03 19:16:51.000000 hnt_nf_jira_library-0.2.4/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-03 19:16:51.000000 hnt_nf_jira_library-0.2.4/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:52.135459 hnt_nf_jira_library-0.2.4/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.4/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:16:52.173781 hnt_nf_jira_library-0.2.4/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/chave_acesso.py
--rw-rw-rw-   0        0        0     1863 2024-04-02 19:42:19.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/dados_basicos.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.4/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    23713 2024-04-03 19:13:33.000000 hnt_nf_jira_library-0.2.4/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-03 19:16:52.195120 hnt_nf_jira_library-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      489 2024-04-03 19:16:45.000000 hnt_nf_jira_library-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:33:44.176933 hnt_nf_jira_library-0.2.5/
+-rw-rw-rw-   0        0        0      286 2024-04-05 13:33:44.175921 hnt_nf_jira_library-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 13:33:44.172921 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 13:33:43.000000 hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 13:33:44.124440 hnt_nf_jira_library-0.2.5/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.2.5/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:33:44.169769 hnt_nf_jira_library-0.2.5/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/chave_acesso.py
+-rw-rw-rw-   0        0        0     1863 2024-04-05 13:32:32.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/dados_basicos.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.5/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    23690 2024-04-05 13:33:00.000000 hnt_nf_jira_library-0.2.5/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 13:33:44.177919 hnt_nf_jira_library-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      489 2024-04-05 13:33:25.000000 hnt_nf_jira_library-0.2.5/setup.py
```

### Comparing `hnt_nf_jira_library-0.2.4/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.2.5/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.2.4/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.2.5/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.2.4/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.2.5/nf_jira/wrapper_nf_jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         if not issue["allocation_data"]:
 
             item = {
                 "centro": issue["domain_data"]["centro"]["centro"],
                 "centro_custo": f"{issue['domain_data']['centro']['centro']}210",
                 "cod_imposto": "C6",
-                "valor_bruto": str(issue["json_data"][VALOR_TOTAL_DA_FATURA]).replace(".", ","),
+                "valor_bruto": str(issue["json_data"][VALOR_TOTAL_DA_FATURA]),
             }
 
             sintese_item = {
                 "categoria_cc": "K",
                 "quantidade": 1,
                 "cod_material": issue["domain_data"]["fornecedor"]["codigo_material"],
                 "item": item,
@@ -98,19 +98,15 @@
 
                 item = {
                     "centro": centro_issue["nome"].split("210")[0],
                     "centro_custo": centro_issue["nome"],
                     "cod_imposto": "C6",
                     "valor_bruto": "{:.2f}".format(
                         issue["json_data"][VALOR_TOTAL_DA_FATURA]
-                        * float(
-                            centro_issue["porcentagem"].replace(
-                                ",",
-                            )
-                        )
+                        * float(centro_issue["porcentagem"])
                         / 100,
                         2,
                     ),
                 }
 
                 sintese_item = {
                     "categoria_cc": "K",
@@ -151,15 +147,16 @@
             .strftime("%b/%y")
             .upper()
         )
 
         if issue[COMPLEMENTO_DE_ÁGUA] is not None:
             leitura_anterior = (
                 datetime.strptime(
-                    issue[COMPLEMENTO_DE_ÁGUA]["DataLeituraAnterior"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_ÁGUA]["DataLeituraAnterior"],
+                    "%Y-%m-%dT%H:%M:%S",
                 )
                 .strftime("%b/%y")
                 .upper()
             )
             leitura_atual = (
                 datetime.strptime(
                     issue[COMPLEMENTO_DE_ÁGUA]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
@@ -174,23 +171,25 @@
                     "%Y-%m-%dT%H:%M:%S",
                 )
                 .strftime("%b/%y")
                 .upper()
             )
             leitura_atual = (
                 datetime.strptime(
-                    issue[COMPLEMENTO_DE_ENERGIA]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_ENERGIA]["DataLeituraAtual"],
+                    "%Y-%m-%dT%H:%M:%S",
                 )
                 .strftime("%b/%y")
                 .upper()
             )
         elif issue[COMPLEMENTO_DE_GÁS] is not None:
             leitura_anterior = (
                 datetime.strptime(
-                    issue[COMPLEMENTO_DE_GÁS]["DataLeituraAnterior"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_GÁS]["DataLeituraAnterior"],
+                    "%Y-%m-%dT%H:%M:%S",
                 )
                 .strftime("%b/%y")
                 .upper()
             )
             leitura_atual = (
                 datetime.strptime(
                     issue[COMPLEMENTO_DE_GÁS]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
@@ -202,15 +201,15 @@
         texto = f"REF: {data_ref} PERIODO: {leitura_anterior} A {leitura_atual}"
 
         dados_basicos = {
             "data_da_fatura": datetime.strptime(
                 issue[DATA_DE_EMISSÃO], "%Y-%m-%dT%H:%M:%S"
             ).strftime("%d%m%Y"),
             "referencia": f"{issue['ChaveAcessoNotaFiscal'][25:34]}-{issue['ChaveAcessoNotaFiscal'][22:25]}",
-            "montante": str(issue[VALOR_TOTAL_DA_FATURA]).replace(".", ","),
+            "montante": str(issue[VALOR_TOTAL_DA_FATURA]),
             "texto": texto,
         }
 
         referencia_pedido = {"numero_pedido": issue["cod_sap"]}
 
         detalhe = {"ctg_nf": issue["domain_data"]["fornecedor"]["categoria_nf"]}
 
@@ -472,21 +471,27 @@
             )
             attachment[nf_type]["DataLeituraAtual"] = (
                 form_data["state"]["answers"]["56"]["date"]
                 if "56" in form_data["state"]["answers"]
                 else attachment[nf_type].get("DataLeituraAtual")
             )
 
-            #Validação de Valor Liquido da Fatura
+            # Validação de Valor Liquido da Fatura
             if "62" in form_data["state"]["answers"]:
-                attachment[VALOR_TOTAL_DA_FATURA] = form_data["state"]["answers"]["62"]["text"]
+                attachment[VALOR_TOTAL_DA_FATURA] = form_data["state"]["answers"]["62"][
+                    "text"
+                ]
             elif "48" in form_data["state"]["answers"]:
-                attachment[VALOR_TOTAL_DA_FATURA] = form_data["state"]["answers"]["48"]["text"]
+                attachment[VALOR_TOTAL_DA_FATURA] = form_data["state"]["answers"]["48"][
+                    "text"
+                ]
             else:
-                attachment[VALOR_TOTAL_DA_FATURA] = attachment.get(VALOR_TOTAL_DA_FATURA)
+                attachment[VALOR_TOTAL_DA_FATURA] = attachment.get(
+                    VALOR_TOTAL_DA_FATURA
+                )
 
             jira_info = {"issue_id": issue_id, "form_id": automacao_form_id}
 
             nf_jira_json = {
                 "issue_data": issue_data,
                 "attachment": attachment_data,
                 "jira_info": jira_info,
@@ -618,17 +623,15 @@
 
         return True
 
     def post_transition(self, transition_id, issue_id):
         payload = json.dumps(
             {
                 "transition": {"id": transition_id},
-                "update": {
-                    "comment": []
-                },
+                "update": {"comment": []},
             }
         )
         res = requests.post(
             f"{self._api_issue_url}/issue/{issue_id}/transitions",
             auth=self._auth,
             headers=self._api_headers,
             data=payload,
```

