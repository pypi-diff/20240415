# Comparing `tmp/google-maps-routing-0.6.7.tar.gz` & `tmp/google-maps-routing-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-routing-0.6.7.tar", last modified: Tue Mar  5 19:01:41 2024, max compression
+gzip compressed data, was "google-maps-routing-0.6.8.tar", last modified: Mon Apr 15 13:58:53 2024, max compression
```

## Comparing `google-maps-routing-0.6.7.tar` & `google-maps-routing-0.6.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.188343 google-maps-routing-0.6.7/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5264 2024-03-05 19:01:41.188343 google-maps-routing-0.6.7/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3855 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.172342 google-maps-routing-0.6.7/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.172342 google-maps-routing-0.6.7/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.176342 google-maps-routing-0.6.7/google/maps/routing/
--rw-rw-r--   0 root         (0)     1003     4023 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.176342 google-maps-routing-0.6.7/google/maps/routing_v2/
--rw-rw-r--   0 root         (0)     1003     3360 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     1387 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.176342 google-maps-routing-0.6.7/google/maps/routing_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.180343 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/
--rw-rw-r--   0 root         (0)     1003      737 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/__init__.py
--rw-rw-r--   0 root         (0)     1003    20681 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/async_client.py
--rw-rw-r--   0 root         (0)     1003    36850 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.180343 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/
--rw-rw-r--   0 root         (0)     1003     1288 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6596 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17076 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17313 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17347 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.184343 google-maps-routing-0.6.7/google/maps/routing_v2/types/
--rw-rw-r--   0 root         (0)     1003     3003 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3426 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/fallback_info.py
--rw-rw-r--   0 root         (0)     1003     4201 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/geocoding_results.py
--rw-rw-r--   0 root         (0)     1003     1659 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/localized_time.py
--rw-rw-r--   0 root         (0)     1003     2027 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/location.py
--rw-rw-r--   0 root         (0)     1003     2766 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/maneuver.py
--rw-rw-r--   0 root         (0)     1003     1685 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/navigation_instruction.py
--rw-rw-r--   0 root         (0)     1003     3876 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/polyline.py
--rw-rw-r--   0 root         (0)     1003    31508 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/route.py
--rw-rw-r--   0 root         (0)     1003     1856 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/route_label.py
--rw-rw-r--   0 root         (0)     1003     3600 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/route_modifiers.py
--rw-rw-r--   0 root         (0)     1003     1962 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/route_travel_mode.py
--rw-rw-r--   0 root         (0)     1003    29064 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/routes_service.py
--rw-rw-r--   0 root         (0)     1003     2609 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/routing_preference.py
--rw-rw-r--   0 root         (0)     1003     2809 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/speed_reading_interval.py
--rw-rw-r--   0 root         (0)     1003     1886 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/toll_info.py
--rw-rw-r--   0 root         (0)     1003    11026 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/toll_passes.py
--rw-rw-r--   0 root         (0)     1003     2240 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/traffic_model.py
--rw-rw-r--   0 root         (0)     1003     7327 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/transit.py
--rw-rw-r--   0 root         (0)     1003     3209 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/transit_preferences.py
--rw-rw-r--   0 root         (0)     1003     1337 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/units.py
--rw-rw-r--   0 root         (0)     1003     1609 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/vehicle_emission_type.py
--rw-rw-r--   0 root         (0)     1003     1502 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/vehicle_info.py
--rw-rw-r--   0 root         (0)     1003     4688 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/google/maps/routing_v2/types/waypoint.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.188343 google-maps-routing-0.6.7/google_maps_routing.egg-info/
--rw-r--r--   0 root         (0)     1003     5264 2024-03-05 19:01:41.000000 google-maps-routing-0.6.7/google_maps_routing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2294 2024-03-05 19:01:41.000000 google-maps-routing-0.6.7/google_maps_routing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:41.000000 google-maps-routing-0.6.7/google_maps_routing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:41.000000 google-maps-routing-0.6.7/google_maps_routing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      338 2024-03-05 19:01:41.000000 google-maps-routing-0.6.7/google_maps_routing.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 19:01:41.000000 google-maps-routing-0.6.7/google_maps_routing.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 19:01:41.188343 google-maps-routing-0.6.7/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3202 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.188343 google-maps-routing-0.6.7/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.188343 google-maps-routing-0.6.7/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.188343 google-maps-routing-0.6.7/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:41.188343 google-maps-routing-0.6.7/tests/unit/gapic/routing_v2/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/tests/unit/gapic/routing_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    89341 2024-03-05 18:46:03.000000 google-maps-routing-0.6.7/tests/unit/gapic/routing_v2/test_routes.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.260053 google-maps-routing-0.6.8/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5264 2024-04-15 13:58:53.260053 google-maps-routing-0.6.8/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3855 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.240051 google-maps-routing-0.6.8/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.240051 google-maps-routing-0.6.8/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.244052 google-maps-routing-0.6.8/google/maps/routing/
+-rw-rw-r--   0 root         (0)     1003     4023 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.248052 google-maps-routing-0.6.8/google/maps/routing_v2/
+-rw-rw-r--   0 root         (0)     1003     3360 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1387 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.248052 google-maps-routing-0.6.8/google/maps/routing_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.248052 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/
+-rw-rw-r--   0 root         (0)     1003      737 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20683 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/async_client.py
+-rw-rw-r--   0 root         (0)     1003    36852 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.248052 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/
+-rw-rw-r--   0 root         (0)     1003     1288 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6596 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17078 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17315 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17347 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.256053 google-maps-routing-0.6.8/google/maps/routing_v2/types/
+-rw-rw-r--   0 root         (0)     1003     3003 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3453 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/fallback_info.py
+-rw-rw-r--   0 root         (0)     1003     4253 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/geocoding_results.py
+-rw-rw-r--   0 root         (0)     1003     1659 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/localized_time.py
+-rw-rw-r--   0 root         (0)     1003     2031 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/location.py
+-rw-rw-r--   0 root         (0)     1003     2774 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/maneuver.py
+-rw-rw-r--   0 root         (0)     1003     1694 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/navigation_instruction.py
+-rw-rw-r--   0 root         (0)     1003     3848 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/polyline.py
+-rw-rw-r--   0 root         (0)     1003    31521 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/route.py
+-rw-rw-r--   0 root         (0)     1003     1864 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/route_label.py
+-rw-rw-r--   0 root         (0)     1003     3620 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/route_modifiers.py
+-rw-rw-r--   0 root         (0)     1003     1962 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/route_travel_mode.py
+-rw-rw-r--   0 root         (0)     1003    29983 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/routes_service.py
+-rw-rw-r--   0 root         (0)     1003     2736 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/routing_preference.py
+-rw-rw-r--   0 root         (0)     1003     2813 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/speed_reading_interval.py
+-rw-rw-r--   0 root         (0)     1003     1902 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/toll_info.py
+-rw-rw-r--   0 root         (0)     1003    11531 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/toll_passes.py
+-rw-rw-r--   0 root         (0)     1003     2240 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/traffic_model.py
+-rw-rw-r--   0 root         (0)     1003     7327 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/transit.py
+-rw-rw-r--   0 root         (0)     1003     3209 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/transit_preferences.py
+-rw-rw-r--   0 root         (0)     1003     1337 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/units.py
+-rw-rw-r--   0 root         (0)     1003     1613 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/vehicle_emission_type.py
+-rw-rw-r--   0 root         (0)     1003     1506 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/vehicle_info.py
+-rw-rw-r--   0 root         (0)     1003     4704 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/google/maps/routing_v2/types/waypoint.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.256053 google-maps-routing-0.6.8/google_maps_routing.egg-info/
+-rw-r--r--   0 root         (0)     1003     5264 2024-04-15 13:58:53.000000 google-maps-routing-0.6.8/google_maps_routing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2294 2024-04-15 13:58:53.000000 google-maps-routing-0.6.8/google_maps_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:58:53.000000 google-maps-routing-0.6.8/google_maps_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:58:53.000000 google-maps-routing-0.6.8/google_maps_routing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      338 2024-04-15 13:58:53.000000 google-maps-routing-0.6.8/google_maps_routing.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-15 13:58:53.000000 google-maps-routing-0.6.8/google_maps_routing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-15 13:58:53.260053 google-maps-routing-0.6.8/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3202 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.256053 google-maps-routing-0.6.8/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.256053 google-maps-routing-0.6.8/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.260053 google-maps-routing-0.6.8/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:53.260053 google-maps-routing-0.6.8/tests/unit/gapic/routing_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/tests/unit/gapic/routing_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    93577 2024-04-15 13:54:45.000000 google-maps-routing-0.6.8/tests/unit/gapic/routing_v2/test_routes.py
```

### Comparing `google-maps-routing-0.6.7/LICENSE` & `google-maps-routing-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.7/MANIFEST.in` & `google-maps-routing-0.6.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.7/PKG-INFO` & `google-maps-routing-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-routing
-Version: 0.6.7
+Version: 0.6.8
 Summary: Google Maps Routing API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-routing
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-routing-0.6.7/README.rst` & `google-maps-routing-0.6.8/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.7/google/maps/routing/__init__.py` & `google-maps-routing-0.6.8/google/maps/routing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing/gapic_version.py` & `google-maps-routing-0.6.8/google/maps/routing/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.7"  # {x-release-please-version}
+__version__ = "0.6.8"  # {x-release-please-version}
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/__init__.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/gapic_metadata.json` & `google-maps-routing-0.6.8/google/maps/routing_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/gapic_version.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.7"  # {x-release-please-version}
+__version__ = "0.6.8"  # {x-release-please-version}
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/services/__init__.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/__init__.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/async_client.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -261,15 +261,15 @@
         given a set of terminal and intermediate waypoints.
 
         **NOTE:** This method requires that you specify a response field
         mask in the input. You can provide the response field mask by
         using URL parameter ``$fields`` or ``fields``, or by using an
         HTTP/gRPC header ``X-Goog-FieldMask`` (see the `available URL
         parameters and
-        headers <https://cloud.google.com/apis/docs/system-parameters>`__.
+        headers <https://cloud.google.com/apis/docs/system-parameters>`__).
         The value is a comma separated list of field paths. See detailed
         documentation about `how to construct the field
         paths <https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/field_mask.proto>`__.
 
         For example, in this method:
 
         -  Field mask of all available fields (for manual inspection):
@@ -371,15 +371,15 @@
         destination.
 
         **NOTE:** This method requires that you specify a response field
         mask in the input. You can provide the response field mask by
         using the URL parameter ``$fields`` or ``fields``, or by using
         the HTTP/gRPC header ``X-Goog-FieldMask`` (see the `available
         URL parameters and
-        headers <https://cloud.google.com/apis/docs/system-parameters>`__.
+        headers <https://cloud.google.com/apis/docs/system-parameters>`__).
         The value is a comma separated list of field paths. See this
         detailed documentation about `how to construct the field
         paths <https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/field_mask.proto>`__.
 
         For example, in this method:
 
         -  Field mask of all available fields (for manual inspection):
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/client.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -658,15 +658,15 @@
         given a set of terminal and intermediate waypoints.
 
         **NOTE:** This method requires that you specify a response field
         mask in the input. You can provide the response field mask by
         using URL parameter ``$fields`` or ``fields``, or by using an
         HTTP/gRPC header ``X-Goog-FieldMask`` (see the `available URL
         parameters and
-        headers <https://cloud.google.com/apis/docs/system-parameters>`__.
+        headers <https://cloud.google.com/apis/docs/system-parameters>`__).
         The value is a comma separated list of field paths. See detailed
         documentation about `how to construct the field
         paths <https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/field_mask.proto>`__.
 
         For example, in this method:
 
         -  Field mask of all available fields (for manual inspection):
@@ -769,15 +769,15 @@
         destination.
 
         **NOTE:** This method requires that you specify a response field
         mask in the input. You can provide the response field mask by
         using the URL parameter ``$fields`` or ``fields``, or by using
         the HTTP/gRPC header ``X-Goog-FieldMask`` (see the `available
         URL parameters and
-        headers <https://cloud.google.com/apis/docs/system-parameters>`__.
+        headers <https://cloud.google.com/apis/docs/system-parameters>`__).
         The value is a comma separated list of field paths. See this
         detailed documentation about `how to construct the field
         paths <https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/field_mask.proto>`__.
 
         For example, in this method:
 
         -  Field mask of all available fields (for manual inspection):
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/__init__.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/base.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/grpc.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -240,15 +240,15 @@
         given a set of terminal and intermediate waypoints.
 
         **NOTE:** This method requires that you specify a response field
         mask in the input. You can provide the response field mask by
         using URL parameter ``$fields`` or ``fields``, or by using an
         HTTP/gRPC header ``X-Goog-FieldMask`` (see the `available URL
         parameters and
-        headers <https://cloud.google.com/apis/docs/system-parameters>`__.
+        headers <https://cloud.google.com/apis/docs/system-parameters>`__).
         The value is a comma separated list of field paths. See detailed
         documentation about `how to construct the field
         paths <https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/field_mask.proto>`__.
 
         For example, in this method:
 
         -  Field mask of all available fields (for manual inspection):
@@ -305,15 +305,15 @@
         destination.
 
         **NOTE:** This method requires that you specify a response field
         mask in the input. You can provide the response field mask by
         using the URL parameter ``$fields`` or ``fields``, or by using
         the HTTP/gRPC header ``X-Goog-FieldMask`` (see the `available
         URL parameters and
-        headers <https://cloud.google.com/apis/docs/system-parameters>`__.
+        headers <https://cloud.google.com/apis/docs/system-parameters>`__).
         The value is a comma separated list of field paths. See this
         detailed documentation about `how to construct the field
         paths <https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/field_mask.proto>`__.
 
         For example, in this method:
 
         -  Field mask of all available fields (for manual inspection):
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -244,15 +244,15 @@
         given a set of terminal and intermediate waypoints.
 
         **NOTE:** This method requires that you specify a response field
         mask in the input. You can provide the response field mask by
         using URL parameter ``$fields`` or ``fields``, or by using an
         HTTP/gRPC header ``X-Goog-FieldMask`` (see the `available URL
         parameters and
-        headers <https://cloud.google.com/apis/docs/system-parameters>`__.
+        headers <https://cloud.google.com/apis/docs/system-parameters>`__).
         The value is a comma separated list of field paths. See detailed
         documentation about `how to construct the field
         paths <https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/field_mask.proto>`__.
 
         For example, in this method:
 
         -  Field mask of all available fields (for manual inspection):
@@ -310,15 +310,15 @@
         destination.
 
         **NOTE:** This method requires that you specify a response field
         mask in the input. You can provide the response field mask by
         using the URL parameter ``$fields`` or ``fields``, or by using
         the HTTP/gRPC header ``X-Goog-FieldMask`` (see the `available
         URL parameters and
-        headers <https://cloud.google.com/apis/docs/system-parameters>`__.
+        headers <https://cloud.google.com/apis/docs/system-parameters>`__).
         The value is a comma separated list of field paths. See this
         detailed documentation about `how to construct the field
         paths <https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/field_mask.proto>`__.
 
         For example, in this method:
 
         -  Field mask of all available fields (for manual inspection):
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/services/routes/transports/rest.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/services/routes/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/__init__.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/fallback_info.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/fallback_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -55,19 +55,19 @@
     r"""Actual routing mode used for returned fallback response.
 
     Values:
         FALLBACK_ROUTING_MODE_UNSPECIFIED (0):
             Not used.
         FALLBACK_TRAFFIC_UNAWARE (1):
             Indicates the ``TRAFFIC_UNAWARE``
-            [google.maps.routing.v2.RoutingPreference] was used to
-            compute the response.
+            [``RoutingPreference``][google.maps.routing.v2.RoutingPreference]
+            was used to compute the response.
         FALLBACK_TRAFFIC_AWARE (2):
             Indicates the ``TRAFFIC_AWARE``
-            [RoutingPreference][google.maps.routing.v2.RoutingPreference]
+            [``RoutingPreference``][google.maps.routing.v2.RoutingPreference]
             was used to compute the response.
     """
     FALLBACK_ROUTING_MODE_UNSPECIFIED = 0
     FALLBACK_TRAFFIC_UNAWARE = 1
     FALLBACK_TRAFFIC_AWARE = 2
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/geocoding_results.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/geocoding_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -27,15 +27,15 @@
         "GeocodedWaypoint",
     },
 )
 
 
 class GeocodingResults(proto.Message):
     r"""Contains
-    [GeocodedWaypoints][google.maps.routing.v2.GeocodedWaypoint] for
+    [``GeocodedWaypoints``][google.maps.routing.v2.GeocodedWaypoint] for
     origin, destination and intermediate waypoints. Only populated for
     address waypoints.
 
     Attributes:
         origin (google.maps.routing_v2.types.GeocodedWaypoint):
             Origin geocoded waypoint.
         destination (google.maps.routing_v2.types.GeocodedWaypoint):
@@ -81,18 +81,17 @@
             The index of the corresponding intermediate
             waypoint in the request. Only populated if the
             corresponding waypoint is an intermediate
             waypoint.
 
             This field is a member of `oneof`_ ``_intermediate_waypoint_request_index``.
         type_ (MutableSequence[str]):
-            The type(s) of the result, in the form of
-            zero or more type tags. Supported types:
-
-            https://developers.google.com/maps/documentation/geocoding/requests-geocoding#Types
+            The type(s) of the result, in the form of zero or more type
+            tags. Supported types: `Address types and address component
+            types <https://developers.google.com/maps/documentation/geocoding/requests-geocoding#Types>`__.
         partial_match (bool):
             Indicates that the geocoder did not return an
             exact match for the original request, though it
             was able to match part of the requested address.
             You may wish to examine the original request for
             misspellings and/or an incomplete address.
         place_id (str):
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/localized_time.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/localized_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/location.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -39,15 +39,15 @@
         heading (google.protobuf.wrappers_pb2.Int32Value):
             The compass heading associated with the direction of the
             flow of traffic. This value specifies the side of the road
             for pickup and drop-off. Heading values can be from 0 to
             360, where 0 specifies a heading of due North, 90 specifies
             a heading of due East, and so on. You can use this field
             only for ``DRIVE`` and ``TWO_WHEELER``
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode].
     """
 
     lat_lng: latlng_pb2.LatLng = proto.Field(
         proto.MESSAGE,
         number=1,
         message=latlng_pb2.LatLng,
     )
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/maneuver.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/maneuver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,15 +25,16 @@
         "Maneuver",
     },
 )
 
 
 class Maneuver(proto.Enum):
     r"""A set of values that specify the navigation action to take
-    for the current step (e.g., turn left, merge, straight, etc.).
+    for the current step (for example, turn left, merge, or
+    straight).
 
     Values:
         MANEUVER_UNSPECIFIED (0):
             Not used.
         TURN_SLIGHT_LEFT (1):
             Turn slightly to the left.
         TURN_SHARP_LEFT (2):
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/navigation_instruction.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/navigation_instruction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -27,22 +27,22 @@
         "NavigationInstruction",
     },
 )
 
 
 class NavigationInstruction(proto.Message):
     r"""Encapsulates navigation instructions for a
-    [RouteLegStep][google.maps.routing.v2.RouteLegStep]
+    [``RouteLegStep``][google.maps.routing.v2.RouteLegStep].
 
     Attributes:
         maneuver (google.maps.routing_v2.types.Maneuver):
             Encapsulates the navigation instructions for
-            the current step (e.g., turn left, merge,
-            straight, etc.). This field determines which
-            icon to display.
+            the current step (for example, turn left, merge,
+            or straight). This field determines which icon
+            to display.
         instructions (str):
             Instructions for navigating this step.
     """
 
     maneuver: gmr_maneuver.Maneuver = proto.Field(
         proto.ENUM,
         number=1,
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/polyline.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/polyline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -57,15 +57,15 @@
 
     Values:
         POLYLINE_ENCODING_UNSPECIFIED (0):
             No polyline type preference specified. Defaults to
             ``ENCODED_POLYLINE``.
         ENCODED_POLYLINE (1):
             Specifies a polyline encoded using the `polyline encoding
-            algorithm <https://developers.google.com/maps/documentation/utilities/polylinealgorithm>`__.
+            algorithm </maps/documentation/utilities/polylinealgorithm>`__.
         GEO_JSON_LINESTRING (2):
             Specifies a polyline using the `GeoJSON LineString
             format <https://tools.ietf.org/html/rfc7946#section-3.1.4>`__
     """
     POLYLINE_ENCODING_UNSPECIFIED = 0
     ENCODED_POLYLINE = 1
     GEO_JSON_LINESTRING = 2
@@ -86,15 +86,15 @@
             The string encoding of the polyline using the `polyline
             encoding
             algorithm <https://developers.google.com/maps/documentation/utilities/polylinealgorithm>`__
 
             This field is a member of `oneof`_ ``polyline_type``.
         geo_json_linestring (google.protobuf.struct_pb2.Struct):
             Specifies a polyline using the `GeoJSON LineString
-            format <https://tools.ietf.org/html/rfc7946#section-3.1.4>`__
+            format <https://tools.ietf.org/html/rfc7946#section-3.1.4>`__.
 
             This field is a member of `oneof`_ ``polyline_type``.
     """
 
     encoded_polyline: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/route.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -60,21 +60,21 @@
         route_labels (MutableSequence[google.maps.routing_v2.types.RouteLabel]):
             Labels for the ``Route`` that are useful to identify
             specific properties of the route to compare against others.
         legs (MutableSequence[google.maps.routing_v2.types.RouteLeg]):
             A collection of legs (path segments between waypoints) that
             make up the route. Each leg corresponds to the trip between
             two non-\ ``via``
-            [Waypoints][google.maps.routing.v2.Waypoint]. For example, a
-            route with no intermediate waypoints has only one leg. A
-            route that includes one non-\ ``via`` intermediate waypoint
-            has two legs. A route that includes one ``via`` intermediate
-            waypoint has one leg. The order of the legs matches the
-            order of waypoints from ``origin`` to ``intermediates`` to
-            ``destination``.
+            [``Waypoints``][google.maps.routing.v2.Waypoint]. For
+            example, a route with no intermediate waypoints has only one
+            leg. A route that includes one non-\ ``via`` intermediate
+            waypoint has two legs. A route that includes one ``via``
+            intermediate waypoint has one leg. The order of the legs
+            matches the order of waypoints from ``origin`` to
+            ``intermediates`` to ``destination``.
         distance_meters (int):
             The travel distance of the route, in meters.
         duration (google.protobuf.duration_pb2.Duration):
             The length of time needed to navigate the route. If you set
             the ``routing_preference`` to ``TRAFFIC_UNAWARE``, then this
             value is the same as ``static_duration``. If you set the
             ``routing_preference`` to either ``TRAFFIC_AWARE`` or
@@ -94,15 +94,15 @@
             the route.
         viewport (google.geo.type.types.Viewport):
             The viewport bounding box of the polyline.
         travel_advisory (google.maps.routing_v2.types.RouteTravelAdvisory):
             Additional information about the route.
         optimized_intermediate_waypoint_index (MutableSequence[int]):
             If you set
-            [optimize_waypoint_order][google.maps.routing.v2.ComputeRoutesRequest.optimize_waypoint_order]
+            [``optimize_waypoint_order``][google.maps.routing.v2.ComputeRoutesRequest.optimize_waypoint_order]
             to true, this field contains the optimized ordering of
             intermediate waypoints. Otherwise, this field is empty. For
             example, if you give an input of Origin: LA; Intermediate
             waypoints: Dallas, Bangor, Phoenix; Destination: New York;
             and the optimized intermediate waypoint order is Phoenix,
             Dallas, Bangor, then this field contains the values [2, 0,
             1]. The index starts with 0 for the first intermediate
@@ -130,15 +130,15 @@
         Attributes:
             distance (google.type.localized_text_pb2.LocalizedText):
                 Travel distance represented in text form.
             duration (google.type.localized_text_pb2.LocalizedText):
                 Duration taking traffic conditions into consideration,
                 represented in text form. Note: If you did not request
                 traffic information, this value will be the same value as
-                static_duration.
+                ``static_duration``.
             static_duration (google.type.localized_text_pb2.LocalizedText):
                 Duration without taking traffic conditions
                 into consideration, represented in text form.
             transit_fare (google.type.localized_text_pb2.LocalizedText):
                 Transit fare represented in text form.
         """
 
@@ -227,21 +227,20 @@
 
 class RouteTravelAdvisory(proto.Message):
     r"""Contains the additional information that the user should be
     informed about, such as possible traffic zone restrictions.
 
     Attributes:
         toll_info (google.maps.routing_v2.types.TollInfo):
-            Contains information about tolls on the
-            route. This field is only populated if tolls are
-            expected on the route. If this field is set, but
-            the estimatedPrice subfield is not populated,
-            then the route contains tolls, but the estimated
-            price is unknown. If this field is not set, then
-            there are no tolls expected on the route.
+            Contains information about tolls on the route. This field is
+            only populated if tolls are expected on the route. If this
+            field is set, but the ``estimatedPrice`` subfield is not
+            populated, then the route contains tolls, but the estimated
+            price is unknown. If this field is not set, then there are
+            no tolls expected on the route.
         speed_reading_intervals (MutableSequence[google.maps.routing_v2.types.SpeedReadingInterval]):
             Speed reading intervals detailing traffic density.
             Applicable in case of ``TRAFFIC_AWARE`` and
             ``TRAFFIC_AWARE_OPTIMAL`` routing preferences. The intervals
             cover the entire polyline of the route without overlap. The
             start point of a specified interval is the same as the end
             point of the preceding interval.
@@ -552,17 +551,17 @@
         proto.MESSAGE,
         number=10,
         message=StepsOverview,
     )
 
 
 class RouteLegStep(proto.Message):
-    r"""Contains a segment of a [RouteLeg][google.maps.routing.v2.RouteLeg].
-    A step corresponds to a single navigation instruction. Route legs
-    are made up of steps.
+    r"""Contains a segment of a
+    [``RouteLeg``][google.maps.routing.v2.RouteLeg]. A step corresponds
+    to a single navigation instruction. Route legs are made up of steps.
 
     Attributes:
         distance_meters (int):
             The travel distance of this step, in meters.
             In some circumstances, this field might not have
             a value.
         static_duration (google.protobuf.duration_pb2.Duration):
@@ -702,15 +701,15 @@
             identify a transit trip to passengers. The text should
             uniquely identify a trip within a service day. For example,
             "538" is the ``trip_short_text`` of the Amtrak train that
             leaves San Jose, CA at 15:10 on weekdays to Sacramento, CA.
     """
 
     class TransitStopDetails(proto.Message):
-        r"""Details about the transit stops for the ``RouteLegStep``
+        r"""Details about the transit stops for the ``RouteLegStep``.
 
         Attributes:
             arrival_stop (google.maps.routing_v2.types.TransitStop):
                 Information about the arrival stop for the
                 step.
             arrival_time (google.protobuf.timestamp_pb2.Timestamp):
                 The estimated time of arrival for the step.
@@ -739,15 +738,15 @@
         departure_time: timestamp_pb2.Timestamp = proto.Field(
             proto.MESSAGE,
             number=4,
             message=timestamp_pb2.Timestamp,
         )
 
     class TransitDetailsLocalizedValues(proto.Message):
-        r"""Localized descriptions of values for RouteTransitDetails.
+        r"""Localized descriptions of values for ``RouteTransitDetails``.
 
         Attributes:
             arrival_time (google.maps.routing_v2.types.LocalizedTime):
                 Time in its formatted text representation
                 with a corresponding time zone.
             departure_time (google.maps.routing_v2.types.LocalizedTime):
                 Time in its formatted text representation
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/route_label.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/route_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,28 +24,28 @@
     manifest={
         "RouteLabel",
     },
 )
 
 
 class RouteLabel(proto.Enum):
-    r"""Labels for the [Route][google.maps.routing.v2.Route] that are useful
-    to identify specific properties of the route to compare against
-    others.
+    r"""Labels for the [``Route``][google.maps.routing.v2.Route] that are
+    useful to identify specific properties of the route to compare
+    against others.
 
     Values:
         ROUTE_LABEL_UNSPECIFIED (0):
             Default - not used.
         DEFAULT_ROUTE (1):
             The default "best" route returned for the
             route computation.
         DEFAULT_ROUTE_ALTERNATE (2):
             An alternative to the default "best" route. Routes like this
             will be returned when
-            [compute_alternative_routes][google.maps.routing.v2.ComputeRoutesRequest.compute_alternative_routes]
+            [``compute_alternative_routes``][google.maps.routing.v2.ComputeRoutesRequest.compute_alternative_routes]
             is specified.
         FUEL_EFFICIENT (3):
             Fuel efficient route. Routes labeled with
             this value are determined to be optimized for
             Eco parameters such as fuel consumption.
     """
     ROUTE_LABEL_UNSPECIFIED = 0
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/route_modifiers.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/route_modifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -35,39 +35,39 @@
     calculating the routes.
 
     Attributes:
         avoid_tolls (bool):
             When set to true, avoids toll roads where reasonable, giving
             preference to routes not containing toll roads. Applies only
             to the ``DRIVE`` and ``TWO_WHEELER``
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode].
         avoid_highways (bool):
             When set to true, avoids highways where reasonable, giving
             preference to routes not containing highways. Applies only
             to the ``DRIVE`` and ``TWO_WHEELER``
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode].
         avoid_ferries (bool):
             When set to true, avoids ferries where reasonable, giving
             preference to routes not containing ferries. Applies only to
             the ``DRIVE`` and\ ``TWO_WHEELER``
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode].
         avoid_indoor (bool):
             When set to true, avoids navigating indoors where
             reasonable, giving preference to routes not containing
             indoor navigation. Applies only to the ``WALK``
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode].
         vehicle_info (google.maps.routing_v2.types.VehicleInfo):
             Specifies the vehicle information.
         toll_passes (MutableSequence[google.maps.routing_v2.types.TollPass]):
             Encapsulates information about toll passes. If toll passes
             are provided, the API tries to return the pass price. If
             toll passes are not provided, the API treats the toll pass
             as unknown and tries to return the cash price. Applies only
             to the ``DRIVE`` and ``TWO_WHEELER``
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode].
     """
 
     avoid_tolls: bool = proto.Field(
         proto.BOOL,
         number=1,
     )
     avoid_highways: bool = proto.Field(
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/route_travel_mode.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/route_travel_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/routes_service.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/routes_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -97,46 +97,50 @@
             Optional. Specifies the preferred encoding
             for the polyline.
         departure_time (google.protobuf.timestamp_pb2.Timestamp):
             Optional. The departure time. If you don't set this value,
             then this value defaults to the time that you made the
             request. NOTE: You can only specify a ``departure_time`` in
             the past when
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
-            set to ``TRANSIT``.
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode]
+            is set to ``TRANSIT``. Transit trips are available for up to
+            7 days in the past or 100 days in the future.
         arrival_time (google.protobuf.timestamp_pb2.Timestamp):
             Optional. The arrival time. NOTE: Can only be set when
             [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
-            set to ``TRANSIT``. You can specify either departure_time or
-            arrival_time, but not both.
+            set to ``TRANSIT``. You can specify either
+            ``departure_time`` or ``arrival_time``, but not both.
+            Transit trips are available for up to 7 days in the past or
+            100 days in the future.
         compute_alternative_routes (bool):
             Optional. Specifies whether to calculate
             alternate routes in addition to the route. No
             alternative routes are returned for requests
             that have intermediate waypoints.
         route_modifiers (google.maps.routing_v2.types.RouteModifiers):
             Optional. A set of conditions to satisfy that
             affect the way routes are calculated.
         language_code (str):
             Optional. The BCP-47 language code, such as "en-US" or
-            "sr-Latn". For more information, see
-            http://www.unicode.org/reports/tr35/#Unicode_locale_identifier.
+            "sr-Latn". For more information, see `Unicode Locale
+            Identifier <http://www.unicode.org/reports/tr35/#Unicode_locale_identifier>`__.
             See `Language
             Support <https://developers.google.com/maps/faq#languagesupport>`__
             for the list of supported languages. When you don't provide
             this value, the display language is inferred from the
             location of the route request.
         region_code (str):
             Optional. The region code, specified as a ccTLD ("top-level
             domain") two-character value. For more information see
-            https://en.wikipedia.org/wiki/List_of_Internet_top-level_domains#Country_code_top-level_domains
+            `Country code top-level
+            domains <https://en.wikipedia.org/wiki/List_of_Internet_top-level_domains#Country_code_top-level_domains>`__.
         units (google.maps.routing_v2.types.Units):
             Optional. Specifies the units of measure for the display
             fields. These fields include the ``instruction`` field in
-            [NavigationInstruction][google.maps.routing.v2.NavigationInstruction].
+            [``NavigationInstruction``][google.maps.routing.v2.NavigationInstruction].
             The units of measure used for the route, leg, step distance,
             and duration are not affected by this value. If you don't
             provide this value, then the display units are inferred from
             the location of the first origin.
         optimize_waypoint_order (bool):
             Optional. If set to true, the service attempts to minimize
             the overall cost of the route by re-ordering the specified
@@ -165,30 +169,30 @@
             the response. These extra fields must also be
             specified in the field mask to be returned in
             the response.
         traffic_model (google.maps.routing_v2.types.TrafficModel):
             Optional. Specifies the assumptions to use when calculating
             time in traffic. This setting affects the value returned in
             the duration field in the
-            [Route][google.maps.routing.v2.Route] and
-            [RouteLeg][google.maps.routing.v2.RouteLeg] which contains
-            the predicted time in traffic based on historical averages.
-            ``TrafficModel`` is only available for requests that have
-            set
-            [RoutingPreference][google.maps.routing.v2.RoutingPreference]
+            [``Route``][google.maps.routing.v2.Route] and
+            [``RouteLeg``][google.maps.routing.v2.RouteLeg] which
+            contains the predicted time in traffic based on historical
+            averages. ``TrafficModel`` is only available for requests
+            that have set
+            [``RoutingPreference``][google.maps.routing.v2.RoutingPreference]
             to ``TRAFFIC_AWARE_OPTIMAL`` and
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] to
-            ``DRIVE``. Defaults to ``BEST_GUESS`` if traffic is
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode]
+            to ``DRIVE``. Defaults to ``BEST_GUESS`` if traffic is
             requested and ``TrafficModel`` is not specified.
         transit_preferences (google.maps.routing_v2.types.TransitPreferences):
             Optional. Specifies preferences that influence the route
             returned for ``TRANSIT`` routes. NOTE: You can only specify
             a ``transit_preferences`` when
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
-            set to ``TRANSIT``.
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode]
+            is set to ``TRANSIT``.
     """
 
     class ReferenceRoute(proto.Enum):
         r"""A supported reference route on the ComputeRoutesRequest.
 
         Values:
             REFERENCE_ROUTE_UNSPECIFIED (0):
@@ -212,16 +216,15 @@
             TOLLS (1):
                 Toll information for the route(s).
             FUEL_CONSUMPTION (2):
                 Estimated fuel consumption for the route(s).
             TRAFFIC_ON_POLYLINE (3):
                 Traffic aware polylines for the route(s).
             HTML_FORMATTED_NAVIGATION_INSTRUCTIONS (4):
-                [Navigation
-                Instructions][google.maps.routing.v2.NavigationInstructions.instructions]
+                ```NavigationInstructions`` <google.maps.routing.v2.NavigationInstructions.instructions>`__
                 presented as a formatted HTML text string. This content is
                 meant to be read as-is. This content is for display only. Do
                 not programmatically parse it.
         """
         EXTRA_COMPUTATION_UNSPECIFIED = 0
         TOLLS = 1
         FUEL_CONSUMPTION = 2
@@ -323,16 +326,16 @@
 
 class ComputeRoutesResponse(proto.Message):
     r"""ComputeRoutes the response message.
 
     Attributes:
         routes (MutableSequence[google.maps.routing_v2.types.Route]):
             Contains an array of computed routes (up to three) when you
-            specify compute_alternatives_routes, and contains just one
-            route when you don't. When this array contains multiple
+            specify ``compute_alternatives_routes``, and contains just
+            one route when you don't. When this array contains multiple
             entries, the first one is the most recommended route. If the
             array is empty, then it means no route could be found.
         fallback_info (google.maps.routing_v2.types.FallbackInfo):
             In some cases when the server is not able to
             compute the route results with all of the input
             preferences, it may fallback to using a
             different way of computation. When fallback mode
@@ -366,21 +369,25 @@
 
     Attributes:
         origins (MutableSequence[google.maps.routing_v2.types.RouteMatrixOrigin]):
             Required. Array of origins, which determines the rows of the
             response matrix. Several size restrictions apply to the
             cardinality of origins and destinations:
 
-            -  The number of elements (origins × destinations) must be
-               no greater than 625 in any case.
-            -  The number of elements (origins × destinations) must be
-               no greater than 100 if routing_preference is set to
-               ``TRAFFIC_AWARE_OPTIMAL``.
-            -  The number of waypoints (origins + destinations)
-               specified as ``place_id`` must be no greater than 50.
+            -  The sum of the number of origins + the number of
+               destinations specified as either ``place_id`` or
+               ``address`` must be no greater than 50.
+            -  The product of number of origins × number of destinations
+               must be no greater than 625 in any case.
+            -  The product of the number of origins × number of
+               destinations must be no greater than 100 if
+               routing_preference is set to ``TRAFFIC_AWARE_OPTIMAL``.
+            -  The product of the number of origins × number of
+               destinations must be no greater than 100 if travel_mode
+               is set to ``TRANSIT``.
         destinations (MutableSequence[google.maps.routing_v2.types.RouteMatrixDestination]):
             Required. Array of destinations, which
             determines the columns of the response matrix.
         travel_mode (google.maps.routing_v2.types.RouteTravelMode):
             Optional. Specifies the mode of
             transportation.
         routing_preference (google.maps.routing_v2.types.RoutingPreference):
@@ -391,34 +398,38 @@
             this option only when the ``travel_mode`` is ``DRIVE`` or
             ``TWO_WHEELER``, otherwise the request fails.
         departure_time (google.protobuf.timestamp_pb2.Timestamp):
             Optional. The departure time. If you don't set this value,
             then this value defaults to the time that you made the
             request. NOTE: You can only specify a ``departure_time`` in
             the past when
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
-            set to ``TRANSIT``.
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode]
+            is set to ``TRANSIT``.
         arrival_time (google.protobuf.timestamp_pb2.Timestamp):
             Optional. The arrival time. NOTE: Can only be set when
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode] is
-            set to ``TRANSIT``. You can specify either departure_time or
-            arrival_time, but not both.
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode]
+            is set to ``TRANSIT``. You can specify either
+            ``departure_time`` or ``arrival_time``, but not both.
         language_code (str):
             Optional. The BCP-47 language code, such as "en-US" or
