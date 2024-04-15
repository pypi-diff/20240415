# Comparing `tmp/lowatt_grdf-2.1.4.tar.gz` & `tmp/lowatt_grdf-2.2.0.tar.gz`

## Comparing `lowatt_grdf-2.1.4.tar` & `lowatt_grdf-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/.flake8
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/MANIFEST.in
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/dev-requirements.txt
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/mypy.ini
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/pytest.ini
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/tox.ini
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/.github/workflows/tox.yml
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/lowatt_grdf/__init__.py
--rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/lowatt_grdf/api.py
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/lowatt_grdf/main.py
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/lowatt_grdf/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/lowatt_grdf/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/tests/__init__.py
--rw-r--r--   0        0        0    16428 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/tests/test_api.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/tests/test_main.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/tests/test_models.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/LICENSE
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/README.md
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 lowatt_grdf-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/.flake8
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/MANIFEST.in
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/dev-requirements.txt
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/mypy.ini
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/pytest.ini
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/staging-api-requests.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tox.ini
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/.github/workflows/tox.yml
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/__init__.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/api.py
+-rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/main.py
+-rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    16435 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tests/test_api.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tests/test_main.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tests/test_models.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/README.md
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/PKG-INFO
```

### Comparing `lowatt_grdf-2.1.4/.pre-commit-config.yaml` & `lowatt_grdf-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.1.4/.github/workflows/tox.yml` & `lowatt_grdf-2.2.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.1.4/lowatt_grdf/__init__.py` & `lowatt_grdf-2.2.0/lowatt_grdf/__init__.py`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.1.4/lowatt_grdf/api.py` & `lowatt_grdf-2.2.0/lowatt_grdf/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,20 @@
 from typing import Any, Literal, Optional, get_args
 
 import ndjson
 import requests
 
 from . import LOGGER, models
 
-OPENID_ENDPOINT = "https://sofit-sso-oidc.grdf.fr/openam/oauth2/realms/externeGrdf"
+OLD_AUTH_ENDPOINT = (
+    "https://sofit-sso-oidc.grdf.fr/openam/oauth2/realms/externeGrdf/access_token"
+)
+NEW_AUTH_ENDPOINT = (
+    "https://adict-connexion.grdf.fr/oauth2/aus5y2ta2uEHjCWIR417/v1/token"
+)
 
 
 def raise_for_status(resp: requests.Response) -> None:
     try:
         resp.raise_for_status()
     except requests.HTTPError:
         try:
@@ -57,42 +62,50 @@
     def __init__(self, client_id: str, client_secret: str):
         self.client_id = client_id
         self.client_secret = client_secret
         self._access_token: Optional[str] = None
         self._last_request: Optional[float] = None
         self._access_expires: Optional[float] = None
 
+    def _parse_response(self, resp: requests.Response) -> Any:
+        return ndjson.loads(resp.text)
+
     def request(self, verb: str, *args: Any, **kwargs: Any) -> Any:
         headers = kwargs.setdefault("headers", {})
         headers["Authorization"] = f"Bearer {self.access_token}"
         if self._last_request is not None:
             time.sleep(min(max(time.time() - self._last_request, 1), 1))
         resp = requests.request(verb, *args, **kwargs)
         self._last_request = time.time()
         raise_for_status(resp)
-        # XXX: duno why but without strip it doesn't work.
-        # Either an implementation error of ndjson module
-        # or bad response from GrDF API (at least on staging environment)
-        return ndjson.loads(resp.content.strip())
+        return self._parse_response(resp)
 
     get = functools.partialmethod(request, "GET")
     post = functools.partialmethod(request, "POST")
     put = functools.partialmethod(request, "PUT")
 
     @property
     def access_token(self) -> str:
         if self._access_token is None or (
             self._access_expires is not None and self._access_expires < time.time()
         ):
-            self._access_token, self._access_expires = self._authenticate()
+            self._access_token, self._access_expires = (
+                self._authenticate_with_fallback()
+            )
         return self._access_token
 
-    def _authenticate(self) -> tuple[str, float]:
+    def _authenticate_with_fallback(self) -> tuple[str, float]:
+        try:
+            return self._authenticate(auth_endpoint=NEW_AUTH_ENDPOINT)
+        except requests.exceptions.HTTPError:
+            return self._authenticate(auth_endpoint=OLD_AUTH_ENDPOINT)
+
+    def _authenticate(self, auth_endpoint: str) -> tuple[str, float]:
         resp = requests.post(
-            f"{OPENID_ENDPOINT}/access_token",
+            auth_endpoint,
             data={
                 "grant_type": "client_credentials",
                 "client_id": self.client_id,
                 "client_secret": self.client_secret,
                 "scope": self.scope,
             },
         )
@@ -106,15 +119,20 @@
         return (token, access_expires)
 
     def droits_acces(self, pce: Optional[list[str]] = None) -> Any:
         if not pce:
             return self.get(f"{self.api}/droits_acces")
         return self.post(f"{self.api}/droits_acces", json={"id_pce": pce})
 
-    ThirdRole = Literal["AUTORISE_CONTRAT_FOURNITURE", "DETENTEUR_CONTRAT_FOURNITURE"]
+    ThirdRole = Literal[
+        "AUTORISE_CONTRAT_FOURNITURE",
+        "DETENTEUR_CONTRAT_FOURNITURE",
+        "AUTORISE_CONTRAT_INJECTION",
+        "DETENTEUR_CONTRAT_INJECTION",
+    ]
     DEFAULT_THIRD_ROLE = get_args(ThirdRole)
     AccessRightState = Literal[
         "Active", "A valider", "Révoquée", "A revérifier", "Obsolète", "Refusée"
     ]
     DEFAULT_ACCESS_RIGHT_STATE = get_args(AccessRightState)
     ProofControlStatus = Literal[
         "Preuve en attente",
@@ -198,24 +216,56 @@
             f"{self.api}/pce/{pce}/donnees_consos_informatives",
             params={
                 "date_debut": from_date,
                 "date_fin": to_date,
             },
         )
 
+    def donnees_injections_publiees(
+        self, pce: str, from_date: str, to_date: str
+    ) -> Any:
+        return self.get(
+            f"{self.api}/pce/{pce}/donnees_injections_publiees",
+            params={
+                "date_debut": from_date,
+                "date_fin": to_date,
+            },
+        )
+
     def donnees_contractuelles(self, pce: str) -> Any:
         (payload,) = self.get(f"{self.api}/pce/{pce}/donnees_contractuelles")
         return payload
 
     def donnees_techniques(self, pce: str) -> Any:
         (payload,) = self.get(f"{self.api}/pce/{pce}/donnees_techniques")
         return payload
 
 
 class StagingAPI(BaseAPI):
-    scope = "/adict/bas/v4"
-    api = "https://api.grdf.fr/adict/bas/v4"
+    scope = "/adict/bas/v6"
+    api = "https://api.grdf.fr/adict/bas/v6"
+
+    def _authenticate_with_fallback(self) -> tuple[str, float]:
+        return self._authenticate(auth_endpoint=OLD_AUTH_ENDPOINT)
+
+    def _parse_response(self, resp: requests.Response) -> Any:
+        # XXX: Adjusts GRDF API responses to fit ndjson expected input because
+        # GRDF Staging API v6 responses contain multiple-lines JSON objects
+        # whereas ndjson expects one-line JSON objects
+        return ndjson.loads(resp.text.replace("\n", "").replace("}{", "}\n{"))
+
+    def donnees_injections_publiees(
+        self, pce: str, from_date: str, to_date: str
+    ) -> Any:
+        # XXX: Temporary fix for Staging API v6 that as an incorrect endpoint
+        return self.get(
+            f"{self.api}/pce/{pce}/donnees_injection_publiees",
+            params={
+                "date_debut": from_date,
+                "date_fin": to_date,
+            },
+        )
 
 
 class API(BaseAPI):
     scope = "/adict/v2"
     api = "https://api.grdf.fr/adict/v2"
```

