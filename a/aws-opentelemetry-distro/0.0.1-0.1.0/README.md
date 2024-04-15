# Comparing `tmp/aws_opentelemetry_distro-0.0.1-py3-none-any.whl.zip` & `tmp/aws_opentelemetry_distro-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,35 +1,37 @@
-Zip file size: 47374 bytes, number of entries: 33
+Zip file size: 49087 bytes, number of entries: 35
 -rw-r--r--  2.0 unx      887 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/_aws_attribute_keys.py
 -rw-r--r--  2.0 unx    16342 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/_aws_metric_attribute_generator.py
--rw-r--r--  2.0 unx     7186 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/_aws_span_processing_util.py
--rw-r--r--  2.0 unx     6206 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/_instrumentation_patch.py
+-rw-r--r--  2.0 unx     7337 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/_aws_span_processing_util.py
 -rw-r--r--  2.0 unx     2539 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/always_record_sampler.py
 -rw-r--r--  2.0 unx     4671 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/attribute_propagating_span_processor.py
 -rw-r--r--  2.0 unx     2408 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/attribute_propagating_span_processor_builder.py
 -rw-r--r--  2.0 unx     5992 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/aws_metric_attributes_span_exporter.py
 -rw-r--r--  2.0 unx     1466 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/aws_metric_attributes_span_exporter_builder.py
--rw-r--r--  2.0 unx    12418 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/aws_opentelemetry_configurator.py
--rw-r--r--  2.0 unx     1786 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/aws_opentelemetry_distro.py
+-rw-r--r--  2.0 unx    13432 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/aws_opentelemetry_configurator.py
+-rw-r--r--  2.0 unx     1528 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/aws_opentelemetry_distro.py
 -rw-r--r--  2.0 unx     5235 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/aws_span_metrics_processor.py
 -rw-r--r--  2.0 unx     2872 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/aws_span_metrics_processor_builder.py
 -rw-r--r--  2.0 unx     1425 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/metric_attribute_generator.py
 -rw-r--r--  2.0 unx     4072 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sqs_url_parser.py
 -rw-r--r--  2.0 unx      130 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/version.py
 -rw-r--r--  2.0 unx    16500 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/configuration/sql_dialect_keywords.json
+-rw-r--r--  2.0 unx     4172 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/patches/_botocore_patches.py
+-rw-r--r--  2.0 unx     1841 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/patches/_instrumentation_patch.py
+-rw-r--r--  2.0 unx     1623 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/patches/_resource_detector_patches.py
 -rw-r--r--  2.0 unx     4146 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_aws_xray_sampling_client.py
 -rw-r--r--  2.0 unx      642 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_clock.py
 -rw-r--r--  2.0 unx     1833 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_fallback_sampler.py
 -rw-r--r--  2.0 unx     2532 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_matcher.py
 -rw-r--r--  2.0 unx     1662 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_rate_limiter.py
 -rw-r--r--  2.0 unx     1615 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_rate_limiting_sampler.py
 -rw-r--r--  2.0 unx     6041 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_rule_cache.py
 -rw-r--r--  2.0 unx     2729 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_sampling_rule.py
 -rw-r--r--  2.0 unx     9461 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_sampling_rule_applier.py
 -rw-r--r--  2.0 unx     1017 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_sampling_statistics_document.py
 -rw-r--r--  2.0 unx     2263 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/_sampling_target.py
 -rw-r--r--  2.0 unx     6747 b- defN 20-Feb-02 00:00 amazon/opentelemetry/distro/sampler/aws_xray_remote_sampler.py
-?rw-r--r--  2.0 unx     4201 b- defN 20-Feb-02 00:00 aws_opentelemetry_distro-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 aws_opentelemetry_distro-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      249 b- defN 20-Feb-02 00:00 aws_opentelemetry_distro-0.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     3697 b- defN 20-Feb-02 00:00 aws_opentelemetry_distro-0.0.1.dist-info/RECORD
-33 files, 141057 bytes uncompressed, 41098 bytes compressed:  70.9%
+?rw-r--r--  2.0 unx     4682 b- defN 20-Feb-02 00:00 aws_opentelemetry_distro-0.1.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 aws_opentelemetry_distro-0.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      249 b- defN 20-Feb-02 00:00 aws_opentelemetry_distro-0.1.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     3940 b- defN 20-Feb-02 00:00 aws_opentelemetry_distro-0.1.0.dist-info/RECORD
+35 files, 144118 bytes uncompressed, 42401 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -3,17 +3,14 @@
 
 Filename: amazon/opentelemetry/distro/_aws_metric_attribute_generator.py
 Comment: 
 
 Filename: amazon/opentelemetry/distro/_aws_span_processing_util.py
 Comment: 
 
