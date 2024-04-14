# Comparing `tmp/detadoc-0.2.7.tar.gz` & `tmp/detadoc-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detadoc-0.2.7.tar", max compression
+gzip compressed data, was "detadoc-0.2.8.tar", max compression
```

## Comparing `detadoc-0.2.7.tar` & `detadoc-0.2.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-12-30 15:32:37.773402 detadoc-0.2.7/detadoc/__init__.py
--rw-r--r--   0        0        0     1871 2024-02-04 21:38:04.629317 detadoc-0.2.7/detadoc/annotations.py
--rw-r--r--   0        0        0     3745 2024-03-27 03:28:40.331199 detadoc-0.2.7/detadoc/bases.py
--rw-r--r--   0        0        0     9746 2024-04-01 19:44:24.905798 detadoc-0.2.7/detadoc/enum.py
--rw-r--r--   0        0        0     2336 2024-03-04 23:54:12.920957 detadoc-0.2.7/detadoc/helper.py
--rw-r--r--   0        0        0    46634 2024-04-02 00:56:53.301351 detadoc-0.2.7/detadoc/models.py
--rw-r--r--   0        0        0     4988 2024-03-24 19:05:37.271242 detadoc-0.2.7/detadoc/regex.py
--rw-r--r--   0        0        0      519 2024-04-02 14:18:14.244967 detadoc-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      760 2024-04-02 14:18:53.755564 detadoc-0.2.7/setup.py
--rw-r--r--   0        0        0      593 2024-04-02 14:18:53.755780 detadoc-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-30 15:32:37.773402 detadoc-0.2.8/detadoc/__init__.py
+-rw-r--r--   0        0        0     1871 2024-02-04 21:38:04.629317 detadoc-0.2.8/detadoc/annotations.py
+-rw-r--r--   0        0        0     3745 2024-03-27 03:28:40.331199 detadoc-0.2.8/detadoc/bases.py
+-rw-r--r--   0        0        0     9746 2024-04-01 19:44:24.905798 detadoc-0.2.8/detadoc/enum.py
+-rw-r--r--   0        0        0     2336 2024-03-04 23:54:12.920957 detadoc-0.2.8/detadoc/helper.py
+-rw-r--r--   0        0        0    55246 2024-04-14 21:34:01.033666 detadoc-0.2.8/detadoc/models.py
+-rw-r--r--   0        0        0     4988 2024-03-24 19:05:37.271242 detadoc-0.2.8/detadoc/regex.py
+-rw-r--r--   0        0        0      519 2024-04-14 22:50:02.232567 detadoc-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-14 22:51:03.569157 detadoc-0.2.8/setup.py
+-rw-r--r--   0        0        0      593 2024-04-14 22:51:03.569388 detadoc-0.2.8/PKG-INFO
```

### Comparing `detadoc-0.2.7/detadoc/annotations.py` & `detadoc-0.2.8/detadoc/annotations.py`

 * *Files identical despite different names*

### Comparing `detadoc-0.2.7/detadoc/bases.py` & `detadoc-0.2.8/detadoc/bases.py`

 * *Files identical despite different names*

### Comparing `detadoc-0.2.7/detadoc/enum.py` & `detadoc-0.2.8/detadoc/enum.py`

 * *Files identical despite different names*

### Comparing `detadoc-0.2.7/detadoc/helper.py` & `detadoc-0.2.8/detadoc/helper.py`

 * *Files identical despite different names*

### Comparing `detadoc-0.2.7/detadoc/models.py` & `detadoc-0.2.8/detadoc/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from ormspace import functions
 from ormspace.enum import StrEnum
 from ormspace.functions import string_to_list
 from ormspace.keys import TableKey
 from ormspace.metainfo import MetaInfo
 from spacestar.model import SpaceModel
 from ormspace.model import getmodel, modelmap, SearchModel
-from ormspace.annotations import DateField, DateTimeField, ListOfStrings, OptionalDate, OptionalFloat, PasswordField, \
+from ormspace.annotations import DateField, DateTimeField, ListOfStrings, OptionalDate, OptionalFloat, OptionalInteger, \
+    PasswordField, \
     PositiveDecimalField, \
     PositiveIntegerField
 from pydantic import BaseModel, BeforeValidator, computed_field, Field
 from starlette.requests import Request
 from typing_extensions import Self
 
 from detadoc.annotations import BodyMeasureFloat, BodyMeasureInteger, OptionalBoolean
@@ -527,19 +528,21 @@
 
 @modelmap
 class ServiceInvoice(Invoice, PatientKeyBase):
     REVENUE_ACCOUNT = Account.SRE
     EXPENSE_ACCOUNT = Account.SEX
     INVOICE_TYPE = InvoiceType.S
     TABLE_NAME = 'Invoice'