### Comparing `lowatt_grdf-2.1.4/lowatt_grdf/main.py` & `lowatt_grdf-2.2.0/lowatt_grdf/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,14 +178,31 @@
 ) -> None:
     grdf = {True: api.StagingAPI, False: api.API}[bas](client_id, client_secret)
     rich.print_json(data=grdf.donnees_consos_informatives(pce, from_date, to_date))
 
 
 @main.command()
 @click.argument("pce")
+@click.option("--from-date", required=True)
+@click.option("--to-date", required=True)
+@api_options
+def donnees_injections_publiees(
+    client_id: str,
+    client_secret: str,
+    bas: bool,
+    pce: str,
+    from_date: str,
+    to_date: str,
+) -> None:
+    grdf = {True: api.StagingAPI, False: api.API}[bas](client_id, client_secret)
+    rich.print_json(data=grdf.donnees_injections_publiees(pce, from_date, to_date))
+
+
+@main.command()
+@click.argument("pce")
 @api_options
 def donnees_contractuelles(
     client_id: str,
     client_secret: str,
     bas: bool,
     pce: str,
 ) -> None:
```

### Comparing `lowatt_grdf-2.1.4/lowatt_grdf/models.py` & `lowatt_grdf-2.2.0/lowatt_grdf/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 from . import LOGGER
 
 
 def validate_date_format(
     instance: Any, attribute: "attrs.Attribute[str]", value: Any
 ) -> None:
+    if value is None:
+        return
     assert isinstance(value, str), type(value)
     try:
         time.strptime(value, "%Y-%m-%d")
     except ValueError as exc:
         raise ValueError(
             f"format of {attribute} must be 'YYYY-MM-DD', got {value}"
         ) from exc
@@ -46,49 +48,78 @@
 
 
 @attrs.frozen
 class DeclareAccess(BaseModel):
     pce: str
     code_postal: str
     courriel_titulaire: str
-    date_consentement_declaree: str = attrs.field(validator=validate_date_format)
     date_debut_droit_acces: str = attrs.field(validator=validate_date_format)
     date_fin_droit_acces: str = attrs.field(validator=validate_date_format)
-    perim_donnees_conso_debut: str = attrs.field(validator=validate_date_format)
-    perim_donnees_conso_fin: str = attrs.field(validator=validate_date_format)
+    perim_donnees_conso_debut: Optional[str] = attrs.field(
+        validator=validate_date_format, default=None
+    )
+    perim_donnees_conso_fin: Optional[str] = attrs.field(
+        validator=validate_date_format, default=None
+    )
+    perim_donnees_inj_debut: Optional[str] = attrs.field(
+        validator=validate_date_format, default=None
+    )
+    perim_donnees_inj_fin: Optional[str] = attrs.field(
+        validator=validate_date_format, default=None
+    )
     raison_sociale: Optional[str] = None
     nom_titulaire: Optional[str] = None
     role_tiers: str = "AUTORISE_CONTRAT_FOURNITURE"
-    numero_telephone_titulaire: Optional[str] = None
+    numero_telephone_mobile_titulaire: Optional[str] = None
     perim_donnees_contractuelles: bool = False
     perim_donnees_techniques: bool = False
     perim_donnees_informatives: bool = False
     perim_donnees_publiees: bool = False
 
     def __attrs_post_init__(self) -> None:
         if not self.raison_sociale and not self.nom_titulaire:
             raise ValueError("One of raison-sociale or nom-titulaire must be specified")
 
