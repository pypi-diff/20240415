# Comparing `tmp/airbyte_source_shopify-2.0.5.dev202404132257.tar.gz` & `tmp/airbyte_source_shopify-2.0.5.dev202404151411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.0.5.dev202404132257.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.0.5.dev202404151411.tar", max compression
```

## Comparing `airbyte_source_shopify-2.0.5.dev202404132257.tar` & `airbyte_source_shopify-2.0.5.dev202404151411.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4519 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/README.md
--rw-r--r--   0        0        0      812 2024-04-13 22:57:27.729467 airbyte_source_shopify-2.0.5.dev202404132257/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/run.py
--rw-r--r--   0        0        0    16103 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     1272 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     1009 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     1109 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0      928 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0      610 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     1170 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     1488 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     1217 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      485 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0     5313 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0      736 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0      909 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    13381 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     5226 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    14757 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     1027 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0      536 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     1329 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0      911 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    17520 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0      728 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0    80187 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     1104 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     3891 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0      907 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     2336 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0     7060 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     1675 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     4059 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0      985 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0      951 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     3750 2024-04-13 22:55:09.758199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-04-13 22:55:09.762199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/scopes.py
--rw-r--r--   0        0        0     1734 2024-04-13 22:55:09.762199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    18577 2024-04-13 22:55:09.762199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    56188 2024-04-13 22:55:09.762199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6517 2024-04-13 22:55:09.762199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     3629 2024-04-13 22:55:09.762199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-04-13 22:55:09.762199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-04-13 22:55:09.770199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8540 2024-04-13 22:55:09.770199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-04-13 22:55:09.770199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/spec.json
--rw-r--r--   0        0        0    37655 2024-04-13 22:55:09.770199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11968 2024-04-13 22:55:09.770199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-04-13 22:55:09.770199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/transform.py
--rw-r--r--   0        0        0    14320 2024-04-13 22:55:09.770199 airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/utils.py
--rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.5.dev202404132257/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-04-15 14:08:14.682491 airbyte_source_shopify-2.0.5.dev202404151411/README.md
+-rw-r--r--   0        0        0      812 2024-04-15 14:11:06.634669 airbyte_source_shopify-2.0.5.dev202404151411/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/run.py
+-rw-r--r--   0        0        0    16103 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     1272 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     1009 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     1109 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0      928 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0      610 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     1170 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     1488 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     1217 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      485 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0     5313 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0      736 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0      909 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    13381 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     5226 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    14757 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     1027 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0      536 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     1329 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    17520 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0      728 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0    80187 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     1104 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     3891 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0      907 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     2336 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0     7060 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     1675 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     4059 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0      985 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0      951 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     3750 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/scopes.py
+-rw-r--r--   0        0        0     1734 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    19666 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    56188 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6517 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     3629 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8540 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/spec.json
+-rw-r--r--   0        0        0    37308 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11968 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/transform.py
+-rw-r--r--   0        0        0    13944 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/utils.py
+-rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.5.dev202404151411/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/README.md` & `airbyte_source_shopify-2.0.5.dev202404151411/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/pyproject.toml` & `airbyte_source_shopify-2.0.5.dev202404151411/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.5.dev202404132257"
+version = "2.0.5.dev202404151411"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/__init__.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/auth.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/inventory_levels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/order_risks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/smart_collections.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/tender_transactions.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/tender_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/scopes.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import logging
 from dataclasses import dataclass, field
+from datetime import datetime
 from enum import Enum
 from time import sleep, time
 from typing import Any, Final, Iterable, List, Mapping, Optional, Union
 
 import pendulum as pdm
 import requests
 from airbyte_cdk import AirbyteLogger
@@ -39,34 +40,30 @@
 
     # default logger
     logger: Final[AirbyteLogger] = logging.getLogger("airbyte")
 
     # 10Mb chunk size to save the file
     retrieve_chunk_size: Final[int] = 1024 * 1024 * 10
     # time between job status checks
-    job_check_interval_sec: Final[int] = 5
-
-    # PLATFORM HEARTBEAT NOTES:
-    # 30 sec / attempt * 19 attempts = 570 sec of wait time in total,
-    # which is < 10 min of retrying, before Heartbeat will kill the source as non-responsive
+    job_check_interval_sec: Final[int] = 2
 
     # sleep time per creation attempt
     concurrent_interval_sec: Final[int] = 30
     # max attempts for job creation