+    EXIST_QUERY = None
     service_key: Service.Key
     description: Optional[str] = Field('Receita de Serviço')
     discount: Annotated[
         PositiveDecimalField, Field(Decimal('0')), BeforeValidator(lambda x: Decimal('0') if not x else Decimal(x))]
     flow: CashFlow = CashFlow.RE
+    tax: bool = False
 
     def __str__(self):
         self.description = f'{self.service or self.service_key} {self.patient or self.patient_key}'
         return super().__str__()
 
     async def setup_instance(self):
         if not self.patient:
@@ -720,14 +723,175 @@
         return self.date < other.date
     
     
     def __str__(self):
         return f'{self.date} ({functions.years(self.date, self.patient.bdate)} anos): {self.title}'
     
     
+def concatenate(items: list[str]) -> str:
+    if len(items) > 0:
+        return items[0] if len(items) == 1 else " e ".join(items) if len(items) == 2 else ", ".join(items[:-1]) + f' e {items[-1]}'
+    return ''
+    
+@modelmap
+class MedicalReport(PatientKeyBase):
+    EXIST_QUERY = None
+    
+    @enummap
+    class EvolutionType(StrEnum):
+        A = 'Aguda'
+        B = 'Subaguda'
+        C = 'Crônica'
+        I = 'Indefinida'
+        
+    @enummap
+    class ReportType(StrEnum):
+        A = 'Relatório Médico'
+        B = 'Atestado Médico'
+        C = 'Laudo Médico'
+        
+        def write(self, applicant: str = 'pelo paciente', authorizer: str = 'pelo paciente'):
+            with io.StringIO() as buf:
+                buf.write(f'Documento solicitado {applicant} para fins de ')
+                if self.name == 'A':
+                    buf.write('informação sobre quadro clínico, diagnóstico e tratamento atuais. ')
+                elif self.name == 'B':
+                    buf.write('afastamento por motivo de doença. ')
+                elif self.name == 'C':
+                    buf.write(
+                        'documentação do tratamento médico do quadro inicial a apresentação atual, discussão diagnóstica e terapêutica. ')
+                buf.write(
+                    f'O conteúdo é sigiloso e proveniente de prontuário médico. A divulgação destes dados foi expressamente autorizada {authorizer}. ')
+                return buf.getvalue()
+            
+    report_type: ReportType
+    since: OptionalInteger
+    start_date: OptionalDate
+    start_symptoms: ListOfStrings
+    evolution_type: EvolutionType
+    episode_symptoms: ListOfStrings
+    episode_treatment: ListOfStrings
+    current_symptoms: ListOfStrings
+    current_treatment: ListOfStrings
+    triggering_factors: ListOfStrings
+    maintenance_factors: ListOfStrings
+    constitutional_factors: ListOfStrings
+    assessment: str
+    
+    @enummap
+    class Disability(StrEnum):
+        A = 'Capaz'
+        B = 'Incapacidade Parcial Temporária'
+        C = 'Incapacidade Parcial Definitiva'
+        D = 'Incapacidade Total Temporária'
+        E = 'Incapacidade Total Definitiva'
+        I = 'Indefinido'
+        
+        @property
+        def phrase(self):
+            if self.name == 'A':
+                return 'O paciente não exibe prejuízo de funcionalidade e é considerado capaz para o exercício das suas atividades. '
+            elif self.name == 'B':
+                return 'O paciente apresenta limitação da funcionalidade de forma parcial e temporária, com expectativa de recuperação completa. '
+            elif self.name == 'C':
+                return 'O paciente apresenta limitação da funcionalidade de forma parcial porém definitiva, sem expectativa de recuperação completa. Encontra-se apto para parte das atividades. '
+            elif self.name == 'D':
+                return 'O paciente encontra-se no momento incapacitado para o exercício de suas atividades. Esta limitação é temporária, com expectativa de recuperação completa. '
+            elif self.name == 'E':
+                return 'Do ponto de vista funcional o paciente é considerado definitivamente incapaz para o exercício de suas atividades, sem expectativa de recuperação. '
+    
+    disability_status: Disability
+    disability_issues: ListOfStrings
+    cids: ListOfStrings
+    licence_days: OptionalInteger
+    
+    def __str__(self):
+        return f'{self.report_type.value} {self.date.day} de {Month.read_int(self.date.month).value} de {self.date.year}'
+    
+    @property
+    def symptoms(self):
+        with io.StringIO() as buf:
+            if self.since:
+                buf.write(f'Paciente em acompanhamento médico desde {self.since}')
+            else:
+                buf.write(f'Paciente em acompanhamento médico')
+            if self.start_symptoms:
+                if self.start_date:
+                    buf.write(f' com quadro inicial de *{concatenate(self.start_symptoms)}*')
+                    buf.write(f' em {Month.read_int(self.start_date.month).value} de {self.start_date.year}')
+                else:
+                    buf.write(f' com quadro inicial de *{concatenate(self.start_symptoms)}*')
+                buf.write(f'. ')
+            if self.episode_symptoms:
+                if self.evolution_type.name != "I":
+                    buf.write(f'A evolução ocorreu de forma {self.evolution_type.value.lower()} apresentando {concatenate(self.episode_symptoms)}. ')
+                else:
+                    buf.write(f'Ao longo da evolução apresentou {concatenate(self.episode_symptoms)}. ')
+            if self.episode_treatment:
+                if len(self.episode_treatment) == 1:
+                    buf.write(f'Foi utilizado como tratamento medicamentoso {concatenate(self.episode_treatment)} sem evidência de resposta adequada. ')
+                else:
+                    buf.write(f'Foram utilizadas como estratégia medicamentosa {concatenate(self.episode_treatment)} sem evidência de resposta adequada. ')
+            if self.current_symptoms:
+                if len(self.current_symptoms) == 1:
+                    buf.write(f'Atualmente o principal sintoma é **{concatenate(self.current_symptoms)}**')
+                else:
+                    buf.write(f'Atualmente os principais sintomas são **{concatenate(self.current_symptoms)}**')
+                if self.current_treatment:
+                    buf.write(f' e está em uso no momento de **{concatenate(self.current_treatment)}**')
+                buf.write(f'. ')
+            return buf.getvalue()
+        
+    @property
+    def factors(self):
+        if any([self.triggering_factors, self.maintenance_factors, self.constitutional_factors]):
+            with io.StringIO() as buf:
+                if self.triggering_factors:
+                    if len(self.triggering_factors) == 1:
+                        buf.write(f'Fator possivelmente desencadeador do quadro clínico foi {concatenate(self.triggering_factors)}.\n')
+                    else:
+                        buf.write(f'Fatores possivelmente desencadeadores do quadro clínico foram {concatenate(self.triggering_factors)}.\n')
+                if self.maintenance_factors:
+                    buf.write(f'A recuperação tem sido prejudicada por {concatenate(self.maintenance_factors)}.\n')
+                if self.constitutional_factors:
+                    buf.write(f'O paciente é constitucionalmente afetado por {concatenate(self.constitutional_factors)}.\n')
+                return buf.getvalue()
+        return ''
+    
+    @property
+    def conclusion(self):
+        with io.StringIO() as buf:
+            if self.assessment:
+                buf.write(f'{self.assessment} ')
+            if self.disability_issues:
+                buf.write(f'A funcionalidade encontra-se prejudicada por {concatenate(self.disability_issues)}. ')
+            if self.disability_status.name != 'I':
+                buf.write(self.disability_status.phrase)
+            if self.licence_days:
+                buf.write(
+                    f' Solicito licença médica por **{self.licence_days} dias a partir de {self.date.day} de {Month.read_int(self.date.month).value} de {self.date.year}** para acompanhamento e controle do quadro. ')
+            return buf.getvalue()
+        
+    def markup(self) -> Markup:
+        with io.StringIO() as buf:
+            buf.write(f'# {self.report_type.value}\n\n')
+            buf.write(f'{self.date.day} de {Month.read_int(self.date.month).value} de {self.date.year}')
+            buf.write(f'\n\n---\n\n')
+            buf.write(f'\n{self.report_type.write()}\n\n')
+            buf.write(self.symptoms)
+            buf.write(self.factors)
+            buf.write('\n')
+            buf.write(self.conclusion)
+            if self.cids:
+                buf.write('\n\n```CID: {}```\n\n'.format(' + '.join(self.cids)))
+            buf.write(f'\nSem mais para o momento, me encontro à disposição para esclarecimentos adicionais caso necessário.\n')
+            return Markup(markdown(buf.getvalue()))
+    
+
+
 @modelmap
 class Report(PatientKeyBase):
     SINGULAR = 'Relatório'
     title: str = 'Relatório Médico'
     content: str
     
     @property
