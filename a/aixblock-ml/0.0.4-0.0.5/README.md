# Comparing `tmp/aixblock_ml-0.0.4.tar.gz` & `tmp/aixblock_ml-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_ml-0.0.4.tar", max compression
+gzip compressed data, was "aixblock_ml-0.0.5.tar", max compression
```

## Comparing `aixblock_ml-0.0.4.tar` & `aixblock_ml-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       11 2024-04-03 07:28:40.006140 aixblock_ml-0.0.4/README.md
--rw-r--r--   0        0        0       84 2024-04-04 08:01:18.783734 aixblock_ml-0.0.4/aixblock_ml/__init__.py
--rw-r--r--   0        0        0     8928 2024-04-03 08:23:03.325146 aixblock_ml-0.0.4/aixblock_ml/api.py
--rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.4/aixblock_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2024-04-01 06:20:49.119434 aixblock_ml-0.0.4/aixblock_ml/default_configs/README.md
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.490661 aixblock_ml-0.0.4/aixblock_ml/default_configs/_wsgi.py
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.0.4/aixblock_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.0.4/aixblock_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0     2139 2024-04-04 03:08:16.489392 aixblock_ml-0.0.4/aixblock_ml/default_configs/model.py
--rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.4/aixblock_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.4/aixblock_ml/exceptions.py
--rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.4/aixblock_ml/helpers.py
--rw-r--r--   0        0        0    34692 2024-04-03 08:23:03.374785 aixblock_ml-0.0.4/aixblock_ml/model.py
--rw-r--r--   0        0        0     7487 2024-04-04 02:14:25.160523 aixblock_ml-0.0.4/aixblock_ml/server.py
--rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.4/aixblock_ml/templates/preview.html
--rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.0.4/aixblock_ml/utils.py
--rw-r--r--   0        0        0      313 2024-04-04 08:03:41.454706 aixblock_ml-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 aixblock_ml-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-04-03 07:28:40.006140 aixblock_ml-0.0.5/README.md
+-rw-r--r--   0        0        0       84 2024-04-04 08:01:18.783734 aixblock_ml-0.0.5/aixblock_ml/__init__.py
+-rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.0.5/aixblock_ml/api.py
+-rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.5/aixblock_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.0.5/aixblock_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.490661 aixblock_ml-0.0.5/aixblock_ml/default_configs/_wsgi.py
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.0.5/aixblock_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.0.5/aixblock_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0     2129 2024-04-15 02:26:57.535807 aixblock_ml-0.0.5/aixblock_ml/default_configs/model.py
+-rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.5/aixblock_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.5/aixblock_ml/exceptions.py
+-rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.5/aixblock_ml/helpers.py
+-rw-r--r--   0        0        0    35732 2024-04-15 02:32:53.891767 aixblock_ml-0.0.5/aixblock_ml/model.py
+-rw-r--r--   0        0        0     7477 2024-04-15 02:26:57.534982 aixblock_ml-0.0.5/aixblock_ml/server.py
+-rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.5/aixblock_ml/templates/preview.html
+-rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.0.5/aixblock_ml/utils.py
+-rw-r--r--   0        0        0      314 2024-04-15 02:46:13.033061 aixblock_ml-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 aixblock_ml-0.0.5/PKG-INFO
```

### Comparing `aixblock_ml-0.0.4/aixblock_ml/api.py` & `aixblock_ml-0.0.5/aixblock_ml/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 def init_app(model_class, **kwargs):
     global _manager
     _manager.initialize(model_class, **kwargs)
     CORS(_server)
     return _server
 
 
-@_server.route('/predict', methods=['POST'])
-@exception_handler
-def _predict():
-    data = request.json
-    tasks = data.get('tasks')
-    project = data.get('project')
-    label_config = data.get('label_config')
-    force_reload = data.get('force_reload', False)
-    try_fetch = data.get('try_fetch', True)
-    params = data.get('params') or {}
-    predictions, model = _manager.predict(
-        tasks, project, label_config, force_reload, try_fetch, **params)
-    response = {
-        'results': predictions,
-        'model_version': model.model_version
-    }
-    return jsonify(response)
+# @_server.route('/predict', methods=['POST'])
+# @exception_handler
+# def _predict():
+#     data = request.json
+#     tasks = data.get('tasks')
+#     project = data.get('project')
+#     label_config = data.get('label_config')
+#     force_reload = data.get('force_reload', False)
+#     try_fetch = data.get('try_fetch', True)
+#     params = data.get('params') or {}
+#     predictions, model = _manager.predict(
+#         tasks, project, label_config, force_reload, try_fetch, **params)
+#     response = {
+#         'results': predictions,
+#         'model_version': model.model_version
+#     }
+#     return jsonify(response)
 
 
 @_server.route('/setup', methods=['POST'])
 @exception_handler
 def _setup():
     data = request.json
     logger.debug(data)
