# Comparing `tmp/red_web_dashboard-1.1.tar.gz` & `tmp/red_web_dashboard-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red_web_dashboard-1.1.tar", last modified: Fri Apr 12 18:11:14 2024, max compression
+gzip compressed data, was "red_web_dashboard-1.2.0.tar", last modified: Sun Apr 14 22:44:29 2024, max compression
```

## Comparing `red_web_dashboard-1.1.tar` & `red_web_dashboard-1.2.0.tar`

### file list

```diff
@@ -1,293 +1,293 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.853525 red_web_dashboard-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-12 18:11:14.853525 red_web_dashboard-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 18:11:14.000000 red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.797523 red_web_dashboard-1.1/reddash/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.797523 red_web_dashboard-1.1/reddash/app/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.797523 red_web_dashboard-1.1/reddash/app/base/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35780 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/base/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.797523 red_web_dashboard-1.1/reddash/app/login/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/login/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.789523 red_web_dashboard-1.1/reddash/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.805523 red_web_dashboard-1.1/reddash/app/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/biometric-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.809523 red_web_dashboard-1.1/reddash/app/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)   480516 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/nucleo-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/nucleo-svg.css
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/css/simplemde.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/error-403.gif
--rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/error-404.gif
--rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/error-500.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.809523 red_web_dashboard-1.1/reddash/app/static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.eot
--rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/icon-documentation.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.809523 red_web_dashboard-1.1/reddash/app/static/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    27282 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/argon-dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/argon-dashboard.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.813524 red_web_dashboard-1.1/reddash/app/static/assets/js/core/
--rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/core/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/core/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/core/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.813524 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/Chart.extension.js
--rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/chartjs.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/oauth.png
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/random.svg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.813524 red_web_dashboard-1.1/reddash/app/static/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.821524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.829524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.829524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.829524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/custom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.837525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.793523 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.841524 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/tasks_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/blacklisted.html
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/errors/custom.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/fixed-plugin.html
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/scripts.html
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/includes/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.845525 red_web_dashboard-1.1/reddash/app/templates/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/layouts/base-fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/layouts/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/reddash/app/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    28559 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/admin.html
--rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/commands.html
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/credits.html
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/dashboard_guild.html
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/guild_profile.html
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/reddash/app/templates/pages/login/
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/login/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/oauth.html
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/third_parties.html
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/third_parties_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/third_party.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:14.849525 red_web_dashboard-1.1/reddash/app/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/third_parties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8892 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/third_parties/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    27177 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/reddash/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-12 18:11:14.853525 red_web_dashboard-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 18:11:10.000000 red_web_dashboard-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 22:44:29.000000 red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.722575 red_web_dashboard-1.2.0/reddash/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.726575 red_web_dashboard-1.2.0/reddash/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.726575 red_web_dashboard-1.2.0/reddash/app/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42435 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/base/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.726575 red_web_dashboard-1.2.0/reddash/app/login/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/login/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.718575 red_web_dashboard-1.2.0/reddash/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.730575 red_web_dashboard-1.2.0/reddash/app/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/biometric-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.734575 red_web_dashboard-1.2.0/reddash/app/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   480516 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/nucleo-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/nucleo-svg.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/css/simplemde.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/error-403.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/error-404.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/error-500.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.734575 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/icon-documentation.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.734575 red_web_dashboard-1.2.0/reddash/app/static/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    27200 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/argon-dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/argon-dashboard.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.734575 red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.738575 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/Chart.extension.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/chartjs.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/oauth.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/random.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.738575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.742575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.750575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.750575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.754575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.758575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.722575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.762575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/tasks_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/blacklisted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/errors/custom.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/fixed-plugin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/includes/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/layouts/base-fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/layouts/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    28545 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/commands.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/credits.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)    30505 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/dashboard_guild.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/guild_profile.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.766575 red_web_dashboard-1.2.0/reddash/app/templates/pages/login/
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/login/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/oauth.html
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_parties.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_parties_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_party.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/reddash/app/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/third_parties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8892 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/third_parties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27213 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/reddash/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-14 22:44:29.770575 red_web_dashboard-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-14 22:44:22.000000 red_web_dashboard-1.2.0/setup.py
```

### Comparing `red_web_dashboard-1.1/LICENSE` & `red_web_dashboard-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/PKG-INFO` & `red_web_dashboard-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.1.0
+Version: 1.2.0
 Summary: An easy-to-use interactive web dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.1/README.md` & `red_web_dashboard-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/PKG-INFO` & `red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.1.0
+Version: 1.2.0
 Summary: An easy-to-use interactive web dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.1/Red_Web_Dashboard.egg-info/SOURCES.txt` & `red_web_dashboard-1.2.0/Red_Web_Dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/pyproject.toml` & `red_web_dashboard-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/__main__.py` & `red_web_dashboard-1.2.0/reddash/__main__.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/app.py` & `red_web_dashboard-1.2.0/reddash/app/app.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/base/routes.py` & `red_web_dashboard-1.2.0/reddash/app/base/routes.py`

 * *Files 10% similar despite different names*

```diff
@@ -263,15 +263,15 @@
     return {"guild": guild, "leave_guild_form": leave_guild_form}
 
 
 class PrefixesCheck:
     def __call__(self, form: FlaskForm, field: wtforms.Field) -> None:
         if field.data == field.default:
             return
-        for prefix in field.data.split(";;;;;"):
+        for prefix in field.data.split(";;|;;"):
             if (
                 not app.variables["constants"]["MIN_PREFIX_LENGTH"]
                 <= len(prefix)
                 <= app.variables["constants"]["MAX_PREFIX_LENGTH"]
             ):
                 raise wtforms.validators.ValidationError(
                     _(
@@ -314,24 +314,24 @@
 class GuildSettingsForm(FlaskForm):
     def __init__(self, guild: typing.Dict[str, typing.Any]) -> None:
         super().__init__(prefix="guild_settings_form_")
         if not guild["settings"]["edit_permission"]:
             for field in self:
                 field.render_kw = {"disabled": True}
         self.bot_nickname.default = guild["settings"]["bot_nickname"]
-        self.prefixes.default = ";;;;;".join(guild["settings"]["prefixes"])
+        self.prefixes.default = ";;|;;".join(guild["settings"]["prefixes"])
         self.admin_roles.choices = [
             (str(role["id"]), f"{role['name']} ({role['id']})") for role in guild["roles"][1:]
         ]
         self.admin_roles.default = [str(role["id"]) for role in guild["settings"]["admin_roles"]]
         self.mod_roles.choices = [
             (str(role["id"]), f"{role['name']} ({role['id']})") for role in guild["roles"][1:]
         ]
         self.mod_roles.default = [str(role["id"]) for role in guild["settings"]["mod_roles"]]
-        self.ignored.default = guild["settings"]["ignored"]
+        self.ignored.default = self.ignored.checked = guild["settings"]["ignored"]
         available_commands = []
         all_commands = deepcopy(app.variables["commands"])
         for cog_data in all_commands.values():
             for command in cog_data["commands"]:
                 if command["privilege_level"] == "BOT_OWNER" or command["name"] == "command":
                     continue
                 available_commands.append((command["name"], command["name"]))
@@ -345,26 +345,26 @@
                         if sub["subs"]:
                             check_subs(sub["subs"])
                     return _subs
 
                 check_subs(command["subs"])
         self.disabled_commands.choices = sorted(available_commands)
         self.disabled_commands.default = guild["settings"]["disabled_commands"].copy()
-        self.embeds.default = guild["settings"]["embeds"]
-        self.use_bot_color.default = guild["settings"]["use_bot_color"]
-        self.fuzzy.default = guild["settings"]["fuzzy"]
+        self.embeds.default = self.embeds.checked = guild["settings"]["embeds"]
+        self.use_bot_color.default = self.use_bot_color.checked = guild["settings"]["use_bot_color"]
+        self.fuzzy.default = self.fuzzy.checked = guild["settings"]["fuzzy"]
         self.delete_delay.default = guild["settings"]["delete_delay"]
         self.locale.default = guild["settings"]["locale"]
         self.regional_format.default = guild["settings"]["regional_format"]
 
     bot_nickname: wtforms.StringField = wtforms.StringField(
         _("Bot Nickname"), validators=[wtforms.validators.Length(max=32)]
     )
     prefixes: wtforms.StringField = wtforms.StringField(
-        _("Prefixes"), validators=[PrefixesCheck()]
+        _("Prefixes"), validators=[wtforms.validators.Optional(), PrefixesCheck()]
     )
     admin_roles: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
         _("Admin Roles"), choices=[]
     )
     mod_roles: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
         _("Mod Roles"), choices=[]
     )