-Filename: amazon/opentelemetry/distro/_instrumentation_patch.py
-Comment: 
-
 Filename: amazon/opentelemetry/distro/always_record_sampler.py
 Comment: 
 
 Filename: amazon/opentelemetry/distro/attribute_propagating_span_processor.py
 Comment: 
 
 Filename: amazon/opentelemetry/distro/attribute_propagating_span_processor_builder.py
@@ -45,14 +42,23 @@
 
 Filename: amazon/opentelemetry/distro/version.py
 Comment: 
 
 Filename: amazon/opentelemetry/distro/configuration/sql_dialect_keywords.json
 Comment: 
 
+Filename: amazon/opentelemetry/distro/patches/_botocore_patches.py
+Comment: 
+
+Filename: amazon/opentelemetry/distro/patches/_instrumentation_patch.py
+Comment: 
+
+Filename: amazon/opentelemetry/distro/patches/_resource_detector_patches.py
+Comment: 
+
 Filename: amazon/opentelemetry/distro/sampler/_aws_xray_sampling_client.py
 Comment: 
 
 Filename: amazon/opentelemetry/distro/sampler/_clock.py
 Comment: 
 
 Filename: amazon/opentelemetry/distro/sampler/_fallback_sampler.py
@@ -81,20 +87,20 @@
 
 Filename: amazon/opentelemetry/distro/sampler/_sampling_target.py
 Comment: 
 
 Filename: amazon/opentelemetry/distro/sampler/aws_xray_remote_sampler.py
 Comment: 
 
-Filename: aws_opentelemetry_distro-0.0.1.dist-info/METADATA
+Filename: aws_opentelemetry_distro-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: aws_opentelemetry_distro-0.0.1.dist-info/WHEEL
+Filename: aws_opentelemetry_distro-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: aws_opentelemetry_distro-0.0.1.dist-info/entry_points.txt
+Filename: aws_opentelemetry_distro-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: aws_opentelemetry_distro-0.0.1.dist-info/RECORD
+Filename: aws_opentelemetry_distro-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## amazon/opentelemetry/distro/_aws_span_processing_util.py