-            "sr-Latn". For more information, see
-            http://www.unicode.org/reports/tr35/#Unicode_locale_identifier.
+            "sr-Latn". For more information, see `Unicode Locale
+            Identifier <http://www.unicode.org/reports/tr35/#Unicode_locale_identifier>`__.
             See `Language
             Support <https://developers.google.com/maps/faq#languagesupport>`__
             for the list of supported languages. When you don't provide
             this value, the display language is inferred from the
             location of the first origin.
         region_code (str):
             Optional. The region code, specified as a ccTLD ("top-level
             domain") two-character value. For more information see
-            https://en.wikipedia.org/wiki/List_of_Internet_top-level_domains#Country_code_top-level_domains
+            `Country code top-level
+            domains <https://en.wikipedia.org/wiki/List_of_Internet_top-level_domains#Country_code_top-level_domains>`__.
+        units (google.maps.routing_v2.types.Units):
+            Optional. Specifies the units of measure for
+            the display fields.
         extra_computations (MutableSequence[google.maps.routing_v2.types.ComputeRouteMatrixRequest.ExtraComputation]):
             Optional. A list of extra computations which
             may be used to complete the request. Note: These
             extra computations may return extra fields on
             the response. These extra fields must also be
             specified in the field mask to be returned in
             the response.
@@ -489,14 +500,19 @@
         proto.STRING,
         number=6,
     )
     region_code: str = proto.Field(
         proto.STRING,
         number=9,
     )