+        if "FOURNITURE" in self.role_tiers:
+            if not self.perim_donnees_conso_debut or not self.perim_donnees_conso_fin:
+                raise ValueError(
+                    f"Both perim-donnees-conso-debut and perim-donnees-conso-fin must be specified when role-tiers is set to {self.role_tiers}"
+                )
+            if self.perim_donnees_inj_debut or self.perim_donnees_inj_fin:
+                raise ValueError(
+                    f"Neither perim-donnees-inj-debut nor perim-donnees-inj-fin should be specified when role-tiers is set to {self.role_tiers}"
+                )
+        elif "INJECTION" in self.role_tiers:
+            if not self.perim_donnees_inj_debut or not self.perim_donnees_inj_fin:
+                raise ValueError(
+                    f"Both perim_donnees_inj_debut and perim_donnees_inj_fin must be specified when role-tiers is set to {self.role_tiers}"
+                )
+            if self.perim_donnees_conso_debut or self.perim_donnees_conso_fin:
+                raise ValueError(
+                    f"Neither perim_donnees_conso_debut nor perim_donnees_conso_fin should be specified when role-tiers is set to {self.role_tiers}"
+                )
+
 
 @attrs.frozen
 class Access(BaseModel):
     pce: str
     etat_droit_acces: str
     perim_donnees_publiees: bool
     perim_donnees_informatives: bool
     courriel_titulaire: str
     statut_controle_preuve: Optional[str]
     date_debut_droit_acces: str
     date_fin_droit_acces: str
-    perim_donnees_conso_debut: str
-    perim_donnees_conso_fin: str
+    perim_donnees_conso_debut: Optional[str] = None
+    perim_donnees_conso_fin: Optional[str] = None
+    perim_donnees_inj_debut: Optional[str] = None
+    perim_donnees_inj_fin: Optional[str] = None
     raison_sociale_du_titulaire: Optional[str] = None
     nom_titulaire: Optional[str] = None
-    date_consentement_declaree: Optional[str] = None
-    numero_telephone_titulaire: Optional[str] = None
+    numero_telephone_mobile_titulaire: Optional[str] = None
     perim_donnees_contractuelles: bool = False
     perim_donnees_techniques: bool = False
 
     def __attrs_post_init__(self) -> None:
         if not self.raison_sociale_du_titulaire and not self.nom_titulaire:
             raise ValueError(
                 "One of raison_sociale_du_titulaire or nom_titulaire is expected"
@@ -161,17 +192,14 @@
 )
 converter.register_unstructure_hook(
     DeclareAccess,
     cattrs.gen.make_dict_unstructure_fn(
         DeclareAccess,
         converter,
         pce=cattrs.gen.override(omit=True),
-        date_consentement_declaree=cattrs.gen.override(
-            unstruct_hook=lambda v: v + " 00:00:00"
-        ),
         **{  # type: ignore[arg-type]
             f.name: cattrs.gen.override(unstruct_hook=unstructure_grdf_bool)
-            for f in attrs.fields(Access)
+            for f in attrs.fields(DeclareAccess)
             if f.type == bool
         },
     ),
 )
```

### Comparing `lowatt_grdf-2.1.4/tests/test_api.py` & `lowatt_grdf-2.2.0/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from lowatt_grdf import api, models
 
 
 @pytest.fixture
 def grdf() -> api.API:
     responses.add(
         responses.POST,
-        f"{api.OPENID_ENDPOINT}/access_token",
+        api.NEW_AUTH_ENDPOINT,
         json={
             "access_token": "xxx",
             "expires_in": 14400,
         },
     )
     return api.API("id", "secret")
 
@@ -99,20 +99,22 @@
     "id_pce": "GI000000",
     "role_tiers": "AUTORISE_CONTRAT_FOURNITURE",
     "raison_sociale_du_tiers": "DUMMY",
     "nom_titulaire": None,
     "raison_sociale_du_titulaire": "John Doe Inc.",
     "courriel_titulaire": "jdoe@example.com",
     "code_postal": "99099",
-    "numero_telephone_titulaire": "0600000000",
+    "numero_telephone_mobile_titulaire": "0600000000",
     "perim_donnees_informatives": "Vrai",
     "perim_donnees_contractuelles": "Vrai",
     "perim_donnees_techniques:": "Vrai",
     "perim_donnees_conso_debut": "2020-01-01",
     "perim_donnees_conso_fin": "2025-01-01",
+    "perim_donnees_inj_debut": None,
+    "perim_donnees_inj_fin": None,
     "perim_donnees_publiees": "Vrai",
     "date_creation": "2021-07-02 16:41:14",
     "date_debut_droit_acces": "2021-07-02",
     "date_fin_droit_acces": "2030-01-01",
     "etat_droit_acces": "Active",
     "date_revocation": None,
     "source_revocation": None,