```diff
@@ -1,13 +1,14 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 """Utility module designed to support shared logic across AWS Span Processors."""
 import json
 import os
 from typing import Dict, List
+from urllib.parse import ParseResult, urlparse
 
 from amazon.opentelemetry.distro._aws_attribute_keys import AWS_CONSUMER_PARENT_SPAN_KIND, AWS_LOCAL_OPERATION
 from opentelemetry.sdk.trace import InstrumentationScope, ReadableSpan
 from opentelemetry.semconv.trace import MessagingOperationValues, SpanAttributes
 from opentelemetry.trace import SpanKind
 
 # Default attribute values if no valid span attribute value is identified
@@ -15,16 +16,15 @@
 UNKNOWN_OPERATION: str = "UnknownOperation"
 UNKNOWN_REMOTE_SERVICE: str = "UnknownRemoteService"
 UNKNOWN_REMOTE_OPERATION: str = "UnknownRemoteOperation"
 INTERNAL_OPERATION: str = "InternalOperation"
 LOCAL_ROOT: str = "LOCAL_ROOT"
 
 # Useful constants
-_SQS_RECEIVE_MESSAGE_SPAN_NAME: str = "Sqs.ReceiveMessage"
-_AWS_SDK_INSTRUMENTATION_SCOPE_PREFIX: str = "io.opentelemetry.aws-sdk-"
+_BOTO3SQS_INSTRUMENTATION_SCOPE: str = "opentelemetry.instrumentation.boto3sqs"
 
 # Max keyword length supported by parsing into remote_operation from DB_STATEMENT
 MAX_KEYWORD_LENGTH = 27
 
 
 # Get dialect keywords retrieved from dialect_keywords.json file.
 # Only meant to be invoked by SQL_KEYWORD_PATTERN and unit tests
@@ -82,22 +82,22 @@
 
 def is_aws_sdk_span(span: ReadableSpan) -> bool:
     # https://opentelemetry.io/docs/specs/otel/trace/semantic_conventions/instrumentation/aws-sdk/#common-attributes
     return "aws-api" == span.attributes.get(SpanAttributes.RPC_SYSTEM)
 
 
 def should_generate_service_metric_attributes(span: ReadableSpan) -> bool:
-    return (is_local_root(span) and not _is_sqs_receive_message_consumer_span(span)) or SpanKind.SERVER == span.kind
+    return (is_local_root(span) and not _is_boto3sqs_span(span)) or SpanKind.SERVER == span.kind
 
 
 def should_generate_dependency_metric_attributes(span: ReadableSpan) -> bool:
     return (
         SpanKind.CLIENT == span.kind
-        or SpanKind.PRODUCER == span.kind
-        or (_is_dependency_consumer_span(span) and not _is_sqs_receive_message_consumer_span(span))
+        or (SpanKind.PRODUCER == span.kind and not _is_boto3sqs_span(span))
+        or (_is_dependency_consumer_span(span) and not _is_boto3sqs_span(span))
     )
 
 
 def is_consumer_process_span(span: ReadableSpan) -> bool:
     messaging_operation: str = span.attributes.get(SpanAttributes.MESSAGING_OPERATION)
     return SpanKind.CONSUMER == span.kind and MessagingOperationValues.PROCESS == messaging_operation
 
@@ -113,25 +113,26 @@
     """
     A span is a local root if it has no parent or if the parent is remote. This function checks the parent context
     and returns true if it is a local root.
     """
     return span.parent is None or not span.parent.is_valid or span.parent.is_remote
 
 
-def _is_sqs_receive_message_consumer_span(span: ReadableSpan) -> bool:
-    """To identify the SQS consumer spans produced by AWS SDK instrumentation"""
-    messaging_operation: str = span.attributes.get(SpanAttributes.MESSAGING_OPERATION)
+def _is_boto3sqs_span(span: ReadableSpan) -> bool:
+    """
+    To identify if the span produced is from the boto3sqs instrumentation.
+    We use this to identify the boto3sqs spans and not generate metrics from the since we will generate
+    the same metrics from botocore spans.
+    """
+    # TODO: Evaluate if we can bring the boto3sqs spans back to generate metrics and not have to suppress them.
     instrumentation_scope: InstrumentationScope = span.instrumentation_scope
-
     return (
-        (span.name is not None and _SQS_RECEIVE_MESSAGE_SPAN_NAME.casefold() == span.name.casefold())
-        and SpanKind.CONSUMER == span.kind
-        and instrumentation_scope is not None
-        and instrumentation_scope.name.startswith(_AWS_SDK_INSTRUMENTATION_SCOPE_PREFIX)
-        and (messaging_operation is None or messaging_operation == MessagingOperationValues.PROCESS)
+        instrumentation_scope is not None
+        and instrumentation_scope.name is not None
+        and _BOTO3SQS_INSTRUMENTATION_SCOPE.casefold() == instrumentation_scope.name.casefold()
     )
 
 
 def _is_dependency_consumer_span(span: ReadableSpan) -> bool:
     if SpanKind.CONSUMER != span.kind:
         return False
 
@@ -157,23 +158,29 @@
         return operation != http_method
 
     return True
 
 
 def _generate_ingress_operation(span: ReadableSpan) -> str:
     """
-    When span name is not meaningful(null, unknown or http_method value) as operation name for http use cases. Will try
-    to extract the operation name from http target string
+    When span name is not meaningful, this method is invoked to try to extract the operation name from either
+    `http.target`, if present, or from `http.url`, and combine with `http.method`.
     """
     operation: str = UNKNOWN_OPERATION
+    http_path: str = None
     if is_key_present(span, SpanAttributes.HTTP_TARGET):
-        http_target: str = span.attributes.get(SpanAttributes.HTTP_TARGET)
-        # get the first part from API path string as operation value
-        # the more levels/parts we get from API path the higher chance for getting high cardinality data
-        if http_target is not None:
-            operation = extract_api_path_value(http_target)
-            if is_key_present(span, SpanAttributes.HTTP_METHOD):
-                http_method: str = span.attributes.get(SpanAttributes.HTTP_METHOD)
-                if http_method is not None:
-                    operation = http_method + " " + operation
+        http_path = span.attributes.get(SpanAttributes.HTTP_TARGET)
+    elif is_key_present(span, SpanAttributes.HTTP_URL):
+        http_url = span.attributes.get(SpanAttributes.HTTP_URL)
+        url: ParseResult = urlparse(http_url)
+        http_path = url.path
+
+    # get the first part from API path string as operation value
+    # the more levels/parts we get from API path the higher chance for getting high cardinality data
+    if http_path is not None:
+        operation = extract_api_path_value(http_path)
+        if is_key_present(span, SpanAttributes.HTTP_METHOD):
+            http_method: str = span.attributes.get(SpanAttributes.HTTP_METHOD)
+            if http_method is not None:
+                operation = http_method + " " + operation
 
     return operation
```