-    concurrent_max_retry: Final[int] = 19
+    concurrent_max_retry: Final[int] = 30
     # Each job ideally should be executed within the specified time (in sec),
-    # to maximize the performance for multi-connection syncs and control the bulk job size within +- 7 mins (420 sec),
+    # to maximize the performance for multi-connection syncs and control the bulk job size within +- 10 mins (600 sec),
     # Ideally the source will balance on it's own rate, based on the time taken to return the data for the slice.
-    job_max_elapsed_time_sec: Final[float] = 420.0
+    job_max_elapsed_time_sec: Final[float] = 600.0
     # 0.1 ~= P2H, default value, lower boundary for slice size
     job_size_min: Final[float] = 0.1
     # P365D, upper boundary for slice size
     job_size_max: Final[float] = 365.0
     # running job logger constrain
-    log_job_state_msg_frequency: Final[int] = 3
+    log_job_state_msg_frequency: Final[int] = 10
     # attempt limit indicator
     concurrent_max_attempt_reached: bool = field(init=False, default=False)
     # attempt counter
     concurrent_attempt: int = field(init=False, default=0)
     # currents: job_id, job_state, job_created_at, job_self_canceled
     job_id: Optional[str] = field(init=False, default=None)
     job_created_at: Optional[str] = field(init=False, default=None)
@@ -132,90 +129,113 @@
     @property
     def is_long_running_job(self) -> bool:
         if self.job_elapsed_time_in_state:
             if self.job_elapsed_time_in_state > self.job_max_elapsed_time_sec:
                 # set the slicer to revert mode
                 self.job_should_revert_slice = True
                 return True
-        else:
-            # reset slicer to normal mode
-            self.job_should_revert_slice = False
-            return False
+        # reset slicer to normal mode
+        self.job_should_revert_slice = False
+        return False
 
     def expand_job_size(self) -> None:
         self.job_size += self.job_size_adjusted_expand_factor
 
     def reduce_job_size(self) -> None:
         self.job_size /= self.job_size_adjusted_reduce_factor
 
+    def job_size_normalize(self, start: datetime, end: datetime) -> datetime:
+        # adjust slice size when it's bigger than the loop point when it should end,
+        # to preserve correct job size adjustments when this is the only job we need to run, based on STATE provided
+        requested_slice_size = (end - start).total_days()
+        self.job_size = requested_slice_size if requested_slice_size < self.job_size else self.job_size
+
+    def get_adjusted_job_end(self, slice_start: datetime, slice_end: datetime) -> datetime:
+        if self.is_long_running_job:
+            self._job_size_reduce_next()
+            return slice_start
+        else:
+            return slice_end
+
+    def get_adjusted_job_start(self, slice_start: datetime) -> datetime:
+        step = self.job_size if self.job_size else self.job_size_min
+        return slice_start.add(days=step)
+
+    def _job_size_reduce_next(self) -> None:
+        # revert the flag
+        self.job_should_revert_slice = False
+        self.reduce_job_size()
+
     def __adjust_job_size(self, job_current_elapsed_time: float) -> None:
-        if not self.job_should_revert_slice:
-            if job_current_elapsed_time > self.job_max_elapsed_time_sec:
-                self.reduce_job_size()
-            elif job_current_elapsed_time < 1 or job_current_elapsed_time < self.job_last_elapsed_time:
+        if self.job_should_revert_slice:
+            pass
+        else:
+            if job_current_elapsed_time < 1 or job_current_elapsed_time < self.job_last_elapsed_time:
                 self.expand_job_size()
             elif job_current_elapsed_time > self.job_last_elapsed_time < self.job_max_elapsed_time_sec:
                 pass
-
             # set the last job time
             self.job_last_elapsed_time = job_current_elapsed_time
             # check the job size slice interval are acceptable
             self.job_size = max(self.job_size_min, min(self.job_size, self.job_size_max))
-        else:
-            pass
 
     def __reset_state(self) -> None:
         # set current job state to default values
-        self.job_state, self.job_id, self.job_self_canceled = None, None, False
+        self.job_state, self.job_id = None, None
+        # setting self-cancelation to default
+        self.job_self_canceled = False
         # set the running job message counter to default
         self.log_job_state_msg_count = 0
 
     def job_completed(self) -> bool:
         return self.job_state == ShopifyBulkStatus.COMPLETED.value
 
     def job_canceled(self) -> bool:
         return self.job_state == ShopifyBulkStatus.CANCELED.value
 