@@ -830,16 +994,16 @@
     
     def __lt__(self, other):
         assert isinstance(other, type(self))
         return self.start < other.start
     
     def __str__(self):
         if self.end:
-            return f'{self.created}: {self.medication.name} {self.dosage} {self.medication.dosage_form.value.lower()} {self.frequency.value}/{self.period.value}  {self.notes or ""}. [{self.start} a {self.end}]'
-        return f'{self.created}: {self.medication.name} {self.dosage} {self.medication.dosage_form.value.lower()} {self.frequency.value}/{self.period.value}  {self.notes or ""}. [{self.remaining_days}/{self.duration} dias, {self.computed_boxes} cx]'
+            return f'{self.start}: {self.medication.name} {self.dosage} {self.medication.dosage_form.value.lower()} {self.frequency.value}/{self.period.value}  {self.notes or ""}. [{self.start} a {self.end}]'
+        return f'{self.start}: {self.medication.name} {self.dosage} {self.medication.dosage_form.value.lower()} {self.frequency.value}/{self.period.value}  {self.notes or ""}. [{self.remaining_days}/{self.duration} dias, {self.computed_boxes} cx]'
     
     # def asjson(self):
     #     data = super().asjson()
     #     data.pop('search', None)
     #     return data
 
     @property
@@ -899,14 +1063,21 @@
     bed_time: DayTime
     sleep_time: DayTime
     awake_time: DayTime
     rise_time: DayTime
     quality: Quality
     awakes: PositiveIntegerField = 0
     notes: str = Field(default_factory=str)