@@ -387,14 +387,81 @@
     )
     regional_format: wtforms.StringField = wtforms.StringField(
         _("Region"), validators=[wtforms.validators.Optional(), BabelCheck(check_reset=True)]
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
 
+class MarkdownTextAreaField(wtforms.TextAreaField):
+    def __call__(
+        self,
+        auto_save: bool = False,
+        max_height: bool = False,
+        disable_toolbar: bool = False,
+        **kwargs,
+    ) -> Markup:
+        if "class" not in kwargs:
+            kwargs["class"] = "markdown-text-area-field"
+        else:
+            kwargs["class"] += " markdown-text-area-field"
+        if auto_save:
+            kwargs["class"] += " markdown-text-area-field-autosave"
+        if max_height:
+            kwargs["class"] += " markdown-text-area-field-max-height"
+        if disable_toolbar:
+            kwargs["class"] += " markdown-text-area-field-toolbar-disabled"
+        return super().__call__(**kwargs)
+
+
+class AliasForm(FlaskForm):
+    alias_name: wtforms.StringField = wtforms.StringField(_("Name"), validators=[wtforms.validators.DataRequired(), wtforms.validators.Regexp(r"^[^\s]+$"), wtforms.validators.Length(max=300)])
+    command: MarkdownTextAreaField = MarkdownTextAreaField(_("Command"), validators=[wtforms.validators.DataRequired(), wtforms.validators.Length(max=1700)])
+
+
+class AliasesForm(FlaskForm):
+    def __init__(self, aliases: typing.Dict[str, str]) -> None:
+        super().__init__(prefix="aliases_form_")
+        for name, command in aliases.items():
+            self.aliases.append_entry({"alias_name": name, "command": command})
+        self.aliases.default = [entry for entry in self.aliases.entries if entry.csrf_token.data is None]
+        self.aliases.entries = [entry for entry in self.aliases.entries if entry.csrf_token.data is not None]
+
+    aliases: wtforms.FieldList = wtforms.FieldList(wtforms.FormField(AliasForm))
+    submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
+
+
+class CustomCommandResponseForm(FlaskForm):
+    response: MarkdownTextAreaField = MarkdownTextAreaField(_("Response"), validators=[wtforms.validators.DataRequired(), wtforms.validators.Length(max=2000)])
+
+
+class CustomCommandForm(FlaskForm):
+    def __init__(self, *args, **kwargs) -> None:
+        responses = kwargs.pop("responses", {})
+        super().__init__(*args, **kwargs)
+        for response in responses:
+            self.responses.append_entry({"response": response})
+        self.responses.default = [entry for entry in self.responses.entries if entry.response.data and entry.csrf_token.data is None]
+        self.responses.entries = [entry for entry in self.responses.entries if not entry.response.data or entry.csrf_token.data is not None]
+
+    command: wtforms.StringField = wtforms.StringField(_("Name"), validators=[wtforms.validators.DataRequired(), wtforms.validators.Regexp(r"^[^\sA-Z]+$"), wtforms.validators.Length(max=300)])
+    responses: wtforms.FieldList = wtforms.FieldList(wtforms.FormField(CustomCommandResponseForm), _("Responses"), min_entries=1)
+
+
+class CustomCommandsForm(FlaskForm):
+    def __init__(self, custom_commands: typing.Dict[str, typing.List[str]]) -> None:
+        super().__init__(prefix="custom_commands_form_")
+        for command, responses in custom_commands.items():
+            self.custom_commands.append_entry({"command": command, "responses": [responses] if isinstance(responses, str) else responses})
+        self.custom_commands.default = [entry for entry in self.custom_commands.entries if entry.csrf_token.data is None]
+        self.custom_commands.entries = [entry for entry in self.custom_commands.entries if entry.csrf_token.data is not None]
+
+    custom_commands: wtforms.FieldList = wtforms.FieldList(wtforms.FormField(CustomCommandForm))
+    submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
+
+
 @blueprint.route("/dashboard/<guild_id>/<page>/<third_party>", methods=("GET", "POST"))
 @blueprint.route("/dashboard/<guild_id>/<page>", methods=("GET", "POST"))
 @blueprint.route("/dashboard/<guild_id>", methods=("GET", "POST"))
 @login_required
 async def dashboard_guild(
     guild_id: str,
     page: typing.Optional[typing.Literal["overview", "settings", "third-parties"]] = None,
@@ -404,29 +471,102 @@
         guild_id = int(guild_id)
     except ValueError:
         return abort(404, description=_("Guild ID must be an integer."))
     return_guild = await get_guild(guild_id)
     if return_guild["guild"]["status"] == 1:
         return return_guild["guild"]
 
+    requeststr = {
+        "jsonrpc": "2.0",
+        "id": 0,
+        "method": "DASHBOARDRPC_DEFAULTCOGS__GET_ALIASES",
+        "params": [current_user.id, guild_id],
+    }
+    aliases = await get_result(app, requeststr)
+    if aliases["status"] == 0:
+        aliases_form: AliasesForm = AliasesForm(aliases=aliases["aliases"])
+        if aliases_form.validate_on_submit():
+            requeststr = {
+                "jsonrpc": "2.0",
+                "id": 0,
+                "method": "DASHBOARDRPC_DEFAULTCOGS__SET_ALIASES",
+                "params": [
+                    current_user.id,
+                    guild_id,
+                    {
+                        alias["alias_name"]: alias["command"]
+                        for alias in aliases_form.aliases.data
+                    },
+                ],
+            }
+            result = await get_result(app, requeststr)
+            if result["status"] == 0:
+                flash(_("Successfully saved the modifications."), category="success")
+            else:
+                for error in result["errors"]:
+                    flash(error, category="warning")
+                flash(_("Failed to save the modifications."), category="danger")
+            return redirect(request.url)
+        elif aliases_form.submit.data and aliases_form.errors:
+            for field_name, error_messages in aliases_form.errors.items():
+                if isinstance(error_messages[0], typing.Dict):
+                    for sub_field_name, sub_error_messages in error_messages[0].items():
+                        flash(f"{field_name}-{sub_field_name}: {' '.join(sub_error_messages)}", category="warning")
+                    continue
+                flash(f"{field_name}: {' '.join(error_messages)}", category="warning")
+    else:
+        aliases_form = None
+
+    requeststr = {
+        "jsonrpc": "2.0",
+        "id": 0,
+        "method": "DASHBOARDRPC_DEFAULTCOGS__GET_CUSTOM_COMMANDS",
+        "params": [current_user.id, guild_id],
+    }
+    custom_commands = await get_result(app, requeststr)
+    if custom_commands["status"] == 0:
+        custom_commands_form: CustomCommandsForm = CustomCommandsForm(custom_commands=custom_commands["custom_commands"])
+        if custom_commands_form.validate_on_submit():
+            requeststr = {
+                "jsonrpc": "2.0",
+                "id": 0,
+                "method": "DASHBOARDRPC_DEFAULTCOGS__SET_CUSTOM_COMMANDS",
+                "params": [
+                    current_user.id,
+                    guild_id,
+                    {
+                        custom_command["command"]: (custom_command["responses"][0]["response"] if len(custom_command["responses"]) == 1 else [response["response"] for response in custom_command["responses"]])
+                        for custom_command in custom_commands_form.custom_commands.data
+                    },
+                ],
+            }
+            result = await get_result(app, requeststr)
+            if result["status"] == 0:
+                flash(_("Successfully saved the modifications."), category="success")
+            else:
+                for error in result["errors"]:
+                    flash(error, category="warning")
+                flash(_("Failed to save the modifications."), category="danger")
+            return redirect(request.url)
+
     guild_settings_form: GuildSettingsForm = GuildSettingsForm(guild=return_guild["guild"])
     if (
         guild_settings_form.validate_on_submit()
         and return_guild["guild"]["settings"]["edit_permission"]
     ):
         requeststr = {
             "jsonrpc": "2.0",
             "id": 0,
             "method": "DASHBOARDRPC__SET_GUILD_SETTINGS",
             "params": [
                 current_user.id,
                 guild_id,
                 {
                     "bot_nickname": guild_settings_form.bot_nickname.data.strip() or None,
-                    "prefixes": guild_settings_form.prefixes.data.split(";;;;;"),
+                    "prefixes": (prefixes if (prefixes := guild_settings_form.prefixes.data.split(";;|;;")) != [""] else []),
                     "admin_roles": guild_settings_form.admin_roles.data,
                     "mod_roles": guild_settings_form.mod_roles.data,
                     "ignored": guild_settings_form.ignored.data,
                     "disabled_commands": guild_settings_form.disabled_commands.data,
                     "embeds": guild_settings_form.embeds.data,
                     "use_bot_color": guild_settings_form.use_bot_color.data,
                     "fuzzy": guild_settings_form.fuzzy.data,
@@ -439,15 +579,15 @@
         result = await get_result(app, requeststr)
         if result["status"] == 0:
             if result.get("change_nickname_error"):
                 flash(
                     _(
                         "Failed to change the bot's nickname. Make sure the bot has the required permissions."
                     ),
-                    category="danger",
+                    category="warning",
                 )
             flash(_("Successfully saved the modifications."), category="success")
         else:
             flash(_("Failed to save the modifications."), category="danger")
         return redirect(request.url)
     elif guild_settings_form.submit.data and guild_settings_form.errors:
         for field_name, error_messages in guild_settings_form.errors.items():
@@ -457,14 +597,16 @@
 
     return render_template(
         "pages/dashboard_guild.html",
         **return_guild,
         page=page
         if page is not None and page in ("overview", "settings", "third-parties")
         else "overview",
+        aliases_form=aliases_form,
+        custom_commands_form=custom_commands_form,
         guild_settings_form=guild_settings_form,
         **return_third_parties,
         tab_name=None
         if third_party is None or third_party not in return_third_parties["third_parties"]
         else third_party,
     )
 
@@ -520,35 +662,14 @@
     def __init__(self) -> None:
         super().__init__(prefix="dashboard_actions_form_")
 
     lock: wtforms.SubmitField = wtforms.SubmitField(_("Lock Dashboard"))
     refresh_sessions: wtforms.SubmitField = wtforms.SubmitField(_("Refresh Sessions"))
 
 
-class MarkdownTextAreaField(wtforms.TextAreaField):
-    def __call__(
-        self,
-        auto_save: bool = False,
-        max_height: bool = False,
-        disable_toolbar: bool = False,
-        **kwargs,
-    ) -> Markup:
-        if "class" not in kwargs:
-            kwargs["class"] = "markdown-text-area-field"
-        else:
-            kwargs["class"] += " markdown-text-area-field"
-        if auto_save:
-            kwargs["class"] += " markdown-text-area-field-autosave"
-        if max_height:
-            kwargs["class"] += " markdown-text-area-field-max-height"
-        if disable_toolbar:
-            kwargs["class"] += " markdown-text-area-field-toolbar-disabled"
-        return super().__call__(**kwargs)
-
-
 class DiscordProfileForm(FlaskForm):
     def __init__(self) -> None:
         super().__init__(prefix="bot_profile_form_")
         self.username.default = app.variables["bot"]["name"]
         self.description.default = app.variables["bot"]["profile_description"]
 
     avatar: FileField = FileField(_("Avatar"))
@@ -578,15 +699,15 @@
         ]
         self.disabled_third_parties.default = settings["disabled_third_parties"].copy()
 
     title: wtforms.StringField = wtforms.StringField(_("Title"))
     icon: wtforms.StringField = wtforms.StringField(_("Icon"))
     website_description: wtforms.StringField = wtforms.StringField(_("Website Short Description"))
     description: MarkdownTextAreaField = MarkdownTextAreaField(_("Description"))
-    support_server: wtforms.StringField = wtforms.StringField(_("Support Server"))
+    support_server: wtforms.URLField = wtforms.URLField(_("Support Server"))
     default_color: wtforms.SelectField = wtforms.SelectField(
         _("Default Color"),
         choices=[(color, color.capitalize()) for color in AVAILABLE_COLORS],
         validators=[wtforms.validators.DataRequired()],
     )
     default_background_theme: wtforms.SelectField = wtforms.SelectField(
         _("Default Background Theme"),
@@ -603,15 +724,15 @@
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
 
 class BotSettingsForm(FlaskForm):
     def __init__(self, settings: typing.Dict[str, typing.Any]) -> None:
         super().__init__(prefix="bot_settings_form_")
-        self.prefixes.default = ";;;;;".join(settings["prefixes"])
+        self.prefixes.default = ";;|;;".join(settings["prefixes"])
         self.invoke_error_msg.default = settings["invoke_error_msg"]
         available_commands = []
         all_commands = deepcopy(app.variables["commands"])
         for cog_data in all_commands.values():
             for command in cog_data["commands"]:
                 if command["privilege_level"] == "BOT_OWNER" or command["name"] == "command":
                     continue
@@ -629,20 +750,20 @@
 
                 check_subs(command["subs"])
         self.disabled_commands.choices = sorted(available_commands)
         self.disabled_commands.default = settings["disabled_commands"].copy()
         self.disabled_command_msg.default = settings["disabled_command_msg"]
         self.description.default = settings["description"]
         self.custom_info.default = settings["custom_info"]
-        self.embeds.default = settings["embeds"]
+        self.embeds.default = self.embeds.checked = settings["embeds"]
         self.color.default = settings["color"]
-        self.fuzzy.default = settings["fuzzy"]
-        self.use_buttons.default = settings["use_buttons"]
-        self.invite_public.default = settings["invite_public"]
-        self.invite_commands_scope.default = settings["invite_commands_scope"]
+        self.fuzzy.default = self.fuzzy.checked = settings["fuzzy"]
+        self.use_buttons.default = self.use_buttons.checked = settings["use_buttons"]
+        self.invite_public.default = self.invite_public.checked = settings["invite_public"]
+        self.invite_commands_scope.default = self.invite_commands_scope.checked = settings["invite_commands_scope"]
         self.invite_perms.validators.append(wtforms.validators.NumberRange(min=0, max=app.variables["constants"]["MAX_DISCORD_PERMISSIONS_VALUE"]))
         self.invite_perms.default = settings["invite_perms"]
         self.locale.default = settings["locale"]
         self.regional_format.default = settings["regional_format"]
 
     prefixes: wtforms.StringField = wtforms.StringField(
         _("Prefixes"), validators=[wtforms.validators.DataRequired(), PrefixesCheck()]
@@ -804,15 +925,15 @@
         requeststr = {
             "jsonrpc": "2.0",
             "id": 0,
             "method": "DASHBOARDRPC__SET_BOT_SETTINGS",
             "params": [
                 current_user.id,
                 {
-                    "prefixes": bot_settings_form.prefixes.data.split(";;;;;"),
+                    "prefixes": (prefixes if (prefixes := bot_settings_form.prefixes.data.split(";;|;;")) != [""] else []),
                     "invoke_error_msg": bot_settings_form.invoke_error_msg.data.strip() or None,
                     "disabled_commands": bot_settings_form.disabled_commands.data,
                     "disabled_command_msg": bot_settings_form.disabled_command_msg.data.strip()
                     or None,
                     "description": bot_settings_form.description.data.strip() or None,
                     "custom_info": bot_settings_form.custom_info.data.strip() or None,
                     "embeds": bot_settings_form.embeds.data,
```

### Comparing `red_web_dashboard-1.1/reddash/app/login/routes.py` & `red_web_dashboard-1.2.0/reddash/app/login/routes.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/pagination.py` & `red_web_dashboard-1.2.0/reddash/app/pagination.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/biometric-icon.svg` & `red_web_dashboard-1.2.0/reddash/app/static/assets/biometric-icon.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.css` & `red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.css`

 * *Files 0% similar despite different names*

```diff
@@ -18681,15 +18681,15 @@
   background: linear-gradient(-45deg, #1171ef, #f5365c, #fb6340, #5e72e4, #344767);
   background-size: 400% 400% !important;
   animation: gradient 10s ease infinite;
 }
 
 hr {
   border-top: none;
-  height: 1px;
+  height: 3px;
 }
 
 hr.vertical {
   position: absolute;
   background-color: transparent;
   height: 100%;
   right: 0;
@@ -18709,15 +18709,15 @@
 hr.horizontal {
   background-color: transparent;
 }
 hr.horizontal.light {
   background-image: linear-gradient(to right, rgba(255, 255, 255, 0), white, rgba(255, 255, 255, 0));
 }
 hr.horizontal.dark {
-  background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0));
+  background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0));
 }
 hr.horizontal.gray-light {
   background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0));
 }
 
 .lock-size {
   width: 1.7rem;
```

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.css.map` & `red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.css.map`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/css/argon-dashboard.min.css` & `red_web_dashboard-1.2.0/reddash/app/static/assets/css/argon-dashboard.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/css/nucleo-icons.css` & `red_web_dashboard-1.2.0/reddash/app/static/assets/css/nucleo-icons.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/css/nucleo-svg.css` & `red_web_dashboard-1.2.0/reddash/app/static/assets/css/nucleo-svg.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/css/simplemde.min.css` & `red_web_dashboard-1.2.0/reddash/app/static/assets/css/simplemde.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/error-403.gif` & `red_web_dashboard-1.2.0/reddash/app/static/assets/error-403.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/error-404.gif` & `red_web_dashboard-1.2.0/reddash/app/static/assets/error-404.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/error-500.gif` & `red_web_dashboard-1.2.0/reddash/app/static/assets/error-500.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.eot` & `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.svg` & `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.ttf` & `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.woff` & `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo-icons.woff2` & `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo-icons.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.eot` & `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.ttf` & `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.woff` & `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/fonts/nucleo.woff2` & `red_web_dashboard-1.2.0/reddash/app/static/assets/fonts/nucleo.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/gulpfile.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/gulpfile.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/icon-documentation.svg` & `red_web_dashboard-1.2.0/reddash/app/static/assets/icon-documentation.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/argon-dashboard.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/argon-dashboard.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -245,15 +245,15 @@
         }
     }
 }
 
 // Set Navbar Fixed.
 function navbarFixed(el) {
     let classes = ['position-sticky', 'bg-white', 'left-auto', 'top-2', 'z-index-sticky'];
-    const navbar = document.getElementById('navbarBlur');
+    let navbar = document.getElementById('navbarBlur');
 
     if (!el.getAttribute("checked")) {
         toggleNavLinksColor('blur');
         navbar.classList.add(...classes);
         navbar.setAttribute('data-scroll', 'true');
         navbarBlurOnScroll('navbarBlur');
         el.setAttribute("checked", "true");
@@ -305,15 +305,15 @@
         });
     }
 }
 
 
 // Navbar blur on scroll.
 function navbarBlurOnScroll(id) {
-    const navbar = document.getElementById(id);
+    let navbar = document.getElementById(id);
     let navbarScrollActive = navbar ? navbar.getAttribute("data-scroll") : false;
     let scrollDistance = 5;
     let classes = ["bg-white", "left-auto", "position-sticky"];
     let toggleClasses = ["shadow-none"];
 
     if (navbarScrollActive == 'true') {
         window.onscroll = debounce(function() {
@@ -382,17 +382,17 @@
         clearTimeout(timeout);
         timeout = setTimeout(later, wait);
         if (callNow) func.apply(context, args);
     };
 };
 
 // Toggle Sidenav.
-const iconNavbarSidenav = document.getElementById("iconNavbarSidenav");
-const iconSidenav = document.getElementById("iconSidenav");
-const sidenav = document.getElementById("sidenav-main");
+let iconNavbarSidenav = document.getElementById("iconNavbarSidenav");
+let iconSidenav = document.getElementById("iconSidenav");
+let sidenav = document.getElementById("sidenav-main");
 let body = document.getElementsByTagName("body")[0];
 let className = "g-sidenav-pinned";
 
 if (iconNavbarSidenav) {
     iconNavbarSidenav.addEventListener("click", toggleSidenav);
 }
 
@@ -582,38 +582,38 @@
     return e.target || e.srcElement;
 }
 
 // End tabs navigation.
 
 // Light Mode / Dark Mode.
 function darkMode(el) {
-    const body = document.getElementsByTagName("body")[0];
-    const hr = document.querySelectorAll("div:not(.sidenav) > hr");
-    const sidebar = document.querySelector(".sidenav");
-    const sidebarWhite = document.querySelectorAll(".sidenav.bg-white");
-    const hr_card = document.querySelectorAll("div:not(.bg-gradient-dark) hr");
-    const text_btn = document.querySelectorAll("button:not(.btn) > .text-dark");
-    const text_span = document.querySelectorAll("span.text-dark");
-    const text_span_white = document.querySelectorAll("span.text-white");
-    const text_strong = document.querySelectorAll("strong.text-dark");
-    const text_strong_white = document.querySelectorAll("strong.text-white");
-    const text_nav_link = document.querySelectorAll("a.nav-link.text-dark");
-    const secondary = document.querySelectorAll(".text-secondary");
-    const bg_gray_100 = document.querySelectorAll(".bg-gray-100");
-    const bg_gray_600 = document.querySelectorAll(".bg-gray-600");
-    const btn_text_dark = document.querySelectorAll(".btn.btn-link.text-dark, .btn .ni.text-dark");
-    const btn_text_white = document.querySelectorAll(".btn.btn-link.text-white, .btn .ni.text-white");
-    const card_border = document.querySelectorAll(".card.border");
-    const card_border_dark = document.querySelectorAll(".card.border.border-dark");
-    const svg = document.querySelectorAll("g");
-    const navbarBrand = document.querySelector(".navbar-brand-img");
-    const navbarBrandImg = navbarBrand.src;
-    const navLinks = document.querySelectorAll(".navbar-main .nav-link, .navbar-main .breadcrumb-item, .navbar-main .breadcrumb-item a, .navbar-main h6");
-    const cardNavLinksIcons = document.querySelectorAll(".card .nav .nav-link i");
-    const cardNavSpan = document.querySelectorAll(".card .nav .nav-link span");
+    let body = document.getElementsByTagName("body")[0];
+    let hr = document.querySelectorAll("div:not(.sidenav) > hr");
+    let sidebar = document.querySelector(".sidenav");
+    let sidebarWhite = document.querySelectorAll(".sidenav.bg-white");
+    let hr_card = document.querySelectorAll("div:not(.bg-gradient-dark) hr");
+    let text_btn = document.querySelectorAll("button:not(.btn) > .text-dark");
+    let text_span = document.querySelectorAll("span.text-dark");
+    let text_span_white = document.querySelectorAll("span.text-white");
+    let text_strong = document.querySelectorAll("strong.text-dark");
+    let text_strong_white = document.querySelectorAll("strong.text-white");
+    let text_nav_link = document.querySelectorAll("a.nav-link.text-dark");
+    let secondary = document.querySelectorAll(".text-secondary");
+    let bg_gray_100 = document.querySelectorAll(".bg-gray-100");
+    let bg_gray_600 = document.querySelectorAll(".bg-gray-600");
+    let btn_text_dark = document.querySelectorAll(".btn.btn-link.text-dark, .btn .ni.text-dark");
+    let btn_text_white = document.querySelectorAll(".btn.btn-link.text-white, .btn .ni.text-white");
+    let card_border = document.querySelectorAll(".card.border");
+    let card_border_dark = document.querySelectorAll(".card.border.border-dark");
+    let svg = document.querySelectorAll("g");
+    let navbarBrand = document.querySelector(".navbar-brand-img");
+    let navbarBrandImg = navbarBrand.src;
+    let navLinks = document.querySelectorAll(".navbar-main .nav-link, .navbar-main .breadcrumb-item, .navbar-main .breadcrumb-item a, .navbar-main h6");
+    let cardNavLinksIcons = document.querySelectorAll(".card .nav .nav-link i");
+    let cardNavSpan = document.querySelectorAll(".card .nav .nav-link span");
 
 
     if (!el.getAttribute("checked")) {
         body.classList.add("dark-version");
         if (navbarBrandImg.includes("logo-ct-dark.png")) {
             let navbarBrandImgNew = navbarBrandImg.replace("logo-ct-dark", "logo-ct");
             navbarBrand.src = navbarBrandImgNew;
@@ -691,15 +691,15 @@
             }
         }
         for (let i = 0; i < card_border.length; i++) {
             card_border[i].classList.add("border-dark");
         }
         el.setAttribute("checked", "true");
 
-        document.querySelector("#sidebar-theme-select").children[1].click(); // Even the sidebar change of theme when theme changing, but the change wasn"t saved in a cookie.
+        document.querySelector("#sidebar-theme-select").children[1].click(); // Toggle sidebar dark theme, even if the change isn't asked by the user.
     } else {
         body.classList.remove("dark-version");
         sidebar.classList.add("bg-white");
         if (navbarBrandImg.includes("logo-ct.png")) {
             let navbarBrandImgNew = navbarBrandImg.replace("logo-ct", "logo-ct-dark");
             navbarBrand.src = navbarBrandImgNew;
         }
```

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/argon-dashboard.js.map` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/argon-dashboard.js.map`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/core/bootstrap.min.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/core/jquery.min.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/jquery.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/core/popper.min.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/core/popper.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/Chart.extension.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/Chart.extension.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/bootstrap-notify.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/chartjs.min.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/chartjs.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/js/plugins/utils.js` & `red_web_dashboard-1.2.0/reddash/app/static/assets/js/plugins/utils.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/oauth.png` & `red_web_dashboard-1.2.0/reddash/app/static/assets/oauth.png`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/pdf.svg` & `red_web_dashboard-1.2.0/reddash/app/static/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/random.svg` & `red_web_dashboard-1.2.0/reddash/app/static/assets/random.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_cards.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_forms.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_header.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_misc.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_nav.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_tables.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_typography.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/_variables.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/theme.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/static/assets/scss/argon-dashboard.scss` & `red_web_dashboard-1.2.0/reddash/app/static/assets/scss/argon-dashboard.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/tasks_manager.py` & `red_web_dashboard-1.2.0/reddash/app/tasks_manager.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/errors/403.html` & `red_web_dashboard-1.2.0/reddash/app/templates/errors/403.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/errors/404.html` & `red_web_dashboard-1.2.0/reddash/app/templates/errors/404.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/errors/500.html` & `red_web_dashboard-1.2.0/reddash/app/templates/errors/500.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/errors/blacklisted.html` & `red_web_dashboard-1.2.0/reddash/app/templates/errors/blacklisted.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/errors/custom.html` & `red_web_dashboard-1.2.0/reddash/app/templates/errors/custom.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/includes/fixed-plugin.html` & `red_web_dashboard-1.2.0/reddash/app/templates/includes/fixed-plugin.html`

 * *Files 8% similar despite different names*

```diff
@@ -16,34 +16,34 @@
       <!-- Theme Color -->
       <div>
         <h6 class="mb-0">{{ _("Theme Color") }}</h6>
       </div>
       <a href="javascript:void(0)" class="switch-trigger background-color" id="background-color-select">
         <div class="badge-colors my-2 text-start">
           {% for color in variables["meta"]["available_colors"] %}
-            <span class="badge filter bg-gradient-{{ color }} {% if color == variables["meta"]["color"] %}active{% endif %}" data-color="{{ color }}" onclick="sidebarColor(this);$.postData({'color': {% if color != variables["meta"]["default_color"] %}'{{ color }}'{% else %}null{% endif %}},'{{ url_for("base_blueprint.set_color") }}')"></span>
+            <span class="badge filter bg-gradient-{{ color }} {% if color == variables["meta"]["color"] %}active{% endif %}" data-color="{{ color }}" onclick='sidebarColor(this); $.postData({"color": {% if color != variables["meta"]["default_color"] %}"{{ color }}"{% else %}null{% endif %}},"{{ url_for("base_blueprint.set_color") }}")'></span>
           {% endfor %}
         </div>
       </a>
       <hr class="horizontal dark my-sm-4" />
       <!-- Theme Light/Dark -->
       <div class="mt-2 mb-5 d-flex">
         <h6 class="mb-0">{{ _("Light / Dark") }}</h6>
         <div class="form-check form-switch ps-0 ms-auto my-auto" id="background-theme-select">
-          <input class="form-check-input mt-1 ms-auto" type="checkbox" id="dark-version" onclick="darkMode(this);$.postData({'background_theme': this.getAttribute('checked') ? 'dark' : 'white'},'{{ url_for("base_blueprint.set_background_theme") }}');" />
+          <input class="form-check-input mt-1 ms-auto" type="checkbox" id="dark-version" onclick='darkMode(this); $.postData({"background_theme": this.getAttribute("checked") ? "dark" : "white"},"{{ url_for("base_blueprint.set_background_theme") }}");' />
         </div>
       </div>
       <hr class="horizontal dark my-sm-4" />
       <!-- Sidenav Type -->
       <div class="mt-3">
         <h6 class="mb-0">{{ _("Sidenav Theme") }}</h6>
       </div>
       <div class="d-flex" id="sidebar-theme-select">
-        <a class="btn btn-outline-{{ variables["meta"]["color"] }} w-100 px-3 mb-2 me-2 active" data-class="bg-white" onclick="sidebarType(this);$.postData({'sidebar_theme': {% if 'white' != variables["meta"]["default_theme"] %}'white'{% else %}null{% endif %}},'{{ url_for("base_blueprint.set_sidebar_theme") }}')">{{ _("White") }}</a>
-        <a class="btn btn-outline-{{ variables["meta"]["color"] }} w-100 px-3 mb-2 me-2" data-class="bg-default" onclick="sidebarType(this);$.postData({'sidebar_theme': {% if 'dark' != variables["meta"]["default_theme"] %}'dark'{% else %}null{% endif %}},'{{ url_for("base_blueprint.set_sidebar_theme") }}')">{{ _("Dark") }}</a>
+        <a class="btn btn-outline-{{ variables["meta"]["color"] }} w-100 px-3 mb-2 me-2 active" data-class="bg-white" onclick='sidebarType(this); $.postData({"sidebar_theme": {% if "white" != variables["meta"]["default_theme"] %}"white"{% else %}null{% endif %}},"{{ url_for("base_blueprint.set_sidebar_theme") }}")'>{{ _("White") }}</a>
+        <a class="btn btn-outline-{{ variables["meta"]["color"] }} w-100 px-3 mb-2 me-2" data-class="bg-default" onclick='sidebarType(this); $.postData({"sidebar_theme": {% if "dark" != variables["meta"]["default_theme"] %}"dark"{% else %}null{% endif %}},"{{ url_for("base_blueprint.set_sidebar_theme") }}")'>{{ _("Dark") }}</a>
       </div>
       <p class="text-sm d-xl-none d-block mt-2">{{ _("You can change the sidenav theme just on desktop view.") }}</p>
       <!-- Navbar Fixed -->
       <div class="d-flex my-3">
         <h6 class="mb-0">{{ _("Navbar Fixed") }}</h6>
         <div class="form-check form-switch ps-0 ms-auto my-auto">
           <input class="form-check-input mt-1 ms-auto" type="checkbox" id="navbarFixed" onclick="navbarFixed(this)" />
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
 **** {{{{ __((""DDaasshhbbooaarrdd CCoonnffiigguurraattoorr"")) }}}} ****
 {{ _("Choose your custom options!") }}
 ===============================================================================
 ** {{{{ __((""TThheemmee CCoolloorr"")) }}}} **
 _{_%_ _f_o_r_ _c_o_l_o_r_ _i_n_ _v_a_r_i_a_b_l_e_s_[_"_m_e_t_a_"_]_[_"_a_v_a_i_l_a_b_l_e___c_o_l_o_r_s_"_]_ _%_}
-_}_a_c_t_i_v_e_{_%_ _e_n_d_i_f_ _%_}_"_ _d_a_t_a_-_c_o_l_o_r_=_"_{_{_ _c_o_l_o_r_ _}_}_"_ _o_n_c_l_i_c_k_=_"_s_i_d_e_b_a_r_C_o_l_o_r
-_(_t_h_i_s_)_;_$_._p_o_s_t_D_a_t_a_(_{_'_c_o_l_o_r_'_:_ _{_%_ _i_f_ _c_o_l_o_r_ _!_=_ _v_a_r_i_a_b_l_e_s_[_"_m_e_t_a_"_]_[_"_d_e_f_a_u_l_t___c_o_l_o_r_"_]
-_%_}_'_{_{_ _c_o_l_o_r_ _}_}_'_{_%_ _e_l_s_e_ _%_}_n_u_l_l_{_%_ _e_n_d_i_f_ _%_}_}_,_'_{_{_ _u_r_l___f_o_r
-_(_"_b_a_s_e___b_l_u_e_p_r_i_n_t_._s_e_t___c_o_l_o_r_"_)_ _}_}_'_)_"_>_ _{_%_ _e_n_d_f_o_r_ _%_}
+_}_a_c_t_i_v_e_{_%_ _e_n_d_i_f_ _%_}_"_ _d_a_t_a_-_c_o_l_o_r_=_"_{_{_ _c_o_l_o_r_ _}_}_"_ _o_n_c_l_i_c_k_=_'_s_i_d_e_b_a_r_C_o_l_o_r_(_t_h_i_s_)_;
+_$_._p_o_s_t_D_a_t_a_(_{_"_c_o_l_o_r_"_:_ _{_%_ _i_f_ _c_o_l_o_r_ _!_=_ _v_a_r_i_a_b_l_e_s_[_"_m_e_t_a_"_]_[_"_d_e_f_a_u_l_t___c_o_l_o_r_"_]_ _%_}_"_{
+_{_ _c_o_l_o_r_ _}_}_"_{_%_ _e_l_s_e_ _%_}_n_u_l_l_{_%_ _e_n_d_i_f_ _%_}_}_,_"_{_{_ _u_r_l___f_o_r_(_"_b_a_s_e___b_l_u_e_p_r_i_n_t_._s_e_t___c_o_l_o_r_"_)
+_}_}_"_)_'_>_ _{_%_ _e_n_d_f_o_r_ _%_}
 ===============================================================================
 ** {{{{ __((""LLiigghhtt // DDaarrkk"")) }}}} **
-}');" />
+??
 ===============================================================================
 ** {{{{ __((""SSiiddeennaavv TThheemmee"")) }}}} **
-} w-100 px-3 mb-2 me-2 active" data-class="bg-white" onclick="sidebarType
-(this);$.postData({'sidebar_theme': {% if 'white' != variables["meta"]
-["default_theme"] %}'white'{% else %}null{% endif %}},'{{ url_for
-("base_blueprint.set_sidebar_theme") }}')">{{ _("White") }}
+} w-100 px-3 mb-2 me-2 active" data-class="bg-white" onclick='sidebarType
+(this); $.postData({"sidebar_theme": {% if "white" != variables["meta"]
+["default_theme"] %}"white"{% else %}null{% endif %}},"{{ url_for
+("base_blueprint.set_sidebar_theme") }}")'>{{ _("White") }}
 
-} w-100 px-3 mb-2 me-2" data-class="bg-default" onclick="sidebarType
-(this);$.postData({'sidebar_theme': {% if 'dark' != variables["meta"]
-["default_theme"] %}'dark'{% else %}null{% endif %}},'{{ url_for
-("base_blueprint.set_sidebar_theme") }}')">{{ _("Dark") }}
+} w-100 px-3 mb-2 me-2" data-class="bg-default" onclick='sidebarType(this);
+$.postData({"sidebar_theme": {% if "dark" != variables["meta"]["default_theme"]
+%}"dark"{% else %}null{% endif %}},"{{ url_for
+("base_blueprint.set_sidebar_theme") }}")'>{{ _("Dark") }}
 {{ _("You can change the sidenav theme just on desktop view.") }}
 ** {{{{ __((""NNaavvbbaarr FFiixxeedd"")) }}}} **
 ??