## amazon/opentelemetry/distro/aws_opentelemetry_configurator.py

```diff
@@ -53,34 +53,35 @@
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SpanExporter
 from opentelemetry.sdk.trace.id_generator import IdGenerator
 from opentelemetry.sdk.trace.sampling import Sampler
 from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.trace import set_tracer_provider
 
-OTEL_AWS_APP_SIGNALS_ENABLED = "OTEL_AWS_APP_SIGNALS_ENABLED"
-OTEL_METRIC_EXPORT_INTERVAL = "OTEL_METRIC_EXPORT_INTERVAL"
-OTEL_AWS_APP_SIGNALS_EXPORTER_ENDPOINT = "OTEL_AWS_APP_SIGNALS_EXPORTER_ENDPOINT"
-OTEL_AWS_SMP_EXPORTER_ENDPOINT = "OTEL_AWS_SMP_EXPORTER_ENDPOINT"
+APP_SIGNALS_ENABLED_CONFIG = "OTEL_AWS_APP_SIGNALS_ENABLED"
+APPLICATION_SIGNALS_ENABLED_CONFIG = "OTEL_AWS_APPLICATION_SIGNALS_ENABLED"
+APP_SIGNALS_EXPORTER_ENDPOINT_CONFIG = "OTEL_AWS_APP_SIGNALS_EXPORTER_ENDPOINT"
+APPLICATION_SIGNALS_EXPORTER_ENDPOINT_CONFIG = "OTEL_AWS_APPLICATION_SIGNALS_EXPORTER_ENDPOINT"
+METRIC_EXPORT_INTERVAL_CONFIG = "OTEL_METRIC_EXPORT_INTERVAL"
 DEFAULT_METRIC_EXPORT_INTERVAL = 60000.0
 
 _logger: Logger = getLogger(__name__)
 
 
 class AwsOpenTelemetryConfigurator(_OTelSDKConfigurator):
     """
     This AwsOpenTelemetryConfigurator extend _OTelSDKConfigurator configuration with the following change:
 
     - Use AlwaysRecordSampler to record all spans.
     - Add SpanMetricsProcessor to create metrics.
     - Add AttributePropagatingSpanProcessor to propagate span attributes from parent to child spans.
     - Add AwsMetricAttributesSpanExporter to add more attributes to all spans.
 
-    You can control when these customizations are applied using the environment variable OTEL_AWS_APP_SIGNALS_ENABLED.
-    This flag is disabled by default.
+    You can control when these customizations are applied using the environment variable
+    OTEL_AWS_APPLICATION_SIGNALS_ENABLED. This flag is disabled by default.
     """
 
     # pylint: disable=no-self-use
     @override
     def _configure(self, **kwargs):
         _initialize_components()
 
@@ -166,14 +167,22 @@
     else:
         urllib3_excluded_urls = urls_to_exclude_instr
     os.environ.setdefault("OTEL_PYTHON_URLLIB3_EXCLUDED_URLS", requests_excluded_urls)
     os.environ.setdefault("OTEL_PYTHON_REQUESTS_EXCLUDED_URLS", urllib3_excluded_urls)
 
 
 def _custom_import_sampler(sampler_name: str, resource: Resource) -> Sampler:
+    # sampler_name from _get_sampler() can be None if `OTEL_TRACES_SAMPLER` is unset. Upstream TracerProvider is able to
+    # accept None as sampler, however we require the sampler to be not None to create `AlwaysRecordSampler` beforehand.
+    # Default value of `OTEL_TRACES_SAMPLER` should be `parentbased_always_on`.
+    # https://opentelemetry.io/docs/languages/sdk-configuration/general/#otel_traces_sampler
+    # Ideally, _get_sampler() should default to `parentbased_always_on` in upstream.
+    if sampler_name is None:
+        sampler_name = "parentbased_always_on"
+
     if sampler_name == "xray":
         # Example env var value
         # OTEL_TRACES_SAMPLER_ARG=endpoint=http://localhost:2000,polling_interval=360
         sampler_argument_env: str = os.getenv(OTEL_TRACES_SAMPLER_ARG, None)
         endpoint: str = None
         polling_interval: int = None
 
@@ -199,95 +208,102 @@
         _logger.debug("XRay Sampler Endpoint: %s", str(endpoint))
         _logger.debug("XRay Sampler Polling Interval: %s", str(polling_interval))
         return AwsXRayRemoteSampler(resource=resource, endpoint=endpoint, polling_interval=polling_interval)
     return _import_sampler(sampler_name)
 
 
 def _customize_sampler(sampler: Sampler) -> Sampler:
-    if not is_app_signals_enabled():
+    if not _is_application_signals_enabled():
         return sampler
     return AlwaysRecordSampler(sampler)
 
 
 def _customize_exporter(span_exporter: SpanExporter, resource: Resource) -> SpanExporter:
-    if not is_app_signals_enabled():
+    if not _is_application_signals_enabled():
         return span_exporter
     return AwsMetricAttributesSpanExporterBuilder(span_exporter, resource).build()
 
 
 def _customize_span_processors(provider: TracerProvider, resource: Resource) -> None:
-    if not is_app_signals_enabled():
+    if not _is_application_signals_enabled():
         return
 
     # Construct and set local and remote attributes span processor
     provider.add_span_processor(AttributePropagatingSpanProcessorBuilder().build())
 
     # Construct meterProvider
-    _logger.info("AWS AppSignals enabled")
-    otel_metric_exporter = AppSignalsExporterProvider().create_exporter()
-    export_interval_millis = float(os.environ.get(OTEL_METRIC_EXPORT_INTERVAL, DEFAULT_METRIC_EXPORT_INTERVAL))
+    _logger.info("AWS Application Signals enabled")
+    otel_metric_exporter = ApplicationSignalsExporterProvider().create_exporter()
+    export_interval_millis = float(os.environ.get(METRIC_EXPORT_INTERVAL_CONFIG, DEFAULT_METRIC_EXPORT_INTERVAL))
     _logger.debug("Span Metrics export interval: %s", export_interval_millis)
     # Cap export interval to 60 seconds. This is currently required for metrics-trace correlation to work correctly.
     if export_interval_millis > DEFAULT_METRIC_EXPORT_INTERVAL:
         export_interval_millis = DEFAULT_METRIC_EXPORT_INTERVAL
-        _logger.info("AWS AppSignals metrics export interval capped to %s", export_interval_millis)
+        _logger.info("AWS Application Signals metrics export interval capped to %s", export_interval_millis)
     periodic_exporting_metric_reader = PeriodicExportingMetricReader(
         exporter=otel_metric_exporter, export_interval_millis=export_interval_millis
     )
     meter_provider: MeterProvider = MeterProvider(resource=resource, metric_readers=[periodic_exporting_metric_reader])
-    # Construct and set AppSignals metrics processor
+    # Construct and set application signals metrics processor
     provider.add_span_processor(AwsSpanMetricsProcessorBuilder(meter_provider, resource).build())
 
     return
 
 
 def _customize_versions(auto_resource: Dict[str, any]) -> Dict[str, any]:
     distro_version = version("aws-opentelemetry-distro")
     auto_resource[ResourceAttributes.TELEMETRY_AUTO_VERSION] = distro_version + "-aws"
     _logger.debug("aws-opentelementry-distro - version: %s", auto_resource[ResourceAttributes.TELEMETRY_AUTO_VERSION])
     return auto_resource
 
 
-def is_app_signals_enabled():
-    return os.environ.get(OTEL_AWS_APP_SIGNALS_ENABLED, False)
+def _is_application_signals_enabled():
+    return (
+        os.environ.get(APPLICATION_SIGNALS_ENABLED_CONFIG, os.environ.get(APP_SIGNALS_ENABLED_CONFIG, "false")).lower()
+        == "true"
+    )
 
 
-class AppSignalsExporterProvider:
-    _instance: ClassVar["AppSignalsExporterProvider"] = None
+class ApplicationSignalsExporterProvider:
+    _instance: ClassVar["ApplicationSignalsExporterProvider"] = None
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         return cls._instance
 
     # pylint: disable=no-self-use
     def create_exporter(self):
         protocol = os.environ.get(
             OTEL_EXPORTER_OTLP_METRICS_PROTOCOL, os.environ.get(OTEL_EXPORTER_OTLP_PROTOCOL, "grpc")
         )
-        _logger.debug("AppSignals export protocol: %s", protocol)
+        _logger.debug("AWS Application Signals export protocol: %s", protocol)
 
-        app_signals_endpoint = os.environ.get(
-            OTEL_AWS_APP_SIGNALS_EXPORTER_ENDPOINT,
-            os.environ.get(OTEL_AWS_SMP_EXPORTER_ENDPOINT, "http://localhost:4315"),
+        application_signals_endpoint = os.environ.get(
+            APPLICATION_SIGNALS_EXPORTER_ENDPOINT_CONFIG,
+            os.environ.get(APP_SIGNALS_EXPORTER_ENDPOINT_CONFIG, "http://localhost:4315"),
         )
 
-        _logger.debug("AppSignals export endpoint: %s", app_signals_endpoint)
+        _logger.debug("AWS Application Signals export endpoint: %s", application_signals_endpoint)
 
         temporality_dict: Dict[type, AggregationTemporality] = {}
         for typ in [
             Counter,
             UpDownCounter,
             ObservableCounter,
             ObservableCounter,
             ObservableUpDownCounter,
             ObservableGauge,
             Histogram,
         ]:
             temporality_dict[typ] = AggregationTemporality.DELTA
 
         if protocol == "http/protobuf":
-            return OTLPHttpOTLPMetricExporter(endpoint=app_signals_endpoint, preferred_temporality=temporality_dict)
+            return OTLPHttpOTLPMetricExporter(
+                endpoint=application_signals_endpoint, preferred_temporality=temporality_dict
+            )
         if protocol == "grpc":
-            return OTLPGrpcOTLPMetricExporter(endpoint=app_signals_endpoint, preferred_temporality=temporality_dict)
+            return OTLPGrpcOTLPMetricExporter(
+                endpoint=application_signals_endpoint, preferred_temporality=temporality_dict
+            )
 
-        raise RuntimeError(f"Unsupported AppSignals export protocol: {protocol} ")
+        raise RuntimeError(f"Unsupported AWS Application Signals export protocol: {protocol} ")
```