+    units: gmr_units.Units = proto.Field(
+        proto.ENUM,
+        number=7,
+        enum=gmr_units.Units,
+    )
     extra_computations: MutableSequence[ExtraComputation] = proto.RepeatedField(
         proto.ENUM,
         number=8,
         enum=ExtraComputation,
     )
     traffic_model: gmr_traffic_model.TrafficModel = proto.Field(
         proto.ENUM,
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/routing_preference.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/routing_preference.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -36,22 +36,24 @@
             No routing preference specified. Default to
             ``TRAFFIC_UNAWARE``.
         TRAFFIC_UNAWARE (1):
             Computes routes without taking live traffic conditions into
             consideration. Suitable when traffic conditions don't matter
             or are not applicable. Using this value produces the lowest
             latency. Note: For
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode]
-            ``DRIVE`` and ``TWO_WHEELER`` choice of route and duration
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode]
+            ``DRIVE`` and ``TWO_WHEELER``, the route and duration chosen
             are based on road network and average time-independent
-            traffic conditions. Results for a given request may vary
-            over time due to changes in the road network, updated
-            average traffic conditions, and the distributed nature of
-            the service. Results may also vary between nearly-equivalent
-            routes at any time or frequency.
+            traffic conditions, not current road conditions.
+            Consequently, routes may include roads that are temporarily
+            closed. Results for a given request may vary over time due
+            to changes in the road network, updated average traffic
+            conditions, and the distributed nature of the service.
+            Results may also vary between nearly-equivalent routes at
+            any time or frequency.
         TRAFFIC_AWARE (2):
             Calculates routes taking live traffic conditions into
             consideration. In contrast to ``TRAFFIC_AWARE_OPTIMAL``,
             some optimizations are applied to significantly reduce
             latency.
         TRAFFIC_AWARE_OPTIMAL (3):
             Calculates the routes taking live traffic
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/speed_reading_interval.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/speed_reading_interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,16 +26,16 @@
     },
 )
 
 
 class SpeedReadingInterval(proto.Message):
     r"""Traffic density indicator on a contiguous segment of a polyline or
     path. Given a path with points P_0, P_1, ... , P_N (zero-based
-    index), the SpeedReadingInterval defines an interval and describes
-    its traffic using the following categories.
+    index), the ``SpeedReadingInterval`` defines an interval and
+    describes its traffic using the following categories.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         start_polyline_point_index (int):
             The starting index of this interval in the
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/toll_info.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/toll_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,22 +26,22 @@
         "TollInfo",
     },
 )
 
 
 class TollInfo(proto.Message):
     r"""Encapsulates toll information on a
