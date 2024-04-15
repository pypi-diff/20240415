# Comparing `tmp/pih-plb_ntf_answ-0.12.tar.gz` & `tmp/pih-plb_ntf_answ-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_ntf_answ-0.12.tar", last modified: Wed Apr 10 09:19:00 2024, max compression
+gzip compressed data, was "pih-plb_ntf_answ-0.13.tar", last modified: Mon Apr 15 00:27:42 2024, max compression
```

## Comparing `pih-plb_ntf_answ-0.12.tar` & `pih-plb_ntf_answ-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 09:19:00.886075 pih-plb_ntf_answ-0.12/
--rw-rw-rw-   0        0        0      304 2024-04-10 09:19:00.837422 pih-plb_ntf_answ-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 09:19:00.396335 pih-plb_ntf_answ-0.12/PolibasePersonNotificationAnswerService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_ntf_answ-0.12/PolibasePersonNotificationAnswerService/__init__.py
--rw-rw-rw-   0        0        0      174 2024-04-09 22:27:14.000000 pih-plb_ntf_answ-0.12/PolibasePersonNotificationAnswerService/__main__.py
--rw-rw-rw-   0        0        0      449 2024-04-10 09:18:19.000000 pih-plb_ntf_answ-0.12/PolibasePersonNotificationAnswerService/const.py
--rw-rw-rw-   0        0        0     4021 2024-04-10 09:18:13.000000 pih-plb_ntf_answ-0.12/PolibasePersonNotificationAnswerService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:19:00.790542 pih-plb_ntf_answ-0.12/pih_plb_ntf_answ.egg-info/
--rw-rw-rw-   0        0        0      304 2024-04-10 09:18:59.000000 pih-plb_ntf_answ-0.12/pih_plb_ntf_answ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2024-04-10 09:19:00.000000 pih-plb_ntf_answ-0.12/pih_plb_ntf_answ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 09:18:59.000000 pih-plb_ntf_answ-0.12/pih_plb_ntf_answ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-04-10 09:18:59.000000 pih-plb_ntf_answ-0.12/pih_plb_ntf_answ.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 09:19:00.000000 pih-plb_ntf_answ-0.12/pih_plb_ntf_answ.egg-info/requires.txt
--rw-rw-rw-   0        0        0       40 2024-04-10 09:19:00.000000 pih-plb_ntf_answ-0.12/pih_plb_ntf_answ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 09:19:00.901715 pih-plb_ntf_answ-0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 00:27:42.306873 pih-plb_ntf_answ-0.13/
+-rw-rw-rw-   0        0        0      304 2024-04-15 00:27:42.259968 pih-plb_ntf_answ-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 00:27:41.866638 pih-plb_ntf_answ-0.13/PolibasePersonNotificationAnswerService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_ntf_answ-0.13/PolibasePersonNotificationAnswerService/__init__.py
+-rw-rw-rw-   0        0        0      174 2024-04-09 22:27:14.000000 pih-plb_ntf_answ-0.13/PolibasePersonNotificationAnswerService/__main__.py
+-rw-rw-rw-   0        0        0      449 2024-04-15 00:03:28.000000 pih-plb_ntf_answ-0.13/PolibasePersonNotificationAnswerService/const.py
+-rw-rw-rw-   0        0        0     4066 2024-04-15 00:05:13.000000 pih-plb_ntf_answ-0.13/PolibasePersonNotificationAnswerService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:27:42.213064 pih-plb_ntf_answ-0.13/pih_plb_ntf_answ.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-04-15 00:27:41.000000 pih-plb_ntf_answ-0.13/pih_plb_ntf_answ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2024-04-15 00:27:41.000000 pih-plb_ntf_answ-0.13/pih_plb_ntf_answ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 00:27:41.000000 pih-plb_ntf_answ-0.13/pih_plb_ntf_answ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-04-15 00:27:41.000000 pih-plb_ntf_answ-0.13/pih_plb_ntf_answ.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-15 00:27:41.000000 pih-plb_ntf_answ-0.13/pih_plb_ntf_answ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       40 2024-04-15 00:27:41.000000 pih-plb_ntf_answ-0.13/pih_plb_ntf_answ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 00:27:42.322473 pih-plb_ntf_answ-0.13/setup.cfg
```

### Comparing `pih-plb_ntf_answ-0.12/PolibasePersonNotificationAnswerService/service.py` & `pih-plb_ntf_answ-0.13/PolibasePersonNotificationAnswerService/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,35 +14,35 @@
         Message,
         PolibasePerson,
         WhatsAppMessage,
         PolibasePersonVisitDS as PPVDS,
         PolibasePersonNotificationConfirmation as PPNC,
     )
     from pih import serve, subscribe_on
-    from pih.tools import ParameterList, ne, nn, one, nns, nni, nnt
+    from pih.tools import ParameterList, ne, nn, one, nns, nni, nnt, esc
 
     SENDER: str = A.D.get(A.CT_ME_WH_W.Profiles.CALL_CENTRE)
 
     def server_call_handler(sc: SC, pl: ParameterList) -> bool | None:
         if sc == SC.send_event:
             event: A.CT_E = A.D_Ex_E.get(pl)
             if event == A.CT_E.WHATSAPP_MESSAGE_RECEIVED:
                 message: WhatsAppMessage | None = A.D_Ex_E.whatsapp_message(pl)
                 if ne(message):
-                    sender: str = message.profile_id
+                    sender: str = nns(nnt(message).profile_id)
                     if sender == SENDER:
                         telephone_number: str = A.D_F.telephone_number_international(
-                            message.sender
+                            nns(nnt(message).sender)
                         )
                         notification_confirmation: PPNC | None = A.R_P_N_C.by(
                             telephone_number, sender
                         ).data
                         if (
                             ne(notification_confirmation)
-                            and notification_confirmation.status == 2
+                            and nnt(notification_confirmation).status == 2
                         ):
                             visit_ds: PPVDS | None = one(
                                 A.R_P_V_DS.search(
                                     PPVDS(
                                         telephoneNumber=A.D_F.telephone_number(
                                             telephone_number
                                         )
@@ -50,16 +50,16 @@
                                 )
                             )
                             if nn(visit_ds):
                                 pin: int = nni(visit_ds.pin)
                                 person: PolibasePerson = (
                                     PolibasePerson(
                                         pin,
-                                        visit_ds.FullName,
-                                        visit_ds.telephoneNumber,
+                                        nnt(visit_ds).FullName,
+                                        nnt(visit_ds).telephoneNumber,
                                     )
                                     if pin == A.CT_P.PRERECORDING_PIN
                                     else A.D_P.person_by_pin(pin)
                                 )
                                 if A.A_P_N_C.update(telephone_number, sender, 1):
                                     A.ME_WH_W_Q.add_message(
                                         Message(
@@ -74,15 +74,15 @@
                                         Message(
                                             A.CT_P.TELEGRAM_BOT_URL,
                                             telephone_number,
                                             sender,
                                         )
                                     )
                                     A.E.polibase_person_answered(
-                                        person, nns(nnt(message).message)
+                                        person, esc(nns(nnt(message).message))
                                     )
         return None
 
     def service_starts_handler() -> None:
         subscribe_on(SC.send_event)
 
     serve(
```