-    def job_cancel(self) -> requests.Response:
+    def job_cancel(self) -> None:
         # re-use of `self._session(*, **)` to make BULK Job cancel request
         cancel_args = self.job_get_request_args(ShopifyBulkTemplates.cancel)
         with self.session as cancel_job:
+            self.logger.warn(f"CANCELING THE JOB: {self.job_id}")
             canceled_response = cancel_job.request(**cancel_args)
             # mark the job was self-canceled
             self.job_self_canceled = True
-            return self.job_healthcheck(canceled_response)
+            # check CANCELED Job health
+            self.job_healthcheck(canceled_response)
 
     def log_job_state_with_count(self) -> None:
         """
         Print the status/state Job info message every N request, to minimize the noise in the logs.
         """
         if self.log_job_state_msg_count < self.log_job_state_msg_frequency:
             self.log_job_state_msg_count += 1
         else:
             message = f"Elapsed time: {self.job_elapsed_time_in_state} sec"
             self.log_state(message)
             self.log_job_state_msg_count = 0
 
     def log_state(self, message: Optional[str] = None) -> None:
-        pattern = f"Stream: `{self.stream_name}`, the BULK Job: `{self.job_id}` is {self.job_state}."
+        pattern = f"Stream: `{self.stream_name}`, the BULK Job: `{self.job_id}` is {self.job_state}"
         if message:
             self.logger.info(f"{pattern}. {message}.")
         else:
             self.logger.info(pattern)
 
     def job_get_request_args(self, template: ShopifyBulkTemplates) -> Mapping[str, Any]:
         return {
             "method": "POST",
             "url": self.base_url,
             "data": template(self.job_id),
             "headers": {"Content-Type": "application/graphql"},
         }
 
     def job_get_result(self, response: Optional[requests.Response] = None) -> Optional[str]:
-        job_result_url = response.json().get("data", {}).get("node", {}).get("url") if response else None
+        parsed_response = response.json().get("data", {}).get("node", {}) if response else None
+        job_result_url = parsed_response.get("url") if parsed_response and not self.job_self_canceled else None
         if job_result_url:
             # save to local file using chunks to avoid OOM
             filename = self.tools.filename_from_url(job_result_url)
             with self.session.get(job_result_url, stream=True) as response:
                 response.raise_for_status()
                 with open(filename, "wb") as file:
                     for chunk in response.iter_content(chunk_size=self.retrieve_chunk_size):
@@ -245,17 +265,19 @@
 
     def on_canceling_job(self, **kwargs) -> None:
         sleep(self.job_check_interval_sec)
 
     def on_running_job(self, **kwargs) -> None:
         if self.is_long_running_job:
             self.logger.info(
-                f"Stream: `{self.stream_name}` the BULK Job: {self.job_id} runs longer than expected. The job will be canceled and retried with the smaller Slice Size."
+                f"Stream: `{self.stream_name}` the BULK Job: {self.job_id} runs longer than expected. Retry with the reduced `Slice Size` after self-cancelation."
             )
             self.job_cancel()
+            # sleep to ensure the cancelation
+            sleep(self.job_check_interval_sec)
         else:
             sleep(self.job_check_interval_sec)
 
     def on_completed_job(self, **kwargs) -> None:
         pass
 
     def on_failed_job(self, response: requests.Response) -> AirbyteTracedException:
@@ -298,17 +320,20 @@
             return response
         else:
             # execute ERRORS scenario
             self.on_job_with_errors(errors)
 
     def job_check_state(self) -> Optional[str]:
         while not self.job_completed():
-            response = self.job_track_running()
             if self.job_canceled():