-    [Route][google.maps.routing.v2.Route] or on a
-    [RouteLeg][google.maps.routing.v2.RouteLeg].
+    [``Route``][google.maps.routing.v2.Route] or on a
+    [``RouteLeg``][google.maps.routing.v2.RouteLeg].
 
     Attributes:
         estimated_price (MutableSequence[google.type.money_pb2.Money]):
             The monetary amount of tolls for the corresponding
-            [Route][google.maps.routing.v2.Route] or
-            [RouteLeg][google.maps.routing.v2.RouteLeg]. This list
+            [``Route``][google.maps.routing.v2.Route] or
+            [``RouteLeg``][google.maps.routing.v2.RouteLeg]. This list
             contains a money amount for each currency that is expected
             to be charged by the toll stations. Typically this list will
             contain only one item for routes with tolls in one currency.
             For international trips, this list may contain multiple
             items to reflect tolls in different currencies.
     """
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/toll_passes.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/toll_passes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -91,14 +91,24 @@
             - BCA https://www.bca.co.id/flazz
             - BNI
               https://www.bni.co.id/id-id/ebanking/tapcash
         IN_FASTAG (78):
             India.
         IN_LOCAL_HP_PLATE_EXEMPT (79):
             India, HP state plate exemption.
+        JP_ETC (98):
+            Japan
+            ETC. Electronic wireless system to collect
+            tolls. https://www.go-etc.jp/
+        JP_ETC2 (99):
+            Japan
+            ETC2.0. New version of ETC with further discount
+            and bidirectional communication between devices
+            on vehicles and antennas on the road.
+            https://www.go-etc.jp/etc2/index.html
         MX_IAVE (90):
             Mexico toll pass.
             https://iave.capufe.gob.mx/#/
         MX_PASE (91):
             Mexico
             https://www.pase.com.mx
         MX_QUICKPASS (93):
@@ -253,14 +263,16 @@
             WA, USA.
         US_WA_GOOD_TO_GO (1):
             WA, USA.
         US_WV_EZPASSWV (62):
             WV, USA.
         US_WV_MEMORIAL_BRIDGE_TICKETS (63):
             WV, USA.
+        US_WV_MOV_PASS (100):
+            WV, USA
         US_WV_NEWELL_TOLL_BRIDGE_TICKET (64):
             WV, USA.
     """
     TOLL_PASS_UNSPECIFIED = 0
     AU_ETOLL_TAG = 82
     AU_EWAY_TAG = 83
     AU_LINKT = 2