@@ -57,17 +57,17 @@
     logger.debug('Fetch model version: {}'.format(model.model_version))
     return jsonify({'model_version': model.model_version})
 
 
 @_server.route('/train', methods=['POST'])
 @exception_handler
 def _train():
-    logger.warning("=> Warning: API /train is deprecated since Label Studio 1.4.1. "
+    logger.warning("=> Warning: API /train is deprecated since AIxBlock 1.0.0. "
                    "ML backend used API /train for training previously, "
-                   "but since 1.4.1 Label Studio backend and ML backend use /webhook for the training run.")
+                   "but since 1.0.0 AIxBlock ML and ML backend use /webhook for the training run.")
     data = request.json
     annotations = data.get('annotations', 'No annotations provided')
     project = data.get('project')
     label_config = data.get('label_config')
     params = data.get('params', {})
     if isinstance(project, dict):
         project = ""
@@ -116,87 +116,121 @@
         'v2': os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT)
     })
 
 
 @_server.route('/metrics', methods=['GET'])
 @exception_handler
 def metrics():
+    # from prometheus_client import CollectorRegistry, push_to_gateway
+    # from prometheus_client.core import GaugeMetricFamily
+
+    # class CustomCollector(object):
+    #     # make sure you define collect method
+    #     def collect():
+    #         # float metric you want to push
+    #         metric = "<some_float_value>"
+
+    #         # create gauge metric, define label names
+    #         metric_gauge = GaugeMetricFamily("metric_name", "metric_description", labels=["label1", "label2"])
+    #         # add metric value and label values
+    #         metric_gauge.add_metric(["label1_value", "label2_value"], metric)
+
+    #         yield metric_gauge
+
+
+
+    # registry = CollectorRegistry()
+    # registry.register(CustomCollector())
+
+    # # Push metrics to pushgateway (modify the url accordingly)
+    # push_to_gateway('localhost:9091', job='job_name', registry=registry)
     return jsonify({})
 
 
 @_server.route('/model', methods=['POST'])
 @exception_handler
 def _model():
     data = request.json
     project = data.get('project')
     label_config = data.get('label_config')
     force_reload = data.get('force_reload', False)
     try_fetch = data.get('try_fetch', True)
     params = data.get('params') or {}
     predictions, model = _manager.model(
         project, label_config, force_reload, try_fetch, **params)
+    return jsonify(predictions)
+@_server.route('/model_trial', methods=['POST'])
+@exception_handler
+def _model_trial():
+    data = request.json
+    project = data.get('project')
+    label_config = data.get('label_config')
+    force_reload = data.get('force_reload', False)
+    try_fetch = data.get('try_fetch', True)
+    params = data.get('params') or {}
+    predictions, model = _manager.model_trial(
+        project, label_config, force_reload, try_fetch, **params)
 #     response = {
 #         'model_build_date': predictions.model_build_date,
 #         'model_url': predictions.model_url,
 #         'model_map':  predictions.model_url,
 #         'model_recall':  predictions.model_url,
 #         'model_precision':  predictions.model_url,
 #         'model_version': model.model_version
 #     }
     return jsonify(predictions)
 