+    symptoms: ListOfStrings = Field(default_factory=list)
+    medications: ListOfStrings = Field(default_factory=list)
+    
+    def __str__(self):
+        with io.StringIO() as buf:
+            buf.write(f"dorme em geral das {self.sleep_time.value}h às {self.awake_time.value}; latência de {self.bed_to_sleep_minutes} minutos, e {self.awake_to_rise_minutes} minutos para levantar")
+            return buf.getvalue()
     
     @staticmethod
     def subtracted(value: DayTime):
         return int(DayTime.T23_59) - int(value)
     
     @property
     def bed_to_sleep_minutes(self):
@@ -951,36 +1122,37 @@
     messages: list[ProfileMessage]
     
 
 @modelmap
 class PhysicalExam(PatientKeyBase):
     SINGULAR = 'Exame Físico'
     PLURAL = 'Exames Físicos'
+    EXIST_QUERY = None
     key: Optional[str] = Field(None, title='Chave')
     # created: DateField = Field(title='Criado em')
     weight: BodyMeasureFloat = Field(title='Peso (Kg)')
     height: BodyMeasureFloat = Field(title='Altura (cm)')
     waist: BodyMeasureFloat = Field(title='Cintura (cm)')
     hip: BodyMeasureFloat = Field(title='Quadril (cm)')
     sbp: BodyMeasureInteger = Field(title='PAS')
     dbp: BodyMeasureInteger = Field(title='PAD')
     hr: BodyMeasureInteger = Field(title='FC (bpm)')
     rr: BodyMeasureInteger = Field(title='FR (rpm)')
     notes: Optional[str] = None
     
-    @property
-    def date(self):
-        return self.created
+    # @property
+    # def date(self):
+    #     return self.created
     
     def __lt__(self, other):
-        return self.created < other.created
+        return self.date < other.date
     
     def __str__(self):
         with StringIO() as buf:
-            buf.write(f'{self.created} {self.daytime.value} Exame Físico: ')
+            buf.write(f'{self.date} {self.daytime.value} Exame Físico: ')
             for k, v in self.model_fields.items():
                 if value := getattr(self, k):
                     if k == 'weight':
                         buf.write(f"peso {value}Kg; ")
                     elif k == 'height':
                         buf.write(f"altura {value}cm; ")
                     elif k == 'waist':
```

### Comparing `detadoc-0.2.7/detadoc/regex.py` & `detadoc-0.2.8/detadoc/regex.py`

 * *Files identical despite different names*

### Comparing `detadoc-0.2.7/pyproject.toml` & `detadoc-0.2.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "detadoc"
-version = "0.2.7"
+version = "0.2.8"
 description = ""
 authors = ["Daniel Arantes <arantesdv@me.com>"]
 exclude = ['src', '.space', 'Spacefile', '.env', 'dev.py']
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bcrypt = "^4.1.1"
```

### Comparing `detadoc-0.2.7/setup.py` & `detadoc-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'httpx[http2]>=0.26.0,<0.27.0',
  'hx-markup>=0.2.2,<0.3.0',
  'requests>=2.31.0,<3.0.0',
  'spacestar>=0.3.1,<0.4.0']
 
 setup_kwargs = {
     'name': 'detadoc',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `detadoc-0.2.7/PKG-INFO` & `detadoc-0.2.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detadoc
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