@@ -276,14 +288,16 @@
     CA_US_AKWASASNE_SEAWAY_TRANSIT_CARD = 85
     CA_US_BLUE_WATER_EDGE_PASS = 18
     CA_US_CONNEXION = 19
     CA_US_NEXUS_CARD = 20
     ID_E_TOLL = 16
     IN_FASTAG = 78
     IN_LOCAL_HP_PLATE_EXEMPT = 79
+    JP_ETC = 98
+    JP_ETC2 = 99
     MX_IAVE = 90
     MX_PASE = 91
     MX_QUICKPASS = 93
     MX_SISTEMA_TELEPEAJE_CHIHUAHUA = 89
     MX_TAG_IAVE = 12
     MX_TAG_TELEVIA = 13
     MX_TELEVIA = 92
@@ -351,11 +365,12 @@
     US_TX_XPRESS_CARD = 59
     US_UT_ADAMS_AVE_PARKWAY_EXPRESSCARD = 60
     US_VA_EZPASSVA = 61
     US_WA_BREEZEBY = 17
     US_WA_GOOD_TO_GO = 1
     US_WV_EZPASSWV = 62
     US_WV_MEMORIAL_BRIDGE_TICKETS = 63
+    US_WV_MOV_PASS = 100
     US_WV_NEWELL_TOLL_BRIDGE_TICKET = 64
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/traffic_model.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/traffic_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/transit.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/transit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/transit_preferences.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/transit_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/units.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/units.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/vehicle_emission_type.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/vehicle_emission_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,15 +26,15 @@
     },
 )
 
 
 class VehicleEmissionType(proto.Enum):
     r"""A set of values describing the vehicle's emission type. Applies only
     to the ``DRIVE``
-    [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
+    [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode].
 
     Values:
         VEHICLE_EMISSION_TYPE_UNSPECIFIED (0):
             No emission type specified. Default to ``GASOLINE``.
         GASOLINE (1):
             Gasoline/petrol fueled vehicle.
         ELECTRIC (2):
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/vehicle_info.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/vehicle_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -33,15 +33,15 @@
     r"""Contains the vehicle information, such as the vehicle
     emission type.
 
     Attributes:
         emission_type (google.maps.routing_v2.types.VehicleEmissionType):
             Describes the vehicle's emission type. Applies only to the
             ``DRIVE``
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode].
     """
 
     emission_type: vehicle_emission_type.VehicleEmissionType = proto.Field(
         proto.ENUM,
         number=2,
         enum=vehicle_emission_type.VehicleEmissionType,
     )
```

### Comparing `google-maps-routing-0.6.7/google/maps/routing_v2/types/waypoint.py` & `google-maps-routing-0.6.8/google/maps/routing_v2/types/waypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -57,43 +57,43 @@
             See https://plus.codes for details.
 
             This field is a member of `oneof`_ ``location_type``.
         via (bool):
             Marks this waypoint as a milestone rather a stopping point.
             For each non-via waypoint in the request, the response
             appends an entry to the
-            [legs][google.maps.routing.v2.Route.legs] array to provide
-            the details for stopovers on that leg of the trip. Set this
-            value to true when you want the route to pass through this
-            waypoint without stopping over. Via waypoints don't cause an
-            entry to be added to the ``legs`` array, but they do route
-            the journey through the waypoint. You can only set this
-            value on waypoints that are intermediates. The request fails
-            if you set this field on terminal waypoints. If
-            ``ComputeRoutesRequest.optimize_waypoint_order`` is set to
-            true then this field cannot be set to true; otherwise, the
-            request fails.
+            [``legs``][google.maps.routing.v2.Route.legs] array to
+            provide the details for stopovers on that leg of the trip.
+            Set this value to true when you want the route to pass
+            through this waypoint without stopping over. Via waypoints
+            don't cause an entry to be added to the ``legs`` array, but
+            they do route the journey through the waypoint. You can only
+            set this value on waypoints that are intermediates. The
+            request fails if you set this field on terminal waypoints.
+            If ``ComputeRoutesRequest.optimize_waypoint_order`` is set
+            to true then this field cannot be set to true; otherwise,
+            the request fails.
         vehicle_stopover (bool):
             Indicates that the waypoint is meant for vehicles to stop
             at, where the intention is to either pickup or drop-off.
             When you set this value, the calculated route won't include
             non-\ ``via`` waypoints on roads that are unsuitable for
             pickup and drop-off. This option works only for ``DRIVE``
             and ``TWO_WHEELER`` travel modes, and when the
             ``location_type`` is
-            [Location][google.maps.routing.v2.Location].
+            [``Location``][google.maps.routing.v2.Location].
         side_of_road (bool):
             Indicates that the location of this waypoint is meant to
             have a preference for the vehicle to stop at a particular
             side of road. When you set this value, the route will pass
             through the location so that the vehicle can stop at the
             side of road that the location is biased towards from the
-            center of the road. This option works only for 'DRIVE' and
-            'TWO_WHEELER'
-            [RouteTravelMode][google.maps.routing.v2.RouteTravelMode].
+            center of the road. This option works only for ``DRIVE`` and
+            ``TWO_WHEELER``
+            [``RouteTravelMode``][google.maps.routing.v2.RouteTravelMode].
     """
 
     location: gmr_location.Location = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="location_type",
         message=gmr_location.Location,