-
-@_server.route('/toolbar_predict', methods=['POST'])
-@exception_handler
-def _toolbar_predict():
-    data = request.json
-    project = data.get('project')
-    image = data.get('image')
-    clickpoint = data.get('clickpoint')
-    polygons = data.get('polygons')
-    vertices = data.get('vertices')
-    label_config = data.get('label_config')
-    force_reload = data.get('force_reload', False)
-    try_fetch = data.get('try_fetch', True)
-    text = data.get('text')
-    question = data.get('question')
-    params = data.get('params') or {}
-    params['text'] = text
-    params['question'] = question
-    predictions, model = _manager.toolbar_predict(
-        image, clickpoint, polygons, vertices, project, label_config, force_reload, try_fetch, **params)
-    response = {
-        'results': predictions,
-        'model_version': model.model_version
-    }
-    return jsonify(response)
-@_server.route('/toolbar_predict_sam', methods=['POST'])
-@exception_handler
-def _toolbar_predict_sam():
-    data = request.json
-    project = data.get('project')
-    image = data.get('image')
-    clickpoint = data.get('clickpoint')
-    polygons = data.get('polygons')
-    vertices = data.get('vertices')
-    label_config = data.get('label_config')
-    force_reload = data.get('force_reload', False)
-    try_fetch = data.get('try_fetch', True)
-    voice = data.get('voice')
-    prompt = data.get('prompt')
-    image_pref = data.get('image_pref')
-    draw_polygons = data.get('draw_polygons')
-    params = data.get('params') or {}
-    predictions, model = _manager.toolbar_predict_sam(
-        image, clickpoint, polygons, vertices, project, voice,prompt,image_pref,draw_polygons,label_config, force_reload, try_fetch, **params)
-    response = {
-        'results': predictions,
-        'model_version': model.model_version
-    }
-    return jsonify(response)
+# @_server.route('/toolbar_predict', methods=['POST'])
+# @exception_handler
+# def _toolbar_predict():
+#     data = request.json
+#     project = data.get('project')
+#     image = data.get('image')
+#     clickpoint = data.get('clickpoint')
+#     polygons = data.get('polygons')
+#     vertices = data.get('vertices')
+#     label_config = data.get('label_config')
+#     force_reload = data.get('force_reload', False)
+#     try_fetch = data.get('try_fetch', True)
+#     text = data.get('text')
+#     question = data.get('question')
+#     params = data.get('params') or {}
+#     params['text'] = text
+#     params['question'] = question
+#     predictions, model = _manager.toolbar_predict(
+#         image, clickpoint, polygons, vertices, project, label_config, force_reload, try_fetch, **params)
+#     response = {
+#         'results': predictions,
+#         'model_version': model.model_version
+#     }
+#     return jsonify(response)
+# @_server.route('/toolbar_predict_sam', methods=['POST'])
+# @exception_handler
+# def _toolbar_predict_sam():
+#     data = request.json
+#     project = data.get('project')
+#     image = data.get('image')
+#     clickpoint = data.get('clickpoint')
+#     polygons = data.get('polygons')
+#     vertices = data.get('vertices')
+#     label_config = data.get('label_config')
+#     force_reload = data.get('force_reload', False)
+#     try_fetch = data.get('try_fetch', True)
+#     voice = data.get('voice')
+#     prompt = data.get('prompt')
+#     image_pref = data.get('image_pref')
+#     draw_polygons = data.get('draw_polygons')
+#     params = data.get('params') or {}
+#     predictions, model = _manager.toolbar_predict_sam(
+#         image, clickpoint, polygons, vertices, project, voice,prompt,image_pref,draw_polygons,label_config, force_reload, try_fetch, **params)
+#     response = {
+#         'results': predictions,
+#         'model_version': model.model_version
+#     }
+#     return jsonify(response)
 @_server.route('/action', methods=['POST'])
 @exception_handler
 def _action():
     data = request.json
     project = data.get('project')
     command = data.get('command')
     collection = data.get('data')
@@ -208,27 +242,28 @@
     response_collection, model = _manager.action(
         project,command, collection,label_config, force_reload, try_fetch, **params)
     response = {
         'results': response_collection,
         'model_version': model.model_version
     }
     return jsonify(response)
-@_server.route('/preview', methods=['GET'])
-@exception_handler
-def _preview():
-    project = request.args.get('project')
-    output = _manager.preview(project)
-    return output
+# @_server.route('/preview', methods=['GET'])
+# @exception_handler
+# def _preview():
+#     project = request.args.get('project')
+#     output = _manager.preview(project)
+#     return output
 
 
 @_server.route('/download', methods=['GET'])
 @exception_handler
 def _download():
     import io
     project = request.args.get('project')
+    type = request.args.get('type')
     model_path = _manager.download(project)
     return model_path
 
 
 @_server.errorhandler(NoSuchJobError)
 def no_such_job_error_handler(error):
     logger.warning('Got error: ' + str(error))
```

### Comparing `aixblock_ml-0.0.4/aixblock_ml/default_configs/README.md` & `aixblock_ml-0.0.5/aixblock_ml/default_configs/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Check if it works:
 
 ```bash
 $ curl http://localhost:9090/health
 {"status":"UP"}
 ```
 
