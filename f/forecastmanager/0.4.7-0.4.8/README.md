# Comparing `tmp/forecastmanager-0.4.7.tar.gz` & `tmp/forecastmanager-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastmanager-0.4.7.tar", last modified: Tue Mar 26 13:02:34 2024, max compression
+gzip compressed data, was "forecastmanager-0.4.8.tar", last modified: Mon Apr 15 14:39:51 2024, max compression
```

## Comparing `forecastmanager-0.4.7.tar` & `forecastmanager-0.4.8.tar`

### file list

```diff
@@ -1,204 +1,208 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.172895 forecastmanager-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-26 13:02:34.172895 forecastmanager-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.136895 forecastmanager-0.4.7/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/forecast_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.140895 forecastmanager-0.4.7/forecastmanager/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15641 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.140895 forecastmanager-0.4.7/forecastmanager/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.140895 forecastmanager-0.4.7/forecastmanager/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.140895 forecastmanager-0.4.7/forecastmanager/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.140895 forecastmanager-0.4.7/forecastmanager/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.140895 forecastmanager-0.4.7/forecastmanager/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.140895 forecastmanager-0.4.7/forecastmanager/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.140895 forecastmanager-0.4.7/forecastmanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/management/commands/generate_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.144895 forecastmanager-0.4.7/forecastmanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0003_alter_forecast_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0006_alter_forecastsetting_enable_auto_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0007_remove_forecastsetting_temp_units_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0008_alter_forecastdataparameters_parameter_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0009_alter_forecastdataparameters_parameter_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0010_alter_forecastdataparameters_parameter_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0011_alter_forecastperiod_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0012_alter_forecastperiod_forecast_effective_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0013_alter_city_options_alter_forecast_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0014_alter_forecastsetting_default_city.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0015_alter_forecast_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0016_alter_cityforecast_options_forecast_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0017_forecastsetting_weather_detail_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0018_delete_dailyweather.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0019_city_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0020_alter_city_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/0021_forecastsetting_weather_reports_page.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.144895 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/css/
--rw-r--r--   0 runner    (1001) docker     (127)    38621 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/css/handsontable.full.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/css/weather-symbol-chooser-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.148895 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/
--rw-r--r--   0 runner    (1001) docker     (127)    67320 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/data-utils.js
--rw-r--r--   0 runner    (1001) docker     (127)    38899 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/forecast_basemap.js
--rw-r--r--   0 runner    (1001) docker     (127)  1828709 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/handsontable.full.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/helpers.js
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.164895 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/
--rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/clearsky_day.png
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/clearsky_night.png
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/clearsky_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/cloudy.png
--rw-r--r--   0 runner    (1001) docker     (127)    14964 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/fair_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/fair_night.png
--rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/fair_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/fog.png
--rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrain.png
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    14261 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleet.png
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    14642 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnow.png
--rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    13940 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrain.png
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    14091 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleet.png
--rw-r--r--   0 runner    (1001) docker     (127)    10860 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnow.png
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    14061 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/partlycloudy_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/partlycloudy_night.png
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/partlycloudy_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rain.png
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowers_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowers_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowers_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13199 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleet.png
--rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowers_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowers_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowers_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    10101 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snow.png
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowers_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowers_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowers_polartwilight.png
--rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_day.png
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_night.png
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_polartwilight.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.132895 forecastmanager-0.4.7/forecastmanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.168895 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/city_index.html
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/create_forecast.html
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/edit_forecast.html
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/file_input_include.html
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/forecast_base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.168895 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/direction.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/droplet-degree.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/droplet-percent.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/moonrise.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/moonset.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/pressure-gauge.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/sunrise.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/sunset.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/temperature-half.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/temperature-high.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/temperature-low.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/umbrella-simple.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/wind-sock.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/wind.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/load_cities.html
--rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/view_forecast.html
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/weather_symbol_chooser_widget.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.168895 forecastmanager-0.4.7/forecastmanager/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/templatetags/forecastmanager_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/forecastmanager/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 13:02:34.172895 forecastmanager-0.4.7/forecastmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-26 13:02:34.000000 forecastmanager-0.4.7/forecastmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-03-26 13:02:34.000000 forecastmanager-0.4.7/forecastmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 13:02:34.000000 forecastmanager-0.4.7/forecastmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-26 13:02:34.000000 forecastmanager-0.4.7/forecastmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-26 13:02:34.000000 forecastmanager-0.4.7/forecastmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-26 13:02:21.000000 forecastmanager-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-26 13:02:34.172895 forecastmanager-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.336740 forecastmanager-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-15 14:39:51.336740 forecastmanager-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.300740 forecastmanager-0.4.8/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/forecast_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.296740 forecastmanager-0.4.8/forecastmanager/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.292740 forecastmanager-0.4.8/forecastmanager/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.300740 forecastmanager-0.4.8/forecastmanager/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15641 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.296740 forecastmanager-0.4.8/forecastmanager/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.300740 forecastmanager-0.4.8/forecastmanager/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.296740 forecastmanager-0.4.8/forecastmanager/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.300740 forecastmanager-0.4.8/forecastmanager/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.296740 forecastmanager-0.4.8/forecastmanager/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.304740 forecastmanager-0.4.8/forecastmanager/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.296740 forecastmanager-0.4.8/forecastmanager/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.304740 forecastmanager-0.4.8/forecastmanager/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.296740 forecastmanager-0.4.8/forecastmanager/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.304740 forecastmanager-0.4.8/forecastmanager/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.304740 forecastmanager-0.4.8/forecastmanager/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.304740 forecastmanager-0.4.8/forecastmanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/management/commands/generate_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.308740 forecastmanager-0.4.8/forecastmanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0003_alter_forecast_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0006_alter_forecastsetting_enable_auto_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0007_remove_forecastsetting_temp_units_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0008_alter_forecastdataparameters_parameter_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0009_alter_forecastdataparameters_parameter_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0010_alter_forecastdataparameters_parameter_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0011_alter_forecastperiod_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0012_alter_forecastperiod_forecast_effective_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0013_alter_city_options_alter_forecast_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0014_alter_forecastsetting_default_city.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0015_alter_forecast_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0016_alter_cityforecast_options_forecast_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0017_forecastsetting_weather_detail_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0018_delete_dailyweather.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0019_city_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0020_alter_city_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0021_forecastsetting_weather_reports_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0022_alter_forecastdataparameters_parameter_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/0023_forecastdataparameters_use_known_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.296740 forecastmanager-0.4.8/forecastmanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.296740 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.308740 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    38621 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/css/handsontable.full.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/css/weather-symbol-chooser-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.312740 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    67320 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/data-utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/forecast-data-parameter-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38899 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/forecast_basemap.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1828709 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/handsontable.full.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/helpers.js
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.328740 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/
+-rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/clearsky_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/clearsky_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/clearsky_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/cloudy.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14964 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/fair_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/fair_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/fair_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/fog.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrain.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14261 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleet.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14642 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13940 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrain.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14091 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleet.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10860 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14061 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/partlycloudy_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/partlycloudy_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/partlycloudy_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rain.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowers_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowers_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowers_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13199 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleet.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowers_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowers_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowers_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10101 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowers_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowers_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowers_polartwilight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_day.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_night.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_polartwilight.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.296740 forecastmanager-0.4.8/forecastmanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.332740 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/city_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/create_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/edit_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/file_input_include.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/forecast_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/forecast_data_parameter_widget.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.332740 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/direction.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/droplet-degree.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/droplet-percent.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/moonrise.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/moonset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/pressure-gauge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/sunrise.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/sunset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/temperature-half.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/temperature-high.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/temperature-low.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/umbrella-simple.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/wind-sock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/wind.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/load_cities.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/view_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/weather_symbol_chooser_widget.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.332740 forecastmanager-0.4.8/forecastmanager/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/templatetags/forecastmanager_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/forecastmanager/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:39:51.332740 forecastmanager-0.4.8/forecastmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-15 14:39:51.000000 forecastmanager-0.4.8/forecastmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-15 14:39:51.000000 forecastmanager-0.4.8/forecastmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:39:51.000000 forecastmanager-0.4.8/forecastmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 14:39:51.000000 forecastmanager-0.4.8/forecastmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 14:39:51.000000 forecastmanager-0.4.8/forecastmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 14:39:47.000000 forecastmanager-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-15 14:39:51.336740 forecastmanager-0.4.8/setup.cfg
```

### Comparing `forecastmanager-0.4.7/PKG-INFO` & `forecastmanager-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.4.7
+Version: 0.4.8
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.4.7/forecastmanager/constants.py` & `forecastmanager-0.4.8/forecastmanager/constants.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/forecast_settings.py` & `forecastmanager-0.4.8/forecastmanager/forecast_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     TabbedInterface,
     ObjectList, InlinePanel,
 )
 from wagtail.contrib.settings.models import BaseSiteSetting
 from wagtail.contrib.settings.registry import register_setting
 from wagtail.models import Orderable
 