```

### Comparing `google-maps-routing-0.6.7/google_maps_routing.egg-info/PKG-INFO` & `google-maps-routing-0.6.8/google_maps_routing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-routing
-Version: 0.6.7
+Version: 0.6.8
 Summary: Google Maps Routing API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-routing
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-routing-0.6.7/google_maps_routing.egg-info/SOURCES.txt` & `google-maps-routing-0.6.8/google_maps_routing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.7/setup.py` & `google-maps-routing-0.6.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/tests/__init__.py` & `google-maps-routing-0.6.8/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/tests/unit/__init__.py` & `google-maps-routing-0.6.8/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/tests/unit/gapic/__init__.py` & `google-maps-routing-0.6.8/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/tests/unit/gapic/routing_v2/__init__.py` & `google-maps-routing-0.6.8/tests/unit/gapic/routing_v2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-routing-0.6.7/tests/unit/gapic/routing_v2/test_routes.py` & `google-maps-routing-0.6.8/tests/unit/gapic/routing_v2/test_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1091,15 +1091,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = routes_service.ComputeRoutesResponse()
         response = client.compute_routes(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == routes_service.ComputeRoutesRequest()
+        request = routes_service.ComputeRoutesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, routes_service.ComputeRoutesResponse)
 
 
 def test_compute_routes_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -1113,14 +1114,62 @@
     with mock.patch.object(type(client.transport.compute_routes), "__call__") as call:
         client.compute_routes()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == routes_service.ComputeRoutesRequest()
 
 