-Then connect running backend to Label Studio using Machine Learning settings. 
+Then connect running backend to AIxBlockusing Machine Learning settings. 
 
 
 ## Writing your own model
 1. Place your scripts for model training & inference inside root directory. Follow the [API guidelines](#api-guidelines) described bellow. You can put everything in a single file, or create 2 separate one say `my_training_module.py` and `my_inference_module.py`
 
 2. Write down your python dependencies in `requirements.txt`
 
@@ -45,18 +45,18 @@
 
 ```python
 from htx.base_model import BaseModel
 
 # use BaseModel inheritance provided by pyheartex SDK 
 class MyModel(BaseModel):
     
-    # Describe input types (Label Studio object tags names)
+    # Describe input types (AIxBlockobject tags names)
     INPUT_TYPES = ('Image',)
 
-    # Describe output types (Label Studio control tags names)
+    # Describe output types (AIxBlockcontrol tags names)
     INPUT_TYPES = ('Choices',)
 
     def load(self, resources, **kwargs):
         """Here you load the model into the memory. resources is a dict returned by training script"""
         self.model_path = resources["model_path"]
         self.labels = resources["labels"]
```

### Comparing `aixblock_ml-0.0.4/aixblock_ml/default_configs/_wsgi.py` & `aixblock_ml-0.0.5/aixblock_ml/default_configs/_wsgi.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.4/aixblock_ml/default_configs/_wsgi.py.tmpl` & `aixblock_ml-0.0.5/aixblock_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.4/aixblock_ml/default_configs/docker-compose.yml` & `aixblock_ml-0.0.5/aixblock_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.4/aixblock_ml/default_configs/model.py` & `aixblock_ml-0.0.5/aixblock_ml/default_configs/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from aixblock_ml.model import AIxBlockMLBase
 
 
 class NewModel(AIxBlockMLBase):
 
     def predict(self, tasks: List[Dict], context: Optional[Dict] = None, **kwargs) -> List[Dict]:
         """ Write your inference logic here
-            :param tasks: [Label Studio tasks in JSON format](https://labelstud.io/guide/task_format.html)
-            :param context: [Label Studio context in JSON format](https://labelstud.io/guide/ml.html#Passing-data-to-ML-backend)
+            :param tasks: [AIxBlocktasks in JSON format](https://labelstud.io/guide/task_format.html)
+            :param context: [AIxBlockcontext in JSON format](https://labelstud.io/guide/ml.html#Passing-data-to-ML-backend)
             :return predictions: [Predictions array in JSON format](https://labelstud.io/guide/export.html#Raw-JSON-format-of-completed-tasks)
         """
         print(f'''\
         Run prediction on {tasks}
         Received context: {context}
         Project ID: {self.project_id}
         Label config: {self.label_config}
```

### Comparing `aixblock_ml-0.0.4/aixblock_ml/exceptions.py` & `aixblock_ml-0.0.5/aixblock_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.4/aixblock_ml/helpers.py` & `aixblock_ml-0.0.5/aixblock_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.4/aixblock_ml/model.py` & `aixblock_ml-0.0.5/aixblock_ml/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 
     def job(self, model_class, event: str, data: Dict, job_id: str):
         """
         Job function to be run in background. It actually does the following:
         1. Creates model_class instance, possibly by using artefacts from previously finished jobs
         2. Calls model_class.process_event() method
         :param model_class: AIxBlockMLBase instance
-        :param event: event name (e.g. Label Studio webhook action name)
-        :param data: job data (e.g. Label Studio webhook payload)
+        :param event: event name (e.g. AIxBlockwebhook action name)
+        :param data: job data (e.g. AIxBlockwebhook payload)
         :param job_id: user-defined job identifier
         :return: json-serializable job result
         """
         with self.start_run(event, data, job_id):
             model_version = data.get('model_version') or data.get('project', {}).get('model_version')
             job_result = self.get_result(model_version)
             label_config = data.get('label_config') or data.get('project', {}).get('label_config')
@@ -302,32 +302,35 @@
         self.ml_id = ml_id
         self.label_config = label_config
         self.parsed_label_config = parse_config(self.label_config) if self.label_config else {}
         self.train_output = train_output or {}
         self.hostname = kwargs.get('hostname', '')
         self.access_token = kwargs.get('access_token', '')
 
-    @abstractmethod
-    def predict(self, tasks, **kwargs):
-        pass
-    @abstractmethod
-    def toolbar_predict(self, image, clickpoint, polygons, vertices,project, **kwargs):
-        pass
-    @abstractmethod
-    def toolbar_predict_sam(self, image, clickpoint, polygons, vertices,project,voice,prompt,image_pref,draw_polygons, **kwargs):
-        pass
+    # @abstractmethod
+    # def predict(self, tasks, **kwargs):
+    #     pass
+    # @abstractmethod
+    # def toolbar_predict(self, image, clickpoint, polygons, vertices,project, **kwargs):
+    #     pass
+    # @abstractmethod
+    # def toolbar_predict_sam(self, image, clickpoint, polygons, vertices,project,voice,prompt,image_pref,draw_polygons, **kwargs):
+    #     pass
     @abstractmethod
     def action(self, project,command, collection, **kwargs):
         pass
     @abstractmethod
     def model(self,project, **kwargs):
         pass
     @abstractmethod
-    def preview(self,project, **kwargs):
+    def model_trial(self,project, **kwargs):
         pass
+    # @abstractmethod
+    # def preview(self,project, **kwargs):
+    #     pass
     @abstractmethod
     def download(self,project, **kwargs):
         pass
 
     def process_event(self, event, data, job_id, additional_params):
         if event in self.TRAIN_EVENTS:
             logger.debug(f'Job {job_id}: Received event={event}: calling {self.__class__.__name__}.fit()')
@@ -587,51 +590,51 @@
                     }
             return {
                 'is_training': False,
                 'backend': 'redis',
                 'model_version': m.model_version
             }
 
-    @classmethod
-    def predict(
-        cls, tasks, project=None, label_config=None, force_reload=False, try_fetch=True, **kwargs
-    ):
-        if not os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT):
-            if try_fetch:
-                m = cls.fetch(project, label_config, force_reload)
-            else:
-                m = cls.get(project)
-                if not m:
-                    raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
-            predictions = m.model.predict(tasks, **kwargs)
-            return predictions, m
-
-        if not cls._current_model:
-            raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using predict()')
-
-        predictions = cls._current_model.model.predict(tasks, **kwargs)
-        return predictions, cls._current_model
-    @classmethod
-    def toolbar_predict(
-        cls, image, clickpoint, polygons, vertices, project=None, label_config=None, force_reload=True, try_fetch=False, **kwargs
-    ):
-        if not os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT):
-            if try_fetch:
-                m = cls.fetch(project, label_config, force_reload)
-            else:
-                m = cls.get(project)
-                if not m:
-                    raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
-            predictions = m.model.toolbar_predict(image, clickpoint, polygons, vertices,project, **kwargs)
-            return predictions, m
-
-        if not cls._current_model:
-            raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
-        predictions = m.model.toolbar_predict( image, clickpoint, polygons, vertices,project, **kwargs)
-        return predictions, m
+    # @classmethod
+    # def predict(
+    #     cls, tasks, project=None, label_config=None, force_reload=False, try_fetch=True, **kwargs
+    # ):
+    #     if not os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT):
+    #         if try_fetch:
+    #             m = cls.fetch(project, label_config, force_reload)
+    #         else:
+    #             m = cls.get(project)
+    #             if not m:
+    #                 raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
+    #         predictions = m.model.predict(tasks, **kwargs)
+    #         return predictions, m
+
+    #     if not cls._current_model:
+    #         raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using predict()')
+
+    #     predictions = cls._current_model.model.predict(tasks, **kwargs)
+    #     return predictions, cls._current_model
+    # @classmethod
+    # def toolbar_predict(
+    #     cls, image, clickpoint, polygons, vertices, project=None, label_config=None, force_reload=True, try_fetch=False, **kwargs
+    # ):
+    #     if not os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT):
+    #         if try_fetch:
+    #             m = cls.fetch(project, label_config, force_reload)
+    #         else:
+    #             m = cls.get(project)
+    #             if not m:
+    #                 raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
+    #         predictions = m.model.toolbar_predict(image, clickpoint, polygons, vertices,project, **kwargs)
+    #         return predictions, m
+
+    #     if not cls._current_model:
+    #         raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
+    #     predictions = m.model.toolbar_predict( image, clickpoint, polygons, vertices,project, **kwargs)
+    #     return predictions, m
     @classmethod
     def action(
         cls,  project=None, command=None, collection=None, label_config=None, force_reload=True, try_fetch=False, **kwargs
     ):
         if not os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT):
             if try_fetch:
                 m = cls.fetch(project, label_config, force_reload)
@@ -642,55 +645,71 @@
             predictions = m.model.action(project, command,collection,**kwargs)
             return predictions, m
 
         if not cls._current_model:
             raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
         predictions = m.model.action( project,  command,collection,**kwargs)
         return predictions, m
+    # @classmethod
+    # def toolbar_predict_sam(
+    #     cls, image, clickpoint, polygons, vertices, project=None, voice=None,prompt=None,image_pref=None,draw_polygons=None,label_config=None, force_reload=True, try_fetch=False, **kwargs
+    # ):
+    #     if not os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT):
+    #         if try_fetch:
+    #             m = cls.fetch(project, label_config, force_reload)
+    #         else:
+    #             m = cls.get(project)
+    #             if not m:
+    #                 raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
+    #         predictions = m.model.toolbar_predict_sam(image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+    #         return predictions, m
+
+    #     if not cls._current_model:
+    #         raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
+    #     predictions = m.model.toolbar_predict_sam( image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+    #     return predictions, m
     @classmethod
-    def toolbar_predict_sam(
-        cls, image, clickpoint, polygons, vertices, project=None, voice=None,prompt=None,image_pref=None,draw_polygons=None,label_config=None, force_reload=True, try_fetch=False, **kwargs
-    ):
+    def model(cls,project=None,label_config=None, force_reload=True, try_fetch=False, **kwargs):
         if not os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT):
             if try_fetch:
                 m = cls.fetch(project, label_config, force_reload)
             else:
                 m = cls.get(project)
                 if not m:
                     raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
-            predictions = m.model.toolbar_predict_sam(image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+            predictions = m.model.model(project, **kwargs)
             return predictions, m
 
         if not cls._current_model:
-            raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
-        predictions = m.model.toolbar_predict_sam( image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+            raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using model()')
+        predictions = m.model.model(project, **kwargs)
         return predictions, m
     @classmethod
-    def model(cls,project=None,label_config=None, force_reload=True, try_fetch=False, **kwargs):
+    def model_trial(cls,project=None,label_config=None, force_reload=True, try_fetch=False, **kwargs):
         if not os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT):
             if try_fetch:
                 m = cls.fetch(project, label_config, force_reload)
             else:
                 m = cls.get(project)
                 if not m:
                     raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
             predictions = m.model.model(project, **kwargs)
             return predictions, m
 
         if not cls._current_model:
             raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using model()')
         predictions = m.model.model(project, **kwargs)
         return predictions, m
-    @classmethod
-    def preview(cls, project):
-        if not cls.has_active_model(project):
-            return {}
-        m = cls.get(project)
-        repos = m.model.preview(project)
-        return repos
+    # @classmethod
+    # def preview(cls, project):
+    #     if not cls.has_active_model(project):
+    #         return {}
+    #     m = cls.get(project)
+    #     repos = m.model.preview(project)
+    #     return repos
     @classmethod
     def download(cls, project):
         if not cls.has_active_model(project):
             return {}
         m = cls.get(project)
         repos = m.model.download(project)
         return repos
```

### Comparing `aixblock_ml-0.0.4/aixblock_ml/server.py` & `aixblock_ml-0.0.5/aixblock_ml/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,18 @@
         '--gcp-project-id', dest='gcp_project',
         help='GCP project ID')
     parser_deploy.add_argument(
         '--gcp-region', dest='gcp_region',
         help='GCP region')
     parser_deploy.add_argument(
         '--aixblock-host', dest='AIXBLOCK_host', default='https://app.heartex.com',
-        help='Label Studio hostname')
+        help='AIxBlockhostname')
     parser_deploy.add_argument(
         '--aixblock-api-key', dest='AIXBLOCK_api_key', required=True,
-        help='Label Studio API key')
+        help='AIxBlockAPI key')
 
     args, subargs = parser.parse_known_args()
     return args, subargs
 
 
 def create_dir(args):
     output_dir = os.path.join(args.root_dir, args.project_name)
```

### Comparing `aixblock_ml-0.0.4/aixblock_ml/utils.py` & `aixblock_ml-0.0.5/aixblock_ml/utils.py`

 * *Files identical despite different names*