-                return None
+                response = None
+                break
+            else:
+                response = self.job_track_running()
+
         # return `job_result_url` when status is `COMPLETED`
         return self.job_get_result(response)
 
     def has_running_concurrent_job(self, errors: Optional[Iterable[Mapping[str, Any]]] = None) -> bool:
         """
         When concurent BULK Job is already running for the same SHOP we receive:
         Error example:
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/query.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/source.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/spec.json` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/streams/base_streams.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 import logging
 from abc import ABC, abstractmethod
+from datetime import datetime
 from functools import cached_property
 from typing import Any, Dict, Iterable, Mapping, MutableMapping, Optional, Union
 from urllib.parse import parse_qsl, urlparse
 
 import pendulum as pdm
 import requests
 from airbyte_cdk.sources.streams.http import HttpStream
@@ -183,14 +184,15 @@
     # guarantee for the NestedSubstreams to emit the STATE
     # when we have the abnormal STATE distance between Parent and Substream
     filter_by_state_checkpoint = False
 
     # Setting the default cursor field for all streams
     cursor_field = "updated_at"
     deleted_cursor_field = "deleted_at"
+    _checkpoint_cursor = None
 
     @property
     def default_state_comparison_value(self) -> Union[int, str]:
         # certain streams are using `id` field as `cursor_field`, which requires to use `int` type,
         # but many other use `str` values for this, we determine what to use based on `cursor_field` value
         return 0 if self.cursor_field == "id" else ""
 
@@ -209,14 +211,26 @@
         # If there is a next page token then we should only send pagination-related parameters.
         if not next_page_token:
             params["order"] = f"{self.order_field} asc"
             if stream_state:
                 params[self.filter_field] = stream_state.get(self.cursor_field)
         return params
 
+    def track_checkpoint_cursor(self, record_value: Union[str, int]) -> None:
+        if self.filter_by_state_checkpoint:
+            # set checkpoint cursor
+            if not self._checkpoint_cursor:
+                self._checkpoint_cursor = self.config.get("start_date")
+            # track checkpoint cursor
+            if record_value >= self._checkpoint_cursor:
+                self._checkpoint_cursor = record_value
+
+    def emit_checkpoint_message(self) -> None:
+        self.logger.info(f"Stream `{self.name}`. Tracking cursor at: `{self._checkpoint_cursor}`.")
+
     def should_checkpoint(self, index: int) -> bool:
         return self.filter_by_state_checkpoint and index >= self.state_checkpoint_interval
 
     # Parse the `stream_slice` with respect to `stream_state` for `Incremental refresh`
     # cases where we slice the stream, the endpoints for those classes don't accept any other filtering,
     # but they provide us with the updated_at field in most cases, so we used that as incremental filtering during the order slicing.
     def filter_records_newer_than_state(
@@ -226,22 +240,21 @@
     ) -> Iterable:
         # Getting records >= state
         if stream_state:
             state_value = stream_state.get(self.cursor_field, self.default_state_comparison_value)
             for index, record in enumerate(records_slice, 1):
                 if self.cursor_field in record:
                     record_value = record.get(self.cursor_field, self.default_state_comparison_value)
+                    self.track_checkpoint_cursor(record_value)
                     if record_value:
                         if record_value >= state_value:
                             yield record
                         else:
                             if self.should_checkpoint(index):
-                                self.logger.info(
-                                    f"Stream `{self.name}`. Checkpointing: {{PK: '{record.get(self.primary_key)}', cursor: '{record_value}'}}."
-                                )
+                                self.emit_checkpoint_message()
                                 yield record
                     else:
                         # old entities could have cursor field in place, but set to null
                         self.logger.warning(
                             f"Stream `{self.name}`, Record ID: `{record.get(self.primary_key)}` cursor value is: {record_value}, record is emitted without state comparison"
                         )
                         yield record
@@ -432,15 +445,15 @@
             and `id` is the parent_key named `id`, we take the value from.
 
     ::  @ nested_entity - the name of the nested entity inside of parent stream, helps to reduce the number of
           API Calls, if present, see `OrderRefunds` or `Fulfillments` streams for more info.
     """
 
     # Setting the check point interval to the limit of the records output
-    state_checkpoint_interval = 50
+    state_checkpoint_interval = 100
     filter_by_state_checkpoint = True
     data_field = None
     parent_stream_class: Union[ShopifyStream, IncrementalShopifyStream] = None
     mutation_map: Mapping[str, Any] = None
     nested_entity = None
 
     @property
@@ -639,23 +652,14 @@
         # overide the default job slice size, if provided (it's auto-adjusted, later on)
         self.bulk_window_in_days = config.get("bulk_window_in_days")
         if self.bulk_window_in_days:
             self.job_manager.job_size = self.bulk_window_in_days
         # define Record Producer instance
         self.record_producer: ShopifyBulkRecord = ShopifyBulkRecord(self.query)
 