+def test_compute_routes_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = RoutesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = routes_service.ComputeRoutesRequest(
+        language_code="language_code_value",
+        region_code="region_code_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.compute_routes), "__call__") as call:
+        client.compute_routes(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == routes_service.ComputeRoutesRequest(
+            language_code="language_code_value",
+            region_code="region_code_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_compute_routes_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = RoutesAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.compute_routes), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            routes_service.ComputeRoutesResponse()
+        )
+        response = await client.compute_routes()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == routes_service.ComputeRoutesRequest()
+
+
 @pytest.mark.asyncio
 async def test_compute_routes_async(
     transport: str = "grpc_asyncio", request_type=routes_service.ComputeRoutesRequest
 ):
     client = RoutesAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1137,15 +1186,16 @@
             routes_service.ComputeRoutesResponse()
         )
         response = await client.compute_routes(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == routes_service.ComputeRoutesRequest()
+        request = routes_service.ComputeRoutesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, routes_service.ComputeRoutesResponse)
 
 
 @pytest.mark.asyncio
 async def test_compute_routes_async_from_dict():
@@ -1176,15 +1226,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = iter([routes_service.RouteMatrixElement()])
         response = client.compute_route_matrix(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == routes_service.ComputeRouteMatrixRequest()
+        request = routes_service.ComputeRouteMatrixRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     for message in response:
         assert isinstance(message, routes_service.RouteMatrixElement)
 
 
 def test_compute_route_matrix_empty_call():
@@ -1201,14 +1252,67 @@
     ) as call:
         client.compute_route_matrix()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == routes_service.ComputeRouteMatrixRequest()
 
 
+def test_compute_route_matrix_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = RoutesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = routes_service.ComputeRouteMatrixRequest(
+        language_code="language_code_value",
+        region_code="region_code_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.compute_route_matrix), "__call__"
+    ) as call:
+        client.compute_route_matrix(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == routes_service.ComputeRouteMatrixRequest(
+            language_code="language_code_value",
+            region_code="region_code_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_compute_route_matrix_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = RoutesAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.compute_route_matrix), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = mock.Mock(aio.UnaryStreamCall, autospec=True)
+        call.return_value.read = mock.AsyncMock(
+            side_effect=[routes_service.RouteMatrixElement()]
+        )
+        response = await client.compute_route_matrix()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == routes_service.ComputeRouteMatrixRequest()
+
+
 @pytest.mark.asyncio
 async def test_compute_route_matrix_async(
     transport: str = "grpc_asyncio",
     request_type=routes_service.ComputeRouteMatrixRequest,
 ):
     client = RoutesAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1229,15 +1333,16 @@
             side_effect=[routes_service.RouteMatrixElement()]
         )
         response = await client.compute_route_matrix(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == routes_service.ComputeRouteMatrixRequest()
+        request = routes_service.ComputeRouteMatrixRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     message = await response.read()
     assert isinstance(message, routes_service.RouteMatrixElement)
 
 
 @pytest.mark.asyncio
```