## amazon/opentelemetry/distro/aws_opentelemetry_distro.py

```diff
@@ -1,28 +1,25 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 import os
 
-from amazon.opentelemetry.distro._instrumentation_patch import apply_instrumentation_patches
+from amazon.opentelemetry.distro.patches._instrumentation_patch import apply_instrumentation_patches
 from opentelemetry.distro import OpenTelemetryDistro
 from opentelemetry.environment_variables import OTEL_PROPAGATORS, OTEL_PYTHON_ID_GENERATOR
 from opentelemetry.sdk.environment_variables import OTEL_EXPORTER_OTLP_METRICS_DEFAULT_HISTOGRAM_AGGREGATION
 
 
 class AwsOpenTelemetryDistro(OpenTelemetryDistro):
     def _configure(self, **kwargs):
         """
         kwargs:
             apply_patches: bool - apply patches to upstream instrumentation. Default is True.
 
         TODO:
-         1. Unlike opentelemetry Java, "otel.aws.imds.endpointOverride" is not configured on python. Need to figure out
-            if we rely on ec2 and eks resource to get context about the platform for python and if we need endpoint
-            override support.
-         2. OTLPMetricExporterMixin is using hard coded histogram_aggregation_type, which reads
+         1. OTLPMetricExporterMixin is using hard coded histogram_aggregation_type, which reads
             OTEL_EXPORTER_OTLP_METRICS_DEFAULT_HISTOGRAM_AGGREGATION environment variable. Need to work with upstream to
             make it to be configurable.
         """
         super(AwsOpenTelemetryDistro, self)._configure()
         os.environ.setdefault(
             OTEL_EXPORTER_OTLP_METRICS_DEFAULT_HISTOGRAM_AGGREGATION, "base2_exponential_bucket_histogram"
         )
```