@@ -120,15 +122,14 @@
     "source_passage_a_obsolete": None,
     "date_fin_autorisation": "2023-07-02 00:00:00",
     "date_passage_a_refuse": None,
     "source_passage_a_refuse": None,
     "parcours": "CLIENT_CONNECT",
     "statut_controle_preuve": None,
     "date_limite_transmission_preuve": None,
-    "date_consentement_declaree": None,
 }
 
 
 @responses.activate
 def test_droits_acces(grdf: api.API) -> None:
     payload = [
         ACCESS_PAYLOAD,
@@ -427,38 +428,38 @@
 @responses.activate
 def test_declare_acces(grdf: api.API, caplog: pytest.LogCaptureFixture) -> None:
     access = models.DeclareAccess(
         pce="23000000000000",
         nom_titulaire="jdoe",
         code_postal="99099",
         courriel_titulaire="jdoe@example.com",
-        numero_telephone_titulaire="0600000000",
+        numero_telephone_mobile_titulaire="0600000000",
         date_debut_droit_acces="2020-01-01",
         date_fin_droit_acces="2025-12-31",
         perim_donnees_conso_debut="2020-01-01",
         perim_donnees_conso_fin="2020-01-01",
         raison_sociale="dummy",
-        date_consentement_declaree="2020-01-01",
     )
     # XXX: use a real life response
     responses.add(responses.PUT, f"{grdf.api}/pce/23000000000000/droit_acces", json={})
     with caplog.at_level(logging.INFO, logger="lowatt.grdf"):
         grdf.declare_acces(access)
     body = responses.calls[-1].request.body
     assert body is not None
     assert json.loads(body) == {
         "code_postal": "99099",
         "courriel_titulaire": "jdoe@example.com",
-        "date_consentement_declaree": "2020-01-01 00:00:00",
         "date_debut_droit_acces": "2020-01-01",
         "date_fin_droit_acces": "2025-12-31",
         "nom_titulaire": "jdoe",
-        "numero_telephone_titulaire": "0600000000",
+        "numero_telephone_mobile_titulaire": "0600000000",
         "perim_donnees_conso_debut": "2020-01-01",
         "perim_donnees_conso_fin": "2020-01-01",
+        "perim_donnees_inj_debut": None,
+        "perim_donnees_inj_fin": None,
         "perim_donnees_contractuelles": "Faux",
         "perim_donnees_informatives": "Faux",
         "perim_donnees_publiees": "Faux",
         "perim_donnees_techniques": "Faux",
         "raison_sociale": "dummy",
         "role_tiers": "AUTORISE_CONTRAT_FOURNITURE",
     }
```

### Comparing `lowatt_grdf-2.1.4/tests/test_main.py` & `lowatt_grdf-2.2.0/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
   -h, --help  Show this message and exit.
 
 Commands:
   declare-acces
   donnees-consos-informatives
   donnees-consos-publiees
   donnees-contractuelles
+  donnees-injections-publiees
   donnees-techniques
   droits-acces
   droits-acces-specifiques
 """
     )
 
 
@@ -59,27 +60,26 @@
 Options:
   --bas                           Use staging (bac à sable) environment
   --client-secret TEXT            openid client secret  [required]
   --client-id TEXT                openid client id  [required]
   --pce TEXT                      [required]
   --code-postal TEXT              [required]
   --courriel-titulaire TEXT       [required]
-  --date-consentement-declaree YYYY-MM-DD
-                                  [required]
   --date-debut-droit-acces YYYY-MM-DD
                                   [required]
   --date-fin-droit-acces YYYY-MM-DD
                                   [required]
   --perim-donnees-conso-debut TEXT
-                                  [required]
-  --perim-donnees-conso-fin TEXT  [required]
+  --perim-donnees-conso-fin TEXT
+  --perim-donnees-inj-debut TEXT
+  --perim-donnees-inj-fin TEXT
   --raison-sociale TEXT
   --nom-titulaire TEXT
   --role-tiers TEXT
-  --numero-telephone-titulaire TEXT
+  --numero-telephone-mobile-titulaire TEXT
   --perim-donnees-contractuelles
   --perim-donnees-techniques
   --perim-donnees-informatives
   --perim-donnees-publiees
   -h, --help                      Show this message and exit.
 """
     )