-from forecastmanager.constants import WEATHER_PARAMETER_CHOICES, WEATHER_PARAMETERS_AS_DICT
-from forecastmanager.widgets import WeatherSymbolChooserWidget
+from forecastmanager.constants import WEATHER_PARAMETERS_AS_DICT
+from forecastmanager.widgets import WeatherSymbolChooserWidget, DataParameterWidget
 
 
 @register_setting
 class ForecastSetting(ClusterableModel, BaseSiteSetting):
     enable_auto_forecast = models.BooleanField(default=False, verbose_name=_('Enable automated forecasts'))
-    default_city = models.ForeignKey("City", blank=True, null=True, on_delete=models.CASCADE,
+    default_city = models.ForeignKey("City", blank=True, null=True, on_delete=models.SET_NULL,
                                      verbose_name=_("Default City"))
     weather_detail_page = models.ForeignKey("wagtailcore.Page", blank=True, null=True, on_delete=models.SET_NULL, )
     weather_reports_page = models.ForeignKey("wagtailcore.Page", blank=True, null=True, on_delete=models.SET_NULL,
                                              related_name="weather_reports_page")
 
     edit_handler = TabbedInterface([
         ObjectList([
@@ -94,53 +94,53 @@
             ForecastPeriod.objects.filter(default=True).update(default=False)
         super().save(*args, **kwargs)
 
 
 class ForecastDataParameters(Orderable):
     PARAMETER_TYPE_CHOICES = (
         ("numeric", _("Number")),
-        ("time", _("Time")),
         ("text", _("Text")),
     )
     parent = ParentalKey(ForecastSetting, on_delete=models.CASCADE, related_name="data_parameters")
-    parameter = models.CharField(max_length=100, choices=WEATHER_PARAMETER_CHOICES, unique=True,
-                                 verbose_name=_("Parameter"))
+    use_known_parameters = models.BooleanField(default=True, verbose_name=_("Use predefined parameters"))
+    parameter = models.CharField(max_length=100, unique=True, verbose_name=_("Parameter"))
     name = models.CharField(max_length=100, verbose_name=_("Parameter Label"),
                             help_text=_("Parameter name as locally labelled"))
     parameter_type = models.CharField(max_length=100, choices=PARAMETER_TYPE_CHOICES, verbose_name=_("Parameter Type"),
                                       default="numeric")
     parameter_unit = models.CharField(_("Unit of measurement"), max_length=100, null=True, blank=True,
                                       help_text="e.g °C, %, mm, hPa, etc ")
 
     panels = [
-        FieldPanel('parameter'),
+        FieldPanel('use_known_parameters'),
+        FieldPanel('parameter', widget=DataParameterWidget),
         FieldPanel('name'),
+        FieldPanel('parameter_type'),
+        FieldPanel('parameter_unit'),
     ]
 
     def __str__(self):
         return self.name
 
     @property
-    def parameter_info(self):
-        return WEATHER_PARAMETERS_AS_DICT.get(self.parameter)
+    def units(self):
+        if self.parameter_unit:
+            return self.parameter_unit
 
-    def parse_value(self, value):
-        info = self.parameter_info
+        if self.parameter_info:
+            return self.parameter_info.get("units")
 
-        if not info.get("data_type"):
-            return value
+        return None
 
-        try:
-            if info.get("data_type") == "int":
-                return int(float(value))
-            elif info.get("data_type") == "float":
-                return float(value)
-        except ValueError:
-            pass
+    @property
+    def parameter_info(self):
+        return WEATHER_PARAMETERS_AS_DICT.get(self.parameter)
 
+    def parse_value(self, value):
+        # TODO: Implement parsing for different parameter types
         return value
 
 
 class WeatherCondition(Orderable):
     parent = ParentalKey(ForecastSetting, on_delete=models.CASCADE, related_name="weather_conditions")
     symbol = models.CharField(max_length=100, verbose_name=_("Weather Symbol"))
     label = models.CharField(max_length=100, unique=True, verbose_name=_("Label"))
```

### Comparing `forecastmanager-0.4.7/forecastmanager/forms.py` & `forecastmanager-0.4.8/forecastmanager/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,20 +93,21 @@
             params_data = {}
             for key, value in data_dict.items():
                 if key not in ["City", "Condition"]:
                     params_data[key] = value
 
             # check parameters
             for param, value in params_data.items():
-                param = ForecastDataParameters.objects.filter(name=param).first()
-                if not param:
-                    self.add_error(None, f"Unknown parameter found in table data: {param}")
-                    return cleaned_data
+                if value:
+                    param = ForecastDataParameters.objects.filter(name=param).first()
+                    if not param:
+                        self.add_error(None, f"Unknown parameter found in table data: {param}")
+                        return cleaned_data
 
-                city_data["data_values"].append({"parameter": param, "value": value})
+                    city_data["data_values"].append({"parameter": param, "value": value})
 
             forecast_data.append(city_data)
             added_cities.append(city.id)
 
         cleaned_data["data"] = forecast_data
         return cleaned_data
```

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/am/LC_MESSAGES/django.mo` & `forecastmanager-0.4.8/forecastmanager/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/am/LC_MESSAGES/django.po` & `forecastmanager-0.4.8/forecastmanager/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/ar/LC_MESSAGES/django.mo` & `forecastmanager-0.4.8/forecastmanager/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/ar/LC_MESSAGES/django.po` & `forecastmanager-0.4.8/forecastmanager/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/en/LC_MESSAGES/django.mo` & `forecastmanager-0.4.8/forecastmanager/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/en/LC_MESSAGES/django.po` & `forecastmanager-0.4.8/forecastmanager/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/es/LC_MESSAGES/django.mo` & `forecastmanager-0.4.8/forecastmanager/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/es/LC_MESSAGES/django.po` & `forecastmanager-0.4.8/forecastmanager/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/fr/LC_MESSAGES/django.mo` & `forecastmanager-0.4.8/forecastmanager/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/fr/LC_MESSAGES/django.po` & `forecastmanager-0.4.8/forecastmanager/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/sw/LC_MESSAGES/django.mo` & `forecastmanager-0.4.8/forecastmanager/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/locale/sw/LC_MESSAGES/django.po` & `forecastmanager-0.4.8/forecastmanager/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/management/commands/generate_forecast.py` & `forecastmanager-0.4.8/forecastmanager/management/commands/generate_forecast.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0001_initial.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0007_remove_forecastsetting_temp_units_and_more.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0007_remove_forecastsetting_temp_units_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0008_alter_forecastdataparameters_parameter_unit.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0008_alter_forecastdataparameters_parameter_unit.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0009_alter_forecastdataparameters_parameter_unit.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0009_alter_forecastdataparameters_parameter_unit.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0010_alter_forecastdataparameters_parameter_type_and_more.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0010_alter_forecastdataparameters_parameter_type_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0011_alter_forecastperiod_options_and_more.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0011_alter_forecastperiod_options_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0013_alter_city_options_alter_forecast_unique_together_and_more.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0013_alter_city_options_alter_forecast_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0014_alter_forecastsetting_default_city.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0014_alter_forecastsetting_default_city.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0015_alter_forecast_options_and_more.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0015_alter_forecast_options_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0016_alter_cityforecast_options_forecast_source.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0016_alter_cityforecast_options_forecast_source.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0017_forecastsetting_weather_detail_page.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0017_forecastsetting_weather_detail_page.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0019_city_slug.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0019_city_slug.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/migrations/0021_forecastsetting_weather_reports_page.py` & `forecastmanager-0.4.8/forecastmanager/migrations/0021_forecastsetting_weather_reports_page.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/models.py` & `forecastmanager-0.4.8/forecastmanager/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     effective_period = models.ForeignKey(ForecastPeriod, on_delete=models.PROTECT, null=True)
     source = models.CharField(max_length=100, choices=FORECAST_SOURCE_CHOICES, default="local")
 
     class Meta:
         unique_together = ("forecast_date", "effective_period")
         verbose_name = _("Forecast")
         verbose_name_plural = _("Forecasts")
-        ordering = ["forecast_date", "effective_period"]
+        ordering = ["-forecast_date", "effective_period"]
 
     panels = [
         FieldPanel("forecast_date"),
         FieldPanel("effective_period"),
         FieldPanel("replace_existing"),
         # InlinePanel("city_forecasts", label=_("City Forecast Data")),
     ]
@@ -122,23 +122,30 @@
     def effective_period(self):
         return self.parent.effective_period
 
     @property
     def data_values_dict(self):
         data_values = {}
         for data_value in self.data_values.all():
-            data_values[data_value.parameter.parameter] = {
+            parameter_info = data_value.parameter.parameter_info
+            val = {
                 "value": data_value.parsed_value,
                 "name": data_value.parameter.name,
-                "label": data_value.parameter.parameter_info.get("label"),
-                "units": data_value.parameter.parameter_info.get("unit"),
+                "label": data_value.parameter.name,
+                "units": data_value.parameter.units,
                 "value_with_units": data_value.value_with_units,
-                "icon": data_value.parameter.parameter_info.get("icon"),
             }
 
+            if parameter_info:
+                val.update({
+                    "icon": data_value.parameter.parameter_info.get("icon"),
+                })
+
+            data_values[data_value.parameter.parameter] = val
+
         # Group temperature values
         temperature = {}
         if "air_temperature_max" in data_values:
             temperature["max_temp"] = data_values.get("air_temperature_max")
             # remove air_temperature_max from data_values
             data_values.pop("air_temperature_max")
 
@@ -197,8 +204,14 @@
 
     @property
     def parsed_value(self):
         return self.parameter.parse_value(self.value)
 
     @property
     def value_with_units(self):
-        return f"{self.parsed_value}{self.parameter.parameter_info.get('unit')}"
+        if not self.parsed_value:
+            return None
+
+        if not self.parameter.units:
+            return self.parsed_value
+
+        return f"{self.parsed_value} {self.parameter.units}"
```

### Comparing `forecastmanager-0.4.7/forecastmanager/serializers.py` & `forecastmanager-0.4.8/forecastmanager/serializers.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/css/handsontable.full.min.css` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/css/handsontable.full.min.css`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/css/weather-symbol-chooser-widget.css` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/css/weather-symbol-chooser-widget.css`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/data-utils.js` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/data-utils.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/forecast_basemap.js` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/forecast_basemap.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/handsontable.full.min.js` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/handsontable.full.min.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/helpers.js` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/helpers.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget-telepath.js` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget.js` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/clearsky_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/clearsky_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/clearsky_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/clearsky_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/clearsky_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/clearsky_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/cloudy.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/cloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/fair_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/fair_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/fair_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/fair_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/fair_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/fair_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/fog.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/fog.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrain.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainandthunder.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowers_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavyrainshowersandthunder_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleet.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetandthunder.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowers_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysleetshowersandthunder_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnow.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowandthunder.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowers_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/heavysnowshowersandthunder_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrain.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainandthunder.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowers_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightrainshowersandthunder_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleet.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetandthunder.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowers_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsleetshowersandthunder_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnow.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowandthunder.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowers_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/lightsnowshowersandthunder_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/partlycloudy_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/partlycloudy_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/partlycloudy_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/partlycloudy_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/partlycloudy_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/partlycloudy_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rain.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainandthunder.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowers_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowers_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowers_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowers_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowers_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowers_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/rainshowersandthunder_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleet.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetandthunder.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowers_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowers_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowers_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowers_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowers_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowers_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/sleetshowersandthunder_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snow.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowandthunder.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowers_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowers_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowers_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowers_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowers_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowers_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_day.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_day.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_night.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_night.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_polartwilight.png` & `forecastmanager-0.4.8/forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_polartwilight.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/city_index.html` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/city_index.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/create_forecast.html` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/create_forecast.html`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                         type: 'dropdown',
                         source: cities.map(city => city.name),
                         allowEmpty: false,
                         allowInvalid: false,
                     },
                     ...this.parameters.map((p) => ({
                         type: p.parameter_type,
-                        allowEmpty: false,
+                        allowEmpty: true,
                         allowInvalid: false,
                     })),
                     {
                         type: 'dropdown',
                         source: weatherConditions,
                         allowEmpty: false,
                         allowInvalid: false,
```

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/edit_forecast.html` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/edit_forecast.html`

 * *Files 0% similar despite different names*

```diff
@@ -44,19 +44,21 @@
                                 <h2>{{ city_forecast.city.name }}</h2>
                             </td>
                             <td class="weather-condition">
                                 <img style="height: 70px;width: 70px" src="{{ city_forecast.condition.icon_url }}"
                                      alt="">
                             </td>
                             {% for param in weather_parameters %}
-                                {% for data in city_forecast.data_values.all %}
-                                    {% if data.parameter.parameter == param.parameter %}
-                                        <td>{{ data.value_with_units }}</td>
-                                    {% endif %}
-                                {% endfor %}
+                                <td>
+                                    {% for data in city_forecast.data_values.all %}
+                                        {% if data.parameter.parameter == param.parameter %}
+                                            {{ data.value_with_units }}
+                                        {% endif %}
+                                    {% endfor %}
+                                </td>
                             {% endfor %}
                         </tr>
                     {% endfor %}
                     </tbody>
                 </table>
             </div>
         </div>
```

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/file_input_include.html` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/file_input_include.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/forecast_base.html` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/forecast_base.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/direction.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/direction.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/droplet-degree.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/droplet-degree.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/droplet-percent.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/droplet-percent.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/moonrise.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/moonrise.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/moonset.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/moonset.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/pressure-gauge.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/pressure-gauge.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/sunrise.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/sunset.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/temperature-half.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/temperature-half.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/temperature-high.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/temperature-high.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/temperature-low.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/temperature-low.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/umbrella-simple.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/umbrella-simple.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/wind-sock.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/wind-sock.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/icons/wind.svg` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/icons/wind.svg`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/load_cities.html` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/load_cities.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/view_forecast.html` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/view_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/templates/forecastmanager/weather_symbol_chooser_widget.html` & `forecastmanager-0.4.8/forecastmanager/templates/forecastmanager/weather_symbol_chooser_widget.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/urls.py` & `forecastmanager-0.4.8/forecastmanager/urls.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/views.py` & `forecastmanager-0.4.8/forecastmanager/views.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/wagtail_hooks.py` & `forecastmanager-0.4.8/forecastmanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.4.7/forecastmanager/widgets.py` & `forecastmanager-0.4.8/forecastmanager/widgets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 
-from django.forms import widgets
+from django.forms import widgets, TextInput
 from django.templatetags.static import static
 from wagtail.telepath import register
 from wagtail.utils.widgets import WidgetWithScript
 from wagtail.widget_adapters import WidgetAdapter
 
-from forecastmanager.constants import WEATHER_CONDITION_ICONS
+from forecastmanager.constants import WEATHER_CONDITION_ICONS, WEATHER_PARAMETER_CHOICES
 
 
 class WeatherSymbolChooserWidget(WidgetWithScript, widgets.TextInput):
     template_name = "forecastmanager/weather_symbol_chooser_widget.html"
 
     def __init__(self, attrs=None):
         default_attrs = {
@@ -48,7 +48,44 @@
     class Media:
         js = [
             "forecastmanager/js/weather-symbol-chooser-widget-telepath.js",
         ]
 
 
 register(WeatherSymbolWidgetAdapter(), WeatherSymbolChooserWidget)
+
+
+class DataParameterWidget(WidgetWithScript, TextInput):
+    template_name = "forecastmanager/forecast_data_parameter_widget.html"
+
+    def __init__(self, attrs=None, **kwargs):
+        default_attrs = {}
+
+        if attrs:
+            default_attrs.update(attrs)
+
+        super().__init__(default_attrs)
+
+    def get_context(self, name, value, attrs):
+        context = super().get_context(name, value, attrs)
+
+        options = []
+
+        for choice in WEATHER_PARAMETER_CHOICES:
+            options.append({
+                "value": choice[0],
+                "label": choice[1],
+            })
+
+        context["widget"].update({
+            "parameter_list": options
+        })
+
+        return context
+
+    def render_js_init(self, id_, name, value):
+        return "new DataParameterWidget({0},{1});".format(json.dumps(id_), json.dumps(value))
+
+    class Media:
+        js = [
+            "forecastmanager/js/forecast-data-parameter-widget.js",
+        ]
```

### Comparing `forecastmanager-0.4.7/forecastmanager.egg-info/PKG-INFO` & `forecastmanager-0.4.8/forecastmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.4.7
+Version: 0.4.8
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.4.7/forecastmanager.egg-info/SOURCES.txt` & `forecastmanager-0.4.8/forecastmanager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,21 @@
 forecastmanager/migrations/0015_alter_forecast_options_and_more.py
 forecastmanager/migrations/0016_alter_cityforecast_options_forecast_source.py
 forecastmanager/migrations/0017_forecastsetting_weather_detail_page.py
 forecastmanager/migrations/0018_delete_dailyweather.py
 forecastmanager/migrations/0019_city_slug.py
 forecastmanager/migrations/0020_alter_city_slug.py
 forecastmanager/migrations/0021_forecastsetting_weather_reports_page.py
+forecastmanager/migrations/0022_alter_forecastdataparameters_parameter_type_and_more.py
+forecastmanager/migrations/0023_forecastdataparameters_use_known_parameters.py
 forecastmanager/migrations/__init__.py
 forecastmanager/static/forecastmanager/css/handsontable.full.min.css
 forecastmanager/static/forecastmanager/css/weather-symbol-chooser-widget.css
 forecastmanager/static/forecastmanager/js/data-utils.js
+forecastmanager/static/forecastmanager/js/forecast-data-parameter-widget.js
 forecastmanager/static/forecastmanager/js/forecast_basemap.js
 forecastmanager/static/forecastmanager/js/handsontable.full.min.js
 forecastmanager/static/forecastmanager/js/helpers.js
 forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget-telepath.js
 forecastmanager/static/forecastmanager/js/weather-symbol-chooser-widget.js
 forecastmanager/static/forecastmanager/weathericons/clearsky_day.png
 forecastmanager/static/forecastmanager/weathericons/clearsky_night.png
@@ -150,14 +153,15 @@
 forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_night.png
 forecastmanager/static/forecastmanager/weathericons/snowshowersandthunder_polartwilight.png
 forecastmanager/templates/forecastmanager/city_index.html
 forecastmanager/templates/forecastmanager/create_forecast.html
 forecastmanager/templates/forecastmanager/edit_forecast.html
 forecastmanager/templates/forecastmanager/file_input_include.html
 forecastmanager/templates/forecastmanager/forecast_base.html
+forecastmanager/templates/forecastmanager/forecast_data_parameter_widget.html
 forecastmanager/templates/forecastmanager/load_cities.html
 forecastmanager/templates/forecastmanager/view_forecast.html
 forecastmanager/templates/forecastmanager/weather_symbol_chooser_widget.html
 forecastmanager/templates/forecastmanager/icons/direction.svg
 forecastmanager/templates/forecastmanager/icons/droplet-degree.svg
 forecastmanager/templates/forecastmanager/icons/droplet-percent.svg
 forecastmanager/templates/forecastmanager/icons/moonrise.svg
```

### Comparing `forecastmanager-0.4.7/setup.cfg` & `forecastmanager-0.4.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastmanager
-version = 0.4.7
+version = 0.4.8
 description = Integration of Weather City Forecasts Manager in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/forecastmanager
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
```