## amazon/opentelemetry/distro/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
-__version__ = "0.0.1"
+__version__ = "0.1.0"
```

## Comparing `aws_opentelemetry_distro-0.0.1.dist-info/RECORD` & `aws_opentelemetry_distro-0.1.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 amazon/opentelemetry/distro/_aws_attribute_keys.py,sha256=o8mtmcIUVCJHPd2BKLd8fEcwzmpNW-rhxCPdCyhDieo,887
 amazon/opentelemetry/distro/_aws_metric_attribute_generator.py,sha256=MMKZ5oh51TxFgXp26TTBdoE4edl6F5-pVny0GTUkpjE,16342
-amazon/opentelemetry/distro/_aws_span_processing_util.py,sha256=GRCabecgrymQsLTBYIQ9mtF1S6b_QQ2Dk0Y0VUpWblk,7186
-amazon/opentelemetry/distro/_instrumentation_patch.py,sha256=JxxVHNlh11zE5D-BGuYYBrRT9qgp-2bUqqwA82eOtAg,6206
+amazon/opentelemetry/distro/_aws_span_processing_util.py,sha256=BrqxhYYzpDtVJODWINy3OxfW24dCFX3PRNR2Y-dVRQs,7337
 amazon/opentelemetry/distro/always_record_sampler.py,sha256=zq3EyY56kjTgSZ1-QsKu5uFa952BcFRoHC_ZUisSg2M,2539
 amazon/opentelemetry/distro/attribute_propagating_span_processor.py,sha256=l2sVIrYTi3CROK0aZDs6AA5Wwde-STDYGKrFsmQM4KQ,4671
 amazon/opentelemetry/distro/attribute_propagating_span_processor_builder.py,sha256=4JbXewZ2bMcFc9nGnnsrW9cfGYEpZI4phWO4ztTqjNY,2408
 amazon/opentelemetry/distro/aws_metric_attributes_span_exporter.py,sha256=UtYV9Xfnu2it-WqDjqVlCyUWWGJJz0nNkbuMdXzPnjU,5992
 amazon/opentelemetry/distro/aws_metric_attributes_span_exporter_builder.py,sha256=cP-v9NOFOhhnuL_keFgLO1sBfMctUL5MzDQu71WqenY,1466