-    @property
-    def slice_interval_in_days(self) -> Union[float, int]:
-        # use the adjusted slice size
-        if self.job_manager.job_size:
-            return self.job_manager.job_size
-        else:
-            # accept the slice_size overide from the input configuration, or provide the min value
-            return self.config.get("bulk_window_in_days", self.job_manager.job_size_min)
-
     @cached_property
     def parent_stream(self) -> object:
         """
         Returns the instance of parent stream, if the substream has a `parent_stream_class` dependency.
         """
         return self.parent_stream_class(self.config) if self.parent_stream_class else None
 
@@ -743,43 +747,31 @@
     def get_state_value(self, stream_state: Mapping[str, Any] = None) -> Optional[Union[str, int]]:
         if stream_state:
             return self.get_stream_state_value(stream_state)
         else:
             # for majority of cases we fallback to start_date, otherwise.
             return self.config.get("start_date")
 
-    def job_size_reduce_next_slice(self) -> None:
-        # revert the flag
-        self.job_manager.job_should_revert_slice = False
-        # re-adjust Job Size
-        self.job_manager.reduce_job_size()
+    def emit_slice_message(self, slice_start: datetime, slice_end: datetime) -> None:
+        slice_size_message = f"Slice size: `P{round(self.job_manager.job_size, 1)}D`"
+        self.logger.info(f"Stream: `{self.name}` requesting BULK Job for period: {slice_start} -- {slice_end}. {slice_size_message}")
 
     @stream_state_cache.cache_stream_state
     def stream_slices(self, stream_state: Optional[Mapping[str, Any]] = None, **kwargs) -> Iterable[Optional[Mapping[str, Any]]]:
         if self.filter_field:
             state = self.get_state_value(stream_state)
             start = pdm.parse(state)
             end = pdm.now()
             while start < end:
-                # When the Job is CANCELED intentionally,
-                # we will revert the slice start for the period, and retry with the smaller job size
-                if self.job_manager.is_long_running_job:
-                    start = start.subtract(days=self.slice_interval_in_days)
-                    self.job_size_reduce_next_slice()
-
-                slice_end = start.add(days=self.slice_interval_in_days)
-                # check end period is less than now() or now() is applied otherwise.
-                slice_end = slice_end if slice_end < end else end
-                # making pre-defined sliced query to pass it directly
-                prepared_query = self.query.get(self.filter_field, start.to_rfc3339_string(), slice_end.to_rfc3339_string())
-                self.logger.info(
-                    f"Stream: `{self.name}` requesting BULK Job for period: {start} -- {slice_end}. Slice size: `P{round(self.slice_interval_in_days, 1)}D`."
-                )
-                yield {"query": prepared_query}
-                start = slice_end
+                self.job_manager.job_size_normalize(start, end)
+                slice_end = self.job_manager.get_adjusted_job_start(start)
+                self.emit_slice_message(start, slice_end)
+                yield {"query": self.query.get(self.filter_field, start.to_rfc3339_string(), slice_end.to_rfc3339_string())}
+                # increment the end of the slice or reduce the next slice
+                start = self.job_manager.get_adjusted_job_end(start, slice_end)
         else:
             # for the streams that don't support filtering
             yield {"query": self.query.get()}
 
     def process_bulk_results(
         self,
         response: requests.Response,
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/transform.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/source_shopify/utils.py` & `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,61 +91,62 @@
     on_high_load: float = 5.0
 
     logger = logging.getLogger("airbyte")
 
     log_message_count = 0
     log_message_frequency = 3
 
-    def log_message_counter(message: str, debug_info: Optional[dict] = None) -> None:
+    def log_message_counter(message: str) -> None:
         """
         Print the rate-limit info message every `log_message_frequency` request, to minimize the noise in the logs.
         """
         if ShopifyRateLimiter.log_message_count < ShopifyRateLimiter.log_message_frequency:
             ShopifyRateLimiter.log_message_count += 1
         else:
-            message = (message + f" Info: {debug_info}") if debug_info else message
             ShopifyRateLimiter.logger.info(message)
             ShopifyRateLimiter.log_message_count = 0
 
     def get_response_from_args(*args) -> Optional[requests.Response]:
         for arg in args:
             if isinstance(arg, requests.models.Response):
                 return arg
 
     @staticmethod
-    def _convert_load_to_time(load: Optional[float], threshold: float, debug_info: Optional[dict] = None) -> float:
+    def _convert_load_to_time(load: Optional[float], threshold: float) -> float:
         """
         Define wait_time based on load conditions.
 
         :: load - represents how close we are to being throttled
                 - 0.5 is half way through our allowance
                 - 1 indicates that all of the allowance is used and the api will start rejecting calls
         :: threshold - is the % cutoff for the rate_limits/load
         :: wait_time - time to wait between each request in seconds
 
         """
         mid_load = threshold / 2  # average load based on threshold
         if not load:
             # when there is no rate_limits from header, use the `sleep_on_unknown_load`
             wait_time = ShopifyRateLimiter.on_unknown_load
-            ShopifyRateLimiter.log_message_counter("API Load: `REGULAR`", debug_info)
+            ShopifyRateLimiter.log_message_counter("API Load: `REGULAR`")
         elif load >= threshold:
             wait_time = ShopifyRateLimiter.on_high_load
-            ShopifyRateLimiter.log_message_counter("API Load: `HIGH`", debug_info)
+            ShopifyRateLimiter.log_message_counter("API Load: `HIGH`")
         elif load >= mid_load:
             wait_time = ShopifyRateLimiter.on_mid_load
-            ShopifyRateLimiter.log_message_counter("API Load: `MID`", debug_info)
+            ShopifyRateLimiter.log_message_counter("API Load: `MID`")
         elif load < mid_load:
             wait_time = ShopifyRateLimiter.on_low_load
-            ShopifyRateLimiter.log_message_counter("API Load: `LOW`", debug_info)
+            ShopifyRateLimiter.log_message_counter("API Load: `LOW`")
         return wait_time
 
     @staticmethod
     def get_rest_api_wait_time(
-        *args, threshold: float = 0.9, rate_limit_header: str = "X-Shopify-Shop-Api-Call-Limit", debug_info: Optional[dict] = None
+        *args,
+        threshold: float = 0.9,
+        rate_limit_header: str = "X-Shopify-Shop-Api-Call-Limit",
     ) -> float:
         """
         To avoid reaching Shopify REST API Rate Limits, use the "X-Shopify-Shop-Api-Call-Limit" header value,
         to determine the current rate limits and load and handle wait_time based on load %.
         Recomended wait_time between each request is 1 sec, we would handle this dynamicaly.
 
         :: threshold - is the % cutoff for the rate_limits % load, if this cutoff is crossed,
@@ -164,15 +165,15 @@
         rate_limits = response.headers.get(rate_limit_header) if response else None
         # define current load from rate_limits
         if rate_limits:
             current_rate, max_rate_limit = rate_limits.split("/")
             load = int(current_rate) / int(max_rate_limit)
         else:
             load = None
-        wait_time = ShopifyRateLimiter._convert_load_to_time(load, threshold, debug_info)
+        wait_time = ShopifyRateLimiter._convert_load_to_time(load, threshold)
         return wait_time
 
     @staticmethod
     def get_graphql_api_wait_time(*args, threshold: float = 0.9) -> float:
         """
         To avoid reaching Shopify Graphql API Rate Limits, use the extensions dict in the response.
 
@@ -248,20 +249,17 @@
         The decorator function.
         Adjust `threshold`, `rate_limit_header` and `api_type` if needed.
         """
 
         def decorator(func) -> Callable[..., Any]:
             @wraps(func)
             def wrapper_balance_rate_limit(*args, **kwargs) -> Any:
-                debug_info = ShopifyRateLimiter._debug_info(*args)
                 if api_type == ApiTypeEnum.rest.value:
                     ShopifyRateLimiter.wait_time(
-                        ShopifyRateLimiter.get_rest_api_wait_time(
-                            *args, threshold=threshold, rate_limit_header=rate_limit_header, debug_info=debug_info
-                        )
+                        ShopifyRateLimiter.get_rest_api_wait_time(*args, threshold=threshold, rate_limit_header=rate_limit_header)
                     )
                 elif api_type == ApiTypeEnum.graphql.value:
                     ShopifyRateLimiter.wait_time(ShopifyRateLimiter.get_graphql_api_wait_time(*args, threshold=threshold))
                 else:
                     raise UnrecognisedApiType(f"unrecognised api type: {api_type}. valid values are: {ApiTypeEnum.api_types()}")
                 return func(*args, **kwargs)
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404132257/PKG-INFO` & `airbyte_source_shopify-2.0.5.dev202404151411/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.0.5.dev202404132257
+Version: 2.0.5.dev202404151411
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