```

### Comparing `lowatt_grdf-2.1.4/tests/test_models.py` & `lowatt_grdf-2.2.0/tests/test_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 def test_structure_access() -> None:
     obj = models.converter.structure(
         {
             "id_pce": "0123",
             "perim_donnees_conso_debut": "2023-07-11",
             "perim_donnees_conso_fin": "2022-07-11",
+            "perim_donnees_inj_debut": None,
+            "perim_donnees_inj_fin": None,
             "date_debut_droit_acces": "2022-07-11",
             "date_fin_droit_acces": "2023-07-11",
             "statut_controle_preuve": None,
             "raison_sociale_du_titulaire": "COGIP",
             "courriel_titulaire": "cogip@example.com",
             "perim_donnees_informatives": "Vrai",
             "perim_donnees_publiees": "Faux",
@@ -19,14 +21,16 @@
         },
         models.Access,
     )
     assert obj == models.Access(
         pce="0123",
         perim_donnees_conso_debut="2023-07-11",
         perim_donnees_conso_fin="2022-07-11",
+        perim_donnees_inj_debut=None,
+        perim_donnees_inj_fin=None,
         date_debut_droit_acces="2022-07-11",
         date_fin_droit_acces="2023-07-11",
         statut_controle_preuve=None,
         nom_titulaire=None,
         raison_sociale_du_titulaire="COGIP",
         courriel_titulaire="cogip@example.com",
         perim_donnees_informatives=True,
@@ -36,33 +40,33 @@
 
 
 def test_unstructure_declare_access() -> None:
     obj = models.DeclareAccess(
         pce="0123",
         code_postal="42000",
         courriel_titulaire="cogip@example.com",
-        date_consentement_declaree="2022-07-11",
         date_debut_droit_acces="2022-07-11",
         date_fin_droit_acces="2023-07-11",
         perim_donnees_conso_debut="2023-07-11",
         perim_donnees_conso_fin="2022-07-11",
         raison_sociale="COGIP",
         perim_donnees_informatives=True,
         perim_donnees_publiees=True,
     )
     assert models.converter.unstructure(obj) == {
         "code_postal": "42000",
         "courriel_titulaire": "cogip@example.com",
-        "date_consentement_declaree": "2022-07-11 00:00:00",
         "date_debut_droit_acces": "2022-07-11",
         "date_fin_droit_acces": "2023-07-11",
         "nom_titulaire": None,
-        "numero_telephone_titulaire": None,
+        "numero_telephone_mobile_titulaire": None,
         "perim_donnees_conso_debut": "2023-07-11",
         "perim_donnees_conso_fin": "2022-07-11",
+        "perim_donnees_inj_debut": None,
+        "perim_donnees_inj_fin": None,
         "perim_donnees_contractuelles": "Faux",
         "perim_donnees_informatives": "Vrai",
         "perim_donnees_publiees": "Vrai",
         "perim_donnees_techniques": "Faux",
         "raison_sociale": "COGIP",
         "role_tiers": "AUTORISE_CONTRAT_FOURNITURE",
     }
```

### Comparing `lowatt_grdf-2.1.4/LICENSE` & `lowatt_grdf-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.1.4/README.md` & `lowatt_grdf-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.1.4/pyproject.toml` & `lowatt_grdf-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.1.4/PKG-INFO` & `lowatt_grdf-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lowatt-grdf
-Version: 2.1.4
+Version: 2.2.0
 Summary: Python client for GRDF ADICT API
 Project-URL: Source, https://github.com/lowatt/lowatt-grdf
 Project-URL: Tracker, https://github.com/lowatt/lowatt-grdf/issues
 Author-email: Lowatt <info@lowatt.fr>
 License: GPLv3
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