-amazon/opentelemetry/distro/aws_opentelemetry_configurator.py,sha256=9rZWgCJD77CjrvTC1ZU48qF-BeevXB6DykLHmToa6r4,12418
-amazon/opentelemetry/distro/aws_opentelemetry_distro.py,sha256=oTJUtEqzN4Oy07qIlKz3JReFKKte5tCzDnBbPQXbGGM,1786
+amazon/opentelemetry/distro/aws_opentelemetry_configurator.py,sha256=2SShM4ymJDixnYZgHWjJqPM3BojnddQ_gLu-nMBSqVA,13432
+amazon/opentelemetry/distro/aws_opentelemetry_distro.py,sha256=9Uvz5B6wxa1pvPbZQjYRzNg4JJJH9C2HpHAbdos-d5o,1528
 amazon/opentelemetry/distro/aws_span_metrics_processor.py,sha256=IjxvnxdBwlEzHmFov7N-OSHZXRW5wqLhlRxJHQrlURM,5235
 amazon/opentelemetry/distro/aws_span_metrics_processor_builder.py,sha256=3QUXNpHTJyYK3PSeHAHfL3i7FcHNDAZadovz4MDwEsQ,2872
 amazon/opentelemetry/distro/metric_attribute_generator.py,sha256=2YZymKnnwUJS-7xPPI3zAHRnkTJtHRVQj__tRLTzZ9M,1425
 amazon/opentelemetry/distro/sqs_url_parser.py,sha256=jidMkHwo_jP0Ox1a8zmjfJKTW60qGABtQMKriOPVJBg,4072
-amazon/opentelemetry/distro/version.py,sha256=L3NHiLkg-YSe0SKhUiiNeRXGXm5fSHjQzx65NARJsoM,130
+amazon/opentelemetry/distro/version.py,sha256=YkCT60hA9cyL0OD25MjEPuR04LbOBnqxdv0lc7R6R9M,130
 amazon/opentelemetry/distro/configuration/sql_dialect_keywords.json,sha256=Gl92Xdx7EpPN5HlkZr1RU_BUvCTuklMaVE73kduH0yk,16500