```

### Comparing `red_web_dashboard-1.1/reddash/app/templates/includes/footer.html` & `red_web_dashboard-1.2.0/reddash/app/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/includes/navigation.html` & `red_web_dashboard-1.2.0/reddash/app/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/includes/scripts.html` & `red_web_dashboard-1.2.0/reddash/app/templates/includes/scripts.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         });
     });
 </script>
 {{ moment.include_moment() }}
 {{ moment.locale(auto_detect=true) }}
 <script src="https://cdn.jsdelivr.net/npm/easymde/dist/easymde.min.js"></script>
 <script>
-    document.querySelectorAll(".markdown-text-area-field").forEach(function(element) {
+    function MarkdownField(element) {
         var additionalKwargs = {};
         if (element.classList.contains("markdown-text-area-field-toolbar-disabled")) {
             additionalKwargs.toolbar = false;
             additionalKwargs.status = false;
         }
         if (!element.classList.contains("markdown-text-area-field-max-height")) {
             additionalKwargs.minHeight = "150px";
@@ -104,16 +104,16 @@
                 if (delta > 0) {
                     str = str.substr(0, str.length - delta);
                     change.update(change.from, change.to, str.split("\n"));
                 }
             }
             return true;
         });
-        // document.querySelectorAll(".modal").forEach(function(modal) {$(modal).on("shown.bs.modal", function () {easymde.codemirror.refresh();})});
-    });
+    }
+    document.querySelectorAll(".markdown-text-area-field").forEach(MarkdownField);
 </script>
 <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>
 <script>
     const SwalAlert = Swal.mixin({
         icon: "warning",
         customClass: {
             confirmButton: "btn bg-danger",
@@ -201,15 +201,15 @@
             duplicateItemsAllowed: false,
             paste: true,
             searchEnabled: true,
             searchChoices: true,
             searchFields: ["label", "value"],
             shouldSort: false,
             shouldSortItems: false,
-            delimiter: ";;;;;",
+            delimiter: ";;|;;",
         };
         if (element.ariaPlaceholder) {
             choicesOptions.placeholder = true;
             choicesOptions.placeholderValue = element.ariaPlaceholder;
         }
         if (element.classList.contains("just-display")) {
             choicesOptions.addItems = false;
```

### Comparing `red_web_dashboard-1.1/reddash/app/templates/includes/sidenav.html` & `red_web_dashboard-1.2.0/reddash/app/templates/includes/sidenav.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/layouts/base-fullscreen.html` & `red_web_dashboard-1.2.0/reddash/app/templates/layouts/base-fullscreen.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/layouts/base.html` & `red_web_dashboard-1.2.0/reddash/app/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/pages/admin.html` & `red_web_dashboard-1.2.0/reddash/app/templates/pages/admin.html`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                     <div class="card-body">
                         <div class="row">
                             <div class="col-sm-12 text-left">
                                 <div class="d-flex justify-content-between mb-2">
                                     <h2 class="card-title">{{ _("Dashboard Settings") }}</h2>
                                 </div>
                             </div>
-                            <div class="d-flex mt-4">
+                            <div class="mt-4">
                                 <form action="" method="POST" role="form" enctype="multipart/form-data">
                                     {{ dashboard_settings_form.hidden_tag() }}
                                     <div class="mb-3">
                                         <div class="form-group">
                                             <label class="form-group-label">{{ _("Title:") }}</label>
                                             {{ dashboard_settings_form.title(class="form-control form-control-default") }}
                                         </div>
@@ -204,15 +204,15 @@
                     <div class="card-body">
                         <div class="row">
                             <div class="col-sm-12 text-left">
                                 <div class="d-flex justify-content-between mb-2">
                                     <h2 class="card-title">{{ _("Bot Settings") }}</h2>
                                 </div>
                             </div>
-                            <div class="d-flex mt-4">
+                            <div class="mt-4">
                                 <form action="" method="POST" role="form" enctype="multipart/form-data">
                                     {{ bot_settings_form.hidden_tag() }}
                                     <div class="mb-3">
                                         <div class="form-group">
                                             <label class="form-group-label">{{ _("Prefixes:") }}</label>
                                             {{ bot_settings_form.prefixes(class="form-control form-control-default select-choices") }}
                                         </div>
```

### Comparing `red_web_dashboard-1.1/reddash/app/templates/pages/commands.html` & `red_web_dashboard-1.2.0/reddash/app/templates/pages/commands.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/pages/credits.html` & `red_web_dashboard-1.2.0/reddash/app/templates/pages/credits.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/pages/dashboard.html` & `red_web_dashboard-1.2.0/reddash/app/templates/pages/dashboard.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/pages/guild_profile.html` & `red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_party.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,268 +1,294 @@
-00000000: 3c64 6976 2069 643d 2270 726f 6669 6c65  <div id="profile
-00000010: 2220 636c 6173 733d 2263 6172 6420 6361  " class="card ca
-00000020: 7264 2d62 6f64 7920 636f 6c2d 6d64 2d33  rd-body col-md-3
-00000030: 206d 742d 3420 616c 6967 6e2d 6974 656d   mt-4 align-item
-00000040: 732d 6365 6e74 6572 2220 7374 796c 653d  s-center" style=
-00000050: 226d 6172 6769 6e2d 7269 6768 743a 2031  "margin-right: 1
-00000060: 3070 783b 223e 0a20 2020 203c 6469 7620  0px;">.    <div 
-00000070: 7b25 2069 6620 4661 6c73 6520 257d 636c  {% if False %}cl
-00000080: 6173 733d 2272 6f77 227b 2520 656e 6469  ass="row"{% endi
-00000090: 6620 257d 3e0a 2020 2020 2020 2020 3c62  f %}>.        <b
-000000a0: 7220 2f3e 0a20 2020 2020 2020 203c 6469  r />.        <di
-000000b0: 7620 636c 6173 733d 2263 6f6c 2d73 6d2d  v class="col-sm-
-000000c0: 6175 746f 2063 6f6c 2d34 2074 6578 742d  auto col-4 text-
-000000d0: 6365 6e74 6572 223e 0a20 2020 2020 2020  center">.       
-000000e0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000000f0: 2261 7661 7461 7220 6176 6174 6172 2d78  "avatar avatar-x
-00000100: 6c22 3e3c 696d 6720 7372 633d 227b 7b20  l"><img src="{{ 
-00000110: 6775 696c 642e 6963 6f6e 5f75 726c 207d  guild.icon_url }
-00000120: 7d22 2063 6c61 7373 3d22 7368 6164 6f77  }" class="shadow
-00000130: 2d73 6d20 626f 7264 6572 2d72 6164 6975  -sm border-radiu
-00000140: 732d 6c67 2220 7374 796c 653d 2268 6569  s-lg" style="hei
-00000150: 6768 743a 2031 3730 253b 2077 6964 7468  ght: 170%; width
-00000160: 3a20 3137 3025 3b22 202f 3e3c 2f64 6976  : 170%;" /></div
-00000170: 3e0a 2020 2020 2020 2020 3c2f 6469 763e  >.        </div>
-00000180: 0a20 2020 2020 2020 203c 6469 7620 636c  .        <div cl
-00000190: 6173 733d 2263 6f6c 2d73 6d2d 6175 746f  ass="col-sm-auto
-000001a0: 2063 6f6c 2d38 206d 792d 6175 746f 223e   col-8 my-auto">
-000001b0: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-000001c0: 7620 636c 6173 733d 2268 2d31 3030 223e  v class="h-100">
-000001d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000001e0: 203c 6833 2063 6c61 7373 3d22 636f 6c20   <h3 class="col 
-000001f0: 6d62 2d31 2066 6f6e 742d 7765 6967 6874  mb-1 font-weight
-00000200: 2d62 6f6c 6465 7220 7465 7874 2d63 656e  -bolder text-cen
-00000210: 7465 7222 3e0a 2020 2020 2020 2020 2020  ter">.          
-00000220: 2020 2020 2020 2020 2020 7b7b 2067 7569            {{ gui
-00000230: 6c64 2e6e 616d 6520 7d7d 0a20 2020 2020  ld.name }}.     
-00000240: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000250: 6469 7620 636c 6173 733d 2264 726f 7064  div class="dropd
-00000260: 6f77 6e22 2073 7479 6c65 3d22 6469 7370  own" style="disp
-00000270: 6c61 793a 2075 6e73 6574 3b22 3e0a 2020  lay: unset;">.  
-00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000290: 2020 2020 2020 3c61 2063 6c61 7373 3d22        <a class="
-000002a0: 6e61 762d 6c69 6e6b 2074 6578 742d 6c67  nav-link text-lg
-000002b0: 2074 6578 742d 6461 726b 2220 726f 6c65   text-dark" role
-000002c0: 3d22 6275 7474 6f6e 2220 6964 3d22 6775  ="button" id="gu
-000002d0: 696c 645f 6472 6f70 646f 776e 2220 6461  ild_dropdown" da
-000002e0: 7461 2d74 6f67 676c 653d 2264 726f 7064  ta-toggle="dropd
-000002f0: 6f77 6e22 2061 7269 612d 6861 7370 6f70  own" aria-haspop
-00000300: 7570 3d22 7472 7565 2220 6172 6961 2d65  up="true" aria-e
-00000310: 7870 616e 6465 643d 2266 616c 7365 2220  xpanded="false" 
-00000320: 7374 796c 653d 2264 6973 706c 6179 3a20  style="display: 
-00000330: 756e 7365 743b 2076 6572 7469 6361 6c2d  unset; vertical-
-00000340: 616c 6967 6e3a 2032 2e36 7078 3b20 6d61  align: 2.6px; ma
-00000350: 7267 696e 2d6c 6566 743a 2032 7078 3b22  rgin-left: 2px;"
-00000360: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000370: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00000380: 2063 6c61 7373 3d22 6661 2066 612d 656c   class="fa fa-el
-00000390: 6c69 7073 6973 2d76 223e 3c2f 693e 0a20  lipsis-v"></i>. 
+00000000: 7b25 2065 7874 656e 6473 2022 6c61 796f  {% extends "layo
+00000010: 7574 732f 6261 7365 2e68 746d 6c22 2025  uts/base.html" %
+00000020: 7d0a 7b25 2069 6d70 6f72 7420 2262 6f6f  }.{% import "boo
+00000030: 7473 7472 6170 2f77 7466 2e68 746d 6c22  tstrap/wtf.html"
+00000040: 2061 7320 7774 6620 257d 0a0a 7b25 2062   as wtf %}..{% b
+00000050: 6c6f 636b 2074 6974 6c65 2025 7d0a 2020  lock title %}.  
+00000060: 7b7b 205f 2822 5468 6972 6420 5061 7274  {{ _("Third Part
+00000070: 7922 2920 7d7d 207b 7b20 7468 6972 645f  y") }} {{ third_
+00000080: 7061 7274 7920 7d7d 7b25 2069 6620 6775  party }}{% if gu
+00000090: 696c 6420 257d 202d 207b 7b20 6775 696c  ild %} - {{ guil
+000000a0: 642e 6e61 6d65 207d 7d7b 2520 656e 6469  d.name }}{% endi
+000000b0: 6620 257d 0a7b 2520 656e 6462 6c6f 636b  f %}.{% endblock
+000000c0: 2025 7d0a 0a7b 2520 626c 6f63 6b20 7374   %}..{% block st
+000000d0: 796c 6573 6865 6574 7320 257d 7b25 2065  ylesheets %}{% e
+000000e0: 6e64 626c 6f63 6b20 257d 0a0a 7b25 2062  ndblock %}..{% b
+000000f0: 6c6f 636b 2063 6f6e 7465 6e74 2025 7d0a  lock content %}.
+00000100: 2020 3c6d 6169 6e20 636c 6173 733d 226d    <main class="m
+00000110: 6169 6e2d 636f 6e74 656e 7420 706f 7369  ain-content posi
+00000120: 7469 6f6e 2d72 656c 6174 6976 6520 626f  tion-relative bo
+00000130: 7264 6572 2d72 6164 6975 732d 6c67 223e  rder-radius-lg">
+00000140: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+00000150: 2263 6f6e 7461 696e 6572 2d66 6c75 6964  "container-fluid
+00000160: 223e 0a20 2020 2020 2020 203c 6469 7620  ">.        <div 
+00000170: 636c 6173 733d 2272 6f77 223e 0a20 2020  class="row">.   
+00000180: 2020 2020 2020 2020 207b 2520 6966 2067           {% if g
+00000190: 7569 6c64 2061 6e64 206e 6f74 2066 756c  uild and not ful
+000001a0: 6c73 6372 6565 6e20 257d 0a20 2020 2020  lscreen %}.     
+000001b0: 2020 2020 2020 2020 2020 207b 2520 696e             {% in
+000001c0: 636c 7564 6520 2270 6167 6573 2f67 7569  clude "pages/gui
+000001d0: 6c64 5f70 726f 6669 6c65 2e68 746d 6c22  ld_profile.html"
+000001e0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000001f0: 7b25 2065 6e64 6966 2025 7d0a 0a20 2020  {% endif %}..   
+00000200: 2020 2020 2020 2020 203c 6469 7620 6964           <div id
+00000210: 3d22 6775 696c 642d 636f 6e74 656e 7422  ="guild-content"
+00000220: 7b25 2069 6620 6775 696c 6420 616e 6420  {% if guild and 
+00000230: 6e6f 7420 6675 6c6c 7363 7265 656e 2025  not fullscreen %
+00000240: 7d20 636c 6173 733d 2263 6f6c 2d6d 642d  } class="col-md-
+00000250: 3820 6d74 2d34 227b 2520 656e 6469 6620  8 mt-4"{% endif 
+00000260: 257d 3e0a 2020 2020 2020 2020 2020 2020  %}>.            
+00000270: 2020 2020 7b25 2069 6620 6775 696c 6420      {% if guild 
+00000280: 616e 6420 6e6f 7420 6675 6c6c 7363 7265  and not fullscre
+00000290: 656e 2025 7d0a 2020 2020 2020 2020 2020  en %}.          
+000002a0: 2020 2020 2020 2020 2020 3c75 6c20 636c            <ul cl
+000002b0: 6173 733d 226e 6176 206e 6176 2d70 696c  ass="nav nav-pil
+000002c0: 6c73 2070 6f73 6974 696f 6e2d 7265 6c61  ls position-rela
+000002d0: 7469 7665 2065 6e64 2d30 2220 726f 6c65  tive end-0" role
+000002e0: 3d22 7461 626c 6973 7422 3e0a 2020 2020  ="tablist">.    
+000002f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000300: 2020 2020 3c6c 6920 636c 6173 733d 226e      <li class="n
+00000310: 6176 2d69 7465 6d22 3e0a 2020 2020 2020  av-item">.      
+00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000330: 2020 2020 2020 3c61 2068 7265 663d 227b        <a href="{
+00000340: 7b20 7572 6c5f 666f 7228 2262 6173 655f  { url_for("base_
+00000350: 626c 7565 7072 696e 742e 6461 7368 626f  blueprint.dashbo
+00000360: 6172 645f 6775 696c 6422 2c20 6775 696c  ard_guild", guil
+00000370: 645f 6964 3d67 7569 6c64 2e69 6429 207d  d_id=guild.id) }
+00000380: 7d22 2063 6c61 7373 3d22 6e61 762d 6c69  }" class="nav-li
+00000390: 6e6b 223e 0a20 2020 2020 2020 2020 2020  nk">.           
 000003a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003b0: 2020 2020 2020 203c 2f61 3e0a 2020 2020         </a>.    
-000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003d0: 2020 2020 3c75 6c20 636c 6173 733d 2264      <ul class="d
-000003e0: 726f 7064 6f77 6e2d 6d65 6e75 2220 6172  ropdown-menu" ar
-000003f0: 6961 2d6c 6162 656c 6c65 6462 793d 2267  ia-labelledby="g
-00000400: 7569 6c64 5f64 726f 7064 6f77 6e22 3e0a  uild_dropdown">.
+000003b0: 2020 2020 203c 6920 636c 6173 733d 2266       <i class="f
+000003c0: 6120 6661 2d6d 6170 206f 7061 6369 7479  a fa-map opacity
+000003d0: 2d31 3022 2073 7479 6c65 3d22 7665 7274  -10" style="vert
+000003e0: 6963 616c 2d61 6c69 676e 3a20 2d31 7078  ical-align: -1px
+000003f0: 3b22 3e3c 2f69 3e20 7b7b 205f 2822 4f76  ;"></i> {{ _("Ov
+00000400: 6572 7669 6577 2229 207d 7d0a 2020 2020  erview") }}.    
 00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
-00000430: 636c 6173 733d 226e 6176 2d6c 696e 6b22  class="nav-link"
-00000440: 3e3c 6120 636c 6173 733d 226e 6176 2d69  ><a class="nav-i
-00000450: 7465 6d20 6472 6f70 646f 776e 2d69 7465  tem dropdown-ite
-00000460: 6d22 206f 6e63 6c69 636b 3d27 636f 7079  m" onclick='copy
-00000470: 5465 7874 546f 436c 6970 626f 6172 6428  TextToClipboard(
-00000480: 227b 7b20 6775 696c 642e 6964 207d 7d22  "{{ guild.id }}"
-00000490: 2927 3e3c 6920 636c 6173 733d 2266 6120  )'><i class="fa 
-000004a0: 6661 2d63 6f70 7922 2073 7479 6c65 3d22  fa-copy" style="
-000004b0: 7769 6474 683a 2031 2e33 656d 3b20 7665  width: 1.3em; ve
-000004c0: 7274 6963 616c 2d61 6c69 676e 3a20 302e  rtical-align: 0.
-000004d0: 3270 783b 223e 3c2f 693e 207b 7b20 5f28  2px;"></i> {{ _(
-000004e0: 2243 6f70 7920 4944 2229 207d 7d3c 2f61  "Copy ID") }}</a
-000004f0: 3e3c 2f6c 693e 0a20 2020 2020 2020 2020  ></li>.         
-00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000510: 2020 207b 2520 6966 206c 6561 7665 5f67     {% if leave_g
-00000520: 7569 6c64 5f66 6f72 6d20 257d 0a20 2020  uild_form %}.   
-00000530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000540: 2020 2020 2020 2020 2020 2020 203c 666f               <fo
-00000550: 726d 2061 6374 696f 6e3d 2222 206d 6574  rm action="" met
-00000560: 686f 643d 2250 4f53 5422 2072 6f6c 653d  hod="POST" role=
-00000570: 2266 6f72 6d22 2065 6e63 7479 7065 3d22  "form" enctype="
-00000580: 6d75 6c74 6970 6172 742f 666f 726d 2d64  multipart/form-d
-00000590: 6174 6122 3e0a 2020 2020 2020 2020 2020  ata">.          
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2020 2020 2020 2020 2020 7b7b 206c 6561            {{ lea
-000005c0: 7665 5f67 7569 6c64 5f66 6f72 6d2e 6869  ve_guild_form.hi
-000005d0: 6464 656e 5f74 6167 2829 207d 7d0a 2020  dden_tag() }}.  
-000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000600: 2020 7b7b 206c 6561 7665 5f67 7569 6c64    {{ leave_guild
-00000610: 5f66 6f72 6d2e 7375 626d 6974 2863 6c61  _form.submit(cla
-00000620: 7373 3d22 6e61 762d 6974 656d 2064 726f  ss="nav-item dro
-00000630: 7064 6f77 6e2d 6974 656d 2074 6578 742d  pdown-item text-
-00000640: 6461 6e67 6572 222c 206f 6e63 6c69 636b  danger", onclick
-00000650: 3d22 7265 7475 726e 2063 6f6e 6669 726d  ="return confirm
-00000660: 4c65 6176 6547 7569 6c64 2865 7665 6e74  LeaveGuild(event
-00000670: 293b 222c 2073 7479 6c65 3d22 6469 7370  );", style="disp
-00000680: 6c61 793a 206e 6f6e 653b 2229 207d 7d0a  lay: none;") }}.
-00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006b0: 2020 2020 3c6c 6920 636c 6173 733d 226e      <li class="n
-000006c0: 6176 2d6c 696e 6b22 3e3c 6120 636c 6173  av-link"><a clas
-000006d0: 733d 226e 6176 2d69 7465 6d20 6472 6f70  s="nav-item drop
-000006e0: 646f 776e 2d69 7465 6d20 7465 7874 2d64  down-item text-d
-000006f0: 616e 6765 7222 206f 6e63 6c69 636b 3d27  anger" onclick='
-00000700: 7468 6973 2e70 6172 656e 7445 6c65 6d65  this.parentEleme
-00000710: 6e74 2e70 6172 656e 7445 6c65 6d65 6e74  nt.parentElement
-00000720: 2e71 7565 7279 5365 6c65 6374 6f72 2822  .querySelector("
-00000730: 237b 7b20 6c65 6176 655f 6775 696c 645f  #{{ leave_guild_
-00000740: 666f 726d 2e73 7562 6d69 742e 6964 207d  form.submit.id }
-00000750: 7d22 292e 636c 6963 6b28 293b 273e 3c69  }").click();'><i
-00000760: 2063 6c61 7373 3d22 6661 2066 612d 7472   class="fa fa-tr
-00000770: 6173 682d 6f22 2073 7479 6c65 3d22 7769  ash-o" style="wi
-00000780: 6474 683a 2031 2e33 656d 3b20 7665 7274  dth: 1.3em; vert
-00000790: 6963 616c 2d61 6c69 676e 3a20 302e 3870  ical-align: 0.8p
-000007a0: 783b 223e 3c2f 693e 207b 7b20 6c65 6176  x;"></i> {{ leav
-000007b0: 655f 6775 696c 645f 666f 726d 2e73 7562  e_guild_form.sub
-000007c0: 6d69 742e 6c61 6265 6c2e 7465 7874 207d  mit.label.text }
-000007d0: 7d3c 2f61 3e3c 2f6c 693e 0a20 2020 2020  }</a></li>.     
-000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007f0: 2020 2020 2020 2020 2020 203c 2f66 6f72             </for
-00000800: 6d3e 0a20 2020 2020 2020 2020 2020 2020  m>.             
-00000810: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00000820: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
-00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000840: 2020 203c 2f75 6c3e 0a20 2020 2020 2020     </ul>.       
-00000850: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00000860: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00000870: 2020 2020 3c2f 6833 3e0a 2020 2020 2020      </h3>.      
-00000880: 2020 2020 2020 2020 2020 3c68 3520 636c            <h5 cl
-00000890: 6173 733d 226d 622d 3020 666f 6e74 2d77  ass="mb-0 font-w
-000008a0: 6569 6768 742d 626f 6c64 2074 6578 742d  eight-bold text-
-000008b0: 6c67 2074 6578 742d 6365 6e74 6572 223e  lg text-center">
-000008c0: 7b7b 205f 2822 4f77 6e65 6420 6279 2229  {{ _("Owned by")
-000008d0: 207d 7d20 7b7b 2067 7569 6c64 2e6f 776e   }} {{ guild.own
-000008e0: 6572 207d 7d3c 2f68 353e 0a20 2020 2020  er }}</h5>.     
-000008f0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00000900: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000910: 203c 2f64 6976 3e0a 0a20 2020 203c 6469   </div>..    <di
-00000920: 7620 636c 6173 733d 2263 6172 642d 7072  v class="card-pr
-00000930: 6f66 696c 652d 7374 6174 7320 642d 666c  ofile-stats d-fl
-00000940: 6578 206a 7573 7469 6679 2d63 6f6e 7465  ex justify-conte
-00000950: 6e74 2d63 656e 7465 7222 3e0a 2020 2020  nt-center">.    
-00000960: 2020 2020 3c64 6976 3e0a 2020 2020 2020      <div>.      
-00000970: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-00000980: 733d 2268 6561 6469 6e67 223e 7b7b 206e  s="heading">{{ n
-00000990: 756d 6265 725f 746f 5f74 6578 745f 7769  umber_to_text_wi
-000009a0: 7468 5f73 7566 6669 7828 6775 696c 642e  th_suffix(guild.
-000009b0: 6d65 6d62 6572 735f 6e75 6d62 6572 2920  members_number) 
-000009c0: 7d7d 3c2f 7370 616e 3e0a 2020 2020 2020  }}</span>.      
-000009d0: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-000009e0: 733d 2264 6573 6372 6970 7469 6f6e 223e  s="description">
-000009f0: 7b25 2069 6620 6775 696c 642e 6d65 6d62  {% if guild.memb
-00000a00: 6572 735f 6e75 6d62 6572 203e 2031 2025  ers_number > 1 %
-00000a10: 7d7b 7b20 5f28 224d 656d 6265 7273 2229  }{{ _("Members")
-00000a20: 207d 7d7b 2520 656c 7365 2025 7d7b 7b20   }}{% else %}{{ 
-00000a30: 5f28 224d 656d 6265 7222 2920 7d7d 7b25  _("Member") }}{%
-00000a40: 2065 6e64 6966 2025 7d3c 2f73 7061 6e3e   endif %}</span>
-00000a50: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
-00000a60: 2020 2020 2020 2020 3c64 6976 3e0a 2020          <div>.  
-00000a70: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
-00000a80: 636c 6173 733d 2268 6561 6469 6e67 223e  class="heading">
-00000a90: 7b7b 206e 756d 6265 725f 746f 5f74 6578  {{ number_to_tex
-00000aa0: 745f 7769 7468 5f73 7566 6669 7828 6775  t_with_suffix(gu
-00000ab0: 696c 642e 6368 616e 6e65 6c73 5f6e 756d  ild.channels_num
-00000ac0: 6265 7229 207d 7d3c 2f73 7061 6e3e 0a20  ber) }}</span>. 
-00000ad0: 2020 2020 2020 2020 2020 203c 7370 616e             <span
-00000ae0: 2063 6c61 7373 3d22 6465 7363 7269 7074   class="descript
-00000af0: 696f 6e22 3e7b 2520 6966 2067 7569 6c64  ion">{% if guild
-00000b00: 2e63 6861 6e6e 656c 735f 6e75 6d62 6572  .channels_number
-00000b10: 203e 2031 2025 7d7b 7b20 5f28 2243 6861   > 1 %}{{ _("Cha
-00000b20: 6e6e 656c 7322 2920 7d7d 7b25 2065 6c73  nnels") }}{% els
-00000b30: 6520 257d 7b7b 205f 2822 4368 616e 6e65  e %}{{ _("Channe
-00000b40: 6c22 2920 7d7d 7b25 2065 6e64 6966 2025  l") }}{% endif %
-00000b50: 7d3c 2f73 7061 6e3e 0a20 2020 2020 2020  }</span>.       
-00000b60: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00000b70: 3c64 6976 3e0a 2020 2020 2020 2020 2020  <div>.          
-00000b80: 2020 3c73 7061 6e20 636c 6173 733d 2268    <span class="h
-00000b90: 6561 6469 6e67 223e 7b7b 206e 756d 6265  eading">{{ numbe
-00000ba0: 725f 746f 5f74 6578 745f 7769 7468 5f73  r_to_text_with_s
-00000bb0: 7566 6669 7828 6775 696c 642e 726f 6c65  uffix(guild.role
-00000bc0: 735f 6e75 6d62 6572 2920 7d7d 3c2f 7370  s_number) }}</sp
-00000bd0: 616e 3e0a 2020 2020 2020 2020 2020 2020  an>.            
-00000be0: 3c73 7061 6e20 636c 6173 733d 2264 6573  <span class="des
-00000bf0: 6372 6970 7469 6f6e 223e 7b25 2069 6620  cription">{% if 
-00000c00: 6775 696c 642e 726f 6c65 735f 6e75 6d62  guild.roles_numb
-00000c10: 6572 203e 2031 2025 7d7b 7b20 5f28 2252  er > 1 %}{{ _("R
-00000c20: 6f6c 6573 2229 207d 7d7b 2520 656c 7365  oles") }}{% else
-00000c30: 2025 7d7b 7b20 5f28 2252 6f6c 6522 2920   %}{{ _("Role") 
-00000c40: 7d7d 7b25 2065 6e64 6966 2025 7d3c 2f73  }}{% endif %}</s
-00000c50: 7061 6e3e 0a20 2020 2020 2020 203c 2f64  pan>.        </d
-00000c60: 6976 3e0a 2020 2020 3c2f 6469 763e 0a20  iv>.    </div>. 
-00000c70: 2020 203c 6469 7620 636c 6173 733d 2264     <div class="d
-00000c80: 2d66 6c65 7820 616c 6967 6e2d 6974 656d  -flex align-item
-00000c90: 732d 6365 6e74 6572 206a 7573 7469 6679  s-center justify
-00000ca0: 2d63 6f6e 7465 6e74 2d62 6574 7765 656e  -content-between
-00000cb0: 223e 0a20 2020 2020 2020 203c 703e 3c69  ">.        <p><i
-00000cc0: 2063 6c61 7373 3d22 6661 2066 612d 7573   class="fa fa-us
-00000cd0: 6572 2d63 6972 636c 652d 6f20 7465 7874  er-circle-o text
-00000ce0: 2d73 7563 6365 7373 2220 6172 6961 2d68  -success" aria-h
-00000cf0: 6964 6465 6e3d 2274 7275 6522 3e3c 2f69  idden="true"></i
-00000d00: 3e20 7b7b 2067 7569 6c64 2e6f 6e6c 696e  > {{ guild.onlin
-00000d10: 655f 6e75 6d62 6572 207d 7d3c 6272 202f  e_number }}<br /
-00000d20: 3e3c 6920 636c 6173 733d 2266 6120 6661  ><i class="fa fa
-00000d30: 2d75 7365 722d 6369 7263 6c65 2d6f 2074  -user-circle-o t
-00000d40: 6578 742d 7761 726e 696e 6722 2061 7269  ext-warning" ari
-00000d50: 612d 6869 6464 656e 3d22 7472 7565 223e  a-hidden="true">
-00000d60: 3c2f 693e 207b 7b20 6775 696c 642e 6964  </i> {{ guild.id
-00000d70: 6c65 5f6e 756d 6265 7220 7d7d 3c62 7220  le_number }}<br 
-00000d80: 2f3e 3c62 7220 2f3e 3c69 2063 6c61 7373  /><br /><i class
-00000d90: 3d22 6661 2066 612d 6861 7368 7461 6720  ="fa fa-hashtag 
-00000da0: 7465 7874 2d73 6563 6f6e 6461 7279 2220  text-secondary" 
-00000db0: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
-00000dc0: 6522 3e3c 2f69 3e20 7b7b 2067 7569 6c64  e"></i> {{ guild
-00000dd0: 2e74 6578 745f 6368 616e 6e65 6c73 5f6e  .text_channels_n
-00000de0: 756d 6265 7220 7d7d 3c2f 703e 0a20 2020  umber }}</p>.   
-00000df0: 2020 2020 203c 7020 7374 796c 653d 226d       <p style="m
-00000e00: 6172 6769 6e2d 6c65 6674 3a20 3230 7078  argin-left: 20px
-00000e10: 3b22 3e3c 6920 636c 6173 733d 2266 6120  ;"><i class="fa 
-00000e20: 6661 2d75 7365 722d 6369 7263 6c65 2d6f  fa-user-circle-o
-00000e30: 2074 6578 742d 6461 6e67 6572 2220 6172   text-danger" ar
-00000e40: 6961 2d68 6964 6465 6e3d 2274 7275 6522  ia-hidden="true"
-00000e50: 3e3c 2f69 3e20 7b7b 2067 7569 6c64 2e64  ></i> {{ guild.d
-00000e60: 6e64 5f6e 756d 6265 7220 7d7d 3c62 7220  nd_number }}<br 
-00000e70: 2f3e 3c69 2063 6c61 7373 3d22 6661 2066  /><i class="fa f
-00000e80: 612d 7573 6572 2d63 6972 636c 652d 6f20  a-user-circle-o 
-00000e90: 7465 7874 2d73 6563 6f6e 6461 7279 2220  text-secondary" 
-00000ea0: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
-00000eb0: 6522 3e3c 2f69 3e20 7b7b 2067 7569 6c64  e"></i> {{ guild
-00000ec0: 2e6f 6666 6c69 6e65 5f6e 756d 6265 7220  .offline_number 
-00000ed0: 7d7d 3c62 7220 2f3e 3c62 7220 2f3e 3c69  }}<br /><br /><i
-00000ee0: 2063 6c61 7373 3d22 6661 2066 612d 766f   class="fa fa-vo
-00000ef0: 6c75 6d65 2d75 7020 7465 7874 2d73 6563  lume-up text-sec
-00000f00: 6f6e 6461 7279 2220 6172 6961 2d68 6964  ondary" aria-hid
-00000f10: 6465 6e3d 2274 7275 6522 3e3c 2f69 3e20  den="true"></i> 
-00000f20: 7b7b 2067 7569 6c64 2e76 6f69 6365 5f63  {{ guild.voice_c
-00000f30: 6861 6e6e 656c 735f 6e75 6d62 6572 207d  hannels_number }
-00000f40: 7d3c 2f70 3e0a 2020 2020 3c2f 6469 763e  }</p>.    </div>
-00000f50: 0a0a 2020 2020 3c68 3620 636c 6173 733d  ..    <h6 class=
-00000f60: 2274 6578 742d 7365 636f 6e64 6172 7922  "text-secondary"
-00000f70: 2073 7479 6c65 3d22 6d61 7267 696e 2d62   style="margin-b
-00000f80: 6f74 746f 6d3a 2030 7265 6d3b 223e 7b7b  ottom: 0rem;">{{
-00000f90: 205f 2822 4372 6561 7465 6420 6174 3a22   _("Created at:"
-00000fa0: 2920 7d7d 207b 7b20 6d6f 6d65 6e74 2867  ) }} {{ moment(g
-00000fb0: 7569 6c64 2e63 7265 6174 6564 5f61 7429  uild.created_at)
-00000fc0: 2e66 6f72 6d61 7428 2244 6f20 4d4d 4d4d  .format("Do MMMM
-00000fd0: 2059 5959 5922 2920 7d7d 3c2f 6836 3e0a   YYYY") }}</h6>.
-00000fe0: 2020 2020 7b25 2069 6620 6775 696c 642e      {% if guild.
-00000ff0: 6a6f 696e 6564 5f61 7420 257d 0a20 2020  joined_at %}.   
-00001000: 2020 2020 203c 6836 2063 6c61 7373 3d22       <h6 class="
-00001010: 7465 7874 2d73 6563 6f6e 6461 7279 223e  text-secondary">
-00001020: 7b7b 205f 2822 426f 7420 6a6f 696e 6564  {{ _("Bot joined
-00001030: 2061 743a 2229 207d 7d20 7b7b 206d 6f6d   at:") }} {{ mom
-00001040: 656e 7428 6775 696c 642e 6a6f 696e 6564  ent(guild.joined
-00001050: 5f61 7429 2e66 6f72 6d61 7428 2244 6f20  _at).format("Do 
-00001060: 4d4d 4d4d 2059 5959 5922 2920 7d7d 3c2f  MMMM YYYY") }}</
-00001070: 6836 3e0a 2020 2020 7b25 2065 6e64 6966  h6>.    {% endif
-00001080: 2025 7d0a 3c2f 6469 763e 0a20 2020 2020   %}.</div>.     
-00001090: 2020 2020 2020 200a 7b25 2062 6c6f 636b         .{% block
-000010a0: 206a 6176 6173 6372 6970 7473 2025 7d7b   javascripts %}{
-000010b0: 2520 656e 6462 6c6f 636b 2025 7d0a       % endblock %}.
+00000420: 2020 2020 2020 2020 3c2f 613e 0a20 2020          </a>.   
+00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000440: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
+00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000460: 2020 203c 6c69 2063 6c61 7373 3d22 6e61     <li class="na
+00000470: 762d 6974 656d 223e 0a20 2020 2020 2020  v-item">.       
+00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000490: 2020 2020 203c 6120 6872 6566 3d22 7b7b       <a href="{{
+000004a0: 2075 726c 5f66 6f72 2822 6261 7365 5f62   url_for("base_b
+000004b0: 6c75 6570 7269 6e74 2e64 6173 6862 6f61  lueprint.dashboa
+000004c0: 7264 5f67 7569 6c64 222c 2067 7569 6c64  rd_guild", guild
+000004d0: 5f69 643d 6775 696c 642e 6964 2c20 7061  _id=guild.id, pa
+000004e0: 6765 3d22 7365 7474 696e 6773 2229 207d  ge="settings") }
+000004f0: 7d22 2063 6c61 7373 3d22 6e61 762d 6c69  }" class="nav-li
+00000500: 6e6b 223e 0a20 2020 2020 2020 2020 2020  nk">.           
+00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000520: 2020 2020 203c 6920 636c 6173 733d 226e       <i class="n
+00000530: 6920 6e69 2d73 6574 7469 6e67 732d 6765  i ni-settings-ge
+00000540: 6172 2d36 3520 6f70 6163 6974 792d 3130  ar-65 opacity-10
+00000550: 2220 7374 796c 653d 2276 6572 7469 6361  " style="vertica
+00000560: 6c2d 616c 6967 6e3a 202d 312e 3570 783b  l-align: -1.5px;
+00000570: 223e 3c2f 693e 207b 7b20 5f28 2253 6574  "></i> {{ _("Set
+00000580: 7469 6e67 7322 2920 7d7d 0a20 2020 2020  tings") }}.     
+00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005a0: 2020 2020 2020 203c 2f61 3e0a 2020 2020         </a>.    
+000005b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005c0: 2020 2020 3c2f 6c69 3e0a 2020 2020 2020      </li>.      
+000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005e0: 2020 3c6c 6920 636c 6173 733d 226e 6176    <li class="nav
+000005f0: 2d69 7465 6d22 3e0a 2020 2020 2020 2020  -item">.        
+00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000610: 2020 2020 3c61 2068 7265 663d 227b 7b20      <a href="{{ 
+00000620: 7572 6c5f 666f 7228 2262 6173 655f 626c  url_for("base_bl
+00000630: 7565 7072 696e 742e 6461 7368 626f 6172  ueprint.dashboar
+00000640: 645f 6775 696c 6422 2c20 6775 696c 645f  d_guild", guild_
+00000650: 6964 3d67 7569 6c64 2e69 642c 2070 6167  id=guild.id, pag
+00000660: 653d 2274 6869 7264 2d70 6172 7469 6573  e="third-parties
+00000670: 2229 207d 7d22 2063 6c61 7373 3d22 6e61  ") }}" class="na
+00000680: 762d 6c69 6e6b 2073 686f 7720 6163 7469  v-link show acti
+00000690: 7665 2220 6964 3d22 7468 6972 642d 7061  ve" id="third-pa
+000006a0: 7274 6965 732d 7461 6222 3e0a 2020 2020  rties-tab">.    
+000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006c0: 2020 2020 2020 2020 2020 2020 3c69 2063              <i c
+000006d0: 6c61 7373 3d22 6e69 206e 692d 6275 6c6c  lass="ni ni-bull
+000006e0: 6574 2d6c 6973 742d 3637 206f 7061 6369  et-list-67 opaci
+000006f0: 7479 2d31 3022 2073 7479 6c65 3d22 7665  ty-10" style="ve
+00000700: 7274 6963 616c 2d61 6c69 676e 3a20 2d31  rtical-align: -1
+00000710: 2e35 7078 3b22 3e3c 2f69 3e20 7b7b 205f  .5px;"></i> {{ _
+00000720: 2822 5468 6972 6420 5061 7274 6965 7322  ("Third Parties"
+00000730: 2920 7d7d 0a20 2020 2020 2020 2020 2020  ) }}.           
+00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000750: 203c 2f61 3e0a 2020 2020 2020 2020 2020   </a>.          
+00000760: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000770: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
+00000780: 2020 2020 2020 2020 3c2f 756c 3e0a 2020          </ul>.  
+00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007a0: 2020 3c62 7220 2f3e 0a20 2020 2020 2020    <br />.       
+000007b0: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+000007c0: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
+000007d0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000007e0: 2274 6162 2d63 6f6e 7465 6e74 2220 6964  "tab-content" id
+000007f0: 3d22 6372 6561 746f 722d 7461 6243 6f6e  ="creator-tabCon
+00000800: 7465 6e74 223e 0a20 2020 2020 2020 2020  tent">.         
+00000810: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00000820: 636c 6173 733d 2274 6162 2d70 616e 6520  class="tab-pane 
+00000830: 6661 6465 2073 686f 7720 6163 7469 7665  fade show active
+00000840: 2220 6964 3d22 7468 6972 642d 7061 7274  " id="third-part
+00000850: 6965 7322 2072 6f6c 653d 2274 6162 7061  ies" role="tabpa
+00000860: 6e65 6c22 2061 7269 612d 6c61 6265 6c6c  nel" aria-labell
+00000870: 6564 6279 3d22 7468 6972 642d 7061 7274  edby="third-part
+00000880: 6965 732d 7461 6222 3e0a 2020 2020 2020  ies-tab">.      
+00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008a0: 2020 3c64 6976 2063 6c61 7373 3d22 6361    <div class="ca
+000008b0: 7264 2063 6172 642d 6368 6172 7422 3e0a  rd card-chart">.
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000008e0: 2063 6c61 7373 3d22 6361 7264 2d62 6f64   class="card-bod
+000008f0: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
+00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000910: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00000920: 726f 7722 3e0a 2020 2020 2020 2020 2020  row">.          
+00000930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000940: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000950: 6c61 7373 3d22 636f 6c2d 736d 2d31 3220  lass="col-sm-12 
+00000960: 7465 7874 2d6c 6566 7422 3e0a 2020 2020  text-left">.    
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000009a0: 642d 666c 6578 206a 7573 7469 6679 2d63  d-flex justify-c
+000009b0: 6f6e 7465 6e74 2d62 6574 7765 656e 206d  ontent-between m
+000009c0: 622d 3422 3e0a 2020 2020 2020 2020 2020  b-4">.          
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 2020 7b25 2069 6620 6775 696c 6420 257d    {% if guild %}
+00000a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 207b 2520 6966 206e 6f74 2066 756c 6c73   {% if not fulls
+00000a40: 6372 6565 6e20 257d 0a20 2020 2020 2020  creen %}.       
+00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a70: 2020 2020 2020 2020 2020 2020 203c 6832               <h2
+00000a80: 2063 6c61 7373 3d22 6361 7264 2d74 6974   class="card-tit
+00000a90: 6c65 223e 3c61 2068 7265 663d 227b 7b20  le"><a href="{{ 
+00000aa0: 7572 6c5f 666f 7228 2262 6173 655f 626c  url_for("base_bl
+00000ab0: 7565 7072 696e 742e 6461 7368 626f 6172  ueprint.dashboar
+00000ac0: 645f 6775 696c 6422 2c20 6775 696c 645f  d_guild", guild_
+00000ad0: 6964 3d67 7569 6c64 2e69 642c 2070 6167  id=guild.id, pag
+00000ae0: 653d 2274 6869 7264 2d70 6172 7469 6573  e="third-parties
+00000af0: 222c 2074 6869 7264 5f70 6172 7479 3d6e  ", third_party=n
+00000b00: 616d 6529 207d 7d22 3ef0 9f94 9920 7b7b  ame) }}">.... {{
+00000b10: 206e 616d 6520 7d7d 3c2f 613e 3c2f 6832   name }}</a></h2
+00000b20: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
+00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 203c 6832 2063 6c61 7373 3d22 6361 7264   <h2 class="card
+00000ba0: 2d74 6974 6c65 223e 3c61 2068 7265 663d  -title"><a href=
+00000bb0: 227b 7b20 7572 6c5f 666f 7228 2262 6173  "{{ url_for("bas
+00000bc0: 655f 626c 7565 7072 696e 742e 6461 7368  e_blueprint.dash
+00000bd0: 626f 6172 645f 6775 696c 6422 2c20 6775  board_guild", gu
+00000be0: 696c 645f 6964 3d67 7569 6c64 2e69 6429  ild_id=guild.id)
+00000bf0: 207d 7d22 3e3c 696d 6720 7372 633d 227b   }}"><img src="{
+00000c00: 7b20 6775 696c 642e 6963 6f6e 5f75 726c  { guild.icon_url
+00000c10: 207d 7d22 2073 7479 6c65 3d22 6865 6967   }}" style="heig
+00000c20: 6874 3a20 3530 7078 3b20 7665 7274 6963  ht: 50px; vertic
+00000c30: 616c 2d61 6c69 676e 3a20 2d31 3370 783b  al-align: -13px;
+00000c40: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
+00000c50: 3530 253b 206d 6172 6769 6e3a 206e 6f6e  50%; margin: non
+00000c60: 653b 2064 6973 706c 6179 3a20 696e 6c69  e; display: inli
+00000c70: 6e65 3b22 202f 3e20 7b7b 2067 7569 6c64  ne;" /> {{ guild
+00000c80: 2e6e 616d 6520 7d7d 3c2f 613e 202f 203c  .name }}</a> / <
+00000c90: 6120 6872 6566 3d22 7b7b 2075 726c 5f66  a href="{{ url_f
+00000ca0: 6f72 2822 6261 7365 5f62 6c75 6570 7269  or("base_bluepri
+00000cb0: 6e74 2e64 6173 6862 6f61 7264 5f67 7569  nt.dashboard_gui
+00000cc0: 6c64 222c 2067 7569 6c64 5f69 643d 6775  ld", guild_id=gu
+00000cd0: 696c 642e 6964 2c20 7061 6765 3d22 7468  ild.id, page="th
+00000ce0: 6972 642d 7061 7274 6965 7322 2c20 7468  ird-parties", th
+00000cf0: 6972 645f 7061 7274 793d 6e61 6d65 2920  ird_party=name) 
+00000d00: 7d7d 223e f09f 9499 207b 7b20 6e61 6d65  }}">.... {{ name
+00000d10: 207d 7d3c 2f61 3e3c 2f68 323e 0a20 2020   }}</a></h2>.   
+00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d40: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00000d50: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 2020 2020 207b 2520 656c 7365 2025 7d0a       {% else %}.
+00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dc0: 3c68 3220 636c 6173 733d 2263 6172 642d  <h2 class="card-
+00000dd0: 7469 746c 6522 3e3c 6120 6872 6566 3d22  title"><a href="
+00000de0: 7b7b 2075 726c 5f66 6f72 2822 7468 6972  {{ url_for("thir
+00000df0: 645f 7061 7274 6965 735f 626c 7565 7072  d_parties_bluepr
+00000e00: 696e 742e 7468 6972 645f 7061 7274 6965  int.third_partie
+00000e10: 7322 2c20 7468 6972 645f 7061 7274 793d  s", third_party=
+00000e20: 6e61 6d65 2920 7d7d 223e f09f 9499 207b  name) }}">.... {
+00000e30: 7b20 6e61 6d65 207d 7d3c 2f61 3e3c 2f68  { name }}</a></h
+00000e40: 323e 0a20 2020 2020 2020 2020 2020 2020  2>.             
+00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e60: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000e70: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ea0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000ed0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ef0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f10: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00000f20: 2063 6c61 7373 3d22 636f 6e74 6169 6e65   class="containe
+00000f30: 7220 6d74 2d34 2064 2d66 6c65 7822 3e0a  r mt-4 d-flex">.
+00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f60: 2020 2020 7b7b 2073 6f75 7263 655f 636f      {{ source_co
+00000f70: 6e74 656e 747c 7361 6665 207d 7d0a 2020  ntent|safe }}.  
+00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f90: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000fa0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fc0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000ff0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00001000: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001010: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00001020: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00001030: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
+00001040: 2f64 6976 3e0a 2020 3c2f 6d61 696e 3e0a  /div>.  </main>.
+00001050: 7b25 2065 6e64 626c 6f63 6b20 257d 0a0a  {% endblock %}..
+00001060: 7b25 2062 6c6f 636b 206a 6176 6173 6372  {% block javascr
+00001070: 6970 7473 2025 7d0a 2020 2020 3c73 6372  ipts %}.    <scr
+00001080: 6970 743e 0a20 2020 2020 2020 2066 756e  ipt>.        fun
+00001090: 6374 696f 6e20 6368 616e 6765 5061 6765  ction changePage
+000010a0: 2870 6167 6529 207b 0a20 2020 2020 2020  (page) {.       
+000010b0: 2020 2020 2076 6172 2074 6162 5f6e 6176       var tab_nav
+000010c0: 5f6c 696e 6b20 3d20 646f 6375 6d65 6e74  _link = document
+000010d0: 2e71 7565 7279 5365 6c65 6374 6f72 2822  .querySelector("
+000010e0: 2322 202b 2070 6167 6520 2b20 222d 7461  #" + page + "-ta
+000010f0: 6222 293b 0a20 2020 2020 2020 2020 2020  b");.           
+00001100: 2069 6620 2874 6162 5f6e 6176 5f6c 696e   if (tab_nav_lin
+00001110: 6b29 207b 0a20 2020 2020 2020 2020 2020  k) {.           
+00001120: 2020 2020 2074 6162 5f6e 6176 5f6c 696e       tab_nav_lin
+00001130: 6b2e 7061 7265 6e74 456c 656d 656e 742e  k.parentElement.
+00001140: 7061 7265 6e74 456c 656d 656e 742e 6f6e  parentElement.on
+00001150: 6d6f 7573 656f 7665 7228 7461 625f 6e61  mouseover(tab_na
+00001160: 765f 6c69 6e6b 293b 0a20 2020 2020 2020  v_link);.       
+00001170: 2020 2020 2020 2020 2074 6162 5f6e 6176           tab_nav
+00001180: 5f6c 696e 6b2e 6469 7370 6174 6368 4576  _link.dispatchEv
+00001190: 656e 7428 6e65 7720 4576 656e 7428 2263  ent(new Event("c
+000011a0: 6c69 636b 2229 293b 0a20 2020 2020 2020  lick"));.       
+000011b0: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+000011c0: 0a20 2020 2020 2020 2064 6f63 756d 656e  .        documen
+000011d0: 742e 6164 6445 7665 6e74 4c69 7374 656e  t.addEventListen
+000011e0: 6572 2822 444f 4d43 6f6e 7465 6e74 4c6f  er("DOMContentLo
+000011f0: 6164 6564 222c 2066 756e 6374 696f 6e28  aded", function(
+00001200: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00001210: 6368 616e 6765 5061 6765 2822 7468 6972  changePage("thir
+00001220: 642d 7061 7274 6965 7322 293b 0a20 2020  d-parties");.   
+00001230: 2020 2020 207d 293b 0a20 2020 203c 2f73       });.    </s
+00001240: 6372 6970 743e 0a7b 2520 656e 6462 6c6f  cript>.{% endblo
+00001250: 636b 2025 7d0a                           ck %}.
```

### Comparing `red_web_dashboard-1.1/reddash/app/templates/pages/index.html` & `red_web_dashboard-1.2.0/reddash/app/templates/pages/index.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/pages/login/login.html` & `red_web_dashboard-1.2.0/reddash/app/templates/pages/login/login.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/oauth.html` & `red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/oauth.html`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                     <p>{{ _("Successfully forwarded your account informations. You may now close this tab and go back to Discord.") }}</p>
                     <img src="{{ config.ASSETS_ROOT }}/oauth.png" height="250" />
                     <br /><br />
                     <a class="btn bg-gradient-success mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
                   </div>
                 </div>
                 <div class="card-footer">
-                  {{ _('This is a Third Party integration. By using this application, you acknowledge that you have read the Third Party disclaimer found <a href="{link}">here</a>').format(link="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Third%20Parties%20Disclaimer.md") }}
+                  {{ _('This is a Third Party integration. By using this application, you acknowledge that you have read the Third Party disclaimer found <a href="{link}">here</a>.').format(link="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Third%20Parties%20Disclaimer.md") }}
                 </div>
               </div>
             </div>
           </div>
         </div>
       </div>
     </div>
```

#### html2text {}

```diff
@@ -3,11 +3,11 @@
 ************ {{{{ pprroovviiddeerr||ttiittllee }}}} {{{{ __((""OOAAuutthh"")) }}}} ************
 {{ _("Successfully forwarded your account informations. You may now close this
 tab and go back to Discord.") }}
 [{{ config.ASSETS_ROOT }}/oauth.png]
 
 }">{{ _("Back to Home") }}
 {{ _('This is a Third Party integration. By using this application, you
-acknowledge that you have read the Third Party disclaimer found _h_e_r_e').format
+acknowledge that you have read the Third Party disclaimer found _h_e_r_e.').format
 (link="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/
 Third%20Parties%20Disclaimer.md") }}
 {% endblock %} {% block javascripts %}{% endblock %}
```

### Comparing `red_web_dashboard-1.1/reddash/app/templates/pages/third_parties/third_parties_list.html` & `red_web_dashboard-1.2.0/reddash/app/templates/pages/third_parties/third_parties_list.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/third_parties/routes.py` & `red_web_dashboard-1.2.0/reddash/app/third_parties/routes.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.1/reddash/app/utils.py` & `red_web_dashboard-1.2.0/reddash/app/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 from flask_login import LoginManager, UserMixin, current_user
 from flask_login import login_url as make_login_url
 from flask_moment import Moment
 from flask_sitemapper import Sitemapper
 from flask_talisman import Talisman
 from flask_wtf.csrf import CSRFProtect
 from flask_wtf.file import FileAllowed, FileField, MultipleFileField
+from wtforms import Field, SelectFieldBase, FormField
 from fuzzywuzzy import process
 from markdown import Markdown
 import bleach
 from markupsafe import Markup
-from wtforms import Field, SelectFieldBase
 
 settings.configure()
 from django_user_agents.utils import get_user_agent
 
 AVAILABLE_COLORS: typing.List[str] = [
     "success",
     "danger",
@@ -213,14 +213,16 @@
         g.csrf_valid = False
 
     app.csrf_protect.protect = protect
     initial_init = Field.__init__
 
     def init_field(field, *args, **kwargs):
         initial_init(field, *args, **kwargs)
+        if isinstance(field, FormField):
+            return
         if hasattr(field, "_value"):
             field._real_value = field._value
         field._value = lambda: (field._real_value() if hasattr(field, "_real_value") else "") or (
             (str(field.default) if not isinstance(field.default, typing.List) else field.default)
             if field.default
             else ""
         )
@@ -252,16 +254,14 @@
                     ),
                     None,
                 )
             ) is not None:
                 field.flags.accept = ", ".join(
                     [f".{extension}" for extension in file_allowed.upload_set]
                 )
-        if request.endpoint == "creators_blueprint.creator":
-            field.label.text = field.label.text.replace(_("l'utilisateur"), _("le créateur"))
 
     Field.__init__ = init_field
 
     app.bootstrap: Bootstrap = Bootstrap()
     app.bootstrap.init_app(app)
 
     app.moment: Moment = Moment()
@@ -412,15 +412,16 @@
         new_query_params = {k: v if isinstance(v, str) else v for k, v in query_params.items()}
         new_query_string = urlencode(new_query_params, doseq=True, quote_via=quote_plus).replace(
             "amp%3B", ""
         )
         updated_url_components = url_components._replace(query=new_query_string)
         if _anchor is not None:
             updated_url_components = updated_url_components._replace(fragment=_anchor)
-        return urlunparse(updated_url_components)
+        relative_url = urlunparse(updated_url_components._replace(scheme="", netloc="", params="", fragment=""))
+        return relative_url
 
     def number_to_text_with_suffix(number: float) -> str:
         suffixes = [
             "k",
             "m",
             "b",
             "t",
@@ -642,15 +643,14 @@
         return False
     return True
 
 
 async def get_result(app: Flask, request: typing.Dict[str, typing.Any]):
     if app.cog is not None:
         from aiohttp_json_rpc.protocol import JsonRpcMsg, JsonRpcMsgTyp
-
         try:
             method = app.cog.bot.rpc._rpc.methods[request["method"]]
         except KeyError:
             return {"status": 1, "message": _("Not connected to bot.")}
         result = await method(
             http_request="GET",
             rpc=app.cog.bot.rpc._rpc,
@@ -660,15 +660,15 @@
     app.ws.send(json.dumps(request))
     result = json.loads(app.ws.recv())
     if "error" in result:
         if result["error"]["message"] == "Method not found":
             return {"status": 1, "message": _("Not connected to bot.")}
         app.logger.error(result["error"])
         return {"status": 1, "message": _("Something went wrong.")}
-    if isinstance(result["result"], dict) and result["result"].get("disconnected", False):
+    if not result["result"] or isinstance(result["result"], typing.Dict) and result["result"].get("disconnected", False):
         return {"status": 1, "message": _("Not connected to bot.")}
     return result["result"]
 
 
 def notify_owner_of_blacklist(app: Flask, ip: str) -> None:
     while True:
         if app.cog is not None or app.ws and app.ws.connected:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `red_web_dashboard-1.1/setup.cfg` & `red_web_dashboard-1.2.0/setup.cfg`

 * *Files identical despite different names*