+amazon/opentelemetry/distro/patches/_botocore_patches.py,sha256=t6xsgs31ks0oAyAqPiLI-3Gn7P0Kx8cMImgAKsE3HcU,4172
+amazon/opentelemetry/distro/patches/_instrumentation_patch.py,sha256=e2hEX__FmNZS9W-HzITO5znNkKaztXi6kVeJdHs6kI8,1841
+amazon/opentelemetry/distro/patches/_resource_detector_patches.py,sha256=1f4FQQiC4oJOXdh7TU47AkZ48HrdgK9NrLkdIm2akyo,1623
 amazon/opentelemetry/distro/sampler/_aws_xray_sampling_client.py,sha256=vOztNhoo2KDHqE5vagzsHkHQvaUOLI0Rb9XP9Tr7wvE,4146
 amazon/opentelemetry/distro/sampler/_clock.py,sha256=6M8hhv2FEgmggl3rVnFTB62VkUUzTiwL2G7MQOwPmUc,642
 amazon/opentelemetry/distro/sampler/_fallback_sampler.py,sha256=By1a0jyfy7W7DZn4GJm2OkdDrO9kYuKUepAsRaso3CE,1833
 amazon/opentelemetry/distro/sampler/_matcher.py,sha256=8j05TzCO8mbRorXgnopUuk8guM4WVcXaBxYCQcXm9_k,2532
 amazon/opentelemetry/distro/sampler/_rate_limiter.py,sha256=MilZsphxptVQ4G9W0V7BJWQqeUW_1z7hZCTfRoyunPo,1662
 amazon/opentelemetry/distro/sampler/_rate_limiting_sampler.py,sha256=wJR7AlbXh57FDaoNV2NYWKW4ZjDBz_3OuV4M4UNKKxQ,1615
 amazon/opentelemetry/distro/sampler/_rule_cache.py,sha256=1SxwCUwNNpJFOLYtXXcEOiDkclxo5WLugt7gsJ56yiw,6041
 amazon/opentelemetry/distro/sampler/_sampling_rule.py,sha256=fp-06Ur4bDtBTCXLHU2rN-wHWmOUluL_IAhINj4jRUc,2729
 amazon/opentelemetry/distro/sampler/_sampling_rule_applier.py,sha256=TNpgbhoBVg9TkJp2oZ_0zGLV14tDxJzw8FxadJWW2ic,9461
 amazon/opentelemetry/distro/sampler/_sampling_statistics_document.py,sha256=C9evmg9vfEMJzq5FfRkImBoT191ICJ1Fhth6nTWg6ZI,1017
 amazon/opentelemetry/distro/sampler/_sampling_target.py,sha256=wccite2KK9CsWA6QudlnGUwCgbdCpeo6vGhMq2TPCYM,2263
 amazon/opentelemetry/distro/sampler/aws_xray_remote_sampler.py,sha256=e7hAPPnBtNPukKnThZIyF4SjouIbbH8S-M-of8d5Ees,6747
-aws_opentelemetry_distro-0.0.1.dist-info/METADATA,sha256=P_IBrEVngQrym86IEz_KP2izhaMuYjjFiPG8v6R4yFY,4201
-aws_opentelemetry_distro-0.0.1.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-aws_opentelemetry_distro-0.0.1.dist-info/entry_points.txt,sha256=GgVt2TsDQc86JNySAMv8hwEg9umy3cniBKUFWLzhgSU,249
-aws_opentelemetry_distro-0.0.1.dist-info/RECORD,,
+aws_opentelemetry_distro-0.1.0.dist-info/METADATA,sha256=zvjmHYnjduJAxK0aTGZVTc6vzqeoI7XgshuraT_x1ko,4682
+aws_opentelemetry_distro-0.1.0.dist-info/WHEEL,sha256=xl5aZkiJYVTjhVaiADvIe6UeUVylGNomrxKZ0Zda1CE,87
+aws_opentelemetry_distro-0.1.0.dist-info/entry_points.txt,sha256=GgVt2TsDQc86JNySAMv8hwEg9umy3cniBKUFWLzhgSU,249
+aws_opentelemetry_distro-0.1.0.dist-info/RECORD,,
```

