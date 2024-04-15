# Comparing `tmp/newscatcherapi_python_sdk-6.0.2.tar.gz` & `tmp/newscatcherapi_python_sdk-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newscatcherapi_python_sdk-6.0.2.tar", max compression
+gzip compressed data, was "newscatcherapi_python_sdk-6.0.3.tar", max compression
```

## Comparing `newscatcherapi_python_sdk-6.0.2.tar` & `newscatcherapi_python_sdk-6.0.3.tar`

### file list

```diff
@@ -1,239 +1,239 @@
--rw-r--r--   0        0        0     1081 2024-04-04 23:25:41.400602 newscatcherapi_python_sdk-6.0.2/LICENSE
--rw-r--r--   0        0        0    72300 2024-04-04 23:25:41.400812 newscatcherapi_python_sdk-6.0.2/README.md
--rw-r--r--   0        0        0     1059 2024-04-04 23:25:41.401064 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/__init__.py
--rw-r--r--   0        0        0    77304 2024-04-04 23:25:41.401365 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/api_client.py
--rw-r--r--   0        0        0      663 2024-04-04 23:24:04.332914 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/api_response.py
--rw-r--r--   0        0        0      214 2024-04-04 23:24:04.333003 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/__init__.py
--rw-r--r--   0        0        0     1432 2024-04-04 23:25:41.401502 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/path_to_api.py
--rw-r--r--   0        0        0      248 2024-04-04 23:24:04.333179 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      197 2024-04-04 23:24:04.333269 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/paths/api_authors.py
--rw-r--r--   0        0        0      223 2024-04-04 23:24:04.333361 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/paths/api_latest_headlines.py
--rw-r--r--   0        0        0      194 2024-04-04 23:24:04.333450 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/paths/api_search.py
--rw-r--r--   0        0        0      216 2024-04-04 23:25:41.401570 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/paths/api_search_by_link.py
--rw-r--r--   0        0        0      217 2024-04-04 23:24:04.333627 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/paths/api_search_similar.py
--rw-r--r--   0        0        0      197 2024-04-04 23:24:04.333722 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/paths/api_sources.py
--rw-r--r--   0        0        0      212 2024-04-04 23:24:04.333818 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/paths/api_subscription.py
--rw-r--r--   0        0        0     1339 2024-04-04 23:25:41.401701 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      507 2024-04-04 23:25:41.401828 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/__init__.py
--rw-r--r--   0        0        0      902 2024-04-04 23:25:41.401952 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/authors_api.py
--rw-r--r--   0        0        0      705 2024-04-04 23:25:41.402172 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/authors_api_raw.py
--rw-r--r--   0        0        0      961 2024-04-04 23:25:41.402297 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/latest_headlines_api.py
--rw-r--r--   0        0        0      731 2024-04-04 23:25:41.402418 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py
--rw-r--r--   0        0        0      895 2024-04-04 23:25:41.402537 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_api.py
--rw-r--r--   0        0        0      702 2024-04-04 23:25:41.402650 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_api_raw.py
--rw-r--r--   0        0        0      932 2024-04-04 23:25:41.402717 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_link_api.py
--rw-r--r--   0        0        0      722 2024-04-04 23:25:41.402790 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_link_api_raw.py
--rw-r--r--   0        0        0      947 2024-04-04 23:25:41.402892 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_similar_api.py
--rw-r--r--   0        0        0      725 2024-04-04 23:25:41.402997 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_similar_api_raw.py
--rw-r--r--   0        0        0      902 2024-04-04 23:25:41.403114 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/sources_api.py
--rw-r--r--   0        0        0      705 2024-04-04 23:25:41.403230 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/sources_api_raw.py
--rw-r--r--   0        0        0      937 2024-04-04 23:25:41.403342 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/subscription_api.py
--rw-r--r--   0        0        0      720 2024-04-04 23:25:41.403454 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/subscription_api_raw.py
--rw-r--r--   0        0        0     2114 2024-04-04 23:25:41.403565 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/client.py
--rw-r--r--   0        0        0     2114 2024-04-04 23:25:41.403674 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/client.pyi
--rw-r--r--   0        0        0      950 2024-04-04 23:25:41.403783 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/client_custom.py
--rw-r--r--   0        0        0    18272 2024-04-04 23:25:41.403927 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/configuration.py
--rw-r--r--   0        0        0     7953 2024-04-04 23:25:41.404080 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/exceptions.py
--rw-r--r--   0        0        0     2274 2024-04-04 23:24:04.336002 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/exceptions_base.py
--rw-r--r--   0        0        0      355 2024-04-04 23:24:04.336174 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/__init__.py
--rw-r--r--   0        0        0     3747 2024-04-04 23:25:41.404168 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/additional_source_info.py
--rw-r--r--   0        0        0     3747 2024-04-04 23:25:41.404233 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/additional_source_info.pyi
--rw-r--r--   0        0        0    30052 2024-04-04 23:25:41.404402 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/author_search_request.py
--rw-r--r--   0        0        0    29736 2024-04-04 23:25:41.404588 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/author_search_request.pyi
--rw-r--r--   0        0        0     2575 2024-04-04 23:25:41.404711 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/authors_get_response.py
--rw-r--r--   0        0        0     2575 2024-04-04 23:25:41.404817 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/authors_get_response.pyi
--rw-r--r--   0        0        0     2577 2024-04-04 23:25:41.404924 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/authors_post_response.py
--rw-r--r--   0        0        0     2577 2024-04-04 23:25:41.405026 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/authors_post_response.pyi
--rw-r--r--   0        0        0     3902 2024-04-04 23:25:41.405134 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/cluster.py
--rw-r--r--   0        0        0     3902 2024-04-04 23:25:41.405261 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/cluster.pyi
--rw-r--r--   0        0        0     1483 2024-04-04 23:25:41.405372 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/cluster_articles.py
--rw-r--r--   0        0        0     1483 2024-04-04 23:25:41.405476 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/cluster_articles.pyi
--rw-r--r--   0        0        0     7566 2024-04-04 23:25:41.405607 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/clustering_search_response.py
--rw-r--r--   0        0        0     7566 2024-04-04 23:25:41.405715 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/clustering_search_response.pyi
--rw-r--r--   0        0        0    31356 2024-04-04 23:25:41.405866 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0    31356 2024-04-04 23:25:41.406000 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi
--rw-r--r--   0        0        0     7190 2024-04-04 23:25:41.406144 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     7190 2024-04-04 23:25:41.406260 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi
--rw-r--r--   0        0        0     6467 2024-04-04 23:25:41.406384 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0     6467 2024-04-04 23:25:41.406502 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi
--rw-r--r--   0        0        0     1561 2024-04-04 23:25:41.406617 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1561 2024-04-04 23:25:41.406724 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi
--rw-r--r--   0        0        0    32982 2024-04-04 23:25:41.406876 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0    32982 2024-04-04 23:25:41.407012 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi
--rw-r--r--   0        0        0     7191 2024-04-04 23:25:41.407151 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     7191 2024-04-04 23:25:41.407267 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi
--rw-r--r--   0        0        0     6468 2024-04-04 23:25:41.407385 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0     6468 2024-04-04 23:25:41.407509 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi
--rw-r--r--   0        0        0     1561 2024-04-04 23:25:41.407622 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1561 2024-04-04 23:25:41.407738 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi
--rw-r--r--   0        0        0     6406 2024-04-04 23:25:41.407868 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0     6406 2024-04-04 23:25:41.407978 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi
--rw-r--r--   0        0        0     1549 2024-04-04 23:25:41.408184 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1549 2024-04-04 23:25:41.408308 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi
--rw-r--r--   0        0        0     3525 2024-04-04 23:25:41.408438 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/http_validation_error.py
--rw-r--r--   0        0        0     3525 2024-04-04 23:25:41.408542 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/http_validation_error.pyi
--rw-r--r--   0        0        0     2429 2024-04-04 23:25:41.408660 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_get_response.py
--rw-r--r--   0        0        0     2429 2024-04-04 23:25:41.408776 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_get_response.pyi
--rw-r--r--   0        0        0     2431 2024-04-04 23:25:41.408897 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_post_response.py
--rw-r--r--   0        0        0     2431 2024-04-04 23:25:41.409716 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_post_response.pyi
--rw-r--r--   0        0        0    26820 2024-04-04 23:25:41.409897 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_request.py
--rw-r--r--   0        0        0    26504 2024-04-04 23:25:41.410070 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_request.pyi
--rw-r--r--   0        0        0     6233 2024-04-04 23:25:41.410216 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_response.py
--rw-r--r--   0        0        0     6233 2024-04-04 23:25:41.410342 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_response.pyi
--rw-r--r--   0        0        0     1515 2024-04-04 23:25:41.410463 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     1515 2024-04-04 23:25:41.410653 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_response_articles.pyi
--rw-r--r--   0        0        0    32225 2024-04-04 23:25:41.410829 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/more_like_this_request.py
--rw-r--r--   0        0        0    31830 2024-04-04 23:25:41.411138 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/more_like_this_request.pyi
--rw-r--r--   0        0        0     2465 2024-04-04 23:25:41.411276 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_get_response.py
--rw-r--r--   0        0        0     2465 2024-04-04 23:25:41.411382 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_get_response.pyi
--rw-r--r--   0        0        0     2467 2024-04-04 23:25:41.411488 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_post_response.py
--rw-r--r--   0        0        0     2467 2024-04-04 23:25:41.411601 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_post_response.pyi
--rw-r--r--   0        0        0    35999 2024-04-04 23:25:41.411730 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_request.py
--rw-r--r--   0        0        0    35683 2024-04-04 23:25:41.411890 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_request.pyi
--rw-r--r--   0        0        0     2589 2024-04-04 23:25:41.412032 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_similar_get_response.py
--rw-r--r--   0        0        0     2589 2024-04-04 23:25:41.412150 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_similar_get_response.pyi
--rw-r--r--   0        0        0     2591 2024-04-04 23:25:41.412272 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_similar_post_response.py
--rw-r--r--   0        0        0     2591 2024-04-04 23:25:41.412379 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_similar_post_response.pyi
--rw-r--r--   0        0        0     4688 2024-04-04 23:25:41.412490 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_url_request.py
--rw-r--r--   0        0        0     4530 2024-04-04 23:25:41.412604 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_url_request.pyi
--rw-r--r--   0        0        0     4012 2024-04-04 23:25:41.412719 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/similar_document.py
--rw-r--r--   0        0        0     4012 2024-04-04 23:25:41.412819 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/similar_document.pyi
--rw-r--r--   0        0        0     4460 2024-04-04 23:25:41.412948 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_info.py
--rw-r--r--   0        0        0     4460 2024-04-04 23:25:41.413080 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_info.pyi
--rw-r--r--   0        0        0     3881 2024-04-04 23:25:41.413211 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_response.py
--rw-r--r--   0        0        0     3881 2024-04-04 23:25:41.413334 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_response.pyi
--rw-r--r--   0        0        0     3437 2024-04-04 23:25:41.413665 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_response_sources.py
--rw-r--r--   0        0        0     3437 2024-04-04 23:25:41.413809 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_response_sources.pyi
--rw-r--r--   0        0        0     6829 2024-04-04 23:25:41.413941 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/sources_request.py
--rw-r--r--   0        0        0     6829 2024-04-04 23:25:41.414072 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/sources_request.pyi
--rw-r--r--   0        0        0     5882 2024-04-04 23:25:41.414220 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/subscription_response.py
--rw-r--r--   0        0        0     5882 2024-04-04 23:25:41.414360 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/subscription_response.pyi
--rw-r--r--   0        0        0     3626 2024-04-04 23:25:41.414490 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/validation_error.py
--rw-r--r--   0        0        0     3626 2024-04-04 23:25:41.414607 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/validation_error.pyi
--rw-r--r--   0        0        0     3408 2024-04-04 23:25:41.414728 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/validation_error_loc.py
--rw-r--r--   0        0        0     3408 2024-04-04 23:25:41.414842 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/validation_error_loc.pyi
--rw-r--r--   0        0        0     4137 2024-04-04 23:25:41.415021 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/models/__init__.py
--rw-r--r--   0        0        0    24375 2024-04-04 23:25:41.415134 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/operation_parameter_map.py
--rw-r--r--   0        0        0      582 2024-04-04 23:25:41.415296 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/__init__.py
--rw-r--r--   0        0        0      323 2024-04-04 23:24:04.346252 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_authors/__init__.py
--rw-r--r--   0        0        0    63733 2024-04-04 23:25:41.415474 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_authors/get.py
--rw-r--r--   0        0        0    63424 2024-04-04 23:25:41.416322 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_authors/get.pyi
--rw-r--r--   0        0        0    45283 2024-04-04 23:25:41.417068 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_authors/post.py
--rw-r--r--   0        0        0    45146 2024-04-04 23:25:41.417262 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_authors/post.pyi
--rw-r--r--   0        0        0      341 2024-04-04 23:24:04.347041 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_latest_headlines/__init__.py
--rw-r--r--   0        0        0    62849 2024-04-04 23:25:41.417461 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_latest_headlines/get.py
--rw-r--r--   0        0        0    62540 2024-04-04 23:25:41.418134 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_latest_headlines/get.pyi
--rw-r--r--   0        0        0    47002 2024-04-04 23:25:41.421262 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_latest_headlines/post.py
--rw-r--r--   0        0        0    46865 2024-04-04 23:25:41.421512 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_latest_headlines/post.pyi
--rw-r--r--   0        0        0      321 2024-04-04 23:24:04.347797 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search/__init__.py
--rw-r--r--   0        0        0    75693 2024-04-04 23:25:41.422059 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search/get.py
--rw-r--r--   0        0        0    75384 2024-04-04 23:25:41.422861 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search/get.pyi
--rw-r--r--   0        0        0    53265 2024-04-04 23:25:41.423084 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search/post.py
--rw-r--r--   0        0        0    53128 2024-04-04 23:25:41.423414 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search/post.pyi
--rw-r--r--   0        0        0      337 2024-04-04 23:25:41.423770 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_by_link/__init__.py
--rw-r--r--   0        0        0    19293 2024-04-04 23:25:41.423878 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_by_link/get.py
--rw-r--r--   0        0        0    19070 2024-04-04 23:25:41.424268 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_by_link/get.pyi
--rw-r--r--   0        0        0    17699 2024-04-04 23:25:41.424380 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_by_link/post.py
--rw-r--r--   0        0        0    17562 2024-04-04 23:25:41.424683 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_by_link/post.pyi
--rw-r--r--   0        0        0      337 2024-04-04 23:24:04.350358 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_similar/__init__.py
--rw-r--r--   0        0        0    67713 2024-04-04 23:25:41.425415 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_similar/get.py
--rw-r--r--   0        0        0    67361 2024-04-04 23:25:41.425614 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_similar/get.pyi
--rw-r--r--   0        0        0    47930 2024-04-04 23:25:41.425801 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_similar/post.py
--rw-r--r--   0        0        0    47793 2024-04-04 23:25:41.425958 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_similar/post.pyi
--rw-r--r--   0        0        0      323 2024-04-04 23:24:04.351197 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_sources/__init__.py
--rw-r--r--   0        0        0    22889 2024-04-04 23:25:41.426550 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_sources/get.py
--rw-r--r--   0        0        0    22752 2024-04-04 23:25:41.426774 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_sources/get.pyi
--rw-r--r--   0        0        0    19936 2024-04-04 23:25:41.426988 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_sources/post.py
--rw-r--r--   0        0        0    19799 2024-04-04 23:25:41.427507 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_sources/post.pyi
--rw-r--r--   0        0        0      333 2024-04-04 23:24:04.351850 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_subscription/__init__.py
--rw-r--r--   0        0        0    12067 2024-04-04 23:25:41.428330 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_subscription/get.py
--rw-r--r--   0        0        0    11930 2024-04-04 23:25:41.428503 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_subscription/get.pyi
--rw-r--r--   0        0        0    12093 2024-04-04 23:25:41.428676 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_subscription/post.py
--rw-r--r--   0        0        0    11956 2024-04-04 23:25:41.428880 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_subscription/post.pyi
--rw-r--r--   0        0        0        0 2024-04-04 23:24:04.352525 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/__init__.py
--rw-r--r--   0        0        0      987 2024-04-04 23:25:41.428990 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/additional_source_info.py
--rw-r--r--   0        0        0     4450 2024-04-04 23:25:41.429516 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/author_search_request.py
--rw-r--r--   0        0        0     1061 2024-04-04 23:25:41.429678 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/authors_get_response.py
--rw-r--r--   0        0        0     1062 2024-04-04 23:25:41.429804 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/authors_post_response.py
--rw-r--r--   0        0        0      995 2024-04-04 23:25:41.429928 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/cluster.py
--rw-r--r--   0        0        0      665 2024-04-04 23:25:41.430046 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/cluster_articles.py
--rw-r--r--   0        0        0     1336 2024-04-04 23:25:41.430187 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/clustering_search_response.py
--rw-r--r--   0        0        0     3052 2024-04-04 23:25:41.430308 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0     1542 2024-04-04 23:25:41.430422 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     1436 2024-04-04 23:25:41.430833 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0      704 2024-04-04 23:25:41.431318 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     3239 2024-04-04 23:25:41.431772 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0     1543 2024-04-04 23:25:41.432630 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     1437 2024-04-04 23:25:41.432793 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0      704 2024-04-04 23:25:41.432931 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1411 2024-04-04 23:25:41.433052 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0      698 2024-04-04 23:25:41.433175 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0      937 2024-04-04 23:25:41.433431 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/http_validation_error.py
--rw-r--r--   0        0        0      907 2024-04-04 23:25:41.433565 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_get_response.py
--rw-r--r--   0        0        0      908 2024-04-04 23:25:41.433690 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_post_response.py
--rw-r--r--   0        0        0     4621 2024-04-04 23:25:41.434510 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_request.py
--rw-r--r--   0        0        0     1340 2024-04-04 23:25:41.435791 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_response.py
--rw-r--r--   0        0        0      681 2024-04-04 23:25:41.435929 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     4721 2024-04-04 23:25:41.436087 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/more_like_this_request.py
--rw-r--r--   0        0        0      952 2024-04-04 23:25:41.436322 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_get_response.py
--rw-r--r--   0        0        0      953 2024-04-04 23:25:41.436449 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_post_response.py
--rw-r--r--   0        0        0     5397 2024-04-04 23:25:41.436931 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_request.py
--rw-r--r--   0        0        0     1069 2024-04-04 23:25:41.437209 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_similar_get_response.py
--rw-r--r--   0        0        0     1070 2024-04-04 23:25:41.437332 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_similar_post_response.py
--rw-r--r--   0        0        0     1151 2024-04-04 23:25:41.437432 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_url_request.py
--rw-r--r--   0        0        0      937 2024-04-04 23:25:41.437784 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/similar_document.py
--rw-r--r--   0        0        0     1132 2024-04-04 23:25:41.438059 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/source_info.py
--rw-r--r--   0        0        0     1093 2024-04-04 23:25:41.438580 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/source_response.py
--rw-r--r--   0        0        0      760 2024-04-04 23:25:41.438939 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/source_response_sources.py
--rw-r--r--   0        0        0     1432 2024-04-04 23:25:41.439392 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/sources_request.py
--rw-r--r--   0        0        0     1216 2024-04-04 23:25:41.439721 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/subscription_response.py
--rw-r--r--   0        0        0      973 2024-04-04 23:25:41.440047 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/validation_error.py
--rw-r--r--   0        0        0      684 2024-04-04 23:25:41.440552 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/validation_error_loc.py
--rw-r--r--   0        0        0      913 2024-04-04 23:25:41.440980 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/request_after_hook.py
--rw-r--r--   0        0        0      971 2024-04-04 23:25:41.441325 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/request_before_hook.py
--rw-r--r--   0        0        0      936 2024-04-04 23:25:41.442226 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/request_before_url_hook.py
--rw-r--r--   0        0        0    11233 2024-04-04 23:25:41.442909 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/rest.py
--rw-r--r--   0        0        0    96391 2024-04-04 23:25:41.444305 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/schemas.py
--rw-r--r--   0        0        0        0 2024-04-04 23:24:04.357213 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/__init__.py
--rw-r--r--   0        0        0      842 2024-04-04 23:25:41.444489 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/additional_source_info.py
--rw-r--r--   0        0        0     2525 2024-04-04 23:25:41.444910 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/author_search_request.py
--rw-r--r--   0        0        0      992 2024-04-04 23:25:41.445125 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/authors_get_response.py
--rw-r--r--   0        0        0      993 2024-04-04 23:25:41.445399 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/authors_post_response.py
--rw-r--r--   0        0        0      862 2024-04-04 23:25:41.445568 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/cluster.py
--rw-r--r--   0        0        0      604 2024-04-04 23:25:41.445933 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/cluster_articles.py
--rw-r--r--   0        0        0     1106 2024-04-04 23:25:41.446344 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/clustering_search_response.py
--rw-r--r--   0        0        0     1778 2024-04-04 23:25:41.446642 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0     1341 2024-04-04 23:25:41.446836 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     1326 2024-04-04 23:25:41.447420 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0      643 2024-04-04 23:25:41.448020 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1903 2024-04-04 23:25:41.448583 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0     1342 2024-04-04 23:25:41.448759 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     1327 2024-04-04 23:25:41.449021 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0      643 2024-04-04 23:25:41.449554 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1277 2024-04-04 23:25:41.449697 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0      637 2024-04-04 23:25:41.449846 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0      889 2024-04-04 23:25:41.449982 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/http_validation_error.py
--rw-r--r--   0        0        0      838 2024-04-04 23:25:41.450104 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_get_response.py
--rw-r--r--   0        0        0      839 2024-04-04 23:25:41.450238 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_post_response.py
--rw-r--r--   0        0        0     2638 2024-04-04 23:25:41.450580 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_request.py
--rw-r--r--   0        0        0     1138 2024-04-04 23:25:41.451813 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_response.py
--rw-r--r--   0        0        0      620 2024-04-04 23:25:41.451982 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     2616 2024-04-04 23:25:41.452120 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/more_like_this_request.py
--rw-r--r--   0        0        0      883 2024-04-04 23:25:41.452236 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_get_response.py
--rw-r--r--   0        0        0      884 2024-04-04 23:25:41.452359 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_post_response.py
--rw-r--r--   0        0        0     2942 2024-04-04 23:25:41.452482 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_request.py
--rw-r--r--   0        0        0     1000 2024-04-04 23:25:41.452619 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_similar_get_response.py
--rw-r--r--   0        0        0     1001 2024-04-04 23:25:41.452865 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_similar_post_response.py
--rw-r--r--   0        0        0      957 2024-04-04 23:25:41.453111 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_url_request.py
--rw-r--r--   0        0        0      836 2024-04-04 23:25:41.453539 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/similar_document.py
--rw-r--r--   0        0        0      904 2024-04-04 23:25:41.453662 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/source_info.py
--rw-r--r--   0        0        0      994 2024-04-04 23:25:41.453898 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/source_response.py
--rw-r--r--   0        0        0      695 2024-04-04 23:25:41.454044 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/source_response_sources.py
--rw-r--r--   0        0        0      996 2024-04-04 23:25:41.454170 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/sources_request.py
--rw-r--r--   0        0        0      925 2024-04-04 23:25:41.454301 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/subscription_response.py
--rw-r--r--   0        0        0      892 2024-04-04 23:25:41.454413 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/validation_error.py
--rw-r--r--   0        0        0      623 2024-04-04 23:25:41.454531 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/validation_error_loc.py
--rw-r--r--   0        0        0      758 2024-04-04 23:25:41.454646 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type_util.py
--rw-r--r--   0        0        0     3177 2024-04-04 23:24:04.361356 newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/validation_metadata.py
--rw-r--r--   0        0        0      791 2024-04-04 23:25:41.454770 newscatcherapi_python_sdk-6.0.2/pyproject.toml
--rw-r--r--   0        0        0    73317 1970-01-01 00:00:00.000000 newscatcherapi_python_sdk-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-15 17:14:53.857576 newscatcherapi_python_sdk-6.0.3/LICENSE
+-rw-r--r--   0        0        0    75510 2024-04-15 17:18:13.390065 newscatcherapi_python_sdk-6.0.3/README.md
+-rw-r--r--   0        0        0     1059 2024-04-15 17:18:13.390276 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/__init__.py
+-rw-r--r--   0        0        0    77304 2024-04-15 17:18:13.390586 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/api_client.py
+-rw-r--r--   0        0        0      663 2024-04-15 17:14:53.814746 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/api_response.py
+-rw-r--r--   0        0        0      214 2024-04-15 17:14:53.814890 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/__init__.py
+-rw-r--r--   0        0        0     1432 2024-04-15 17:14:53.815013 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      248 2024-04-15 17:14:53.815202 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-15 17:14:53.815333 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_authors.py
+-rw-r--r--   0        0        0      223 2024-04-15 17:14:53.815446 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_latest_headlines.py
+-rw-r--r--   0        0        0      194 2024-04-15 17:14:53.815563 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_search.py
+-rw-r--r--   0        0        0      216 2024-04-15 17:14:53.815683 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_search_by_link.py
+-rw-r--r--   0        0        0      217 2024-04-15 17:14:53.815806 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_search_similar.py
+-rw-r--r--   0        0        0      197 2024-04-15 17:14:53.815913 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_sources.py
+-rw-r--r--   0        0        0      212 2024-04-15 17:14:53.816025 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/paths/api_subscription.py
+-rw-r--r--   0        0        0     1339 2024-04-15 17:14:53.816145 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      507 2024-04-15 17:14:53.816302 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0      902 2024-04-15 17:14:53.816410 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/authors_api.py
+-rw-r--r--   0        0        0      705 2024-04-15 17:14:53.816516 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/authors_api_raw.py
+-rw-r--r--   0        0        0      961 2024-04-15 17:14:53.816626 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/latest_headlines_api.py
+-rw-r--r--   0        0        0      731 2024-04-15 17:14:53.816733 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py
+-rw-r--r--   0        0        0      895 2024-04-15 17:14:53.816845 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_api.py
+-rw-r--r--   0        0        0      702 2024-04-15 17:14:53.816950 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_api_raw.py
+-rw-r--r--   0        0        0      932 2024-04-15 17:14:53.817060 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_link_api.py
+-rw-r--r--   0        0        0      722 2024-04-15 17:14:53.817181 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_link_api_raw.py
+-rw-r--r--   0        0        0      947 2024-04-15 17:14:53.817302 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_similar_api.py
+-rw-r--r--   0        0        0      725 2024-04-15 17:14:53.817419 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_similar_api_raw.py
+-rw-r--r--   0        0        0      902 2024-04-15 17:14:53.817524 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/sources_api.py
+-rw-r--r--   0        0        0      705 2024-04-15 17:14:53.817634 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/sources_api_raw.py
+-rw-r--r--   0        0        0      937 2024-04-15 17:14:53.817747 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/subscription_api.py
+-rw-r--r--   0        0        0      720 2024-04-15 17:14:53.817867 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/subscription_api_raw.py
+-rw-r--r--   0        0        0     2114 2024-04-15 17:14:53.817992 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client.py
+-rw-r--r--   0        0        0     2114 2024-04-15 17:14:53.818125 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client.pyi
+-rw-r--r--   0        0        0      950 2024-04-15 17:14:53.818250 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client_custom.py
+-rw-r--r--   0        0        0    18272 2024-04-15 17:18:13.390856 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/configuration.py
+-rw-r--r--   0        0        0     7953 2024-04-15 17:14:53.818574 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/exceptions.py
+-rw-r--r--   0        0        0     2274 2024-04-15 17:14:53.818717 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/exceptions_base.py
+-rw-r--r--   0        0        0      355 2024-04-15 17:14:53.818935 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/__init__.py
+-rw-r--r--   0        0        0     3747 2024-04-15 17:14:53.819072 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/additional_source_info.py
+-rw-r--r--   0        0        0     3747 2024-04-15 17:14:53.819207 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/additional_source_info.pyi
+-rw-r--r--   0        0        0    31468 2024-04-15 17:18:13.391130 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/author_search_request.py
+-rw-r--r--   0        0        0    31152 2024-04-15 17:18:13.391406 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/author_search_request.pyi
+-rw-r--r--   0        0        0     2575 2024-04-15 17:14:53.819638 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_get_response.py
+-rw-r--r--   0        0        0     2575 2024-04-15 17:14:53.819784 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_get_response.pyi
+-rw-r--r--   0        0        0     2577 2024-04-15 17:14:53.819936 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_post_response.py
+-rw-r--r--   0        0        0     2577 2024-04-15 17:14:53.820063 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_post_response.pyi
+-rw-r--r--   0        0        0     3902 2024-04-15 17:14:53.820192 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster.py
+-rw-r--r--   0        0        0     3902 2024-04-15 17:14:53.820315 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster.pyi
+-rw-r--r--   0        0        0     1483 2024-04-15 17:14:53.820452 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster_articles.py
+-rw-r--r--   0        0        0     1483 2024-04-15 17:14:53.820577 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster_articles.pyi
+-rw-r--r--   0        0        0     7566 2024-04-15 17:14:53.820718 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/clustering_search_response.py
+-rw-r--r--   0        0        0     7566 2024-04-15 17:14:53.820856 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/clustering_search_response.pyi
+-rw-r--r--   0        0        0    31356 2024-04-15 17:14:53.821010 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0    31356 2024-04-15 17:14:53.821176 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi
+-rw-r--r--   0        0        0     7190 2024-04-15 17:14:53.821335 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     7190 2024-04-15 17:14:53.821484 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi
+-rw-r--r--   0        0        0     6467 2024-04-15 17:14:53.821621 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0     6467 2024-04-15 17:14:53.821766 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi
+-rw-r--r--   0        0        0     1561 2024-04-15 17:14:53.821896 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1561 2024-04-15 17:14:53.822026 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi
+-rw-r--r--   0        0        0    32982 2024-04-15 17:14:53.822180 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0    32982 2024-04-15 17:14:53.822359 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi
+-rw-r--r--   0        0        0     7191 2024-04-15 17:14:53.822515 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     7191 2024-04-15 17:14:53.822648 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi
+-rw-r--r--   0        0        0     6468 2024-04-15 17:14:53.822785 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0     6468 2024-04-15 17:14:53.822915 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi
+-rw-r--r--   0        0        0     1561 2024-04-15 17:14:53.823030 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1561 2024-04-15 17:14:53.823157 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi
+-rw-r--r--   0        0        0     6406 2024-04-15 17:14:53.823288 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0     6406 2024-04-15 17:14:53.823406 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi
+-rw-r--r--   0        0        0     1549 2024-04-15 17:14:53.823525 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1549 2024-04-15 17:14:53.823655 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi
+-rw-r--r--   0        0        0     3525 2024-04-15 17:14:53.823783 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/http_validation_error.py
+-rw-r--r--   0        0        0     3525 2024-04-15 17:14:53.823904 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     2429 2024-04-15 17:14:53.824028 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_get_response.py
+-rw-r--r--   0        0        0     2429 2024-04-15 17:14:53.824139 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_get_response.pyi
+-rw-r--r--   0        0        0     2431 2024-04-15 17:14:53.824258 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     2431 2024-04-15 17:14:53.824381 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_post_response.pyi
+-rw-r--r--   0        0        0    28236 2024-04-15 17:18:13.391685 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_request.py
+-rw-r--r--   0        0        0    27920 2024-04-15 17:18:13.391954 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_request.pyi
+-rw-r--r--   0        0        0     6233 2024-04-15 17:14:53.824809 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response.py
+-rw-r--r--   0        0        0     6233 2024-04-15 17:14:53.824930 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response.pyi
+-rw-r--r--   0        0        0     1515 2024-04-15 17:14:53.825034 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     1515 2024-04-15 17:14:53.825143 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response_articles.pyi
+-rw-r--r--   0        0        0    32225 2024-04-15 17:14:53.825269 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/more_like_this_request.py
+-rw-r--r--   0        0        0    31830 2024-04-15 17:14:53.825416 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/more_like_this_request.pyi
+-rw-r--r--   0        0        0     2465 2024-04-15 17:14:53.825541 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_get_response.py
+-rw-r--r--   0        0        0     2465 2024-04-15 17:14:53.825653 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_get_response.pyi
+-rw-r--r--   0        0        0     2467 2024-04-15 17:14:53.825775 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_post_response.py
+-rw-r--r--   0        0        0     2467 2024-04-15 17:14:53.825877 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_post_response.pyi
+-rw-r--r--   0        0        0    36733 2024-04-15 17:18:13.393918 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_request.py
+-rw-r--r--   0        0        0    36417 2024-04-15 17:18:13.395611 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_request.pyi
+-rw-r--r--   0        0        0     2589 2024-04-15 17:14:53.826283 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_get_response.py
+-rw-r--r--   0        0        0     2589 2024-04-15 17:14:53.826403 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_get_response.pyi
+-rw-r--r--   0        0        0     2591 2024-04-15 17:14:53.826518 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_post_response.py
+-rw-r--r--   0        0        0     2591 2024-04-15 17:14:53.826631 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_post_response.pyi
+-rw-r--r--   0        0        0     4688 2024-04-15 17:14:53.826748 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_url_request.py
+-rw-r--r--   0        0        0     4530 2024-04-15 17:14:53.826871 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_url_request.pyi
+-rw-r--r--   0        0        0     4012 2024-04-15 17:14:53.826972 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/similar_document.py
+-rw-r--r--   0        0        0     4012 2024-04-15 17:14:53.827076 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/similar_document.pyi
+-rw-r--r--   0        0        0     4460 2024-04-15 17:14:53.827191 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_info.py
+-rw-r--r--   0        0        0     4460 2024-04-15 17:14:53.827313 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_info.pyi
+-rw-r--r--   0        0        0     3881 2024-04-15 17:14:53.827424 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response.py
+-rw-r--r--   0        0        0     3881 2024-04-15 17:14:53.827546 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response.pyi
+-rw-r--r--   0        0        0     3437 2024-04-15 17:14:53.827665 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response_sources.py
+-rw-r--r--   0        0        0     3437 2024-04-15 17:14:53.827776 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response_sources.pyi
+-rw-r--r--   0        0        0     6829 2024-04-15 17:14:53.827889 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/sources_request.py
+-rw-r--r--   0        0        0     6829 2024-04-15 17:14:53.828002 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/sources_request.pyi
+-rw-r--r--   0        0        0     5882 2024-04-15 17:14:53.828117 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/subscription_response.py
+-rw-r--r--   0        0        0     5882 2024-04-15 17:14:53.828229 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/subscription_response.pyi
+-rw-r--r--   0        0        0     3626 2024-04-15 17:14:53.828343 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error.py
+-rw-r--r--   0        0        0     3626 2024-04-15 17:14:53.828470 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error.pyi
+-rw-r--r--   0        0        0     3408 2024-04-15 17:14:53.828574 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error_loc.py
+-rw-r--r--   0        0        0     3408 2024-04-15 17:14:53.828676 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error_loc.pyi
+-rw-r--r--   0        0        0     4137 2024-04-15 17:14:53.828797 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/models/__init__.py
+-rw-r--r--   0        0        0    25039 2024-04-15 17:18:13.395926 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/operation_parameter_map.py
+-rw-r--r--   0        0        0      582 2024-04-15 17:14:53.829074 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2024-04-15 17:14:53.829193 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/__init__.py
+-rw-r--r--   0        0        0    66916 2024-04-15 17:18:13.396293 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/get.py
+-rw-r--r--   0        0        0    66607 2024-04-15 17:18:13.396664 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/get.pyi
+-rw-r--r--   0        0        0    47473 2024-04-15 17:18:13.396987 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/post.py
+-rw-r--r--   0        0        0    47336 2024-04-15 17:18:13.397275 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/post.pyi
+-rw-r--r--   0        0        0      341 2024-04-15 17:14:53.830874 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/__init__.py
+-rw-r--r--   0        0        0    66032 2024-04-15 17:18:13.397593 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/get.py
+-rw-r--r--   0        0        0    65723 2024-04-15 17:18:13.397880 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/get.pyi
+-rw-r--r--   0        0        0    49192 2024-04-15 17:18:13.398145 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/post.py
+-rw-r--r--   0        0        0    49055 2024-04-15 17:18:13.398420 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/post.pyi
+-rw-r--r--   0        0        0      321 2024-04-15 17:14:53.832084 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/__init__.py
+-rw-r--r--   0        0        0    77343 2024-04-15 17:18:13.398812 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/get.py
+-rw-r--r--   0        0        0    77034 2024-04-15 17:18:13.399319 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/get.pyi
+-rw-r--r--   0        0        0    54404 2024-04-15 17:18:13.399637 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/post.py
+-rw-r--r--   0        0        0    54267 2024-04-15 17:18:13.399936 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/post.pyi
+-rw-r--r--   0        0        0      337 2024-04-15 17:14:53.832957 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/__init__.py
+-rw-r--r--   0        0        0    19293 2024-04-15 17:14:53.833078 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/get.py
+-rw-r--r--   0        0        0    19070 2024-04-15 17:14:53.833225 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/get.pyi
+-rw-r--r--   0        0        0    17699 2024-04-15 17:14:53.833367 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/post.py
+-rw-r--r--   0        0        0    17562 2024-04-15 17:14:53.835150 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/post.pyi
+-rw-r--r--   0        0        0      337 2024-04-15 17:14:53.835338 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/__init__.py
+-rw-r--r--   0        0        0    67713 2024-04-15 17:14:53.835596 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/get.py
+-rw-r--r--   0        0        0    67361 2024-04-15 17:14:53.835865 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/get.pyi
+-rw-r--r--   0        0        0    47930 2024-04-15 17:14:53.836031 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/post.py
+-rw-r--r--   0        0        0    47793 2024-04-15 17:14:53.836857 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/post.pyi
+-rw-r--r--   0        0        0      323 2024-04-15 17:14:53.837014 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/__init__.py
+-rw-r--r--   0        0        0    22889 2024-04-15 17:14:53.837139 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/get.py
+-rw-r--r--   0        0        0    22752 2024-04-15 17:14:53.837285 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/get.pyi
+-rw-r--r--   0        0        0    19936 2024-04-15 17:14:53.837427 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/post.py
+-rw-r--r--   0        0        0    19799 2024-04-15 17:14:53.837562 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/post.pyi
+-rw-r--r--   0        0        0      333 2024-04-15 17:14:53.837697 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/__init__.py
+-rw-r--r--   0        0        0    12067 2024-04-15 17:14:53.837806 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/get.py
+-rw-r--r--   0        0        0    11930 2024-04-15 17:14:53.837986 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/get.pyi
+-rw-r--r--   0        0        0    12093 2024-04-15 17:14:53.838240 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/post.py
+-rw-r--r--   0        0        0    11956 2024-04-15 17:14:53.838448 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/post.pyi
+-rw-r--r--   0        0        0        0 2024-04-15 17:14:53.838623 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-15 17:14:53.838734 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/additional_source_info.py
+-rw-r--r--   0        0        0     4726 2024-04-15 17:18:13.400226 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/author_search_request.py
+-rw-r--r--   0        0        0     1061 2024-04-15 17:14:53.838987 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/authors_get_response.py
+-rw-r--r--   0        0        0     1062 2024-04-15 17:14:53.839092 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/authors_post_response.py
+-rw-r--r--   0        0        0      995 2024-04-15 17:14:53.839196 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/cluster.py
+-rw-r--r--   0        0        0      665 2024-04-15 17:14:53.839308 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/cluster_articles.py
+-rw-r--r--   0        0        0     1336 2024-04-15 17:14:53.839415 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/clustering_search_response.py
+-rw-r--r--   0        0        0     3052 2024-04-15 17:14:53.839522 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0     1542 2024-04-15 17:14:53.839632 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     1436 2024-04-15 17:14:53.839747 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0      704 2024-04-15 17:14:53.839863 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     3239 2024-04-15 17:14:53.839972 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0     1543 2024-04-15 17:14:53.840077 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     1437 2024-04-15 17:14:53.840183 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0      704 2024-04-15 17:14:53.840297 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1411 2024-04-15 17:14:53.840402 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0      698 2024-04-15 17:14:53.840505 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0      937 2024-04-15 17:14:53.840610 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/http_validation_error.py
+-rw-r--r--   0        0        0      907 2024-04-15 17:14:53.840719 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_get_response.py
+-rw-r--r--   0        0        0      908 2024-04-15 17:14:53.840826 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     4897 2024-04-15 17:18:13.400461 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_request.py
+-rw-r--r--   0        0        0     1340 2024-04-15 17:14:53.841066 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_response.py
+-rw-r--r--   0        0        0      681 2024-04-15 17:14:53.841165 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     4721 2024-04-15 17:14:53.841277 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/more_like_this_request.py
+-rw-r--r--   0        0        0      952 2024-04-15 17:14:53.841381 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_get_response.py
+-rw-r--r--   0        0        0      953 2024-04-15 17:14:53.841482 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_post_response.py
+-rw-r--r--   0        0        0     5539 2024-04-15 17:18:13.400762 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_request.py
+-rw-r--r--   0        0        0     1069 2024-04-15 17:14:53.841699 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_similar_get_response.py
+-rw-r--r--   0        0        0     1070 2024-04-15 17:14:53.841804 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_similar_post_response.py
+-rw-r--r--   0        0        0     1151 2024-04-15 17:14:53.841902 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_url_request.py
+-rw-r--r--   0        0        0      937 2024-04-15 17:14:53.842004 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/similar_document.py
+-rw-r--r--   0        0        0     1132 2024-04-15 17:14:53.842116 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_info.py
+-rw-r--r--   0        0        0     1093 2024-04-15 17:14:53.842221 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_response.py
+-rw-r--r--   0        0        0      760 2024-04-15 17:14:53.842321 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_response_sources.py
+-rw-r--r--   0        0        0     1432 2024-04-15 17:14:53.842420 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/sources_request.py
+-rw-r--r--   0        0        0     1216 2024-04-15 17:14:53.842520 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/subscription_response.py
+-rw-r--r--   0        0        0      973 2024-04-15 17:14:53.842622 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/validation_error.py
+-rw-r--r--   0        0        0      684 2024-04-15 17:14:53.842723 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/validation_error_loc.py
+-rw-r--r--   0        0        0      913 2024-04-15 17:14:53.842835 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_after_hook.py
+-rw-r--r--   0        0        0      971 2024-04-15 17:14:53.842937 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_before_hook.py
+-rw-r--r--   0        0        0      936 2024-04-15 17:14:53.843037 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_before_url_hook.py
+-rw-r--r--   0        0        0    11233 2024-04-15 17:14:53.843143 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/rest.py
+-rw-r--r--   0        0        0    96391 2024-04-15 17:14:53.843395 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-15 17:14:53.843546 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-15 17:14:53.843655 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/additional_source_info.py
+-rw-r--r--   0        0        0     2699 2024-04-15 17:18:13.401083 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/author_search_request.py
+-rw-r--r--   0        0        0      992 2024-04-15 17:14:53.843869 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/authors_get_response.py
+-rw-r--r--   0        0        0      993 2024-04-15 17:14:53.843982 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/authors_post_response.py
+-rw-r--r--   0        0        0      862 2024-04-15 17:14:53.844086 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/cluster.py
+-rw-r--r--   0        0        0      604 2024-04-15 17:14:53.844195 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/cluster_articles.py
+-rw-r--r--   0        0        0     1106 2024-04-15 17:14:53.844317 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/clustering_search_response.py
+-rw-r--r--   0        0        0     1778 2024-04-15 17:14:53.844424 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0     1341 2024-04-15 17:14:53.844534 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     1326 2024-04-15 17:14:53.844641 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0      643 2024-04-15 17:14:53.844750 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1903 2024-04-15 17:14:53.844857 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0     1342 2024-04-15 17:14:53.844980 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     1327 2024-04-15 17:14:53.845092 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0      643 2024-04-15 17:14:53.845204 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1277 2024-04-15 17:14:53.845312 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0      637 2024-04-15 17:14:53.845423 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0      889 2024-04-15 17:14:53.845526 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/http_validation_error.py
+-rw-r--r--   0        0        0      838 2024-04-15 17:14:53.845628 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_get_response.py
+-rw-r--r--   0        0        0      839 2024-04-15 17:14:53.845736 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     2812 2024-04-15 17:18:13.401318 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_request.py
+-rw-r--r--   0        0        0     1138 2024-04-15 17:14:53.845939 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_response.py
+-rw-r--r--   0        0        0      620 2024-04-15 17:14:53.846038 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     2616 2024-04-15 17:14:53.846135 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/more_like_this_request.py
+-rw-r--r--   0        0        0      883 2024-04-15 17:14:53.846241 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_get_response.py
+-rw-r--r--   0        0        0      884 2024-04-15 17:14:53.846342 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_post_response.py
+-rw-r--r--   0        0        0     3031 2024-04-15 17:18:13.401517 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_request.py
+-rw-r--r--   0        0        0     1000 2024-04-15 17:14:53.846554 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_similar_get_response.py
+-rw-r--r--   0        0        0     1001 2024-04-15 17:14:53.846668 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_similar_post_response.py
+-rw-r--r--   0        0        0      957 2024-04-15 17:14:53.846769 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_url_request.py
+-rw-r--r--   0        0        0      836 2024-04-15 17:14:53.846875 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/similar_document.py
+-rw-r--r--   0        0        0      904 2024-04-15 17:14:53.846974 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_info.py
+-rw-r--r--   0        0        0      994 2024-04-15 17:14:53.847077 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_response.py
+-rw-r--r--   0        0        0      695 2024-04-15 17:14:53.847175 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_response_sources.py
+-rw-r--r--   0        0        0      996 2024-04-15 17:14:53.847270 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/sources_request.py
+-rw-r--r--   0        0        0      925 2024-04-15 17:14:53.847369 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/subscription_response.py
+-rw-r--r--   0        0        0      892 2024-04-15 17:14:53.847472 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/validation_error.py
+-rw-r--r--   0        0        0      623 2024-04-15 17:14:53.847570 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/validation_error_loc.py
+-rw-r--r--   0        0        0      758 2024-04-15 17:14:53.847687 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type_util.py
+-rw-r--r--   0        0        0     3177 2024-04-15 17:14:53.847810 newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/validation_metadata.py
+-rw-r--r--   0        0        0      791 2024-04-15 17:18:13.401672 newscatcherapi_python_sdk-6.0.3/pyproject.toml
+-rw-r--r--   0        0        0    76476 1970-01-01 00:00:00.000000 newscatcherapi_python_sdk-6.0.3/PKG-INFO
```

### Comparing `newscatcherapi_python_sdk-6.0.2/LICENSE` & `newscatcherapi_python_sdk-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/README.md` & `newscatcherapi_python_sdk-6.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # newscatcherapi-python-sdk<a id="newscatcherapi-python-sdk"></a>
 
 <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v6.0.2-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.2)
+[![PyPI](https://img.shields.io/badge/PyPI-v6.0.3-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.3)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/konfig-dev/newscatcher-sdks/tree/main/v3/python#readme)
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
 
 - [Requirements](#requirements)
@@ -36,15 +36,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install newscatcherapi-python-sdk==6.0.2
+pip install newscatcherapi-python-sdk==6.0.3
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from pprint import pprint
 from newscatcherapi_client import Newscatcher, ApiException
@@ -89,14 +89,16 @@
         ner_name="string_example",
         title_sentiment_min=3.14,
         title_sentiment_max=3.14,
         content_sentiment_min=3.14,
         content_sentiment_max=3.14,
         iptc_tags=None,
         not_iptc_tags=None,
+        iab_tags=None,
+        not_iab_tags=None,
     )
     print(get_response)
 except ApiException as e:
     print("Exception when calling AuthorsApi.get: %s\n" % e)
     pprint(e.body)
     if e.status == 422:
         pprint(e.body["detail"])
@@ -157,14 +159,16 @@
             ner_name="string_example",
             title_sentiment_min=3.14,
             title_sentiment_max=3.14,
             content_sentiment_min=3.14,
             content_sentiment_max=3.14,
             iptc_tags=None,
             not_iptc_tags=None,
+            iab_tags=None,
+            not_iab_tags=None,
         )
         print(get_response)
     except ApiException as e:
         print("Exception when calling AuthorsApi.get: %s\n" % e)
         pprint(e.body)
         if e.status == 422:
             pprint(e.body["detail"])
@@ -225,14 +229,16 @@
         ner_name="string_example",
         title_sentiment_min=3.14,
         title_sentiment_max=3.14,
         content_sentiment_min=3.14,
         content_sentiment_max=3.14,
         iptc_tags=None,
         not_iptc_tags=None,
+        iab_tags=None,
+        not_iab_tags=None,
     )
     pprint(get_response.body)
     pprint(get_response.headers)
     pprint(get_response.status)
     pprint(get_response.round_trip_time)
 except ApiException as e:
     print("Exception when calling AuthorsApi.get: %s\n" % e)
@@ -288,14 +294,16 @@
     ner_name="string_example",
     title_sentiment_min=3.14,
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
+    iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### author_name: `str`<a id="author_name-str"></a>
 
@@ -369,14 +377,18 @@
 
 ##### content_sentiment_max: `Union[int, float]`<a id="content_sentiment_max-unionint-float"></a>
 
 ##### iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
+##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`AuthorsGetResponse`](./newscatcherapi_client/pydantic/authors_get_response.py)
 
 #### 🌐 Endpoint<a id="🌐-endpoint"></a>
 
 `/api/authors` `get`
@@ -426,14 +438,16 @@
     ner_name="string_example",
     title_sentiment_min=3.14,
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
+    iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### author_name: `str`<a id="author_name-str"></a>
 
@@ -507,14 +521,18 @@
 
 ##### content_sentiment_max: `Union[int, float]`<a id="content_sentiment_max-unionint-float"></a>
 
 ##### iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
+##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`AuthorSearchRequest`](./newscatcherapi_client/type/author_search_request.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`AuthorsPostResponse`](./newscatcherapi_client/pydantic/authors_post_response.py)
 
@@ -567,14 +585,16 @@
     misc_entity_name="string_example",
     title_sentiment_min=3.14,
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
+    iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### when: `str`<a id="when-str"></a>
 
@@ -646,14 +666,18 @@
 
 ##### content_sentiment_max: `Union[int, float]`<a id="content_sentiment_max-unionint-float"></a>
 
 ##### iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
+##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`LatestHeadlinesGetResponse`](./newscatcherapi_client/pydantic/latest_headlines_get_response.py)
 
 #### 🌐 Endpoint<a id="🌐-endpoint"></a>
 
 `/api/latest_headlines` `get`
@@ -703,14 +727,16 @@
     misc_entity_name="string_example",
     title_sentiment_min=3.14,
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
+    iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### when: `str`<a id="when-str"></a>
 
@@ -782,14 +808,18 @@
 
 ##### content_sentiment_max: `Union[int, float]`<a id="content_sentiment_max-unionint-float"></a>
 
 ##### iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
+##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`LatestHeadlinesRequest`](./newscatcherapi_client/type/latest_headlines_request.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`LatestHeadlinesPostResponse`](./newscatcherapi_client/pydantic/latest_headlines_post_response.py)
 
@@ -851,14 +881,15 @@
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
     source_name=None,
     iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### q: `str`<a id="q-str"></a>
 
@@ -950,14 +981,16 @@
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### source_name: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="source_name-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`SearchGetResponse`](./newscatcherapi_client/pydantic/search_get_response.py)
 
 #### 🌐 Endpoint<a id="🌐-endpoint"></a>
 
 `/api/search` `get`
@@ -1016,14 +1049,15 @@
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
     source_name=None,
     iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### q: `str`<a id="q-str"></a>
 
@@ -1115,14 +1149,16 @@
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### source_name: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="source_name-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`SearchRequest`](./newscatcherapi_client/type/search_request.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`SearchPostResponse`](./newscatcherapi_client/pydantic/search_post_response.py)
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/__init__.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
     The version of the OpenAPI document: 3.2.16
     Contact: maksym@newscatcherapi.com
     Generated by: https://konfigthis.com
 """
 
-__version__ = "6.0.2"
+__version__ = "6.0.3"
 
 # import ApiClient
 from newscatcherapi_client.api_client import ApiClient
 
 # import Configuration
 from newscatcherapi_client.configuration import Configuration
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8 # flake8: noqa """ NewsCatcher-V3 Production API [https://
 uploads-ssl.webflow.com/6429857b17973b636c2195c5/
 646c6f1eb774ff2f2997bec5_newscatcher_.svg]
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
-konfigthis.com """ __version__ = "6.0.2" # import ApiClient from
+konfigthis.com """ __version__ = "6.0.3" # import ApiClient from
 newscatcherapi_client.api_client import ApiClient # import Configuration from
 newscatcherapi_client.configuration import Configuration # import exceptions
 from newscatcherapi_client.exceptions import OpenApiException from
 newscatcherapi_client.exceptions import ApiAttributeError from
 newscatcherapi_client.exceptions import ApiTypeError from
 newscatcherapi_client.exceptions import ApiValueError from
 newscatcherapi_client.exceptions import ApiKeyError from
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/api_client.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2984,15 +2984,15 @@
 0000ba70: 655d 203d 2068 6561 6465 725f 7661 6c75  e] = header_valu
 0000ba80: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
 0000ba90: 6f6f 6b69 6520 3d20 636f 6f6b 6965 0a20  ookie = cookie. 
 0000baa0: 2020 2020 2020 2023 2053 6574 2064 6566         # Set def
 0000bab0: 6175 6c74 2055 7365 722d 4167 656e 742e  ault User-Agent.
 0000bac0: 0a20 2020 2020 2020 2073 656c 662e 7573  .        self.us
 0000bad0: 6572 5f61 6765 6e74 203d 2027 4b6f 6e66  er_agent = 'Konf
-0000bae0: 6967 2f36 2e30 2e32 2f70 7974 686f 6e27  ig/6.0.2/python'
+0000bae0: 6967 2f36 2e30 2e33 2f70 7974 686f 6e27  ig/6.0.3/python'
 0000baf0: 0a0a 2020 2020 6465 6620 5f5f 656e 7465  ..    def __ente
 0000bb00: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
 0000bb10: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
 0000bb20: 2020 2020 6465 6620 5f5f 6578 6974 5f5f      def __exit__
 0000bb30: 2873 656c 662c 2065 7863 5f74 7970 652c  (self, exc_type,
 0000bb40: 2065 7863 5f76 616c 7565 2c20 7472 6163   exc_value, trac
 0000bb50: 6562 6163 6b29 3a0a 2020 2020 2020 2020  eback):.
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/api_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/api_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/path_to_api.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tag_to_api.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/authors_api.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/authors_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/authors_api_raw.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/authors_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/latest_headlines_api.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/latest_headlines_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_api.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_api_raw.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_link_api.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_link_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_link_api_raw.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_link_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_similar_api.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_similar_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/search_similar_api_raw.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/search_similar_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/sources_api.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/sources_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/sources_api_raw.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/sources_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/subscription_api.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/subscription_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/apis/tags/subscription_api_raw.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/apis/tags/subscription_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/client.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/client.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/client_custom.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/client_custom.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/configuration.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.2.16\n"\
-               "SDK Package Version: 6.0.2".\
+               "SDK Package Version: 6.0.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/exceptions.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/exceptions_base.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/additional_source_info.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/additional_source_info.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/author_search_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/author_search_request.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -137,56 +137,46 @@
             all_links = schemas.AnyTypeSchema
             all_domain_links = schemas.AnyTypeSchema
             
             
             class word_count_min(
                 schemas.IntSchema
             ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
+                pass
             
             
             class word_count_max(
                 schemas.IntSchema
             ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
+                pass
             
             
             class page(
                 schemas.IntSchema
             ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
+                pass
             
             
             class page_size(
                 schemas.IntSchema
             ):
-            
-            
-                class MetaOapg:
-                    inclusive_minimum = 0
+                pass
             include_nlp_data = schemas.BoolSchema
             has_nlp = schemas.BoolSchema
             theme = schemas.StrSchema
             not_theme = schemas.StrSchema
             ner_name = schemas.StrSchema
             title_sentiment_min = schemas.NumberSchema
             title_sentiment_max = schemas.NumberSchema
             content_sentiment_min = schemas.NumberSchema
             content_sentiment_max = schemas.NumberSchema
             iptc_tags = schemas.AnyTypeSchema
             not_iptc_tags = schemas.AnyTypeSchema
+            iab_tags = schemas.AnyTypeSchema
+            not_iab_tags = schemas.AnyTypeSchema
             __annotations__ = {
                 "author_name": author_name,
                 "not_author_name": not_author_name,
                 "sources": sources,
                 "predefined_sources": predefined_sources,
                 "not_sources": not_sources,
                 "lang": lang,
@@ -217,14 +207,16 @@
                 "ner_name": ner_name,
                 "title_sentiment_min": title_sentiment_min,
                 "title_sentiment_max": title_sentiment_max,
                 "content_sentiment_min": content_sentiment_min,
                 "content_sentiment_max": content_sentiment_max,
                 "iptc_tags": iptc_tags,
                 "not_iptc_tags": not_iptc_tags,
+                "iab_tags": iab_tags,
+                "not_iab_tags": not_iab_tags,
             }
     
     author_name: MetaOapg.properties.author_name
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["author_name"]) -> MetaOapg.properties.author_name: ...
     
@@ -333,17 +325,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["iptc_tags"]) -> MetaOapg.properties.iptc_tags: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["not_iptc_tags"]) -> MetaOapg.properties.not_iptc_tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["author_name", "not_author_name", "sources", "predefined_sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "include_nlp_data", "has_nlp", "theme", "not_theme", "ner_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["author_name", "not_author_name", "sources", "predefined_sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "include_nlp_data", "has_nlp", "theme", "not_theme", "ner_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags", "not_iab_tags", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["author_name"]) -> MetaOapg.properties.author_name: ...
     
@@ -452,17 +450,23 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["iptc_tags"]) -> typing.Union[MetaOapg.properties.iptc_tags, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["not_iptc_tags"]) -> typing.Union[MetaOapg.properties.not_iptc_tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["iab_tags"]) -> typing.Union[MetaOapg.properties.iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["author_name", "not_author_name", "sources", "predefined_sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "include_nlp_data", "has_nlp", "theme", "not_theme", "ner_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["author_name", "not_author_name", "sources", "predefined_sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "include_nlp_data", "has_nlp", "theme", "not_theme", "ner_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags", "not_iab_tags", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         author_name: typing.Union[MetaOapg.properties.author_name, str, ],
@@ -498,14 +502,16 @@
         ner_name: typing.Union[MetaOapg.properties.ner_name, str, schemas.Unset] = schemas.unset,
         title_sentiment_min: typing.Union[MetaOapg.properties.title_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         title_sentiment_max: typing.Union[MetaOapg.properties.title_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_min: typing.Union[MetaOapg.properties.content_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_max: typing.Union[MetaOapg.properties.content_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         iptc_tags: typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        iab_tags: typing.Union[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'AuthorSearchRequest':
         return super().__new__(
             cls,
             *args,
             author_name=author_name,
@@ -541,10 +547,12 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/author_search_request.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/author_search_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,44 +137,58 @@
             all_links = schemas.AnyTypeSchema
             all_domain_links = schemas.AnyTypeSchema
             
             
             class word_count_min(
                 schemas.IntSchema
             ):
-                pass
+            
+            
+                class MetaOapg:
+                    inclusive_minimum = 0
             
             
             class word_count_max(
                 schemas.IntSchema
             ):
-                pass
+            
+            
+                class MetaOapg:
+                    inclusive_minimum = 0
             
             
             class page(
                 schemas.IntSchema
             ):
-                pass
+            
+            
+                class MetaOapg:
+                    inclusive_minimum = 0
             
             
             class page_size(
                 schemas.IntSchema
             ):
-                pass
+            
+            
+                class MetaOapg:
+                    inclusive_minimum = 0
             include_nlp_data = schemas.BoolSchema
             has_nlp = schemas.BoolSchema
             theme = schemas.StrSchema
             not_theme = schemas.StrSchema
             ner_name = schemas.StrSchema
             title_sentiment_min = schemas.NumberSchema
             title_sentiment_max = schemas.NumberSchema
             content_sentiment_min = schemas.NumberSchema
             content_sentiment_max = schemas.NumberSchema
             iptc_tags = schemas.AnyTypeSchema
             not_iptc_tags = schemas.AnyTypeSchema
+            iab_tags = schemas.AnyTypeSchema
+            not_iab_tags = schemas.AnyTypeSchema
             __annotations__ = {
                 "author_name": author_name,
                 "not_author_name": not_author_name,
                 "sources": sources,
                 "predefined_sources": predefined_sources,
                 "not_sources": not_sources,
                 "lang": lang,
@@ -205,14 +219,16 @@
                 "ner_name": ner_name,
                 "title_sentiment_min": title_sentiment_min,
                 "title_sentiment_max": title_sentiment_max,
                 "content_sentiment_min": content_sentiment_min,
                 "content_sentiment_max": content_sentiment_max,
                 "iptc_tags": iptc_tags,
                 "not_iptc_tags": not_iptc_tags,
+                "iab_tags": iab_tags,
+                "not_iab_tags": not_iab_tags,
             }
     
     author_name: MetaOapg.properties.author_name
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["author_name"]) -> MetaOapg.properties.author_name: ...
     
@@ -321,17 +337,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["iptc_tags"]) -> MetaOapg.properties.iptc_tags: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["not_iptc_tags"]) -> MetaOapg.properties.not_iptc_tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["author_name", "not_author_name", "sources", "predefined_sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "include_nlp_data", "has_nlp", "theme", "not_theme", "ner_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["author_name", "not_author_name", "sources", "predefined_sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "include_nlp_data", "has_nlp", "theme", "not_theme", "ner_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags", "not_iab_tags", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["author_name"]) -> MetaOapg.properties.author_name: ...
     
@@ -440,17 +462,23 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["iptc_tags"]) -> typing.Union[MetaOapg.properties.iptc_tags, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["not_iptc_tags"]) -> typing.Union[MetaOapg.properties.not_iptc_tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["iab_tags"]) -> typing.Union[MetaOapg.properties.iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["author_name", "not_author_name", "sources", "predefined_sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "include_nlp_data", "has_nlp", "theme", "not_theme", "ner_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["author_name", "not_author_name", "sources", "predefined_sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "include_nlp_data", "has_nlp", "theme", "not_theme", "ner_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags", "not_iab_tags", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         author_name: typing.Union[MetaOapg.properties.author_name, str, ],
@@ -486,14 +514,16 @@
         ner_name: typing.Union[MetaOapg.properties.ner_name, str, schemas.Unset] = schemas.unset,
         title_sentiment_min: typing.Union[MetaOapg.properties.title_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         title_sentiment_max: typing.Union[MetaOapg.properties.title_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_min: typing.Union[MetaOapg.properties.content_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_max: typing.Union[MetaOapg.properties.content_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         iptc_tags: typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        iab_tags: typing.Union[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'AuthorSearchRequest':
         return super().__new__(
             cls,
             *args,
             author_name=author_name,
@@ -529,10 +559,12 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/authors_get_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/authors_post_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/authors_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/cluster.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/cluster.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/cluster_articles.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/cluster_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/clustering_search_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/clustering_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/http_validation_error.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_get_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_post_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,16 @@
             MISC_entity_name = schemas.StrSchema
             title_sentiment_min = schemas.NumberSchema
             title_sentiment_max = schemas.NumberSchema
             content_sentiment_min = schemas.NumberSchema
             content_sentiment_max = schemas.NumberSchema
             iptc_tags = schemas.AnyTypeSchema
             not_iptc_tags = schemas.AnyTypeSchema
+            iab_tags = schemas.AnyTypeSchema
+            not_iab_tags = schemas.AnyTypeSchema
             __annotations__ = {
                 "when": when,
                 "by_parse_date": by_parse_date,
                 "lang": lang,
                 "not_lang": not_lang,
                 "countries": countries,
                 "not_countries": not_countries,
@@ -138,14 +140,16 @@
                 "MISC_entity_name": MISC_entity_name,
                 "title_sentiment_min": title_sentiment_min,
                 "title_sentiment_max": title_sentiment_max,
                 "content_sentiment_min": content_sentiment_min,
                 "content_sentiment_max": content_sentiment_max,
                 "iptc_tags": iptc_tags,
                 "not_iptc_tags": not_iptc_tags,
+                "iab_tags": iab_tags,
+                "not_iab_tags": not_iab_tags,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["when"]) -> MetaOapg.properties.when: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["by_parse_date"]) -> MetaOapg.properties.by_parse_date: ...
@@ -252,17 +256,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["iptc_tags"]) -> MetaOapg.properties.iptc_tags: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["not_iptc_tags"]) -> MetaOapg.properties.not_iptc_tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources", "predefined_sources", "not_sources", "not_author_name", "ranked_only", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources", "predefined_sources", "not_sources", "not_author_name", "ranked_only", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags", "not_iab_tags", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["when"]) -> typing.Union[MetaOapg.properties.when, schemas.Unset]: ...
     
@@ -371,17 +381,23 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["iptc_tags"]) -> typing.Union[MetaOapg.properties.iptc_tags, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["not_iptc_tags"]) -> typing.Union[MetaOapg.properties.not_iptc_tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["iab_tags"]) -> typing.Union[MetaOapg.properties.iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources", "predefined_sources", "not_sources", "not_author_name", "ranked_only", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources", "predefined_sources", "not_sources", "not_author_name", "ranked_only", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags", "not_iab_tags", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         when: typing.Union[MetaOapg.properties.when, str, schemas.Unset] = schemas.unset,
@@ -417,14 +433,16 @@
         MISC_entity_name: typing.Union[MetaOapg.properties.MISC_entity_name, str, schemas.Unset] = schemas.unset,
         title_sentiment_min: typing.Union[MetaOapg.properties.title_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         title_sentiment_max: typing.Union[MetaOapg.properties.title_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_min: typing.Union[MetaOapg.properties.content_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_max: typing.Union[MetaOapg.properties.content_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         iptc_tags: typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        iab_tags: typing.Union[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'LatestHeadlinesRequest':
         return super().__new__(
             cls,
             *args,
             when=when,
@@ -460,10 +478,12 @@
             MISC_entity_name=MISC_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             _configuration=_configuration,
             **kwargs,
         )
```

#### html2text {}

```diff
@@ -27,15 +27,16 @@
 schemas.NumberSchema include_nlp_data = schemas.BoolSchema has_nlp =
 schemas.BoolSchema theme = schemas.StrSchema not_theme = schemas.StrSchema
 ORG_entity_name = schemas.StrSchema PER_entity_name = schemas.StrSchema
 LOC_entity_name = schemas.StrSchema MISC_entity_name = schemas.StrSchema
 title_sentiment_min = schemas.NumberSchema title_sentiment_max =
 schemas.NumberSchema content_sentiment_min = schemas.NumberSchema
 content_sentiment_max = schemas.NumberSchema iptc_tags = schemas.AnyTypeSchema
-not_iptc_tags = schemas.AnyTypeSchema __annotations__ = { "when": when,
+not_iptc_tags = schemas.AnyTypeSchema iab_tags = schemas.AnyTypeSchema
+not_iab_tags = schemas.AnyTypeSchema __annotations__ = { "when": when,
 "by_parse_date": by_parse_date, "lang": lang, "not_lang": not_lang,
 "countries": countries, "not_countries": not_countries, "sources": sources,
 "predefined_sources": predefined_sources, "not_sources": not_sources,
 "not_author_name": not_author_name, "ranked_only": ranked_only, "is_headline":
 is_headline, "is_paid_content": is_paid_content, "parent_url": parent_url,
 "all_links": all_links, "all_domain_links": all_domain_links, "word_count_min":
 word_count_min, "word_count_max": word_count_max, "page": page, "page_size":
@@ -43,25 +44,25 @@
 clustering_enabled, "clustering_threshold": clustering_threshold,
 "include_nlp_data": include_nlp_data, "has_nlp": has_nlp, "theme": theme,
 "not_theme": not_theme, "ORG_entity_name": ORG_entity_name, "PER_entity_name":
 PER_entity_name, "LOC_entity_name": LOC_entity_name, "MISC_entity_name":
 MISC_entity_name, "title_sentiment_min": title_sentiment_min,
 "title_sentiment_max": title_sentiment_max, "content_sentiment_min":
 content_sentiment_min, "content_sentiment_max": content_sentiment_max,
-"iptc_tags": iptc_tags, "not_iptc_tags": not_iptc_tags, } @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["when"]) -
-> MetaOapg.properties.when: ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["by_parse_date"]) -
-> MetaOapg.properties.by_parse_date: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["lang"]) -> MetaOapg.properties.lang: ...
+"iptc_tags": iptc_tags, "not_iptc_tags": not_iptc_tags, "iab_tags": iab_tags,
+"not_iab_tags": not_iab_tags, } @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["when"]) -> MetaOapg.properties.when: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["not_lang"]) -> MetaOapg.properties.not_lang: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["countries"]) -
-> MetaOapg.properties.countries: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["not_countries"]) -
+["by_parse_date"]) -> MetaOapg.properties.by_parse_date: ... @typing.overload
+def __getitem__(self, name: typing_extensions.Literal["lang"]) -
+> MetaOapg.properties.lang: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["not_lang"]) -> MetaOapg.properties.not_lang: ...
+@typing.overload def __getitem__(self, name: typing_extensions.Literal
+["countries"]) -> MetaOapg.properties.countries: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["not_countries"]) -
 > MetaOapg.properties.not_countries: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["sources"]) -> MetaOapg.properties.sources: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["predefined_sources"]) -> MetaOapg.properties.predefined_sources: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["not_sources"]) -> MetaOapg.properties.not_sources: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["not_author_name"]) -
@@ -113,37 +114,41 @@
 > MetaOapg.properties.content_sentiment_min: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["content_sentiment_max"]) -
 > MetaOapg.properties.content_sentiment_max: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["iptc_tags"]) -
 > MetaOapg.properties.iptc_tags: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["not_iptc_tags"]) -
 > MetaOapg.properties.not_iptc_tags: ... @typing.overload def __getitem__(self,
-name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name:
-typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang",
-"not_lang", "countries", "not_countries", "sources", "predefined_sources",
-"not_sources", "not_author_name", "ranked_only", "is_headline",
-"is_paid_content", "parent_url", "all_links", "all_domain_links",
-"word_count_min", "word_count_max", "page", "page_size", "clustering_variable",
-"clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp",
-"theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name",
-"MISC_entity_name", "title_sentiment_min", "title_sentiment_max",
-"content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags",
-], str]): # dict_instance[name] accessor return super().__getitem__(name)
-@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["when"]) -> typing.Union[MetaOapg.properties.when, schemas.Unset]: ...
-@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["by_parse_date"]) -> typing.Union[MetaOapg.properties.by_parse_date,
-schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["lang"]) -> typing.Union[MetaOapg.properties.lang,
+name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags:
+... @typing.overload def __getitem__(self, name: typing_extensions.Literal
+["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ... @typing.overload def
+__getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__
+(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date",
+"lang", "not_lang", "countries", "not_countries", "sources",
+"predefined_sources", "not_sources", "not_author_name", "ranked_only",
+"is_headline", "is_paid_content", "parent_url", "all_links",
+"all_domain_links", "word_count_min", "word_count_max", "page", "page_size",
+"clustering_variable", "clustering_enabled", "clustering_threshold",
+"include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name",
+"PER_entity_name", "LOC_entity_name", "MISC_entity_name",
+"title_sentiment_min", "title_sentiment_max", "content_sentiment_min",
+"content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags",
+"not_iab_tags", ], str]): # dict_instance[name] accessor return super
+().__getitem__(name) @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["when"]) -> typing.Union[MetaOapg.properties.when,
 schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["not_lang"]) -> typing.Union
-[MetaOapg.properties.not_lang, schemas.Unset]: ... @typing.overload def
-get_item_oapg(self, name: typing_extensions.Literal["countries"]) -
-> typing.Union[MetaOapg.properties.countries, schemas.Unset]: ...
+typing_extensions.Literal["by_parse_date"]) -> typing.Union
+[MetaOapg.properties.by_parse_date, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["lang"]) -> typing.Union
+[MetaOapg.properties.lang, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["not_lang"]) -
+> typing.Union[MetaOapg.properties.not_lang, schemas.Unset]: ...
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
+["countries"]) -> typing.Union[MetaOapg.properties.countries, schemas.Unset]:
+... @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["not_countries"]) -> typing.Union[MetaOapg.properties.not_countries,
 schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
 typing_extensions.Literal["sources"]) -> typing.Union
 [MetaOapg.properties.sources, schemas.Unset]: ... @typing.overload def
 get_item_oapg(self, name: typing_extensions.Literal["predefined_sources"]) -
 > typing.Union[MetaOapg.properties.predefined_sources, schemas.Unset]: ...
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
@@ -209,46 +214,51 @@
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["content_sentiment_max"]) -> typing.Union
 [MetaOapg.properties.content_sentiment_max, schemas.Unset]: ...
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["iptc_tags"]) -> typing.Union[MetaOapg.properties.iptc_tags, schemas.Unset]:
 ... @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["not_iptc_tags"]) -> typing.Union[MetaOapg.properties.not_iptc_tags,
-schemas.Unset]: ... @typing.overload def get_item_oapg(self, name: str) -
-> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ... def
-get_item_oapg(self, name: typing.Union[typing_extensions.Literal["when",
-"by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources",
-"predefined_sources", "not_sources", "not_author_name", "ranked_only",
-"is_headline", "is_paid_content", "parent_url", "all_links",
-"all_domain_links", "word_count_min", "word_count_max", "page", "page_size",
-"clustering_variable", "clustering_enabled", "clustering_threshold",
-"include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name",
-"PER_entity_name", "LOC_entity_name", "MISC_entity_name",
-"title_sentiment_min", "title_sentiment_max", "content_sentiment_min",
-"content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]): return super
-().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
-frozendict.frozendict, ], when: typing.Union[MetaOapg.properties.when, str,
-schemas.Unset] = schemas.unset, by_parse_date: typing.Union
-[MetaOapg.properties.by_parse_date, bool, schemas.Unset] = schemas.unset, lang:
-typing.Union[MetaOapg.properties.lang, dict, frozendict.frozendict, str, date,
+schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["iab_tags"]) -> typing.Union
+[MetaOapg.properties.iab_tags, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -
+> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
+@typing.overload def get_item_oapg(self, name: str) -> typing.Union
+[schemas.UnsetAnyTypeSchema, schemas.Unset]: ... def get_item_oapg(self, name:
+typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang",
+"not_lang", "countries", "not_countries", "sources", "predefined_sources",
+"not_sources", "not_author_name", "ranked_only", "is_headline",
+"is_paid_content", "parent_url", "all_links", "all_domain_links",
+"word_count_min", "word_count_max", "page", "page_size", "clustering_variable",
+"clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp",
+"theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name",
+"MISC_entity_name", "title_sentiment_min", "title_sentiment_max",
+"content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags",
+"iab_tags", "not_iab_tags", ], str]): return super().get_item_oapg(name) def
+__new__( cls, *args: typing.Union[dict, frozendict.frozendict, ], when:
+typing.Union[MetaOapg.properties.when, str, schemas.Unset] = schemas.unset,
+by_parse_date: typing.Union[MetaOapg.properties.by_parse_date, bool,
+schemas.Unset] = schemas.unset, lang: typing.Union[MetaOapg.properties.lang,
+dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+schemas.Unset] = schemas.unset, not_lang: typing.Union
+[MetaOapg.properties.not_lang, dict, frozendict.frozendict, str, date,
 datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple,
-bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset, not_lang:
-typing.Union[MetaOapg.properties.not_lang, dict, frozendict.frozendict, str,
+bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset, countries:
+typing.Union[MetaOapg.properties.countries, dict, frozendict.frozendict, str,
 date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list,
 tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-countries: typing.Union[MetaOapg.properties.countries, dict,
+not_countries: typing.Union[MetaOapg.properties.not_countries, dict,
 frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
-schemas.Unset] = schemas.unset, not_countries: typing.Union
-[MetaOapg.properties.not_countries, dict, frozendict.frozendict, str, date,
-datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple,
-bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset, sources:
-typing.Union[MetaOapg.properties.sources, dict, frozendict.frozendict, str,
-date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list,
-tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+schemas.Unset] = schemas.unset, sources: typing.Union
+[MetaOapg.properties.sources, dict, frozendict.frozendict, str, date, datetime,
+uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes,
+io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
 predefined_sources: typing.Union[MetaOapg.properties.predefined_sources, dict,
 frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
 schemas.Unset] = schemas.unset, not_sources: typing.Union
 [MetaOapg.properties.not_sources, dict, frozendict.frozendict, str, date,
 datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple,
 bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
@@ -303,14 +313,21 @@
 decimal.Decimal, int, float, schemas.Unset] = schemas.unset, iptc_tags:
 typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str,
 date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list,
 tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
 not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict,
 frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+schemas.Unset] = schemas.unset, iab_tags: typing.Union
+[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date,
+datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple,
+bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict,
+frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
 schemas.Unset] = schemas.unset, _configuration: typing.Optional
 [schemas.Configuration] = None, **kwargs: typing.Union[schemas.AnyTypeSchema,
 dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, None, list, tuple, bytes], ) -> 'LatestHeadlinesRequest':
 return super().__new__( cls, *args, when=when, by_parse_date=by_parse_date,
 lang=lang, not_lang=not_lang, countries=countries, not_countries=not_countries,
 sources=sources, predefined_sources=predefined_sources,
@@ -324,8 +341,9 @@
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 ORG_entity_name=ORG_entity_name, PER_entity_name=PER_entity_name,
 LOC_entity_name=LOC_entity_name, MISC_entity_name=MISC_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, _configuration=_configuration, **kwargs, )
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags,
+_configuration=_configuration, **kwargs, )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_request.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_request.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,16 @@
             MISC_entity_name = schemas.StrSchema
             title_sentiment_min = schemas.NumberSchema
             title_sentiment_max = schemas.NumberSchema
             content_sentiment_min = schemas.NumberSchema
             content_sentiment_max = schemas.NumberSchema
             iptc_tags = schemas.AnyTypeSchema
             not_iptc_tags = schemas.AnyTypeSchema
+            iab_tags = schemas.AnyTypeSchema
+            not_iab_tags = schemas.AnyTypeSchema
             __annotations__ = {
                 "when": when,
                 "by_parse_date": by_parse_date,
                 "lang": lang,
                 "not_lang": not_lang,
                 "countries": countries,
                 "not_countries": not_countries,
@@ -126,14 +128,16 @@
                 "MISC_entity_name": MISC_entity_name,
                 "title_sentiment_min": title_sentiment_min,
                 "title_sentiment_max": title_sentiment_max,
                 "content_sentiment_min": content_sentiment_min,
                 "content_sentiment_max": content_sentiment_max,
                 "iptc_tags": iptc_tags,
                 "not_iptc_tags": not_iptc_tags,
+                "iab_tags": iab_tags,
+                "not_iab_tags": not_iab_tags,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["when"]) -> MetaOapg.properties.when: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["by_parse_date"]) -> MetaOapg.properties.by_parse_date: ...
@@ -240,17 +244,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["iptc_tags"]) -> MetaOapg.properties.iptc_tags: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["not_iptc_tags"]) -> MetaOapg.properties.not_iptc_tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources", "predefined_sources", "not_sources", "not_author_name", "ranked_only", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources", "predefined_sources", "not_sources", "not_author_name", "ranked_only", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags", "not_iab_tags", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["when"]) -> typing.Union[MetaOapg.properties.when, schemas.Unset]: ...
     
@@ -359,17 +369,23 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["iptc_tags"]) -> typing.Union[MetaOapg.properties.iptc_tags, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["not_iptc_tags"]) -> typing.Union[MetaOapg.properties.not_iptc_tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["iab_tags"]) -> typing.Union[MetaOapg.properties.iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources", "predefined_sources", "not_sources", "not_author_name", "ranked_only", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources", "predefined_sources", "not_sources", "not_author_name", "ranked_only", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags", "not_iab_tags", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         when: typing.Union[MetaOapg.properties.when, str, schemas.Unset] = schemas.unset,
@@ -405,14 +421,16 @@
         MISC_entity_name: typing.Union[MetaOapg.properties.MISC_entity_name, str, schemas.Unset] = schemas.unset,
         title_sentiment_min: typing.Union[MetaOapg.properties.title_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         title_sentiment_max: typing.Union[MetaOapg.properties.title_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_min: typing.Union[MetaOapg.properties.content_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_max: typing.Union[MetaOapg.properties.content_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         iptc_tags: typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        iab_tags: typing.Union[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'LatestHeadlinesRequest':
         return super().__new__(
             cls,
             *args,
             when=when,
@@ -448,10 +466,12 @@
             MISC_entity_name=MISC_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             _configuration=_configuration,
             **kwargs,
         )
```

#### html2text {}

```diff
@@ -25,15 +25,16 @@
 = schemas.NumberSchema include_nlp_data = schemas.BoolSchema has_nlp =
 schemas.BoolSchema theme = schemas.StrSchema not_theme = schemas.StrSchema
 ORG_entity_name = schemas.StrSchema PER_entity_name = schemas.StrSchema
 LOC_entity_name = schemas.StrSchema MISC_entity_name = schemas.StrSchema
 title_sentiment_min = schemas.NumberSchema title_sentiment_max =
 schemas.NumberSchema content_sentiment_min = schemas.NumberSchema
 content_sentiment_max = schemas.NumberSchema iptc_tags = schemas.AnyTypeSchema
-not_iptc_tags = schemas.AnyTypeSchema __annotations__ = { "when": when,
+not_iptc_tags = schemas.AnyTypeSchema iab_tags = schemas.AnyTypeSchema
+not_iab_tags = schemas.AnyTypeSchema __annotations__ = { "when": when,
 "by_parse_date": by_parse_date, "lang": lang, "not_lang": not_lang,
 "countries": countries, "not_countries": not_countries, "sources": sources,
 "predefined_sources": predefined_sources, "not_sources": not_sources,
 "not_author_name": not_author_name, "ranked_only": ranked_only, "is_headline":
 is_headline, "is_paid_content": is_paid_content, "parent_url": parent_url,
 "all_links": all_links, "all_domain_links": all_domain_links, "word_count_min":
 word_count_min, "word_count_max": word_count_max, "page": page, "page_size":
@@ -41,25 +42,25 @@
 clustering_enabled, "clustering_threshold": clustering_threshold,
 "include_nlp_data": include_nlp_data, "has_nlp": has_nlp, "theme": theme,
 "not_theme": not_theme, "ORG_entity_name": ORG_entity_name, "PER_entity_name":
 PER_entity_name, "LOC_entity_name": LOC_entity_name, "MISC_entity_name":
 MISC_entity_name, "title_sentiment_min": title_sentiment_min,
 "title_sentiment_max": title_sentiment_max, "content_sentiment_min":
 content_sentiment_min, "content_sentiment_max": content_sentiment_max,
-"iptc_tags": iptc_tags, "not_iptc_tags": not_iptc_tags, } @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["when"]) -
-> MetaOapg.properties.when: ... @typing.overload def __getitem__(self, name:
-typing_extensions.Literal["by_parse_date"]) -
-> MetaOapg.properties.by_parse_date: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["lang"]) -> MetaOapg.properties.lang: ...
+"iptc_tags": iptc_tags, "not_iptc_tags": not_iptc_tags, "iab_tags": iab_tags,
+"not_iab_tags": not_iab_tags, } @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["when"]) -> MetaOapg.properties.when: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
-["not_lang"]) -> MetaOapg.properties.not_lang: ... @typing.overload def
-__getitem__(self, name: typing_extensions.Literal["countries"]) -
-> MetaOapg.properties.countries: ... @typing.overload def __getitem__(self,
-name: typing_extensions.Literal["not_countries"]) -
+["by_parse_date"]) -> MetaOapg.properties.by_parse_date: ... @typing.overload
+def __getitem__(self, name: typing_extensions.Literal["lang"]) -
+> MetaOapg.properties.lang: ... @typing.overload def __getitem__(self, name:
+typing_extensions.Literal["not_lang"]) -> MetaOapg.properties.not_lang: ...
+@typing.overload def __getitem__(self, name: typing_extensions.Literal
+["countries"]) -> MetaOapg.properties.countries: ... @typing.overload def
+__getitem__(self, name: typing_extensions.Literal["not_countries"]) -
 > MetaOapg.properties.not_countries: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["sources"]) -> MetaOapg.properties.sources: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["predefined_sources"]) -> MetaOapg.properties.predefined_sources: ...
 @typing.overload def __getitem__(self, name: typing_extensions.Literal
 ["not_sources"]) -> MetaOapg.properties.not_sources: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["not_author_name"]) -
@@ -111,37 +112,41 @@
 > MetaOapg.properties.content_sentiment_min: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["content_sentiment_max"]) -
 > MetaOapg.properties.content_sentiment_max: ... @typing.overload def
 __getitem__(self, name: typing_extensions.Literal["iptc_tags"]) -
 > MetaOapg.properties.iptc_tags: ... @typing.overload def __getitem__(self,
 name: typing_extensions.Literal["not_iptc_tags"]) -
 > MetaOapg.properties.not_iptc_tags: ... @typing.overload def __getitem__(self,
-name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__(self, name:
-typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang",
-"not_lang", "countries", "not_countries", "sources", "predefined_sources",
-"not_sources", "not_author_name", "ranked_only", "is_headline",
-"is_paid_content", "parent_url", "all_links", "all_domain_links",
-"word_count_min", "word_count_max", "page", "page_size", "clustering_variable",
-"clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp",
-"theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name",
-"MISC_entity_name", "title_sentiment_min", "title_sentiment_max",
-"content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags",
-], str]): # dict_instance[name] accessor return super().__getitem__(name)
-@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["when"]) -> typing.Union[MetaOapg.properties.when, schemas.Unset]: ...
-@typing.overload def get_item_oapg(self, name: typing_extensions.Literal
-["by_parse_date"]) -> typing.Union[MetaOapg.properties.by_parse_date,
-schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["lang"]) -> typing.Union[MetaOapg.properties.lang,
+name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags:
+... @typing.overload def __getitem__(self, name: typing_extensions.Literal
+["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ... @typing.overload def
+__getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ... def __getitem__
+(self, name: typing.Union[typing_extensions.Literal["when", "by_parse_date",
+"lang", "not_lang", "countries", "not_countries", "sources",
+"predefined_sources", "not_sources", "not_author_name", "ranked_only",
+"is_headline", "is_paid_content", "parent_url", "all_links",
+"all_domain_links", "word_count_min", "word_count_max", "page", "page_size",
+"clustering_variable", "clustering_enabled", "clustering_threshold",
+"include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name",
+"PER_entity_name", "LOC_entity_name", "MISC_entity_name",
+"title_sentiment_min", "title_sentiment_max", "content_sentiment_min",
+"content_sentiment_max", "iptc_tags", "not_iptc_tags", "iab_tags",
+"not_iab_tags", ], str]): # dict_instance[name] accessor return super
+().__getitem__(name) @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["when"]) -> typing.Union[MetaOapg.properties.when,
 schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
-typing_extensions.Literal["not_lang"]) -> typing.Union
-[MetaOapg.properties.not_lang, schemas.Unset]: ... @typing.overload def
-get_item_oapg(self, name: typing_extensions.Literal["countries"]) -
-> typing.Union[MetaOapg.properties.countries, schemas.Unset]: ...
+typing_extensions.Literal["by_parse_date"]) -> typing.Union
+[MetaOapg.properties.by_parse_date, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["lang"]) -> typing.Union
+[MetaOapg.properties.lang, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["not_lang"]) -
+> typing.Union[MetaOapg.properties.not_lang, schemas.Unset]: ...
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
+["countries"]) -> typing.Union[MetaOapg.properties.countries, schemas.Unset]:
+... @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["not_countries"]) -> typing.Union[MetaOapg.properties.not_countries,
 schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
 typing_extensions.Literal["sources"]) -> typing.Union
 [MetaOapg.properties.sources, schemas.Unset]: ... @typing.overload def
 get_item_oapg(self, name: typing_extensions.Literal["predefined_sources"]) -
 > typing.Union[MetaOapg.properties.predefined_sources, schemas.Unset]: ...
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
@@ -207,46 +212,51 @@
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["content_sentiment_max"]) -> typing.Union
 [MetaOapg.properties.content_sentiment_max, schemas.Unset]: ...
 @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["iptc_tags"]) -> typing.Union[MetaOapg.properties.iptc_tags, schemas.Unset]:
 ... @typing.overload def get_item_oapg(self, name: typing_extensions.Literal
 ["not_iptc_tags"]) -> typing.Union[MetaOapg.properties.not_iptc_tags,
-schemas.Unset]: ... @typing.overload def get_item_oapg(self, name: str) -
-> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ... def
-get_item_oapg(self, name: typing.Union[typing_extensions.Literal["when",
-"by_parse_date", "lang", "not_lang", "countries", "not_countries", "sources",
-"predefined_sources", "not_sources", "not_author_name", "ranked_only",
-"is_headline", "is_paid_content", "parent_url", "all_links",
-"all_domain_links", "word_count_min", "word_count_max", "page", "page_size",
-"clustering_variable", "clustering_enabled", "clustering_threshold",
-"include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name",
-"PER_entity_name", "LOC_entity_name", "MISC_entity_name",
-"title_sentiment_min", "title_sentiment_max", "content_sentiment_min",
-"content_sentiment_max", "iptc_tags", "not_iptc_tags", ], str]): return super
-().get_item_oapg(name) def __new__( cls, *args: typing.Union[dict,
-frozendict.frozendict, ], when: typing.Union[MetaOapg.properties.when, str,
-schemas.Unset] = schemas.unset, by_parse_date: typing.Union
-[MetaOapg.properties.by_parse_date, bool, schemas.Unset] = schemas.unset, lang:
-typing.Union[MetaOapg.properties.lang, dict, frozendict.frozendict, str, date,
+schemas.Unset]: ... @typing.overload def get_item_oapg(self, name:
+typing_extensions.Literal["iab_tags"]) -> typing.Union
+[MetaOapg.properties.iab_tags, schemas.Unset]: ... @typing.overload def
+get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -
+> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
+@typing.overload def get_item_oapg(self, name: str) -> typing.Union
+[schemas.UnsetAnyTypeSchema, schemas.Unset]: ... def get_item_oapg(self, name:
+typing.Union[typing_extensions.Literal["when", "by_parse_date", "lang",
+"not_lang", "countries", "not_countries", "sources", "predefined_sources",
+"not_sources", "not_author_name", "ranked_only", "is_headline",
+"is_paid_content", "parent_url", "all_links", "all_domain_links",
+"word_count_min", "word_count_max", "page", "page_size", "clustering_variable",
+"clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp",
+"theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name",
+"MISC_entity_name", "title_sentiment_min", "title_sentiment_max",
+"content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags",
+"iab_tags", "not_iab_tags", ], str]): return super().get_item_oapg(name) def
+__new__( cls, *args: typing.Union[dict, frozendict.frozendict, ], when:
+typing.Union[MetaOapg.properties.when, str, schemas.Unset] = schemas.unset,
+by_parse_date: typing.Union[MetaOapg.properties.by_parse_date, bool,
+schemas.Unset] = schemas.unset, lang: typing.Union[MetaOapg.properties.lang,
+dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+schemas.Unset] = schemas.unset, not_lang: typing.Union
+[MetaOapg.properties.not_lang, dict, frozendict.frozendict, str, date,
 datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple,
-bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset, not_lang:
-typing.Union[MetaOapg.properties.not_lang, dict, frozendict.frozendict, str,
+bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset, countries:
+typing.Union[MetaOapg.properties.countries, dict, frozendict.frozendict, str,
 date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list,
 tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-countries: typing.Union[MetaOapg.properties.countries, dict,
+not_countries: typing.Union[MetaOapg.properties.not_countries, dict,
 frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
-schemas.Unset] = schemas.unset, not_countries: typing.Union
-[MetaOapg.properties.not_countries, dict, frozendict.frozendict, str, date,
-datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple,
-bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset, sources:
-typing.Union[MetaOapg.properties.sources, dict, frozendict.frozendict, str,
-date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list,
-tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+schemas.Unset] = schemas.unset, sources: typing.Union
+[MetaOapg.properties.sources, dict, frozendict.frozendict, str, date, datetime,
+uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes,
+io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
 predefined_sources: typing.Union[MetaOapg.properties.predefined_sources, dict,
 frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
 schemas.Unset] = schemas.unset, not_sources: typing.Union
 [MetaOapg.properties.not_sources, dict, frozendict.frozendict, str, date,
 datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple,
 bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
@@ -301,14 +311,21 @@
 decimal.Decimal, int, float, schemas.Unset] = schemas.unset, iptc_tags:
 typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str,
 date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list,
 tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
 not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict,
 frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+schemas.Unset] = schemas.unset, iab_tags: typing.Union
+[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date,
+datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple,
+bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict,
+frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
 schemas.Unset] = schemas.unset, _configuration: typing.Optional
 [schemas.Configuration] = None, **kwargs: typing.Union[schemas.AnyTypeSchema,
 dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, None, list, tuple, bytes], ) -> 'LatestHeadlinesRequest':
 return super().__new__( cls, *args, when=when, by_parse_date=by_parse_date,
 lang=lang, not_lang=not_lang, countries=countries, not_countries=not_countries,
 sources=sources, predefined_sources=predefined_sources,
@@ -322,8 +339,9 @@
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 ORG_entity_name=ORG_entity_name, PER_entity_name=PER_entity_name,
 LOC_entity_name=LOC_entity_name, MISC_entity_name=MISC_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, _configuration=_configuration, **kwargs, )
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags,
+_configuration=_configuration, **kwargs, )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/latest_headlines_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/latest_headlines_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/more_like_this_request.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/more_like_this_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_get_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_post_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,15 @@
             title_sentiment_max = schemas.NumberSchema
             content_sentiment_min = schemas.NumberSchema
             content_sentiment_max = schemas.NumberSchema
             iptc_tags = schemas.AnyTypeSchema
             not_iptc_tags = schemas.AnyTypeSchema
             source_name = schemas.AnyTypeSchema
             iab_tags = schemas.AnyTypeSchema
+            not_iab_tags = schemas.AnyTypeSchema
             __annotations__ = {
                 "q": q,
                 "search_in": search_in,
                 "predefined_sources": predefined_sources,
                 "sources": sources,
                 "not_sources": not_sources,
                 "lang": lang,
@@ -235,14 +236,15 @@
                 "title_sentiment_max": title_sentiment_max,
                 "content_sentiment_min": content_sentiment_min,
                 "content_sentiment_max": content_sentiment_max,
                 "iptc_tags": iptc_tags,
                 "not_iptc_tags": not_iptc_tags,
                 "source_name": source_name,
                 "iab_tags": iab_tags,
+                "not_iab_tags": not_iab_tags,
             }
     
     q: MetaOapg.properties.q
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["q"]) -> MetaOapg.properties.q: ...
     
@@ -378,17 +380,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source_name"]) -> MetaOapg.properties.source_name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["q"]) -> MetaOapg.properties.q: ...
     
@@ -524,17 +529,20 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source_name"]) -> typing.Union[MetaOapg.properties.source_name, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["iab_tags"]) -> typing.Union[MetaOapg.properties.iab_tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         q: typing.Union[MetaOapg.properties.q, str, ],
@@ -579,14 +587,15 @@
         title_sentiment_max: typing.Union[MetaOapg.properties.title_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_min: typing.Union[MetaOapg.properties.content_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_max: typing.Union[MetaOapg.properties.content_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         iptc_tags: typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         source_name: typing.Union[MetaOapg.properties.source_name, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         iab_tags: typing.Union[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'SearchRequest':
         return super().__new__(
             cls,
             *args,
             q=q,
@@ -631,10 +640,11 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_request.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_request.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
             title_sentiment_max = schemas.NumberSchema
             content_sentiment_min = schemas.NumberSchema
             content_sentiment_max = schemas.NumberSchema
             iptc_tags = schemas.AnyTypeSchema
             not_iptc_tags = schemas.AnyTypeSchema
             source_name = schemas.AnyTypeSchema
             iab_tags = schemas.AnyTypeSchema
+            not_iab_tags = schemas.AnyTypeSchema
             __annotations__ = {
                 "q": q,
                 "search_in": search_in,
                 "predefined_sources": predefined_sources,
                 "sources": sources,
                 "not_sources": not_sources,
                 "lang": lang,
@@ -223,14 +224,15 @@
                 "title_sentiment_max": title_sentiment_max,
                 "content_sentiment_min": content_sentiment_min,
                 "content_sentiment_max": content_sentiment_max,
                 "iptc_tags": iptc_tags,
                 "not_iptc_tags": not_iptc_tags,
                 "source_name": source_name,
                 "iab_tags": iab_tags,
+                "not_iab_tags": not_iab_tags,
             }
     
     q: MetaOapg.properties.q
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["q"]) -> MetaOapg.properties.q: ...
     
@@ -366,17 +368,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source_name"]) -> MetaOapg.properties.source_name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["q"]) -> MetaOapg.properties.q: ...
     
@@ -512,17 +517,20 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source_name"]) -> typing.Union[MetaOapg.properties.source_name, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["iab_tags"]) -> typing.Union[MetaOapg.properties.iab_tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         q: typing.Union[MetaOapg.properties.q, str, ],
@@ -567,14 +575,15 @@
         title_sentiment_max: typing.Union[MetaOapg.properties.title_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_min: typing.Union[MetaOapg.properties.content_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_max: typing.Union[MetaOapg.properties.content_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         iptc_tags: typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         source_name: typing.Union[MetaOapg.properties.source_name, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         iab_tags: typing.Union[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'SearchRequest':
         return super().__new__(
             cls,
             *args,
             q=q,
@@ -619,10 +628,11 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_similar_get_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_similar_post_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_similar_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_url_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_url_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/search_url_request.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/search_url_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/similar_document.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/similar_document.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/similar_document.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_info.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_info.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_info.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/source_response_sources.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/source_response_sources.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/sources_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/sources_request.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/sources_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/subscription_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/subscription_response.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/subscription_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/validation_error.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/validation_error.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/model/validation_error_loc.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/model/validation_error_loc.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/models/__init__.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/operation_parameter_map.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/operation_parameter_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,20 @@
             },
             {
                 'name': 'iptc_tags'
             },
             {
                 'name': 'not_iptc_tags'
             },
+            {
+                'name': 'iab_tags'
+            },
+            {
+                'name': 'not_iab_tags'
+            },
         ]
     },
     '/api/authors-POST': {
         'parameters': [
             {
                 'name': 'author_name'
             },
@@ -223,14 +229,20 @@
             },
             {
                 'name': 'iptc_tags'
             },
             {
                 'name': 'not_iptc_tags'
             },
+            {
+                'name': 'iab_tags'
+            },
+            {
+                'name': 'not_iab_tags'
+            },
         ]
     },
     '/api/latest_headlines-GET': {
         'parameters': [
             {
                 'name': 'when'
             },
@@ -338,14 +350,20 @@
             },
             {
                 'name': 'iptc_tags'
             },
             {
                 'name': 'not_iptc_tags'
             },
+            {
+                'name': 'iab_tags'
+            },
+            {
+                'name': 'not_iab_tags'
+            },
         ]
     },
     '/api/latest_headlines-POST': {
         'parameters': [
             {
                 'name': 'when'
             },
@@ -453,14 +471,20 @@
             },
             {
                 'name': 'iptc_tags'
             },
             {
                 'name': 'not_iptc_tags'
             },
+            {
+                'name': 'iab_tags'
+            },
+            {
+                'name': 'not_iab_tags'
+            },
         ]
     },
     '/api/search-GET': {
         'parameters': [
             {
                 'name': 'q'
             },
@@ -595,14 +619,17 @@
             },
             {
                 'name': 'source_name'
             },
             {
                 'name': 'iab_tags'
             },
+            {
+                'name': 'not_iab_tags'
+            },
         ]
     },
     '/api/search-POST': {
         'parameters': [
             {
                 'name': 'q'
             },
@@ -737,14 +764,17 @@
             },
             {
                 'name': 'source_name'
             },
             {
                 'name': 'iab_tags'
             },
+            {
+                'name': 'not_iab_tags'
+            },
         ]
     },
     '/api/search_by_link-GET': {
         'parameters': [
             {
                 'name': 'ids'
             },
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/__init__.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_authors/get.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,14 +187,16 @@
 NerNameSchema = schemas.StrSchema
 TitleSentimentMinSchema = schemas.NumberSchema
 TitleSentimentMaxSchema = schemas.NumberSchema
 ContentSentimentMinSchema = schemas.NumberSchema
 ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema
 NotIptcTagsSchema = schemas.AnyTypeSchema
+IabTagsSchema = schemas.AnyTypeSchema
+NotIabTagsSchema = schemas.AnyTypeSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
         'author_name': typing.Union[AuthorNameSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
@@ -232,14 +234,16 @@
         'ner_name': typing.Union[NerNameSchema, str, ],
         'title_sentiment_min': typing.Union[TitleSentimentMinSchema, decimal.Decimal, int, float, ],
         'title_sentiment_max': typing.Union[TitleSentimentMaxSchema, decimal.Decimal, int, float, ],
         'content_sentiment_min': typing.Union[ContentSentimentMinSchema, decimal.Decimal, int, float, ],
         'content_sentiment_max': typing.Union[ContentSentimentMaxSchema, decimal.Decimal, int, float, ],
         'iptc_tags': typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iptc_tags': typing.Union[NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'iab_tags': typing.Union[IabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -464,14 +468,26 @@
 )
 request_query_not_iptc_tags = api_client.QueryParameter(
     name="not_iptc_tags",
     style=api_client.ParameterStyle.FORM,
     schema=NotIptcTagsSchema,
     explode=True,
 )
+request_query_iab_tags = api_client.QueryParameter(
+    name="iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=IabTagsSchema,
+    explode=True,
+)
+request_query_not_iab_tags = api_client.QueryParameter(
+    name="not_iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=NotIabTagsSchema,
+    explode=True,
+)
 _auth = [
     'apiKey',
 ]
 SchemaFor200ResponseBodyApplicationJson = AuthorsGetResponseSchema
 
 
 @dataclass
@@ -559,14 +575,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
         if author_name is not None:
             _query_params["author_name"] = author_name
         if not_author_name is not None:
             _query_params["not_author_name"] = not_author_name
@@ -636,14 +654,18 @@
             _query_params["content_sentiment_min"] = content_sentiment_min
         if content_sentiment_max is not None:
             _query_params["content_sentiment_max"] = content_sentiment_max
         if iptc_tags is not None:
             _query_params["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _query_params["not_iptc_tags"] = not_iptc_tags
+        if iab_tags is not None:
+            _query_params["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _query_params["not_iab_tags"] = not_iab_tags
         args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -700,14 +722,16 @@
             request_query_ner_name,
             request_query_title_sentiment_min,
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
+            request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -848,14 +872,16 @@
             request_query_ner_name,
             request_query_title_sentiment_min,
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
+            request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -948,14 +974,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -992,14 +1020,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1037,14 +1067,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             author_name=author_name,
             not_author_name=not_author_name,
@@ -1079,14 +1111,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
 
 class Get(BaseApi):
 
@@ -1125,14 +1159,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> AuthorsGetResponsePydantic:
         raw_response = await self.raw.aget(
             author_name=author_name,
             not_author_name=not_author_name,
             sources=sources,
@@ -1166,14 +1202,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[AuthorsGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(AuthorsGetResponsePydantic, raw_response.body)
     
     
@@ -1212,14 +1250,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> AuthorsGetResponsePydantic:
         raw_response = self.raw.get(
             author_name=author_name,
             not_author_name=not_author_name,
             sources=sources,
             predefined_sources=predefined_sources,
@@ -1252,14 +1292,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[AuthorsGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(AuthorsGetResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
@@ -1300,14 +1342,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1344,14 +1388,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1389,14 +1435,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             author_name=author_name,
             not_author_name=not_author_name,
@@ -1431,12 +1479,14 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_authors/get.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/get.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -173,14 +173,16 @@
 NerNameSchema = schemas.StrSchema
 TitleSentimentMinSchema = schemas.NumberSchema
 TitleSentimentMaxSchema = schemas.NumberSchema
 ContentSentimentMinSchema = schemas.NumberSchema
 ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema
 NotIptcTagsSchema = schemas.AnyTypeSchema
+IabTagsSchema = schemas.AnyTypeSchema
+NotIabTagsSchema = schemas.AnyTypeSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
         'author_name': typing.Union[AuthorNameSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
@@ -218,14 +220,16 @@
         'ner_name': typing.Union[NerNameSchema, str, ],
         'title_sentiment_min': typing.Union[TitleSentimentMinSchema, decimal.Decimal, int, float, ],
         'title_sentiment_max': typing.Union[TitleSentimentMaxSchema, decimal.Decimal, int, float, ],
         'content_sentiment_min': typing.Union[ContentSentimentMinSchema, decimal.Decimal, int, float, ],
         'content_sentiment_max': typing.Union[ContentSentimentMaxSchema, decimal.Decimal, int, float, ],
         'iptc_tags': typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iptc_tags': typing.Union[NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'iab_tags': typing.Union[IabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -450,14 +454,26 @@
 )
 request_query_not_iptc_tags = api_client.QueryParameter(
     name="not_iptc_tags",
     style=api_client.ParameterStyle.FORM,
     schema=NotIptcTagsSchema,
     explode=True,
 )
+request_query_iab_tags = api_client.QueryParameter(
+    name="iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=IabTagsSchema,
+    explode=True,
+)
+request_query_not_iab_tags = api_client.QueryParameter(
+    name="not_iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=NotIabTagsSchema,
+    explode=True,
+)
 SchemaFor200ResponseBodyApplicationJson = AuthorsGetResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: AuthorsGetResponse
 
@@ -538,14 +554,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
         if author_name is not None:
             _query_params["author_name"] = author_name
         if not_author_name is not None:
             _query_params["not_author_name"] = not_author_name
@@ -615,14 +633,18 @@
             _query_params["content_sentiment_min"] = content_sentiment_min
         if content_sentiment_max is not None:
             _query_params["content_sentiment_max"] = content_sentiment_max
         if iptc_tags is not None:
             _query_params["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _query_params["not_iptc_tags"] = not_iptc_tags
+        if iab_tags is not None:
+            _query_params["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _query_params["not_iab_tags"] = not_iab_tags
         args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -679,14 +701,16 @@
             request_query_ner_name,
             request_query_title_sentiment_min,
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
+            request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -827,14 +851,16 @@
             request_query_ner_name,
             request_query_title_sentiment_min,
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
+            request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -927,14 +953,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -971,14 +999,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1016,14 +1046,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             author_name=author_name,
             not_author_name=not_author_name,
@@ -1058,14 +1090,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
 
 class Get(BaseApi):
 
@@ -1104,14 +1138,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> AuthorsGetResponsePydantic:
         raw_response = await self.raw.aget(
             author_name=author_name,
             not_author_name=not_author_name,
             sources=sources,
@@ -1145,14 +1181,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[AuthorsGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(AuthorsGetResponsePydantic, raw_response.body)
     
     
@@ -1191,14 +1229,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> AuthorsGetResponsePydantic:
         raw_response = self.raw.get(
             author_name=author_name,
             not_author_name=not_author_name,
             sources=sources,
             predefined_sources=predefined_sources,
@@ -1231,14 +1271,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[AuthorsGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(AuthorsGetResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
@@ -1279,14 +1321,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1323,14 +1367,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1368,14 +1414,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             author_name=author_name,
             not_author_name=not_author_name,
@@ -1410,12 +1458,14 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_authors/post.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,14 +150,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if author_name is not None:
             _body["author_name"] = author_name
         if not_author_name is not None:
             _body["not_author_name"] = not_author_name
@@ -227,14 +229,18 @@
             _body["content_sentiment_min"] = content_sentiment_min
         if content_sentiment_max is not None:
             _body["content_sentiment_max"] = content_sentiment_max
         if iptc_tags is not None:
             _body["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _body["not_iptc_tags"] = not_iptc_tags
+        if iab_tags is not None:
+            _body["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _body["not_iab_tags"] = not_iab_tags
         args.body = _body
         return args
 
     async def _apost_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -471,14 +477,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -515,14 +523,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -560,14 +570,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             author_name=author_name,
             not_author_name=not_author_name,
@@ -602,14 +614,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
 
 class Post(BaseApi):
 
@@ -648,14 +662,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> AuthorsPostResponsePydantic:
         raw_response = await self.raw.apost(
             author_name=author_name,
             not_author_name=not_author_name,
             sources=sources,
@@ -689,14 +705,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[AuthorsPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(AuthorsPostResponsePydantic, raw_response.body)
     
     
@@ -735,14 +753,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> AuthorsPostResponsePydantic:
         raw_response = self.raw.post(
             author_name=author_name,
             not_author_name=not_author_name,
             sources=sources,
             predefined_sources=predefined_sources,
@@ -775,14 +795,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[AuthorsPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(AuthorsPostResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
@@ -823,14 +845,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -867,14 +891,16 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -912,14 +938,16 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             author_name=author_name,
             not_author_name=not_author_name,
@@ -954,12 +982,14 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_authors/post.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/post.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,49 +29,54 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
+from newscatcherapi_client.model.search_similar_post_response import SearchSimilarPostResponse as SearchSimilarPostResponseSchema
+from newscatcherapi_client.model.more_like_this_request import MoreLikeThisRequest as MoreLikeThisRequestSchema
 from newscatcherapi_client.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from newscatcherapi_client.model.author_search_request import AuthorSearchRequest as AuthorSearchRequestSchema
-from newscatcherapi_client.model.authors_post_response import AuthorsPostResponse as AuthorsPostResponseSchema
 
+from newscatcherapi_client.type.more_like_this_request import MoreLikeThisRequest
+from newscatcherapi_client.type.search_similar_post_response import SearchSimilarPostResponse
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
-from newscatcherapi_client.type.authors_post_response import AuthorsPostResponse
-from newscatcherapi_client.type.author_search_request import AuthorSearchRequest
 
 from ...api_client import Dictionary
-from newscatcherapi_client.pydantic.author_search_request import AuthorSearchRequest as AuthorSearchRequestPydantic
+from newscatcherapi_client.pydantic.search_similar_post_response import SearchSimilarPostResponse as SearchSimilarPostResponsePydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
-from newscatcherapi_client.pydantic.authors_post_response import AuthorsPostResponse as AuthorsPostResponsePydantic
+from newscatcherapi_client.pydantic.more_like_this_request import MoreLikeThisRequest as MoreLikeThisRequestPydantic
+
+from . import path
 
 # body param
-SchemaForRequestBodyApplicationJson = AuthorSearchRequestSchema
+SchemaForRequestBodyApplicationJson = MoreLikeThisRequestSchema
 
 
-request_body_author_search_request = api_client.RequestBody(
+request_body_more_like_this_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = AuthorsPostResponseSchema
+_auth = [
+    'apiKey',
+]
+SchemaFor200ResponseBodyApplicationJson = SearchSimilarPostResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: AuthorsPostResponse
+    body: SearchSimilarPostResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: AuthorsPostResponse
+    body: SearchSimilarPostResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -95,36 +100,43 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
     def _post_mapped_args(
         self,
-        author_name: str,
-        not_author_name: typing.Optional[str] = None,
-        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        q: str,
+        search_in: typing.Optional[str] = None,
+        include_similar_documents: typing.Optional[bool] = None,
+        similar_documents_number: typing.Optional[int] = None,
+        similar_documents_fields: typing.Optional[str] = None,
         predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        published_date_precision: typing.Optional[str] = None,
         by_parse_date: typing.Optional[bool] = None,
+        published_date_precision: typing.Optional[str] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -144,40 +156,46 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
-        if author_name is not None:
-            _body["author_name"] = author_name
-        if not_author_name is not None:
-            _body["not_author_name"] = not_author_name
-        if sources is not None:
-            _body["sources"] = sources
+        if q is not None:
+            _body["q"] = q
+        if search_in is not None:
+            _body["search_in"] = search_in
+        if include_similar_documents is not None:
+            _body["include_similar_documents"] = include_similar_documents
+        if similar_documents_number is not None:
+            _body["similar_documents_number"] = similar_documents_number
+        if similar_documents_fields is not None:
+            _body["similar_documents_fields"] = similar_documents_fields
         if predefined_sources is not None:
             _body["predefined_sources"] = predefined_sources
+        if sources is not None:
+            _body["sources"] = sources
         if not_sources is not None:
             _body["not_sources"] = not_sources
         if lang is not None:
             _body["lang"] = lang
         if not_lang is not None:
             _body["not_lang"] = not_lang
         if countries is not None:
             _body["countries"] = countries
         if not_countries is not None:
             _body["not_countries"] = not_countries
         if from_ is not None:
             _body["from_"] = from_
         if to_ is not None:
             _body["to_"] = to_
-        if published_date_precision is not None:
-            _body["published_date_precision"] = published_date_precision
         if by_parse_date is not None:
             _body["by_parse_date"] = by_parse_date
+        if published_date_precision is not None:
+            _body["published_date_precision"] = published_date_precision
         if sort_by is not None:
             _body["sort_by"] = sort_by
         if ranked_only is not None:
             _body["ranked_only"] = ranked_only
         if from_rank is not None:
             _body["from_rank"] = from_rank
         if to_rank is not None:
@@ -236,15 +254,15 @@
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        [Post] Search By Author Request
+        [Post] Search For Similar Articles Request
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -260,20 +278,20 @@
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/authors',
+            path_template='/api/search_similar',
             body=body,
             auth_settings=_auth,
             headers=_headers,
         )
-        serialized_data = request_body_author_search_request.serialize(body, content_type)
+        serialized_data = request_body_more_like_this_request.serialize(body, content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
@@ -350,15 +368,15 @@
         content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        [Post] Search By Author Request
+        [Post] Search For Similar Articles Request
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -374,20 +392,20 @@
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/authors',
+            path_template='/api/search_similar',
             body=body,
             auth_settings=_auth,
             headers=_headers,
         )
-        serialized_data = request_body_author_search_request.serialize(body, content_type)
+        serialized_data = request_body_more_like_this_request.serialize(body, content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']
     
         response = self.api_client.call_api(
             resource_path=used_path,
@@ -425,27 +443,30 @@
 
 
 class PostRaw(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def apost(
         self,
-        author_name: str,
-        not_author_name: typing.Optional[str] = None,
-        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        q: str,
+        search_in: typing.Optional[str] = None,
+        include_similar_documents: typing.Optional[bool] = None,
+        similar_documents_number: typing.Optional[int] = None,
+        similar_documents_fields: typing.Optional[str] = None,
         predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        published_date_precision: typing.Optional[str] = None,
         by_parse_date: typing.Optional[bool] = None,
+        published_date_precision: typing.Optional[str] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -469,27 +490,30 @@
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
-            author_name=author_name,
-            not_author_name=not_author_name,
-            sources=sources,
+            q=q,
+            search_in=search_in,
+            include_similar_documents=include_similar_documents,
+            similar_documents_number=similar_documents_number,
+            similar_documents_fields=similar_documents_fields,
             predefined_sources=predefined_sources,
+            sources=sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            published_date_precision=published_date_precision,
             by_parse_date=by_parse_date,
+            published_date_precision=published_date_precision,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -514,27 +538,30 @@
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
         self,
-        author_name: str,
-        not_author_name: typing.Optional[str] = None,
-        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        q: str,
+        search_in: typing.Optional[str] = None,
+        include_similar_documents: typing.Optional[bool] = None,
+        similar_documents_number: typing.Optional[int] = None,
+        similar_documents_fields: typing.Optional[str] = None,
         predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        published_date_precision: typing.Optional[str] = None,
         by_parse_date: typing.Optional[bool] = None,
+        published_date_precision: typing.Optional[str] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -556,27 +583,30 @@
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
-            author_name=author_name,
-            not_author_name=not_author_name,
-            sources=sources,
+            q=q,
+            search_in=search_in,
+            include_similar_documents=include_similar_documents,
+            similar_documents_number=similar_documents_number,
+            similar_documents_fields=similar_documents_fields,
             predefined_sources=predefined_sources,
+            sources=sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            published_date_precision=published_date_precision,
             by_parse_date=by_parse_date,
+            published_date_precision=published_date_precision,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -602,27 +632,30 @@
             body=args.body,
         )
 
 class Post(BaseApi):
 
     async def apost(
         self,
-        author_name: str,
-        not_author_name: typing.Optional[str] = None,
-        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        q: str,
+        search_in: typing.Optional[str] = None,
+        include_similar_documents: typing.Optional[bool] = None,
+        similar_documents_number: typing.Optional[int] = None,
+        similar_documents_fields: typing.Optional[str] = None,
         predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        published_date_precision: typing.Optional[str] = None,
         by_parse_date: typing.Optional[bool] = None,
+        published_date_precision: typing.Optional[str] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -641,29 +674,32 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
-    ) -> AuthorsPostResponsePydantic:
+    ) -> SearchSimilarPostResponsePydantic:
         raw_response = await self.raw.apost(
-            author_name=author_name,
-            not_author_name=not_author_name,
-            sources=sources,
+            q=q,
+            search_in=search_in,
+            include_similar_documents=include_similar_documents,
+            similar_documents_number=similar_documents_number,
+            similar_documents_fields=similar_documents_fields,
             predefined_sources=predefined_sources,
+            sources=sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            published_date_precision=published_date_precision,
             by_parse_date=by_parse_date,
+            published_date_precision=published_date_precision,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -683,33 +719,36 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             **kwargs,
         )
         if validate:
-            return RootModel[AuthorsPostResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(AuthorsPostResponsePydantic, raw_response.body)
+            return RootModel[SearchSimilarPostResponsePydantic](raw_response.body).root
+        return api_client.construct_model_instance(SearchSimilarPostResponsePydantic, raw_response.body)
     
     
     def post(
         self,
-        author_name: str,
-        not_author_name: typing.Optional[str] = None,
-        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        q: str,
+        search_in: typing.Optional[str] = None,
+        include_similar_documents: typing.Optional[bool] = None,
+        similar_documents_number: typing.Optional[int] = None,
+        similar_documents_fields: typing.Optional[str] = None,
         predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        published_date_precision: typing.Optional[str] = None,
         by_parse_date: typing.Optional[bool] = None,
+        published_date_precision: typing.Optional[str] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -727,29 +766,32 @@
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
-    ) -> AuthorsPostResponsePydantic:
+    ) -> SearchSimilarPostResponsePydantic:
         raw_response = self.raw.post(
-            author_name=author_name,
-            not_author_name=not_author_name,
-            sources=sources,
+            q=q,
+            search_in=search_in,
+            include_similar_documents=include_similar_documents,
+            similar_documents_number=similar_documents_number,
+            similar_documents_fields=similar_documents_fields,
             predefined_sources=predefined_sources,
+            sources=sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            published_date_precision=published_date_precision,
             by_parse_date=by_parse_date,
+            published_date_precision=published_date_precision,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -768,36 +810,39 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
         )
         if validate:
-            return RootModel[AuthorsPostResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(AuthorsPostResponsePydantic, raw_response.body)
+            return RootModel[SearchSimilarPostResponsePydantic](raw_response.body).root
+        return api_client.construct_model_instance(SearchSimilarPostResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
-        author_name: str,
-        not_author_name: typing.Optional[str] = None,
-        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        q: str,
+        search_in: typing.Optional[str] = None,
+        include_similar_documents: typing.Optional[bool] = None,
+        similar_documents_number: typing.Optional[int] = None,
+        similar_documents_fields: typing.Optional[str] = None,
         predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        published_date_precision: typing.Optional[str] = None,
         by_parse_date: typing.Optional[bool] = None,
+        published_date_precision: typing.Optional[str] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -821,27 +866,30 @@
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
-            author_name=author_name,
-            not_author_name=not_author_name,
-            sources=sources,
+            q=q,
+            search_in=search_in,
+            include_similar_documents=include_similar_documents,
+            similar_documents_number=similar_documents_number,
+            similar_documents_fields=similar_documents_fields,
             predefined_sources=predefined_sources,
+            sources=sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            published_date_precision=published_date_precision,
             by_parse_date=by_parse_date,
+            published_date_precision=published_date_precision,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -866,27 +914,30 @@
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
         self,
-        author_name: str,
-        not_author_name: typing.Optional[str] = None,
-        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        q: str,
+        search_in: typing.Optional[str] = None,
+        include_similar_documents: typing.Optional[bool] = None,
+        similar_documents_number: typing.Optional[int] = None,
+        similar_documents_fields: typing.Optional[str] = None,
         predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        published_date_precision: typing.Optional[str] = None,
         by_parse_date: typing.Optional[bool] = None,
+        published_date_precision: typing.Optional[str] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -908,27 +959,30 @@
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
-            author_name=author_name,
-            not_author_name=not_author_name,
-            sources=sources,
+            q=q,
+            search_in=search_in,
+            include_similar_documents=include_similar_documents,
+            similar_documents_number=similar_documents_number,
+            similar_documents_fields=similar_documents_fields,
             predefined_sources=predefined_sources,
+            sources=sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            published_date_precision=published_date_precision,
             by_parse_date=by_parse_date,
+            published_date_precision=published_date_precision,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_latest_headlines/get.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,16 @@
 MISCEntityNameSchema = schemas.StrSchema
 TitleSentimentMinSchema = schemas.NumberSchema
 TitleSentimentMaxSchema = schemas.NumberSchema
 ContentSentimentMinSchema = schemas.NumberSchema
 ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema
 NotIptcTagsSchema = schemas.AnyTypeSchema
+IabTagsSchema = schemas.AnyTypeSchema
+NotIabTagsSchema = schemas.AnyTypeSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
@@ -156,14 +158,16 @@
         'MISC_entity_name': typing.Union[MISCEntityNameSchema, str, ],
         'title_sentiment_min': typing.Union[TitleSentimentMinSchema, decimal.Decimal, int, float, ],
         'title_sentiment_max': typing.Union[TitleSentimentMaxSchema, decimal.Decimal, int, float, ],
         'content_sentiment_min': typing.Union[ContentSentimentMinSchema, decimal.Decimal, int, float, ],
         'content_sentiment_max': typing.Union[ContentSentimentMaxSchema, decimal.Decimal, int, float, ],
         'iptc_tags': typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iptc_tags': typing.Union[NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'iab_tags': typing.Union[IabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -387,14 +391,26 @@
 )
 request_query_not_iptc_tags = api_client.QueryParameter(
     name="not_iptc_tags",
     style=api_client.ParameterStyle.FORM,
     schema=NotIptcTagsSchema,
     explode=True,
 )
+request_query_iab_tags = api_client.QueryParameter(
+    name="iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=IabTagsSchema,
+    explode=True,
+)
+request_query_not_iab_tags = api_client.QueryParameter(
+    name="not_iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=NotIabTagsSchema,
+    explode=True,
+)
 _auth = [
     'apiKey',
 ]
 SchemaFor200ResponseBodyApplicationJson = LatestHeadlinesGetResponseSchema
 
 
 @dataclass
@@ -482,14 +498,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
         if when is not None:
             _query_params["when"] = when
         if by_parse_date is not None:
             _query_params["by_parse_date"] = by_parse_date
@@ -559,14 +577,18 @@
             _query_params["content_sentiment_min"] = content_sentiment_min
         if content_sentiment_max is not None:
             _query_params["content_sentiment_max"] = content_sentiment_max
         if iptc_tags is not None:
             _query_params["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _query_params["not_iptc_tags"] = not_iptc_tags
+        if iab_tags is not None:
+            _query_params["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _query_params["not_iab_tags"] = not_iab_tags
         args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -623,14 +645,16 @@
             request_query_misc_entity_name,
             request_query_title_sentiment_min,
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
+            request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -771,14 +795,16 @@
             request_query_misc_entity_name,
             request_query_title_sentiment_min,
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
+            request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -871,14 +897,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -915,14 +943,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -960,14 +990,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             when=when,
             by_parse_date=by_parse_date,
@@ -1002,14 +1034,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
 
 class Get(BaseApi):
 
@@ -1048,14 +1082,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> LatestHeadlinesGetResponsePydantic:
         raw_response = await self.raw.aget(
             when=when,
             by_parse_date=by_parse_date,
             lang=lang,
@@ -1089,14 +1125,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[LatestHeadlinesGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(LatestHeadlinesGetResponsePydantic, raw_response.body)
     
     
@@ -1135,14 +1173,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> LatestHeadlinesGetResponsePydantic:
         raw_response = self.raw.get(
             when=when,
             by_parse_date=by_parse_date,
             lang=lang,
             not_lang=not_lang,
@@ -1175,14 +1215,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[LatestHeadlinesGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(LatestHeadlinesGetResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
@@ -1223,14 +1265,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1267,14 +1311,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1312,14 +1358,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             when=when,
             by_parse_date=by_parse_date,
@@ -1354,12 +1402,14 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
```

#### html2text {}

```diff
@@ -45,14 +45,15 @@
 ThemeSchema = schemas.StrSchema NotThemeSchema = schemas.StrSchema
 ORGEntityNameSchema = schemas.StrSchema PEREntityNameSchema = schemas.StrSchema
 LOCEntityNameSchema = schemas.StrSchema MISCEntityNameSchema =
 schemas.StrSchema TitleSentimentMinSchema = schemas.NumberSchema
 TitleSentimentMaxSchema = schemas.NumberSchema ContentSentimentMinSchema =
 schemas.NumberSchema ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema NotIptcTagsSchema =
+schemas.AnyTypeSchema IabTagsSchema = schemas.AnyTypeSchema NotIabTagsSchema =
 schemas.AnyTypeSchema RequestRequiredQueryParams = typing_extensions.TypedDict
 ( 'RequestRequiredQueryParams', { } ) RequestOptionalQueryParams =
 typing_extensions.TypedDict( 'RequestOptionalQueryParams', { 'when':
 typing.Union[WhenSchema, str, ], 'by_parse_date': typing.Union
 [ByParseDateSchema, bool, ], 'lang': typing.Union[LangSchema, dict,
 frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
@@ -106,17 +107,22 @@
 decimal.Decimal, int, float, ], 'content_sentiment_max': typing.Union
 [ContentSentimentMaxSchema, decimal.Decimal, int, float, ], 'iptc_tags':
 typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime,
 uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes,
 io.FileIO, io.BufferedReader, ], 'not_iptc_tags': typing.Union
 [NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime,
 uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes,
-io.FileIO, io.BufferedReader, ], }, total=False ) class RequestQueryParams
-(RequestRequiredQueryParams, RequestOptionalQueryParams): pass
-request_query_when = api_client.QueryParameter( name="when",
+io.FileIO, io.BufferedReader, ], 'iab_tags': typing.Union[IabTagsSchema, dict,
+frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+], 'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict,
+str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list,
+tuple, bytes, io.FileIO, io.BufferedReader, ], }, total=False ) class
+RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
+pass request_query_when = api_client.QueryParameter( name="when",
 style=api_client.ParameterStyle.FORM, schema=WhenSchema, explode=True, )
 request_query_by_parse_date = api_client.QueryParameter( name="by_parse_date",
 style=api_client.ParameterStyle.FORM, schema=ByParseDateSchema, explode=True, )
 request_query_lang = api_client.QueryParameter( name="lang",
 style=api_client.ParameterStyle.FORM, schema=LangSchema, explode=True, )
 request_query_not_lang = api_client.QueryParameter( name="not_lang",
 style=api_client.ParameterStyle.FORM, schema=NotLangSchema, explode=True, )
@@ -197,14 +203,18 @@
 request_query_content_sentiment_max = api_client.QueryParameter
 ( name="content_sentiment_max", style=api_client.ParameterStyle.FORM,
 schema=ContentSentimentMaxSchema, explode=True, ) request_query_iptc_tags =
 api_client.QueryParameter( name="iptc_tags",
 style=api_client.ParameterStyle.FORM, schema=IptcTagsSchema, explode=True, )
 request_query_not_iptc_tags = api_client.QueryParameter( name="not_iptc_tags",
 style=api_client.ParameterStyle.FORM, schema=NotIptcTagsSchema, explode=True, )
+request_query_iab_tags = api_client.QueryParameter( name="iab_tags",
+style=api_client.ParameterStyle.FORM, schema=IabTagsSchema, explode=True, )
+request_query_not_iab_tags = api_client.QueryParameter( name="not_iab_tags",
+style=api_client.ParameterStyle.FORM, schema=NotIabTagsSchema, explode=True, )
 _auth = [ 'apiKey', ] SchemaFor200ResponseBodyApplicationJson =
 LatestHeadlinesGetResponseSchema @dataclass class ApiResponseFor200
 (api_client.ApiResponse): body: LatestHeadlinesGetResponse @dataclass class
 ApiResponseFor200Async(api_client.AsyncApiResponse): body:
 LatestHeadlinesGetResponse _response_for_200 = api_client.OpenApiResponse
 ( response_cls=ApiResponseFor200, response_cls_async=ApiResponseFor200Async,
 content={ 'application/json': api_client.MediaType
@@ -248,58 +258,62 @@
 typing.Optional[str] = None, misc_entity_name: typing.Optional[str] = None,
 title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
 list, str, None]] = None, not_iptc_tags: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, ) -
-> api_client.MappedArgs: args: api_client.MappedArgs = api_client.MappedArgs()
-_query_params = {} if when is not None: _query_params["when"] = when if
-by_parse_date is not None: _query_params["by_parse_date"] = by_parse_date if
-lang is not None: _query_params["lang"] = lang if not_lang is not None:
-_query_params["not_lang"] = not_lang if countries is not None: _query_params
-["countries"] = countries if not_countries is not None: _query_params
-["not_countries"] = not_countries if sources is not None: _query_params
-["sources"] = sources if predefined_sources is not None: _query_params
-["predefined_sources"] = predefined_sources if not_sources is not None:
-_query_params["not_sources"] = not_sources if not_author_name is not None:
-_query_params["not_author_name"] = not_author_name if ranked_only is not None:
-_query_params["ranked_only"] = ranked_only if is_headline is not None:
-_query_params["is_headline"] = is_headline if is_paid_content is not None:
-_query_params["is_paid_content"] = is_paid_content if parent_url is not None:
-_query_params["parent_url"] = parent_url if all_links is not None:
-_query_params["all_links"] = all_links if all_domain_links is not None:
-_query_params["all_domain_links"] = all_domain_links if word_count_min is not
-None: _query_params["word_count_min"] = word_count_min if word_count_max is not
-None: _query_params["word_count_max"] = word_count_max if page is not None:
-_query_params["page"] = page if page_size is not None: _query_params
-["page_size"] = page_size if clustering_variable is not None: _query_params
-["clustering_variable"] = clustering_variable if clustering_enabled is not
-None: _query_params["clustering_enabled"] = clustering_enabled if
-clustering_threshold is not None: _query_params["clustering_threshold"] =
-clustering_threshold if include_nlp_data is not None: _query_params
-["include_nlp_data"] = include_nlp_data if has_nlp is not None: _query_params
-["has_nlp"] = has_nlp if theme is not None: _query_params["theme"] = theme if
-not_theme is not None: _query_params["not_theme"] = not_theme if
-org_entity_name is not None: _query_params["ORG_entity_name"] = org_entity_name
-if per_entity_name is not None: _query_params["PER_entity_name"] =
-per_entity_name if loc_entity_name is not None: _query_params
-["LOC_entity_name"] = loc_entity_name if misc_entity_name is not None:
-_query_params["MISC_entity_name"] = misc_entity_name if title_sentiment_min is
-not None: _query_params["title_sentiment_min"] = title_sentiment_min if
-title_sentiment_max is not None: _query_params["title_sentiment_max"] =
-title_sentiment_max if content_sentiment_min is not None: _query_params
-["content_sentiment_min"] = content_sentiment_min if content_sentiment_max is
-not None: _query_params["content_sentiment_max"] = content_sentiment_max if
-iptc_tags is not None: _query_params["iptc_tags"] = iptc_tags if not_iptc_tags
-is not None: _query_params["not_iptc_tags"] = not_iptc_tags args.query =
-_query_params return args async def _aget_oapg( self, query_params:
-typing.Optional[dict] = {}, skip_deserialization: bool = True, timeout:
-typing.Optional[typing.Union[float, typing.Tuple]] = None,
+date, datetime, dict, float, int, list, str, None]] = None, iab_tags:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, not_iab_tags: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, ) -> api_client.MappedArgs: args:
+api_client.MappedArgs = api_client.MappedArgs() _query_params = {} if when is
+not None: _query_params["when"] = when if by_parse_date is not None:
+_query_params["by_parse_date"] = by_parse_date if lang is not None:
+_query_params["lang"] = lang if not_lang is not None: _query_params["not_lang"]
+= not_lang if countries is not None: _query_params["countries"] = countries if
+not_countries is not None: _query_params["not_countries"] = not_countries if
+sources is not None: _query_params["sources"] = sources if predefined_sources
+is not None: _query_params["predefined_sources"] = predefined_sources if
+not_sources is not None: _query_params["not_sources"] = not_sources if
+not_author_name is not None: _query_params["not_author_name"] = not_author_name
+if ranked_only is not None: _query_params["ranked_only"] = ranked_only if
+is_headline is not None: _query_params["is_headline"] = is_headline if
+is_paid_content is not None: _query_params["is_paid_content"] = is_paid_content
+if parent_url is not None: _query_params["parent_url"] = parent_url if
+all_links is not None: _query_params["all_links"] = all_links if
+all_domain_links is not None: _query_params["all_domain_links"] =
+all_domain_links if word_count_min is not None: _query_params["word_count_min"]
+= word_count_min if word_count_max is not None: _query_params["word_count_max"]
+= word_count_max if page is not None: _query_params["page"] = page if page_size
+is not None: _query_params["page_size"] = page_size if clustering_variable is
+not None: _query_params["clustering_variable"] = clustering_variable if
+clustering_enabled is not None: _query_params["clustering_enabled"] =
+clustering_enabled if clustering_threshold is not None: _query_params
+["clustering_threshold"] = clustering_threshold if include_nlp_data is not
+None: _query_params["include_nlp_data"] = include_nlp_data if has_nlp is not
+None: _query_params["has_nlp"] = has_nlp if theme is not None: _query_params
+["theme"] = theme if not_theme is not None: _query_params["not_theme"] =
+not_theme if org_entity_name is not None: _query_params["ORG_entity_name"] =
+org_entity_name if per_entity_name is not None: _query_params
+["PER_entity_name"] = per_entity_name if loc_entity_name is not None:
+_query_params["LOC_entity_name"] = loc_entity_name if misc_entity_name is not
+None: _query_params["MISC_entity_name"] = misc_entity_name if
+title_sentiment_min is not None: _query_params["title_sentiment_min"] =
+title_sentiment_min if title_sentiment_max is not None: _query_params
+["title_sentiment_max"] = title_sentiment_max if content_sentiment_min is not
+None: _query_params["content_sentiment_min"] = content_sentiment_min if
+content_sentiment_max is not None: _query_params["content_sentiment_max"] =
+content_sentiment_max if iptc_tags is not None: _query_params["iptc_tags"] =
+iptc_tags if not_iptc_tags is not None: _query_params["not_iptc_tags"] =
+not_iptc_tags if iab_tags is not None: _query_params["iab_tags"] = iab_tags if
+not_iab_tags is not None: _query_params["not_iab_tags"] = not_iab_tags
+args.query = _query_params return args async def _aget_oapg( self,
+query_params: typing.Optional[dict] = {}, skip_deserialization: bool = True,
+timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
 accept_content_types: typing.Tuple[str] = _all_accept_content_types, stream:
 bool = False, **kwargs, ) -> typing.Union[ ApiResponseFor200Async,
 api_client.ApiResponseWithoutDeserializationAsync, AsyncGeneratorResponse, ]:
 """ [Get] Search For Latest Headlines Request :param skip_deserialization: If
 true then api_response.response will be set but api_response.body and
 api_response.headers will not be deserialized into schema class instances """
 self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params) used_path
@@ -316,15 +330,16 @@
 request_query_clustering_enabled, request_query_clustering_threshold,
 request_query_include_nlp_data, request_query_has_nlp, request_query_theme,
 request_query_not_theme, request_query_org_entity_name,
 request_query_per_entity_name, request_query_loc_entity_name,
 request_query_misc_entity_name, request_query_title_sentiment_min,
 request_query_title_sentiment_max, request_query_content_sentiment_min,
 request_query_content_sentiment_max, request_query_iptc_tags,
-request_query_not_iptc_tags, ): parameter_data = query_params.get
+request_query_not_iptc_tags, request_query_iab_tags,
+request_query_not_iab_tags, ): parameter_data = query_params.get
 (parameter.name, schemas.unset) if parameter_data is schemas.unset: continue if
 prefix_separator_iterator is None: prefix_separator_iterator =
 parameter.get_prefix_separator_iterator() serialized_data = parameter.serialize
 (parameter_data, prefix_separator_iterator) for serialized_value in
 serialized_data.values(): used_path += serialized_value _headers =
 HTTPHeaderDict() # TODO add cookie handling if accept_content_types: for
 accept_content_type in accept_content_types: _headers.add('Accept',
@@ -381,15 +396,16 @@
 request_query_clustering_enabled, request_query_clustering_threshold,
 request_query_include_nlp_data, request_query_has_nlp, request_query_theme,
 request_query_not_theme, request_query_org_entity_name,
 request_query_per_entity_name, request_query_loc_entity_name,
 request_query_misc_entity_name, request_query_title_sentiment_min,
 request_query_title_sentiment_max, request_query_content_sentiment_min,
 request_query_content_sentiment_max, request_query_iptc_tags,
-request_query_not_iptc_tags, ): parameter_data = query_params.get
+request_query_not_iptc_tags, request_query_iab_tags,
+request_query_not_iab_tags, ): parameter_data = query_params.get
 (parameter.name, schemas.unset) if parameter_data is schemas.unset: continue if
 prefix_separator_iterator is None: prefix_separator_iterator =
 parameter.get_prefix_separator_iterator() serialized_data = parameter.serialize
 (parameter_data, prefix_separator_iterator) for serialized_value in
 serialized_data.values(): used_path += serialized_value _headers =
 HTTPHeaderDict() # TODO add cookie handling if accept_content_types: for
 accept_content_type in accept_content_types: _headers.add('Accept',
@@ -444,37 +460,158 @@
 typing.Optional[str] = None, misc_entity_name: typing.Optional[str] = None,
 title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
 list, str, None]] = None, not_iptc_tags: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, **kwargs, ) -
-> typing.Union[ ApiResponseFor200Async,
-api_client.ApiResponseWithoutDeserializationAsync, AsyncGeneratorResponse, ]:
-args = self._get_mapped_args( when=when, by_parse_date=by_parse_date,
-lang=lang, not_lang=not_lang, countries=countries, not_countries=not_countries,
-sources=sources, predefined_sources=predefined_sources,
-not_sources=not_sources, not_author_name=not_author_name,
-ranked_only=ranked_only, is_headline=is_headline,
-is_paid_content=is_paid_content, parent_url=parent_url, all_links=all_links,
-all_domain_links=all_domain_links, word_count_min=word_count_min,
-word_count_max=word_count_max, page=page, page_size=page_size,
-clustering_variable=clustering_variable, clustering_enabled=clustering_enabled,
+date, datetime, dict, float, int, list, str, None]] = None, iab_tags:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, not_iab_tags: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, **kwargs, ) -> typing.Union
+[ ApiResponseFor200Async, api_client.ApiResponseWithoutDeserializationAsync,
+AsyncGeneratorResponse, ]: args = self._get_mapped_args( when=when,
+by_parse_date=by_parse_date, lang=lang, not_lang=not_lang, countries=countries,
+not_countries=not_countries, sources=sources,
+predefined_sources=predefined_sources, not_sources=not_sources,
+not_author_name=not_author_name, ranked_only=ranked_only,
+is_headline=is_headline, is_paid_content=is_paid_content,
+parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
+word_count_min=word_count_min, word_count_max=word_count_max, page=page,
+page_size=page_size, clustering_variable=clustering_variable,
+clustering_enabled=clustering_enabled,
+clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
+has_nlp=has_nlp, theme=theme, not_theme=not_theme,
+org_entity_name=org_entity_name, per_entity_name=per_entity_name,
+loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
+title_sentiment_min=title_sentiment_min,
+title_sentiment_max=title_sentiment_max,
+content_sentiment_min=content_sentiment_min,
+content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, )
+return await self._aget_oapg( query_params=args.query, **kwargs, ) def get
+( self, when: typing.Optional[str] = None, by_parse_date: typing.Optional[bool]
+= None, lang: typing.Optional[typing.Union[bool, date, datetime, dict, float,
+int, list, str, None]] = None, not_lang: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, countries:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, not_countries: typing.Optional[typing.Union[bool, date,
+datetime, dict, float, int, list, str, None]] = None, sources: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, not_sources: typing.Optional[typing.Union
+[bool, date, datetime, dict, float, int, list, str, None]] = None,
+not_author_name: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, ranked_only: typing.Optional[str] = None,
+is_headline: typing.Optional[bool] = None, is_paid_content: typing.Optional
+[bool] = None, parent_url: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, all_links: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+all_domain_links: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, word_count_min: typing.Optional[int] =
+None, word_count_max: typing.Optional[int] = None, page: typing.Optional[int] =
+None, page_size: typing.Optional[int] = None, clustering_variable:
+typing.Optional[str] = None, clustering_enabled: typing.Optional[bool] = None,
+clustering_threshold: typing.Optional[typing.Union[int, float]] = None,
+include_nlp_data: typing.Optional[bool] = None, has_nlp: typing.Optional[bool]
+= None, theme: typing.Optional[str] = None, not_theme: typing.Optional[str] =
+None, org_entity_name: typing.Optional[str] = None, per_entity_name:
+typing.Optional[str] = None, loc_entity_name: typing.Optional[str] = None,
+misc_entity_name: typing.Optional[str] = None, title_sentiment_min:
+typing.Optional[typing.Union[int, float]] = None, title_sentiment_max:
+typing.Optional[typing.Union[int, float]] = None, content_sentiment_min:
+typing.Optional[typing.Union[int, float]] = None, content_sentiment_max:
+typing.Optional[typing.Union[int, float]] = None, iptc_tags: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float,
+int, list, str, None]] = None, iab_tags: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, not_iab_tags:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, ) -> typing.Union[ ApiResponseFor200,
+api_client.ApiResponseWithoutDeserialization, ]: args = self._get_mapped_args
+( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
+countries=countries, not_countries=not_countries, sources=sources,
+predefined_sources=predefined_sources, not_sources=not_sources,
+not_author_name=not_author_name, ranked_only=ranked_only,
+is_headline=is_headline, is_paid_content=is_paid_content,
+parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
+word_count_min=word_count_min, word_count_max=word_count_max, page=page,
+page_size=page_size, clustering_variable=clustering_variable,
+clustering_enabled=clustering_enabled,
+clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
+has_nlp=has_nlp, theme=theme, not_theme=not_theme,
+org_entity_name=org_entity_name, per_entity_name=per_entity_name,
+loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
+title_sentiment_min=title_sentiment_min,
+title_sentiment_max=title_sentiment_max,
+content_sentiment_min=content_sentiment_min,
+content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, )
+return self._get_oapg( query_params=args.query, ) class Get(BaseApi): async def
+aget( self, when: typing.Optional[str] = None, by_parse_date: typing.Optional
+[bool] = None, lang: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, not_lang: typing.Optional[typing.Union
+[bool, date, datetime, dict, float, int, list, str, None]] = None, countries:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, not_countries: typing.Optional[typing.Union[bool, date,
+datetime, dict, float, int, list, str, None]] = None, sources: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, not_sources: typing.Optional[typing.Union
+[bool, date, datetime, dict, float, int, list, str, None]] = None,
+not_author_name: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, ranked_only: typing.Optional[str] = None,
+is_headline: typing.Optional[bool] = None, is_paid_content: typing.Optional
+[bool] = None, parent_url: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, all_links: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+all_domain_links: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, word_count_min: typing.Optional[int] =
+None, word_count_max: typing.Optional[int] = None, page: typing.Optional[int] =
+None, page_size: typing.Optional[int] = None, clustering_variable:
+typing.Optional[str] = None, clustering_enabled: typing.Optional[bool] = None,
+clustering_threshold: typing.Optional[typing.Union[int, float]] = None,
+include_nlp_data: typing.Optional[bool] = None, has_nlp: typing.Optional[bool]
+= None, theme: typing.Optional[str] = None, not_theme: typing.Optional[str] =
+None, org_entity_name: typing.Optional[str] = None, per_entity_name:
+typing.Optional[str] = None, loc_entity_name: typing.Optional[str] = None,
+misc_entity_name: typing.Optional[str] = None, title_sentiment_min:
+typing.Optional[typing.Union[int, float]] = None, title_sentiment_max:
+typing.Optional[typing.Union[int, float]] = None, content_sentiment_min:
+typing.Optional[typing.Union[int, float]] = None, content_sentiment_max:
+typing.Optional[typing.Union[int, float]] = None, iptc_tags: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float,
+int, list, str, None]] = None, iab_tags: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, not_iab_tags:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, validate: bool = False, **kwargs, ) -
+> LatestHeadlinesGetResponsePydantic: raw_response = await self.raw.aget
+( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
+countries=countries, not_countries=not_countries, sources=sources,
+predefined_sources=predefined_sources, not_sources=not_sources,
+not_author_name=not_author_name, ranked_only=ranked_only,
+is_headline=is_headline, is_paid_content=is_paid_content,
+parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
+word_count_min=word_count_min, word_count_max=word_count_max, page=page,
+page_size=page_size, clustering_variable=clustering_variable,
+clustering_enabled=clustering_enabled,
 clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 org_entity_name=org_entity_name, per_entity_name=per_entity_name,
 loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) return await self._aget_oapg
-( query_params=args.query, **kwargs, ) def get( self, when: typing.Optional
-[str] = None, by_parse_date: typing.Optional[bool] = None, lang:
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags,
+**kwargs, ) if validate: return RootModel[LatestHeadlinesGetResponsePydantic]
+(raw_response.body).root return api_client.construct_model_instance
+(LatestHeadlinesGetResponsePydantic, raw_response.body) def get( self, when:
+typing.Optional[str] = None, by_parse_date: typing.Optional[bool] = None, lang:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
 None]] = None, not_lang: typing.Optional[typing.Union[bool, date, datetime,
 dict, float, int, list, str, None]] = None, countries: typing.Optional
 [typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
 not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float,
 int, list, str, None]] = None, sources: typing.Optional[typing.Union[bool,
 date, datetime, dict, float, int, list, str, None]] = None, predefined_sources:
@@ -500,16 +637,18 @@
 typing.Optional[str] = None, title_sentiment_min: typing.Optional[typing.Union
 [int, float]] = None, title_sentiment_max: typing.Optional[typing.Union[int,
 float]] = None, content_sentiment_min: typing.Optional[typing.Union[int,
 float]] = None, content_sentiment_max: typing.Optional[typing.Union[int,
 float]] = None, iptc_tags: typing.Optional[typing.Union[bool, date, datetime,
 dict, float, int, list, str, None]] = None, not_iptc_tags: typing.Optional
 [typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-) -> typing.Union[ ApiResponseFor200,
-api_client.ApiResponseWithoutDeserialization, ]: args = self._get_mapped_args
+iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
+list, str, None]] = None, not_iab_tags: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, validate: bool =
+False, ) -> LatestHeadlinesGetResponsePydantic: raw_response = self.raw.get
 ( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
 countries=countries, not_countries=not_countries, sources=sources,
 predefined_sources=predefined_sources, not_sources=not_sources,
 not_author_name=not_author_name, ranked_only=ranked_only,
 is_headline=is_headline, is_paid_content=is_paid_content,
 parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
 word_count_min=word_count_min, word_count_max=word_count_max, page=page,
@@ -519,16 +658,20 @@
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 org_entity_name=org_entity_name, per_entity_name=per_entity_name,
 loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) return self._get_oapg( query_params=args.query,
-) class Get(BaseApi): async def aget( self, when: typing.Optional[str] = None,
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, ) if
+validate: return RootModel[LatestHeadlinesGetResponsePydantic]
+(raw_response.body).root return api_client.construct_model_instance
+(LatestHeadlinesGetResponsePydantic, raw_response.body) class ApiForget
+(BaseApi): # this class is used by api classes that refer to endpoints by path
+and http method names async def aget( self, when: typing.Optional[str] = None,
 by_parse_date: typing.Optional[bool] = None, lang: typing.Optional[typing.Union
 [bool, date, datetime, dict, float, int, list, str, None]] = None, not_lang:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
 None]] = None, countries: typing.Optional[typing.Union[bool, date, datetime,
 dict, float, int, list, str, None]] = None, not_countries: typing.Optional
 [typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
 sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
@@ -554,74 +697,22 @@
 typing.Optional[str] = None, misc_entity_name: typing.Optional[str] = None,
 title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
 list, str, None]] = None, not_iptc_tags: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, validate: bool =
-False, **kwargs, ) -> LatestHeadlinesGetResponsePydantic: raw_response = await
-self.raw.aget( when=when, by_parse_date=by_parse_date, lang=lang,
-not_lang=not_lang, countries=countries, not_countries=not_countries,
-sources=sources, predefined_sources=predefined_sources,
-not_sources=not_sources, not_author_name=not_author_name,
-ranked_only=ranked_only, is_headline=is_headline,
-is_paid_content=is_paid_content, parent_url=parent_url, all_links=all_links,
-all_domain_links=all_domain_links, word_count_min=word_count_min,
-word_count_max=word_count_max, page=page, page_size=page_size,
-clustering_variable=clustering_variable, clustering_enabled=clustering_enabled,
-clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
-has_nlp=has_nlp, theme=theme, not_theme=not_theme,
-org_entity_name=org_entity_name, per_entity_name=per_entity_name,
-loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
-title_sentiment_min=title_sentiment_min,
-title_sentiment_max=title_sentiment_max,
-content_sentiment_min=content_sentiment_min,
-content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, **kwargs, ) if validate: return RootModel
-[LatestHeadlinesGetResponsePydantic](raw_response.body).root return
-api_client.construct_model_instance(LatestHeadlinesGetResponsePydantic,
-raw_response.body) def get( self, when: typing.Optional[str] = None,
-by_parse_date: typing.Optional[bool] = None, lang: typing.Optional[typing.Union
-[bool, date, datetime, dict, float, int, list, str, None]] = None, not_lang:
-typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, countries: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, not_countries: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
-list, str, None]] = None, predefined_sources: typing.Optional[typing.Union
-[bool, date, datetime, dict, float, int, list, str, None]] = None, not_sources:
+date, datetime, dict, float, int, list, str, None]] = None, iab_tags:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, not_author_name: typing.Optional[typing.Union[bool, date,
-datetime, dict, float, int, list, str, None]] = None, ranked_only:
-typing.Optional[str] = None, is_headline: typing.Optional[bool] = None,
-is_paid_content: typing.Optional[bool] = None, parent_url: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-all_links: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
-list, str, None]] = None, all_domain_links: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, word_count_min:
-typing.Optional[int] = None, word_count_max: typing.Optional[int] = None, page:
-typing.Optional[int] = None, page_size: typing.Optional[int] = None,
-clustering_variable: typing.Optional[str] = None, clustering_enabled:
-typing.Optional[bool] = None, clustering_threshold: typing.Optional
-[typing.Union[int, float]] = None, include_nlp_data: typing.Optional[bool] =
-None, has_nlp: typing.Optional[bool] = None, theme: typing.Optional[str] =
-None, not_theme: typing.Optional[str] = None, org_entity_name: typing.Optional
-[str] = None, per_entity_name: typing.Optional[str] = None, loc_entity_name:
-typing.Optional[str] = None, misc_entity_name: typing.Optional[str] = None,
-title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
-title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
-content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
-content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
-iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
-list, str, None]] = None, not_iptc_tags: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, validate: bool =
-False, ) -> LatestHeadlinesGetResponsePydantic: raw_response = self.raw.get
-( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
-countries=countries, not_countries=not_countries, sources=sources,
+None]] = None, not_iab_tags: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, **kwargs, ) -> typing.Union
+[ ApiResponseFor200Async, api_client.ApiResponseWithoutDeserializationAsync,
+AsyncGeneratorResponse, ]: args = self._get_mapped_args( when=when,
+by_parse_date=by_parse_date, lang=lang, not_lang=not_lang, countries=countries,
+not_countries=not_countries, sources=sources,
 predefined_sources=predefined_sources, not_sources=not_sources,
 not_author_name=not_author_name, ranked_only=ranked_only,
 is_headline=is_headline, is_paid_content=is_paid_content,
 parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
 word_count_min=word_count_min, word_count_max=word_count_max, page=page,
 page_size=page_size, clustering_variable=clustering_variable,
 clustering_enabled=clustering_enabled,
@@ -629,19 +720,16 @@
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 org_entity_name=org_entity_name, per_entity_name=per_entity_name,
 loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) if validate: return RootModel
-[LatestHeadlinesGetResponsePydantic](raw_response.body).root return
-api_client.construct_model_instance(LatestHeadlinesGetResponsePydantic,
-raw_response.body) class ApiForget(BaseApi): # this class is used by api
-classes that refer to endpoints by path and http method names async def aget
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, )
+return await self._aget_oapg( query_params=args.query, **kwargs, ) def get
 ( self, when: typing.Optional[str] = None, by_parse_date: typing.Optional[bool]
 = None, lang: typing.Optional[typing.Union[bool, date, datetime, dict, float,
 int, list, str, None]] = None, not_lang: typing.Optional[typing.Union[bool,
 date, datetime, dict, float, int, list, str, None]] = None, countries:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
 None]] = None, not_countries: typing.Optional[typing.Union[bool, date,
 datetime, dict, float, int, list, str, None]] = None, sources: typing.Optional
@@ -668,71 +756,18 @@
 misc_entity_name: typing.Optional[str] = None, title_sentiment_min:
 typing.Optional[typing.Union[int, float]] = None, title_sentiment_max:
 typing.Optional[typing.Union[int, float]] = None, content_sentiment_min:
 typing.Optional[typing.Union[int, float]] = None, content_sentiment_max:
 typing.Optional[typing.Union[int, float]] = None, iptc_tags: typing.Optional
 [typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
 not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float,
-int, list, str, None]] = None, **kwargs, ) -> typing.Union
-[ ApiResponseFor200Async, api_client.ApiResponseWithoutDeserializationAsync,
-AsyncGeneratorResponse, ]: args = self._get_mapped_args( when=when,
-by_parse_date=by_parse_date, lang=lang, not_lang=not_lang, countries=countries,
-not_countries=not_countries, sources=sources,
-predefined_sources=predefined_sources, not_sources=not_sources,
-not_author_name=not_author_name, ranked_only=ranked_only,
-is_headline=is_headline, is_paid_content=is_paid_content,
-parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
-word_count_min=word_count_min, word_count_max=word_count_max, page=page,
-page_size=page_size, clustering_variable=clustering_variable,
-clustering_enabled=clustering_enabled,
-clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
-has_nlp=has_nlp, theme=theme, not_theme=not_theme,
-org_entity_name=org_entity_name, per_entity_name=per_entity_name,
-loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
-title_sentiment_min=title_sentiment_min,
-title_sentiment_max=title_sentiment_max,
-content_sentiment_min=content_sentiment_min,
-content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) return await self._aget_oapg
-( query_params=args.query, **kwargs, ) def get( self, when: typing.Optional
-[str] = None, by_parse_date: typing.Optional[bool] = None, lang:
+int, list, str, None]] = None, iab_tags: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, not_iab_tags:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, not_lang: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, countries: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float,
-int, list, str, None]] = None, sources: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, predefined_sources:
-typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, not_sources: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, not_author_name: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-ranked_only: typing.Optional[str] = None, is_headline: typing.Optional[bool] =
-None, is_paid_content: typing.Optional[bool] = None, parent_url:
-typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, all_links: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, all_domain_links: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-word_count_min: typing.Optional[int] = None, word_count_max: typing.Optional
-[int] = None, page: typing.Optional[int] = None, page_size: typing.Optional
-[int] = None, clustering_variable: typing.Optional[str] = None,
-clustering_enabled: typing.Optional[bool] = None, clustering_threshold:
-typing.Optional[typing.Union[int, float]] = None, include_nlp_data:
-typing.Optional[bool] = None, has_nlp: typing.Optional[bool] = None, theme:
-typing.Optional[str] = None, not_theme: typing.Optional[str] = None,
-org_entity_name: typing.Optional[str] = None, per_entity_name: typing.Optional
-[str] = None, loc_entity_name: typing.Optional[str] = None, misc_entity_name:
-typing.Optional[str] = None, title_sentiment_min: typing.Optional[typing.Union
-[int, float]] = None, title_sentiment_max: typing.Optional[typing.Union[int,
-float]] = None, content_sentiment_min: typing.Optional[typing.Union[int,
-float]] = None, content_sentiment_max: typing.Optional[typing.Union[int,
-float]] = None, iptc_tags: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, not_iptc_tags: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-) -> typing.Union[ ApiResponseFor200,
+None]] = None, ) -> typing.Union[ ApiResponseFor200,
 api_client.ApiResponseWithoutDeserialization, ]: args = self._get_mapped_args
 ( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
 countries=countries, not_countries=not_countries, sources=sources,
 predefined_sources=predefined_sources, not_sources=not_sources,
 not_author_name=not_author_name, ranked_only=ranked_only,
 is_headline=is_headline, is_paid_content=is_paid_content,
 parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
@@ -743,9 +778,9 @@
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 org_entity_name=org_entity_name, per_entity_name=per_entity_name,
 loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) return self._get_oapg( query_params=args.query,
-)
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, )
+return self._get_oapg( query_params=args.query, )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_latest_headlines/get.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/get.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 MISCEntityNameSchema = schemas.StrSchema
 TitleSentimentMinSchema = schemas.NumberSchema
 TitleSentimentMaxSchema = schemas.NumberSchema
 ContentSentimentMinSchema = schemas.NumberSchema
 ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema
 NotIptcTagsSchema = schemas.AnyTypeSchema
+IabTagsSchema = schemas.AnyTypeSchema
+NotIabTagsSchema = schemas.AnyTypeSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
@@ -142,14 +144,16 @@
         'MISC_entity_name': typing.Union[MISCEntityNameSchema, str, ],
         'title_sentiment_min': typing.Union[TitleSentimentMinSchema, decimal.Decimal, int, float, ],
         'title_sentiment_max': typing.Union[TitleSentimentMaxSchema, decimal.Decimal, int, float, ],
         'content_sentiment_min': typing.Union[ContentSentimentMinSchema, decimal.Decimal, int, float, ],
         'content_sentiment_max': typing.Union[ContentSentimentMaxSchema, decimal.Decimal, int, float, ],
         'iptc_tags': typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iptc_tags': typing.Union[NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'iab_tags': typing.Union[IabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -373,14 +377,26 @@
 )
 request_query_not_iptc_tags = api_client.QueryParameter(
     name="not_iptc_tags",
     style=api_client.ParameterStyle.FORM,
     schema=NotIptcTagsSchema,
     explode=True,
 )
+request_query_iab_tags = api_client.QueryParameter(
+    name="iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=IabTagsSchema,
+    explode=True,
+)
+request_query_not_iab_tags = api_client.QueryParameter(
+    name="not_iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=NotIabTagsSchema,
+    explode=True,
+)
 SchemaFor200ResponseBodyApplicationJson = LatestHeadlinesGetResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: LatestHeadlinesGetResponse
 
@@ -461,14 +477,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
         if when is not None:
             _query_params["when"] = when
         if by_parse_date is not None:
             _query_params["by_parse_date"] = by_parse_date
@@ -538,14 +556,18 @@
             _query_params["content_sentiment_min"] = content_sentiment_min
         if content_sentiment_max is not None:
             _query_params["content_sentiment_max"] = content_sentiment_max
         if iptc_tags is not None:
             _query_params["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _query_params["not_iptc_tags"] = not_iptc_tags
+        if iab_tags is not None:
+            _query_params["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _query_params["not_iab_tags"] = not_iab_tags
         args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -602,14 +624,16 @@
             request_query_misc_entity_name,
             request_query_title_sentiment_min,
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
+            request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -750,14 +774,16 @@
             request_query_misc_entity_name,
             request_query_title_sentiment_min,
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
+            request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -850,14 +876,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -894,14 +922,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -939,14 +969,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             when=when,
             by_parse_date=by_parse_date,
@@ -981,14 +1013,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
 
 class Get(BaseApi):
 
@@ -1027,14 +1061,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> LatestHeadlinesGetResponsePydantic:
         raw_response = await self.raw.aget(
             when=when,
             by_parse_date=by_parse_date,
             lang=lang,
@@ -1068,14 +1104,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[LatestHeadlinesGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(LatestHeadlinesGetResponsePydantic, raw_response.body)
     
     
@@ -1114,14 +1152,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> LatestHeadlinesGetResponsePydantic:
         raw_response = self.raw.get(
             when=when,
             by_parse_date=by_parse_date,
             lang=lang,
             not_lang=not_lang,
@@ -1154,14 +1194,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[LatestHeadlinesGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(LatestHeadlinesGetResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
@@ -1202,14 +1244,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1246,14 +1290,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1291,14 +1337,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             when=when,
             by_parse_date=by_parse_date,
@@ -1333,12 +1381,14 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
```

#### html2text {}

```diff
@@ -43,14 +43,15 @@
 schemas.BoolSchema ThemeSchema = schemas.StrSchema NotThemeSchema =
 schemas.StrSchema ORGEntityNameSchema = schemas.StrSchema PEREntityNameSchema =
 schemas.StrSchema LOCEntityNameSchema = schemas.StrSchema MISCEntityNameSchema
 = schemas.StrSchema TitleSentimentMinSchema = schemas.NumberSchema
 TitleSentimentMaxSchema = schemas.NumberSchema ContentSentimentMinSchema =
 schemas.NumberSchema ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema NotIptcTagsSchema =
+schemas.AnyTypeSchema IabTagsSchema = schemas.AnyTypeSchema NotIabTagsSchema =
 schemas.AnyTypeSchema RequestRequiredQueryParams = typing_extensions.TypedDict
 ( 'RequestRequiredQueryParams', { } ) RequestOptionalQueryParams =
 typing_extensions.TypedDict( 'RequestOptionalQueryParams', { 'when':
 typing.Union[WhenSchema, str, ], 'by_parse_date': typing.Union
 [ByParseDateSchema, bool, ], 'lang': typing.Union[LangSchema, dict,
 frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
 decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
@@ -104,17 +105,22 @@
 decimal.Decimal, int, float, ], 'content_sentiment_max': typing.Union
 [ContentSentimentMaxSchema, decimal.Decimal, int, float, ], 'iptc_tags':
 typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime,
 uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes,
 io.FileIO, io.BufferedReader, ], 'not_iptc_tags': typing.Union
 [NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime,
 uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes,
-io.FileIO, io.BufferedReader, ], }, total=False ) class RequestQueryParams
-(RequestRequiredQueryParams, RequestOptionalQueryParams): pass
-request_query_when = api_client.QueryParameter( name="when",
+io.FileIO, io.BufferedReader, ], 'iab_tags': typing.Union[IabTagsSchema, dict,
+frozendict.frozendict, str, date, datetime, uuid.UUID, int, float,
+decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader,
+], 'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict,
+str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list,
+tuple, bytes, io.FileIO, io.BufferedReader, ], }, total=False ) class
+RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
+pass request_query_when = api_client.QueryParameter( name="when",
 style=api_client.ParameterStyle.FORM, schema=WhenSchema, explode=True, )
 request_query_by_parse_date = api_client.QueryParameter( name="by_parse_date",
 style=api_client.ParameterStyle.FORM, schema=ByParseDateSchema, explode=True, )
 request_query_lang = api_client.QueryParameter( name="lang",
 style=api_client.ParameterStyle.FORM, schema=LangSchema, explode=True, )
 request_query_not_lang = api_client.QueryParameter( name="not_lang",
 style=api_client.ParameterStyle.FORM, schema=NotLangSchema, explode=True, )
@@ -195,14 +201,18 @@
 request_query_content_sentiment_max = api_client.QueryParameter
 ( name="content_sentiment_max", style=api_client.ParameterStyle.FORM,
 schema=ContentSentimentMaxSchema, explode=True, ) request_query_iptc_tags =
 api_client.QueryParameter( name="iptc_tags",
 style=api_client.ParameterStyle.FORM, schema=IptcTagsSchema, explode=True, )
 request_query_not_iptc_tags = api_client.QueryParameter( name="not_iptc_tags",
 style=api_client.ParameterStyle.FORM, schema=NotIptcTagsSchema, explode=True, )
+request_query_iab_tags = api_client.QueryParameter( name="iab_tags",
+style=api_client.ParameterStyle.FORM, schema=IabTagsSchema, explode=True, )
+request_query_not_iab_tags = api_client.QueryParameter( name="not_iab_tags",
+style=api_client.ParameterStyle.FORM, schema=NotIabTagsSchema, explode=True, )
 SchemaFor200ResponseBodyApplicationJson = LatestHeadlinesGetResponseSchema
 @dataclass class ApiResponseFor200(api_client.ApiResponse): body:
 LatestHeadlinesGetResponse @dataclass class ApiResponseFor200Async
 (api_client.AsyncApiResponse): body: LatestHeadlinesGetResponse
 _response_for_200 = api_client.OpenApiResponse( response_cls=ApiResponseFor200,
 response_cls_async=ApiResponseFor200Async, content={ 'application/json':
 api_client.MediaType( schema=SchemaFor200ResponseBodyApplicationJson), }, )
@@ -244,58 +254,62 @@
 typing.Optional[str] = None, misc_entity_name: typing.Optional[str] = None,
 title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
 list, str, None]] = None, not_iptc_tags: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, ) -
-> api_client.MappedArgs: args: api_client.MappedArgs = api_client.MappedArgs()
-_query_params = {} if when is not None: _query_params["when"] = when if
-by_parse_date is not None: _query_params["by_parse_date"] = by_parse_date if
-lang is not None: _query_params["lang"] = lang if not_lang is not None:
-_query_params["not_lang"] = not_lang if countries is not None: _query_params
-["countries"] = countries if not_countries is not None: _query_params
-["not_countries"] = not_countries if sources is not None: _query_params
-["sources"] = sources if predefined_sources is not None: _query_params
-["predefined_sources"] = predefined_sources if not_sources is not None:
-_query_params["not_sources"] = not_sources if not_author_name is not None:
-_query_params["not_author_name"] = not_author_name if ranked_only is not None:
-_query_params["ranked_only"] = ranked_only if is_headline is not None:
-_query_params["is_headline"] = is_headline if is_paid_content is not None:
-_query_params["is_paid_content"] = is_paid_content if parent_url is not None:
-_query_params["parent_url"] = parent_url if all_links is not None:
-_query_params["all_links"] = all_links if all_domain_links is not None:
-_query_params["all_domain_links"] = all_domain_links if word_count_min is not
-None: _query_params["word_count_min"] = word_count_min if word_count_max is not
-None: _query_params["word_count_max"] = word_count_max if page is not None:
-_query_params["page"] = page if page_size is not None: _query_params
-["page_size"] = page_size if clustering_variable is not None: _query_params
-["clustering_variable"] = clustering_variable if clustering_enabled is not
-None: _query_params["clustering_enabled"] = clustering_enabled if
-clustering_threshold is not None: _query_params["clustering_threshold"] =
-clustering_threshold if include_nlp_data is not None: _query_params
-["include_nlp_data"] = include_nlp_data if has_nlp is not None: _query_params
-["has_nlp"] = has_nlp if theme is not None: _query_params["theme"] = theme if
-not_theme is not None: _query_params["not_theme"] = not_theme if
-org_entity_name is not None: _query_params["ORG_entity_name"] = org_entity_name
-if per_entity_name is not None: _query_params["PER_entity_name"] =
-per_entity_name if loc_entity_name is not None: _query_params
-["LOC_entity_name"] = loc_entity_name if misc_entity_name is not None:
-_query_params["MISC_entity_name"] = misc_entity_name if title_sentiment_min is
-not None: _query_params["title_sentiment_min"] = title_sentiment_min if
-title_sentiment_max is not None: _query_params["title_sentiment_max"] =
-title_sentiment_max if content_sentiment_min is not None: _query_params
-["content_sentiment_min"] = content_sentiment_min if content_sentiment_max is
-not None: _query_params["content_sentiment_max"] = content_sentiment_max if
-iptc_tags is not None: _query_params["iptc_tags"] = iptc_tags if not_iptc_tags
-is not None: _query_params["not_iptc_tags"] = not_iptc_tags args.query =
-_query_params return args async def _aget_oapg( self, query_params:
-typing.Optional[dict] = {}, skip_deserialization: bool = True, timeout:
-typing.Optional[typing.Union[float, typing.Tuple]] = None,
+date, datetime, dict, float, int, list, str, None]] = None, iab_tags:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, not_iab_tags: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, ) -> api_client.MappedArgs: args:
+api_client.MappedArgs = api_client.MappedArgs() _query_params = {} if when is
+not None: _query_params["when"] = when if by_parse_date is not None:
+_query_params["by_parse_date"] = by_parse_date if lang is not None:
+_query_params["lang"] = lang if not_lang is not None: _query_params["not_lang"]
+= not_lang if countries is not None: _query_params["countries"] = countries if
+not_countries is not None: _query_params["not_countries"] = not_countries if
+sources is not None: _query_params["sources"] = sources if predefined_sources
+is not None: _query_params["predefined_sources"] = predefined_sources if
+not_sources is not None: _query_params["not_sources"] = not_sources if
+not_author_name is not None: _query_params["not_author_name"] = not_author_name
+if ranked_only is not None: _query_params["ranked_only"] = ranked_only if
+is_headline is not None: _query_params["is_headline"] = is_headline if
+is_paid_content is not None: _query_params["is_paid_content"] = is_paid_content
+if parent_url is not None: _query_params["parent_url"] = parent_url if
+all_links is not None: _query_params["all_links"] = all_links if
+all_domain_links is not None: _query_params["all_domain_links"] =
+all_domain_links if word_count_min is not None: _query_params["word_count_min"]
+= word_count_min if word_count_max is not None: _query_params["word_count_max"]
+= word_count_max if page is not None: _query_params["page"] = page if page_size
+is not None: _query_params["page_size"] = page_size if clustering_variable is
+not None: _query_params["clustering_variable"] = clustering_variable if
+clustering_enabled is not None: _query_params["clustering_enabled"] =
+clustering_enabled if clustering_threshold is not None: _query_params
+["clustering_threshold"] = clustering_threshold if include_nlp_data is not
+None: _query_params["include_nlp_data"] = include_nlp_data if has_nlp is not
+None: _query_params["has_nlp"] = has_nlp if theme is not None: _query_params
+["theme"] = theme if not_theme is not None: _query_params["not_theme"] =
+not_theme if org_entity_name is not None: _query_params["ORG_entity_name"] =
+org_entity_name if per_entity_name is not None: _query_params
+["PER_entity_name"] = per_entity_name if loc_entity_name is not None:
+_query_params["LOC_entity_name"] = loc_entity_name if misc_entity_name is not
+None: _query_params["MISC_entity_name"] = misc_entity_name if
+title_sentiment_min is not None: _query_params["title_sentiment_min"] =
+title_sentiment_min if title_sentiment_max is not None: _query_params
+["title_sentiment_max"] = title_sentiment_max if content_sentiment_min is not
+None: _query_params["content_sentiment_min"] = content_sentiment_min if
+content_sentiment_max is not None: _query_params["content_sentiment_max"] =
+content_sentiment_max if iptc_tags is not None: _query_params["iptc_tags"] =
+iptc_tags if not_iptc_tags is not None: _query_params["not_iptc_tags"] =
+not_iptc_tags if iab_tags is not None: _query_params["iab_tags"] = iab_tags if
+not_iab_tags is not None: _query_params["not_iab_tags"] = not_iab_tags
+args.query = _query_params return args async def _aget_oapg( self,
+query_params: typing.Optional[dict] = {}, skip_deserialization: bool = True,
+timeout: typing.Optional[typing.Union[float, typing.Tuple]] = None,
 accept_content_types: typing.Tuple[str] = _all_accept_content_types, stream:
 bool = False, **kwargs, ) -> typing.Union[ ApiResponseFor200Async,
 api_client.ApiResponseWithoutDeserializationAsync, AsyncGeneratorResponse, ]:
 """ [Get] Search For Latest Headlines Request :param skip_deserialization: If
 true then api_response.response will be set but api_response.body and
 api_response.headers will not be deserialized into schema class instances """
 self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params) used_path
@@ -312,15 +326,16 @@
 request_query_clustering_enabled, request_query_clustering_threshold,
 request_query_include_nlp_data, request_query_has_nlp, request_query_theme,
 request_query_not_theme, request_query_org_entity_name,
 request_query_per_entity_name, request_query_loc_entity_name,
 request_query_misc_entity_name, request_query_title_sentiment_min,
 request_query_title_sentiment_max, request_query_content_sentiment_min,
 request_query_content_sentiment_max, request_query_iptc_tags,
-request_query_not_iptc_tags, ): parameter_data = query_params.get
+request_query_not_iptc_tags, request_query_iab_tags,
+request_query_not_iab_tags, ): parameter_data = query_params.get
 (parameter.name, schemas.unset) if parameter_data is schemas.unset: continue if
 prefix_separator_iterator is None: prefix_separator_iterator =
 parameter.get_prefix_separator_iterator() serialized_data = parameter.serialize
 (parameter_data, prefix_separator_iterator) for serialized_value in
 serialized_data.values(): used_path += serialized_value _headers =
 HTTPHeaderDict() # TODO add cookie handling if accept_content_types: for
 accept_content_type in accept_content_types: _headers.add('Accept',
@@ -377,15 +392,16 @@
 request_query_clustering_enabled, request_query_clustering_threshold,
 request_query_include_nlp_data, request_query_has_nlp, request_query_theme,
 request_query_not_theme, request_query_org_entity_name,
 request_query_per_entity_name, request_query_loc_entity_name,
 request_query_misc_entity_name, request_query_title_sentiment_min,
 request_query_title_sentiment_max, request_query_content_sentiment_min,
 request_query_content_sentiment_max, request_query_iptc_tags,
-request_query_not_iptc_tags, ): parameter_data = query_params.get
+request_query_not_iptc_tags, request_query_iab_tags,
+request_query_not_iab_tags, ): parameter_data = query_params.get
 (parameter.name, schemas.unset) if parameter_data is schemas.unset: continue if
 prefix_separator_iterator is None: prefix_separator_iterator =
 parameter.get_prefix_separator_iterator() serialized_data = parameter.serialize
 (parameter_data, prefix_separator_iterator) for serialized_value in
 serialized_data.values(): used_path += serialized_value _headers =
 HTTPHeaderDict() # TODO add cookie handling if accept_content_types: for
 accept_content_type in accept_content_types: _headers.add('Accept',
@@ -440,37 +456,158 @@
 typing.Optional[str] = None, misc_entity_name: typing.Optional[str] = None,
 title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
 list, str, None]] = None, not_iptc_tags: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, **kwargs, ) -
-> typing.Union[ ApiResponseFor200Async,
-api_client.ApiResponseWithoutDeserializationAsync, AsyncGeneratorResponse, ]:
-args = self._get_mapped_args( when=when, by_parse_date=by_parse_date,
-lang=lang, not_lang=not_lang, countries=countries, not_countries=not_countries,
-sources=sources, predefined_sources=predefined_sources,
-not_sources=not_sources, not_author_name=not_author_name,
-ranked_only=ranked_only, is_headline=is_headline,
-is_paid_content=is_paid_content, parent_url=parent_url, all_links=all_links,
-all_domain_links=all_domain_links, word_count_min=word_count_min,
-word_count_max=word_count_max, page=page, page_size=page_size,
-clustering_variable=clustering_variable, clustering_enabled=clustering_enabled,
+date, datetime, dict, float, int, list, str, None]] = None, iab_tags:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, not_iab_tags: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, **kwargs, ) -> typing.Union
+[ ApiResponseFor200Async, api_client.ApiResponseWithoutDeserializationAsync,
+AsyncGeneratorResponse, ]: args = self._get_mapped_args( when=when,
+by_parse_date=by_parse_date, lang=lang, not_lang=not_lang, countries=countries,
+not_countries=not_countries, sources=sources,
+predefined_sources=predefined_sources, not_sources=not_sources,
+not_author_name=not_author_name, ranked_only=ranked_only,
+is_headline=is_headline, is_paid_content=is_paid_content,
+parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
+word_count_min=word_count_min, word_count_max=word_count_max, page=page,
+page_size=page_size, clustering_variable=clustering_variable,
+clustering_enabled=clustering_enabled,
+clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
+has_nlp=has_nlp, theme=theme, not_theme=not_theme,
+org_entity_name=org_entity_name, per_entity_name=per_entity_name,
+loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
+title_sentiment_min=title_sentiment_min,
+title_sentiment_max=title_sentiment_max,
+content_sentiment_min=content_sentiment_min,
+content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, )
+return await self._aget_oapg( query_params=args.query, **kwargs, ) def get
+( self, when: typing.Optional[str] = None, by_parse_date: typing.Optional[bool]
+= None, lang: typing.Optional[typing.Union[bool, date, datetime, dict, float,
+int, list, str, None]] = None, not_lang: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, countries:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, not_countries: typing.Optional[typing.Union[bool, date,
+datetime, dict, float, int, list, str, None]] = None, sources: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, not_sources: typing.Optional[typing.Union
+[bool, date, datetime, dict, float, int, list, str, None]] = None,
+not_author_name: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, ranked_only: typing.Optional[str] = None,
+is_headline: typing.Optional[bool] = None, is_paid_content: typing.Optional
+[bool] = None, parent_url: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, all_links: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+all_domain_links: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, word_count_min: typing.Optional[int] =
+None, word_count_max: typing.Optional[int] = None, page: typing.Optional[int] =
+None, page_size: typing.Optional[int] = None, clustering_variable:
+typing.Optional[str] = None, clustering_enabled: typing.Optional[bool] = None,
+clustering_threshold: typing.Optional[typing.Union[int, float]] = None,
+include_nlp_data: typing.Optional[bool] = None, has_nlp: typing.Optional[bool]
+= None, theme: typing.Optional[str] = None, not_theme: typing.Optional[str] =
+None, org_entity_name: typing.Optional[str] = None, per_entity_name:
+typing.Optional[str] = None, loc_entity_name: typing.Optional[str] = None,
+misc_entity_name: typing.Optional[str] = None, title_sentiment_min:
+typing.Optional[typing.Union[int, float]] = None, title_sentiment_max:
+typing.Optional[typing.Union[int, float]] = None, content_sentiment_min:
+typing.Optional[typing.Union[int, float]] = None, content_sentiment_max:
+typing.Optional[typing.Union[int, float]] = None, iptc_tags: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float,
+int, list, str, None]] = None, iab_tags: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, not_iab_tags:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, ) -> typing.Union[ ApiResponseFor200,
+api_client.ApiResponseWithoutDeserialization, ]: args = self._get_mapped_args
+( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
+countries=countries, not_countries=not_countries, sources=sources,
+predefined_sources=predefined_sources, not_sources=not_sources,
+not_author_name=not_author_name, ranked_only=ranked_only,
+is_headline=is_headline, is_paid_content=is_paid_content,
+parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
+word_count_min=word_count_min, word_count_max=word_count_max, page=page,
+page_size=page_size, clustering_variable=clustering_variable,
+clustering_enabled=clustering_enabled,
+clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
+has_nlp=has_nlp, theme=theme, not_theme=not_theme,
+org_entity_name=org_entity_name, per_entity_name=per_entity_name,
+loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
+title_sentiment_min=title_sentiment_min,
+title_sentiment_max=title_sentiment_max,
+content_sentiment_min=content_sentiment_min,
+content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, )
+return self._get_oapg( query_params=args.query, ) class Get(BaseApi): async def
+aget( self, when: typing.Optional[str] = None, by_parse_date: typing.Optional
+[bool] = None, lang: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, not_lang: typing.Optional[typing.Union
+[bool, date, datetime, dict, float, int, list, str, None]] = None, countries:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, not_countries: typing.Optional[typing.Union[bool, date,
+datetime, dict, float, int, list, str, None]] = None, sources: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, not_sources: typing.Optional[typing.Union
+[bool, date, datetime, dict, float, int, list, str, None]] = None,
+not_author_name: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, ranked_only: typing.Optional[str] = None,
+is_headline: typing.Optional[bool] = None, is_paid_content: typing.Optional
+[bool] = None, parent_url: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, all_links: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+all_domain_links: typing.Optional[typing.Union[bool, date, datetime, dict,
+float, int, list, str, None]] = None, word_count_min: typing.Optional[int] =
+None, word_count_max: typing.Optional[int] = None, page: typing.Optional[int] =
+None, page_size: typing.Optional[int] = None, clustering_variable:
+typing.Optional[str] = None, clustering_enabled: typing.Optional[bool] = None,
+clustering_threshold: typing.Optional[typing.Union[int, float]] = None,
+include_nlp_data: typing.Optional[bool] = None, has_nlp: typing.Optional[bool]
+= None, theme: typing.Optional[str] = None, not_theme: typing.Optional[str] =
+None, org_entity_name: typing.Optional[str] = None, per_entity_name:
+typing.Optional[str] = None, loc_entity_name: typing.Optional[str] = None,
+misc_entity_name: typing.Optional[str] = None, title_sentiment_min:
+typing.Optional[typing.Union[int, float]] = None, title_sentiment_max:
+typing.Optional[typing.Union[int, float]] = None, content_sentiment_min:
+typing.Optional[typing.Union[int, float]] = None, content_sentiment_max:
+typing.Optional[typing.Union[int, float]] = None, iptc_tags: typing.Optional
+[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float,
+int, list, str, None]] = None, iab_tags: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, not_iab_tags:
+typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
+None]] = None, validate: bool = False, **kwargs, ) -
+> LatestHeadlinesGetResponsePydantic: raw_response = await self.raw.aget
+( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
+countries=countries, not_countries=not_countries, sources=sources,
+predefined_sources=predefined_sources, not_sources=not_sources,
+not_author_name=not_author_name, ranked_only=ranked_only,
+is_headline=is_headline, is_paid_content=is_paid_content,
+parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
+word_count_min=word_count_min, word_count_max=word_count_max, page=page,
+page_size=page_size, clustering_variable=clustering_variable,
+clustering_enabled=clustering_enabled,
 clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 org_entity_name=org_entity_name, per_entity_name=per_entity_name,
 loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) return await self._aget_oapg
-( query_params=args.query, **kwargs, ) def get( self, when: typing.Optional
-[str] = None, by_parse_date: typing.Optional[bool] = None, lang:
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags,
+**kwargs, ) if validate: return RootModel[LatestHeadlinesGetResponsePydantic]
+(raw_response.body).root return api_client.construct_model_instance
+(LatestHeadlinesGetResponsePydantic, raw_response.body) def get( self, when:
+typing.Optional[str] = None, by_parse_date: typing.Optional[bool] = None, lang:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
 None]] = None, not_lang: typing.Optional[typing.Union[bool, date, datetime,
 dict, float, int, list, str, None]] = None, countries: typing.Optional
 [typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
 not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float,
 int, list, str, None]] = None, sources: typing.Optional[typing.Union[bool,
 date, datetime, dict, float, int, list, str, None]] = None, predefined_sources:
@@ -496,16 +633,18 @@
 typing.Optional[str] = None, title_sentiment_min: typing.Optional[typing.Union
 [int, float]] = None, title_sentiment_max: typing.Optional[typing.Union[int,
 float]] = None, content_sentiment_min: typing.Optional[typing.Union[int,
 float]] = None, content_sentiment_max: typing.Optional[typing.Union[int,
 float]] = None, iptc_tags: typing.Optional[typing.Union[bool, date, datetime,
 dict, float, int, list, str, None]] = None, not_iptc_tags: typing.Optional
 [typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-) -> typing.Union[ ApiResponseFor200,
-api_client.ApiResponseWithoutDeserialization, ]: args = self._get_mapped_args
+iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
+list, str, None]] = None, not_iab_tags: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, validate: bool =
+False, ) -> LatestHeadlinesGetResponsePydantic: raw_response = self.raw.get
 ( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
 countries=countries, not_countries=not_countries, sources=sources,
 predefined_sources=predefined_sources, not_sources=not_sources,
 not_author_name=not_author_name, ranked_only=ranked_only,
 is_headline=is_headline, is_paid_content=is_paid_content,
 parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
 word_count_min=word_count_min, word_count_max=word_count_max, page=page,
@@ -515,16 +654,20 @@
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 org_entity_name=org_entity_name, per_entity_name=per_entity_name,
 loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) return self._get_oapg( query_params=args.query,
-) class Get(BaseApi): async def aget( self, when: typing.Optional[str] = None,
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, ) if
+validate: return RootModel[LatestHeadlinesGetResponsePydantic]
+(raw_response.body).root return api_client.construct_model_instance
+(LatestHeadlinesGetResponsePydantic, raw_response.body) class ApiForget
+(BaseApi): # this class is used by api classes that refer to endpoints by path
+and http method names async def aget( self, when: typing.Optional[str] = None,
 by_parse_date: typing.Optional[bool] = None, lang: typing.Optional[typing.Union
 [bool, date, datetime, dict, float, int, list, str, None]] = None, not_lang:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
 None]] = None, countries: typing.Optional[typing.Union[bool, date, datetime,
 dict, float, int, list, str, None]] = None, not_countries: typing.Optional
 [typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
 sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
@@ -550,74 +693,22 @@
 typing.Optional[str] = None, misc_entity_name: typing.Optional[str] = None,
 title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
 content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
 iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
 list, str, None]] = None, not_iptc_tags: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, validate: bool =
-False, **kwargs, ) -> LatestHeadlinesGetResponsePydantic: raw_response = await
-self.raw.aget( when=when, by_parse_date=by_parse_date, lang=lang,
-not_lang=not_lang, countries=countries, not_countries=not_countries,
-sources=sources, predefined_sources=predefined_sources,
-not_sources=not_sources, not_author_name=not_author_name,
-ranked_only=ranked_only, is_headline=is_headline,
-is_paid_content=is_paid_content, parent_url=parent_url, all_links=all_links,
-all_domain_links=all_domain_links, word_count_min=word_count_min,
-word_count_max=word_count_max, page=page, page_size=page_size,
-clustering_variable=clustering_variable, clustering_enabled=clustering_enabled,
-clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
-has_nlp=has_nlp, theme=theme, not_theme=not_theme,
-org_entity_name=org_entity_name, per_entity_name=per_entity_name,
-loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
-title_sentiment_min=title_sentiment_min,
-title_sentiment_max=title_sentiment_max,
-content_sentiment_min=content_sentiment_min,
-content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, **kwargs, ) if validate: return RootModel
-[LatestHeadlinesGetResponsePydantic](raw_response.body).root return
-api_client.construct_model_instance(LatestHeadlinesGetResponsePydantic,
-raw_response.body) def get( self, when: typing.Optional[str] = None,
-by_parse_date: typing.Optional[bool] = None, lang: typing.Optional[typing.Union
-[bool, date, datetime, dict, float, int, list, str, None]] = None, not_lang:
-typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, countries: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, not_countries: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
-list, str, None]] = None, predefined_sources: typing.Optional[typing.Union
-[bool, date, datetime, dict, float, int, list, str, None]] = None, not_sources:
+date, datetime, dict, float, int, list, str, None]] = None, iab_tags:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, not_author_name: typing.Optional[typing.Union[bool, date,
-datetime, dict, float, int, list, str, None]] = None, ranked_only:
-typing.Optional[str] = None, is_headline: typing.Optional[bool] = None,
-is_paid_content: typing.Optional[bool] = None, parent_url: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-all_links: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
-list, str, None]] = None, all_domain_links: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, word_count_min:
-typing.Optional[int] = None, word_count_max: typing.Optional[int] = None, page:
-typing.Optional[int] = None, page_size: typing.Optional[int] = None,
-clustering_variable: typing.Optional[str] = None, clustering_enabled:
-typing.Optional[bool] = None, clustering_threshold: typing.Optional
-[typing.Union[int, float]] = None, include_nlp_data: typing.Optional[bool] =
-None, has_nlp: typing.Optional[bool] = None, theme: typing.Optional[str] =
-None, not_theme: typing.Optional[str] = None, org_entity_name: typing.Optional
-[str] = None, per_entity_name: typing.Optional[str] = None, loc_entity_name:
-typing.Optional[str] = None, misc_entity_name: typing.Optional[str] = None,
-title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
-title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
-content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
-content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
-iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int,
-list, str, None]] = None, not_iptc_tags: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, validate: bool =
-False, ) -> LatestHeadlinesGetResponsePydantic: raw_response = self.raw.get
-( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
-countries=countries, not_countries=not_countries, sources=sources,
+None]] = None, not_iab_tags: typing.Optional[typing.Union[bool, date, datetime,
+dict, float, int, list, str, None]] = None, **kwargs, ) -> typing.Union
+[ ApiResponseFor200Async, api_client.ApiResponseWithoutDeserializationAsync,
+AsyncGeneratorResponse, ]: args = self._get_mapped_args( when=when,
+by_parse_date=by_parse_date, lang=lang, not_lang=not_lang, countries=countries,
+not_countries=not_countries, sources=sources,
 predefined_sources=predefined_sources, not_sources=not_sources,
 not_author_name=not_author_name, ranked_only=ranked_only,
 is_headline=is_headline, is_paid_content=is_paid_content,
 parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
 word_count_min=word_count_min, word_count_max=word_count_max, page=page,
 page_size=page_size, clustering_variable=clustering_variable,
 clustering_enabled=clustering_enabled,
@@ -625,19 +716,16 @@
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 org_entity_name=org_entity_name, per_entity_name=per_entity_name,
 loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) if validate: return RootModel
-[LatestHeadlinesGetResponsePydantic](raw_response.body).root return
-api_client.construct_model_instance(LatestHeadlinesGetResponsePydantic,
-raw_response.body) class ApiForget(BaseApi): # this class is used by api
-classes that refer to endpoints by path and http method names async def aget
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, )
+return await self._aget_oapg( query_params=args.query, **kwargs, ) def get
 ( self, when: typing.Optional[str] = None, by_parse_date: typing.Optional[bool]
 = None, lang: typing.Optional[typing.Union[bool, date, datetime, dict, float,
 int, list, str, None]] = None, not_lang: typing.Optional[typing.Union[bool,
 date, datetime, dict, float, int, list, str, None]] = None, countries:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
 None]] = None, not_countries: typing.Optional[typing.Union[bool, date,
 datetime, dict, float, int, list, str, None]] = None, sources: typing.Optional
@@ -664,71 +752,18 @@
 misc_entity_name: typing.Optional[str] = None, title_sentiment_min:
 typing.Optional[typing.Union[int, float]] = None, title_sentiment_max:
 typing.Optional[typing.Union[int, float]] = None, content_sentiment_min:
 typing.Optional[typing.Union[int, float]] = None, content_sentiment_max:
 typing.Optional[typing.Union[int, float]] = None, iptc_tags: typing.Optional
 [typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
 not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float,
-int, list, str, None]] = None, **kwargs, ) -> typing.Union
-[ ApiResponseFor200Async, api_client.ApiResponseWithoutDeserializationAsync,
-AsyncGeneratorResponse, ]: args = self._get_mapped_args( when=when,
-by_parse_date=by_parse_date, lang=lang, not_lang=not_lang, countries=countries,
-not_countries=not_countries, sources=sources,
-predefined_sources=predefined_sources, not_sources=not_sources,
-not_author_name=not_author_name, ranked_only=ranked_only,
-is_headline=is_headline, is_paid_content=is_paid_content,
-parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
-word_count_min=word_count_min, word_count_max=word_count_max, page=page,
-page_size=page_size, clustering_variable=clustering_variable,
-clustering_enabled=clustering_enabled,
-clustering_threshold=clustering_threshold, include_nlp_data=include_nlp_data,
-has_nlp=has_nlp, theme=theme, not_theme=not_theme,
-org_entity_name=org_entity_name, per_entity_name=per_entity_name,
-loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
-title_sentiment_min=title_sentiment_min,
-title_sentiment_max=title_sentiment_max,
-content_sentiment_min=content_sentiment_min,
-content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) return await self._aget_oapg
-( query_params=args.query, **kwargs, ) def get( self, when: typing.Optional
-[str] = None, by_parse_date: typing.Optional[bool] = None, lang:
+int, list, str, None]] = None, iab_tags: typing.Optional[typing.Union[bool,
+date, datetime, dict, float, int, list, str, None]] = None, not_iab_tags:
 typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, not_lang: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, countries: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float,
-int, list, str, None]] = None, sources: typing.Optional[typing.Union[bool,
-date, datetime, dict, float, int, list, str, None]] = None, predefined_sources:
-typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, not_sources: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, not_author_name: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-ranked_only: typing.Optional[str] = None, is_headline: typing.Optional[bool] =
-None, is_paid_content: typing.Optional[bool] = None, parent_url:
-typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str,
-None]] = None, all_links: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, all_domain_links: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-word_count_min: typing.Optional[int] = None, word_count_max: typing.Optional
-[int] = None, page: typing.Optional[int] = None, page_size: typing.Optional
-[int] = None, clustering_variable: typing.Optional[str] = None,
-clustering_enabled: typing.Optional[bool] = None, clustering_threshold:
-typing.Optional[typing.Union[int, float]] = None, include_nlp_data:
-typing.Optional[bool] = None, has_nlp: typing.Optional[bool] = None, theme:
-typing.Optional[str] = None, not_theme: typing.Optional[str] = None,
-org_entity_name: typing.Optional[str] = None, per_entity_name: typing.Optional
-[str] = None, loc_entity_name: typing.Optional[str] = None, misc_entity_name:
-typing.Optional[str] = None, title_sentiment_min: typing.Optional[typing.Union
-[int, float]] = None, title_sentiment_max: typing.Optional[typing.Union[int,
-float]] = None, content_sentiment_min: typing.Optional[typing.Union[int,
-float]] = None, content_sentiment_max: typing.Optional[typing.Union[int,
-float]] = None, iptc_tags: typing.Optional[typing.Union[bool, date, datetime,
-dict, float, int, list, str, None]] = None, not_iptc_tags: typing.Optional
-[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
-) -> typing.Union[ ApiResponseFor200,
+None]] = None, ) -> typing.Union[ ApiResponseFor200,
 api_client.ApiResponseWithoutDeserialization, ]: args = self._get_mapped_args
 ( when=when, by_parse_date=by_parse_date, lang=lang, not_lang=not_lang,
 countries=countries, not_countries=not_countries, sources=sources,
 predefined_sources=predefined_sources, not_sources=not_sources,
 not_author_name=not_author_name, ranked_only=ranked_only,
 is_headline=is_headline, is_paid_content=is_paid_content,
 parent_url=parent_url, all_links=all_links, all_domain_links=all_domain_links,
@@ -739,9 +774,9 @@
 has_nlp=has_nlp, theme=theme, not_theme=not_theme,
 org_entity_name=org_entity_name, per_entity_name=per_entity_name,
 loc_entity_name=loc_entity_name, misc_entity_name=misc_entity_name,
 title_sentiment_min=title_sentiment_min,
 title_sentiment_max=title_sentiment_max,
 content_sentiment_min=content_sentiment_min,
 content_sentiment_max=content_sentiment_max, iptc_tags=iptc_tags,
-not_iptc_tags=not_iptc_tags, ) return self._get_oapg( query_params=args.query,
-)
+not_iptc_tags=not_iptc_tags, iab_tags=iab_tags, not_iab_tags=not_iab_tags, )
+return self._get_oapg( query_params=args.query, )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_latest_headlines/post.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if when is not None:
             _body["when"] = when
         if by_parse_date is not None:
             _body["by_parse_date"] = by_parse_date
@@ -227,14 +229,18 @@
             _body["content_sentiment_min"] = content_sentiment_min
         if content_sentiment_max is not None:
             _body["content_sentiment_max"] = content_sentiment_max
         if iptc_tags is not None:
             _body["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _body["not_iptc_tags"] = not_iptc_tags
+        if iab_tags is not None:
+            _body["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _body["not_iab_tags"] = not_iab_tags
         args.body = _body
         return args
 
     async def _apost_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -471,14 +477,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -515,14 +523,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -560,14 +570,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             when=when,
             by_parse_date=by_parse_date,
@@ -602,14 +614,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
 
 class Post(BaseApi):
 
@@ -648,14 +662,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> LatestHeadlinesPostResponsePydantic:
         raw_response = await self.raw.apost(
             when=when,
             by_parse_date=by_parse_date,
             lang=lang,
@@ -689,14 +705,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[LatestHeadlinesPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(LatestHeadlinesPostResponsePydantic, raw_response.body)
     
     
@@ -735,14 +753,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> LatestHeadlinesPostResponsePydantic:
         raw_response = self.raw.post(
             when=when,
             by_parse_date=by_parse_date,
             lang=lang,
             not_lang=not_lang,
@@ -775,14 +795,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[LatestHeadlinesPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(LatestHeadlinesPostResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
@@ -823,14 +845,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -867,14 +891,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -912,14 +938,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             when=when,
             by_parse_date=by_parse_date,
@@ -954,12 +982,14 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_latest_headlines/post.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_latest_headlines/post.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if when is not None:
             _body["when"] = when
         if by_parse_date is not None:
             _body["by_parse_date"] = by_parse_date
@@ -218,14 +220,18 @@
             _body["content_sentiment_min"] = content_sentiment_min
         if content_sentiment_max is not None:
             _body["content_sentiment_max"] = content_sentiment_max
         if iptc_tags is not None:
             _body["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _body["not_iptc_tags"] = not_iptc_tags
+        if iab_tags is not None:
+            _body["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _body["not_iab_tags"] = not_iab_tags
         args.body = _body
         return args
 
     async def _apost_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -462,14 +468,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -506,14 +514,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -551,14 +561,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             when=when,
             by_parse_date=by_parse_date,
@@ -593,14 +605,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
 
 class Post(BaseApi):
 
@@ -639,14 +653,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> LatestHeadlinesPostResponsePydantic:
         raw_response = await self.raw.apost(
             when=when,
             by_parse_date=by_parse_date,
             lang=lang,
@@ -680,14 +696,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[LatestHeadlinesPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(LatestHeadlinesPostResponsePydantic, raw_response.body)
     
     
@@ -726,14 +744,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> LatestHeadlinesPostResponsePydantic:
         raw_response = self.raw.post(
             when=when,
             by_parse_date=by_parse_date,
             lang=lang,
             not_lang=not_lang,
@@ -766,14 +786,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[LatestHeadlinesPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(LatestHeadlinesPostResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
@@ -814,14 +836,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -858,14 +882,16 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -903,14 +929,16 @@
         misc_entity_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             when=when,
             by_parse_date=by_parse_date,
@@ -945,12 +973,14 @@
             misc_entity_name=misc_entity_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search/get.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
 TitleSentimentMaxSchema = schemas.NumberSchema
 ContentSentimentMinSchema = schemas.NumberSchema
 ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema
 NotIptcTagsSchema = schemas.AnyTypeSchema
 SourceNameSchema = schemas.AnyTypeSchema
 IabTagsSchema = schemas.AnyTypeSchema
+NotIabTagsSchema = schemas.AnyTypeSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
         'q': typing.Union[QSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
@@ -250,14 +251,15 @@
         'title_sentiment_max': typing.Union[TitleSentimentMaxSchema, decimal.Decimal, int, float, ],
         'content_sentiment_min': typing.Union[ContentSentimentMinSchema, decimal.Decimal, int, float, ],
         'content_sentiment_max': typing.Union[ContentSentimentMaxSchema, decimal.Decimal, int, float, ],
         'iptc_tags': typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iptc_tags': typing.Union[NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'source_name': typing.Union[SourceNameSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'iab_tags': typing.Union[IabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -536,14 +538,20 @@
 )
 request_query_iab_tags = api_client.QueryParameter(
     name="iab_tags",
     style=api_client.ParameterStyle.FORM,
     schema=IabTagsSchema,
     explode=True,
 )
+request_query_not_iab_tags = api_client.QueryParameter(
+    name="not_iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=NotIabTagsSchema,
+    explode=True,
+)
 _auth = [
     'apiKey',
 ]
 SchemaFor200ResponseBodyApplicationJson = SearchGetResponseSchema
 
 
 @dataclass
@@ -640,14 +648,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
         if q is not None:
             _query_params["q"] = q
         if search_in is not None:
             _query_params["search_in"] = search_in
@@ -735,14 +744,16 @@
             _query_params["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _query_params["not_iptc_tags"] = not_iptc_tags
         if source_name is not None:
             _query_params["source_name"] = source_name
         if iab_tags is not None:
             _query_params["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _query_params["not_iab_tags"] = not_iab_tags
         args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -808,14 +819,15 @@
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
             request_query_source_name,
             request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -965,14 +977,15 @@
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
             request_query_source_name,
             request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -1074,14 +1087,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1127,14 +1141,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1181,14 +1196,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             q=q,
             search_in=search_in,
@@ -1232,14 +1248,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
 
 class Get(BaseApi):
 
@@ -1287,14 +1304,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> SearchGetResponsePydantic:
         raw_response = await self.raw.aget(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
@@ -1337,14 +1355,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[SearchGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchGetResponsePydantic, raw_response.body)
     
     
@@ -1392,14 +1411,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> SearchGetResponsePydantic:
         raw_response = self.raw.get(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
             sources=sources,
@@ -1441,14 +1461,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[SearchGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchGetResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
@@ -1498,14 +1519,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1551,14 +1573,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1605,14 +1628,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             q=q,
             search_in=search_in,
@@ -1656,12 +1680,13 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search/get.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/get.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
 TitleSentimentMaxSchema = schemas.NumberSchema
 ContentSentimentMinSchema = schemas.NumberSchema
 ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema
 NotIptcTagsSchema = schemas.AnyTypeSchema
 SourceNameSchema = schemas.AnyTypeSchema
 IabTagsSchema = schemas.AnyTypeSchema
+NotIabTagsSchema = schemas.AnyTypeSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
         'q': typing.Union[QSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
@@ -236,14 +237,15 @@
         'title_sentiment_max': typing.Union[TitleSentimentMaxSchema, decimal.Decimal, int, float, ],
         'content_sentiment_min': typing.Union[ContentSentimentMinSchema, decimal.Decimal, int, float, ],
         'content_sentiment_max': typing.Union[ContentSentimentMaxSchema, decimal.Decimal, int, float, ],
         'iptc_tags': typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iptc_tags': typing.Union[NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'source_name': typing.Union[SourceNameSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'iab_tags': typing.Union[IabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -522,14 +524,20 @@
 )
 request_query_iab_tags = api_client.QueryParameter(
     name="iab_tags",
     style=api_client.ParameterStyle.FORM,
     schema=IabTagsSchema,
     explode=True,
 )
+request_query_not_iab_tags = api_client.QueryParameter(
+    name="not_iab_tags",
+    style=api_client.ParameterStyle.FORM,
+    schema=NotIabTagsSchema,
+    explode=True,
+)
 SchemaFor200ResponseBodyApplicationJson = SearchGetResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: SearchGetResponse
 
@@ -619,14 +627,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
         if q is not None:
             _query_params["q"] = q
         if search_in is not None:
             _query_params["search_in"] = search_in
@@ -714,14 +723,16 @@
             _query_params["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _query_params["not_iptc_tags"] = not_iptc_tags
         if source_name is not None:
             _query_params["source_name"] = source_name
         if iab_tags is not None:
             _query_params["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _query_params["not_iab_tags"] = not_iab_tags
         args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -787,14 +798,15 @@
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
             request_query_source_name,
             request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -944,14 +956,15 @@
             request_query_title_sentiment_max,
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
             request_query_source_name,
             request_query_iab_tags,
+            request_query_not_iab_tags,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -1053,14 +1066,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1106,14 +1120,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1160,14 +1175,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             q=q,
             search_in=search_in,
@@ -1211,14 +1227,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
 
 class Get(BaseApi):
 
@@ -1266,14 +1283,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> SearchGetResponsePydantic:
         raw_response = await self.raw.aget(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
@@ -1316,14 +1334,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[SearchGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchGetResponsePydantic, raw_response.body)
     
     
@@ -1371,14 +1390,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> SearchGetResponsePydantic:
         raw_response = self.raw.get(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
             sources=sources,
@@ -1420,14 +1440,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[SearchGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchGetResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
@@ -1477,14 +1498,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1530,14 +1552,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1584,14 +1607,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             q=q,
             search_in=search_in,
@@ -1635,12 +1659,13 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._get_oapg(
             query_params=args.query,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search/post.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if q is not None:
             _body["q"] = q
         if search_in is not None:
             _body["search_in"] = search_in
@@ -254,14 +255,16 @@
             _body["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _body["not_iptc_tags"] = not_iptc_tags
         if source_name is not None:
             _body["source_name"] = source_name
         if iab_tags is not None:
             _body["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _body["not_iab_tags"] = not_iab_tags
         args.body = _body
         return args
 
     async def _apost_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -507,14 +510,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -560,14 +564,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -614,14 +619,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             q=q,
             search_in=search_in,
@@ -665,14 +671,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
 
 class Post(BaseApi):
 
@@ -720,14 +727,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> SearchPostResponsePydantic:
         raw_response = await self.raw.apost(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
@@ -770,14 +778,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[SearchPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchPostResponsePydantic, raw_response.body)
     
     
@@ -825,14 +834,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> SearchPostResponsePydantic:
         raw_response = self.raw.post(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
             sources=sources,
@@ -874,14 +884,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[SearchPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchPostResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
@@ -931,14 +942,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -984,14 +996,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -1038,14 +1051,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             q=q,
             search_in=search_in,
@@ -1089,12 +1103,13 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search/post.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search/post.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if q is not None:
             _body["q"] = q
         if search_in is not None:
             _body["search_in"] = search_in
@@ -245,14 +246,16 @@
             _body["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _body["not_iptc_tags"] = not_iptc_tags
         if source_name is not None:
             _body["source_name"] = source_name
         if iab_tags is not None:
             _body["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _body["not_iab_tags"] = not_iab_tags
         args.body = _body
         return args
 
     async def _apost_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -498,14 +501,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -551,14 +555,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -605,14 +610,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             q=q,
             search_in=search_in,
@@ -656,14 +662,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
 
 class Post(BaseApi):
 
@@ -711,14 +718,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
     ) -> SearchPostResponsePydantic:
         raw_response = await self.raw.apost(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
@@ -761,14 +769,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
             return RootModel[SearchPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchPostResponsePydantic, raw_response.body)
     
     
@@ -816,14 +825,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
     ) -> SearchPostResponsePydantic:
         raw_response = self.raw.post(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
             sources=sources,
@@ -865,14 +875,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
             return RootModel[SearchPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchPostResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
@@ -922,14 +933,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -975,14 +987,15 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -1029,14 +1042,15 @@
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             q=q,
             search_in=search_in,
@@ -1080,12 +1094,13 @@
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_by_link/get.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_by_link/get.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_by_link/post.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_by_link/post.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_by_link/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_similar/get.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_similar/get.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_similar/post.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_search_similar/post.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -42,30 +42,25 @@
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
 
 from ...api_client import Dictionary
 from newscatcherapi_client.pydantic.search_similar_post_response import SearchSimilarPostResponse as SearchSimilarPostResponsePydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
 from newscatcherapi_client.pydantic.more_like_this_request import MoreLikeThisRequest as MoreLikeThisRequestPydantic
 
-from . import path
-
 # body param
 SchemaForRequestBodyApplicationJson = MoreLikeThisRequestSchema
 
 
 request_body_more_like_this_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'apiKey',
-]
 SchemaFor200ResponseBodyApplicationJson = SearchSimilarPostResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: SearchSimilarPostResponse
 
@@ -100,18 +95,14 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_search_similar/post.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_authors/post.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -29,49 +29,49 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from newscatcherapi_client import schemas  # noqa: F401
 
-from newscatcherapi_client.model.search_similar_post_response import SearchSimilarPostResponse as SearchSimilarPostResponseSchema
-from newscatcherapi_client.model.more_like_this_request import MoreLikeThisRequest as MoreLikeThisRequestSchema
 from newscatcherapi_client.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from newscatcherapi_client.model.author_search_request import AuthorSearchRequest as AuthorSearchRequestSchema
+from newscatcherapi_client.model.authors_post_response import AuthorsPostResponse as AuthorsPostResponseSchema
 
-from newscatcherapi_client.type.more_like_this_request import MoreLikeThisRequest
-from newscatcherapi_client.type.search_similar_post_response import SearchSimilarPostResponse
 from newscatcherapi_client.type.http_validation_error import HTTPValidationError
+from newscatcherapi_client.type.authors_post_response import AuthorsPostResponse
+from newscatcherapi_client.type.author_search_request import AuthorSearchRequest
 
 from ...api_client import Dictionary
-from newscatcherapi_client.pydantic.search_similar_post_response import SearchSimilarPostResponse as SearchSimilarPostResponsePydantic
+from newscatcherapi_client.pydantic.author_search_request import AuthorSearchRequest as AuthorSearchRequestPydantic
 from newscatcherapi_client.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
-from newscatcherapi_client.pydantic.more_like_this_request import MoreLikeThisRequest as MoreLikeThisRequestPydantic
+from newscatcherapi_client.pydantic.authors_post_response import AuthorsPostResponse as AuthorsPostResponsePydantic
 
 # body param
-SchemaForRequestBodyApplicationJson = MoreLikeThisRequestSchema
+SchemaForRequestBodyApplicationJson = AuthorSearchRequestSchema
 
 
-request_body_more_like_this_request = api_client.RequestBody(
+request_body_author_search_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = SearchSimilarPostResponseSchema
+SchemaFor200ResponseBodyApplicationJson = AuthorsPostResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: SearchSimilarPostResponse
+    body: AuthorsPostResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: SearchSimilarPostResponse
+    body: AuthorsPostResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -104,30 +104,27 @@
 )
 
 
 class BaseApi(api_client.Api):
 
     def _post_mapped_args(
         self,
-        q: str,
-        search_in: typing.Optional[str] = None,
-        include_similar_documents: typing.Optional[bool] = None,
-        similar_documents_number: typing.Optional[int] = None,
-        similar_documents_fields: typing.Optional[str] = None,
-        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        author_name: str,
+        not_author_name: typing.Optional[str] = None,
         sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        by_parse_date: typing.Optional[bool] = None,
         published_date_precision: typing.Optional[str] = None,
+        by_parse_date: typing.Optional[bool] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -144,49 +141,45 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
-        if q is not None:
-            _body["q"] = q
-        if search_in is not None:
-            _body["search_in"] = search_in
-        if include_similar_documents is not None:
-            _body["include_similar_documents"] = include_similar_documents
-        if similar_documents_number is not None:
-            _body["similar_documents_number"] = similar_documents_number
-        if similar_documents_fields is not None:
-            _body["similar_documents_fields"] = similar_documents_fields
-        if predefined_sources is not None:
-            _body["predefined_sources"] = predefined_sources
+        if author_name is not None:
+            _body["author_name"] = author_name
+        if not_author_name is not None:
+            _body["not_author_name"] = not_author_name
         if sources is not None:
             _body["sources"] = sources
+        if predefined_sources is not None:
+            _body["predefined_sources"] = predefined_sources
         if not_sources is not None:
             _body["not_sources"] = not_sources
         if lang is not None:
             _body["lang"] = lang
         if not_lang is not None:
             _body["not_lang"] = not_lang
         if countries is not None:
             _body["countries"] = countries
         if not_countries is not None:
             _body["not_countries"] = not_countries
         if from_ is not None:
             _body["from_"] = from_
         if to_ is not None:
             _body["to_"] = to_
-        if by_parse_date is not None:
-            _body["by_parse_date"] = by_parse_date
         if published_date_precision is not None:
             _body["published_date_precision"] = published_date_precision
+        if by_parse_date is not None:
+            _body["by_parse_date"] = by_parse_date
         if sort_by is not None:
             _body["sort_by"] = sort_by
         if ranked_only is not None:
             _body["ranked_only"] = ranked_only
         if from_rank is not None:
             _body["from_rank"] = from_rank
         if to_rank is not None:
@@ -227,14 +220,18 @@
             _body["content_sentiment_min"] = content_sentiment_min
         if content_sentiment_max is not None:
             _body["content_sentiment_max"] = content_sentiment_max
         if iptc_tags is not None:
             _body["iptc_tags"] = iptc_tags
         if not_iptc_tags is not None:
             _body["not_iptc_tags"] = not_iptc_tags
+        if iab_tags is not None:
+            _body["iab_tags"] = iab_tags
+        if not_iab_tags is not None:
+            _body["not_iab_tags"] = not_iab_tags
         args.body = _body
         return args
 
     async def _apost_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -245,15 +242,15 @@
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        [Post] Search For Similar Articles Request
+        [Post] Search By Author Request
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -269,20 +266,20 @@
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_similar',
+            path_template='/api/authors',
             body=body,
             auth_settings=_auth,
             headers=_headers,
         )
-        serialized_data = request_body_more_like_this_request.serialize(body, content_type)
+        serialized_data = request_body_author_search_request.serialize(body, content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
@@ -359,15 +356,15 @@
         content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        [Post] Search For Similar Articles Request
+        [Post] Search By Author Request
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -383,20 +380,20 @@
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
         request_before_hook(
             resource_path=used_path,
             method=method,
             configuration=self.api_client.configuration,
-            path_template='/api/search_similar',
+            path_template='/api/authors',
             body=body,
             auth_settings=_auth,
             headers=_headers,
         )
-        serialized_data = request_body_more_like_this_request.serialize(body, content_type)
+        serialized_data = request_body_author_search_request.serialize(body, content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']
     
         response = self.api_client.call_api(
             resource_path=used_path,
@@ -434,30 +431,27 @@
 
 
 class PostRaw(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def apost(
         self,
-        q: str,
-        search_in: typing.Optional[str] = None,
-        include_similar_documents: typing.Optional[bool] = None,
-        similar_documents_number: typing.Optional[int] = None,
-        similar_documents_fields: typing.Optional[str] = None,
-        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        author_name: str,
+        not_author_name: typing.Optional[str] = None,
         sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        by_parse_date: typing.Optional[bool] = None,
         published_date_precision: typing.Optional[str] = None,
+        by_parse_date: typing.Optional[bool] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -474,37 +468,36 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
-            q=q,
-            search_in=search_in,
-            include_similar_documents=include_similar_documents,
-            similar_documents_number=similar_documents_number,
-            similar_documents_fields=similar_documents_fields,
-            predefined_sources=predefined_sources,
+            author_name=author_name,
+            not_author_name=not_author_name,
             sources=sources,
+            predefined_sources=predefined_sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            by_parse_date=by_parse_date,
             published_date_precision=published_date_precision,
+            by_parse_date=by_parse_date,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -521,38 +514,37 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
         self,
-        q: str,
-        search_in: typing.Optional[str] = None,
-        include_similar_documents: typing.Optional[bool] = None,
-        similar_documents_number: typing.Optional[int] = None,
-        similar_documents_fields: typing.Optional[str] = None,
-        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        author_name: str,
+        not_author_name: typing.Optional[str] = None,
         sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        by_parse_date: typing.Optional[bool] = None,
         published_date_precision: typing.Optional[str] = None,
+        by_parse_date: typing.Optional[bool] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -569,35 +561,34 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
-            q=q,
-            search_in=search_in,
-            include_similar_documents=include_similar_documents,
-            similar_documents_number=similar_documents_number,
-            similar_documents_fields=similar_documents_fields,
-            predefined_sources=predefined_sources,
+            author_name=author_name,
+            not_author_name=not_author_name,
             sources=sources,
+            predefined_sources=predefined_sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            by_parse_date=by_parse_date,
             published_date_precision=published_date_precision,
+            by_parse_date=by_parse_date,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -614,39 +605,38 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
 
 class Post(BaseApi):
 
     async def apost(
         self,
-        q: str,
-        search_in: typing.Optional[str] = None,
-        include_similar_documents: typing.Optional[bool] = None,
-        similar_documents_number: typing.Optional[int] = None,
-        similar_documents_fields: typing.Optional[str] = None,
-        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        author_name: str,
+        not_author_name: typing.Optional[str] = None,
         sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        by_parse_date: typing.Optional[bool] = None,
         published_date_precision: typing.Optional[str] = None,
+        by_parse_date: typing.Optional[bool] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -663,34 +653,33 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
         **kwargs,
-    ) -> SearchSimilarPostResponsePydantic:
+    ) -> AuthorsPostResponsePydantic:
         raw_response = await self.raw.apost(
-            q=q,
-            search_in=search_in,
-            include_similar_documents=include_similar_documents,
-            similar_documents_number=similar_documents_number,
-            similar_documents_fields=similar_documents_fields,
-            predefined_sources=predefined_sources,
+            author_name=author_name,
+            not_author_name=not_author_name,
             sources=sources,
+            predefined_sources=predefined_sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            by_parse_date=by_parse_date,
             published_date_precision=published_date_precision,
+            by_parse_date=by_parse_date,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -707,39 +696,38 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
             **kwargs,
         )
         if validate:
-            return RootModel[SearchSimilarPostResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchSimilarPostResponsePydantic, raw_response.body)
+            return RootModel[AuthorsPostResponsePydantic](raw_response.body).root
+        return api_client.construct_model_instance(AuthorsPostResponsePydantic, raw_response.body)
     
     
     def post(
         self,
-        q: str,
-        search_in: typing.Optional[str] = None,
-        include_similar_documents: typing.Optional[bool] = None,
-        similar_documents_number: typing.Optional[int] = None,
-        similar_documents_fields: typing.Optional[str] = None,
-        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        author_name: str,
+        not_author_name: typing.Optional[str] = None,
         sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        by_parse_date: typing.Optional[bool] = None,
         published_date_precision: typing.Optional[str] = None,
+        by_parse_date: typing.Optional[bool] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -756,33 +744,32 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         validate: bool = False,
-    ) -> SearchSimilarPostResponsePydantic:
+    ) -> AuthorsPostResponsePydantic:
         raw_response = self.raw.post(
-            q=q,
-            search_in=search_in,
-            include_similar_documents=include_similar_documents,
-            similar_documents_number=similar_documents_number,
-            similar_documents_fields=similar_documents_fields,
-            predefined_sources=predefined_sources,
+            author_name=author_name,
+            not_author_name=not_author_name,
             sources=sources,
+            predefined_sources=predefined_sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            by_parse_date=by_parse_date,
             published_date_precision=published_date_precision,
+            by_parse_date=by_parse_date,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -799,41 +786,40 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         if validate:
-            return RootModel[SearchSimilarPostResponsePydantic](raw_response.body).root
-        return api_client.construct_model_instance(SearchSimilarPostResponsePydantic, raw_response.body)
+            return RootModel[AuthorsPostResponsePydantic](raw_response.body).root
+        return api_client.construct_model_instance(AuthorsPostResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
-        q: str,
-        search_in: typing.Optional[str] = None,
-        include_similar_documents: typing.Optional[bool] = None,
-        similar_documents_number: typing.Optional[int] = None,
-        similar_documents_fields: typing.Optional[str] = None,
-        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        author_name: str,
+        not_author_name: typing.Optional[str] = None,
         sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        by_parse_date: typing.Optional[bool] = None,
         published_date_precision: typing.Optional[str] = None,
+        by_parse_date: typing.Optional[bool] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -850,37 +836,36 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
-            q=q,
-            search_in=search_in,
-            include_similar_documents=include_similar_documents,
-            similar_documents_number=similar_documents_number,
-            similar_documents_fields=similar_documents_fields,
-            predefined_sources=predefined_sources,
+            author_name=author_name,
+            not_author_name=not_author_name,
             sources=sources,
+            predefined_sources=predefined_sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            by_parse_date=by_parse_date,
             published_date_precision=published_date_precision,
+            by_parse_date=by_parse_date,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -897,38 +882,37 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
         self,
-        q: str,
-        search_in: typing.Optional[str] = None,
-        include_similar_documents: typing.Optional[bool] = None,
-        similar_documents_number: typing.Optional[int] = None,
-        similar_documents_fields: typing.Optional[str] = None,
-        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        author_name: str,
+        not_author_name: typing.Optional[str] = None,
         sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        predefined_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_sources: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_lang: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_countries: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         from_: typing.Optional[typing.Union[str, datetime]] = None,
         to_: typing.Optional[typing.Union[str, datetime]] = None,
-        by_parse_date: typing.Optional[bool] = None,
         published_date_precision: typing.Optional[str] = None,
+        by_parse_date: typing.Optional[bool] = None,
         sort_by: typing.Optional[str] = None,
         ranked_only: typing.Optional[str] = None,
         from_rank: typing.Optional[int] = None,
         to_rank: typing.Optional[int] = None,
         is_headline: typing.Optional[bool] = None,
         is_paid_content: typing.Optional[bool] = None,
         parent_url: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
@@ -945,35 +929,34 @@
         ner_name: typing.Optional[str] = None,
         title_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         title_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
-            q=q,
-            search_in=search_in,
-            include_similar_documents=include_similar_documents,
-            similar_documents_number=similar_documents_number,
-            similar_documents_fields=similar_documents_fields,
-            predefined_sources=predefined_sources,
+            author_name=author_name,
+            not_author_name=not_author_name,
             sources=sources,
+            predefined_sources=predefined_sources,
             not_sources=not_sources,
             lang=lang,
             not_lang=not_lang,
             countries=countries,
             not_countries=not_countries,
             from_=from_,
             to_=to_,
-            by_parse_date=by_parse_date,
             published_date_precision=published_date_precision,
+            by_parse_date=by_parse_date,
             sort_by=sort_by,
             ranked_only=ranked_only,
             from_rank=from_rank,
             to_rank=to_rank,
             is_headline=is_headline,
             is_paid_content=is_paid_content,
             parent_url=parent_url,
@@ -990,12 +973,14 @@
             ner_name=ner_name,
             title_sentiment_min=title_sentiment_min,
             title_sentiment_max=title_sentiment_max,
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
+            iab_tags=iab_tags,
+            not_iab_tags=not_iab_tags,
         )
         return self._post_oapg(
             body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_sources/get.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_sources/get.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_sources/post.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_sources/post.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_sources/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_subscription/get.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_subscription/get.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_subscription/post.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/paths/api_subscription/post.pyi` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/paths/api_subscription/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/author_search_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/author_search_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,11 +88,15 @@
 
     content_sentiment_max: typing.Optional[typing.Union[int, float]] = Field(None, alias='content_sentiment_max')
 
     iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='iptc_tags')
 
     not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='not_iptc_tags')
 
+    iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='iab_tags')
+
+    not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='not_iab_tags')
+
     model_config = ConfigDict(
         protected_namespaces=(),
         arbitrary_types_allowed=True
     )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/cluster.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,11 +88,15 @@
 
     content_sentiment_max: typing.Optional[typing.Union[int, float]] = Field(None, alias='content_sentiment_max')
 
     iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='iptc_tags')
 
     not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='not_iptc_tags')
 
+    iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='iab_tags')
+
+    not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='not_iab_tags')
+
     model_config = ConfigDict(
         protected_namespaces=(),
         arbitrary_types_allowed=True
     )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,11 +106,13 @@
 
     not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='not_iptc_tags')
 
     source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='source_name')
 
     iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='iab_tags')
 
+    not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='not_iab_tags')
+
     model_config = ConfigDict(
         protected_namespaces=(),
         arbitrary_types_allowed=True
     )
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/search_url_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/search_url_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/similar_document.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/source_info.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/source_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/sources_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/subscription_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/validation_error.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/pydantic/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/pydantic/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/request_after_hook.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/request_before_hook.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/request_before_url_hook.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/request_before_url_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/rest.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/schemas.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/schemas.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/author_search_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/author_search_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,9 +88,13 @@
 
     content_sentiment_max: typing.Union[int, float]
 
     iptc_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
     not_iptc_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
+    iab_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
+
+    not_iab_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
+
 class AuthorSearchRequest(RequiredAuthorSearchRequest, OptionalAuthorSearchRequest):
     pass
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/cluster.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,9 +90,13 @@
 
     content_sentiment_max: typing.Union[int, float]
 
     iptc_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
     not_iptc_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
+    iab_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
+
+    not_iab_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
+
 class LatestHeadlinesRequest(RequiredLatestHeadlinesRequest, OptionalLatestHeadlinesRequest):
     pass
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,9 +106,11 @@
 
     not_iptc_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
     source_name: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
     iab_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
+    not_iab_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
+
 class SearchRequest(RequiredSearchRequest, OptionalSearchRequest):
     pass
```

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/search_url_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/search_url_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/similar_document.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/source_info.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/source_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/sources_request.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/subscription_response.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/validation_error.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/type_util.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/type_util.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/newscatcherapi_client/validation_metadata.py` & `newscatcherapi_python_sdk-6.0.3/newscatcherapi_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.2/pyproject.toml` & `newscatcherapi_python_sdk-6.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "newscatcherapi-python-sdk"
-version = "6.0.2"
+version = "6.0.3"
 description = "Client for NewsCatcher-V3 Production API"
 authors = ["Maksym Sugonyaka <maksym@newscatcherapi.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "newscatcherapi_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `newscatcherapi_python_sdk-6.0.2/PKG-INFO` & `newscatcherapi_python_sdk-6.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: newscatcherapi-python-sdk
-Version: 6.0.2
+Version: 6.0.3
 Summary: Client for NewsCatcher-V3 Production API
 License: MIT
 Author: Maksym Sugonyaka
 Author-email: maksym@newscatcherapi.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: certifi (>=2023.7.22)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
@@ -25,15 +24,15 @@
 Description-Content-Type: text/markdown
 
 # newscatcherapi-python-sdk<a id="newscatcherapi-python-sdk"></a>
 
 <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v6.0.2-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.2)
+[![PyPI](https://img.shields.io/badge/PyPI-v6.0.3-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.3)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/konfig-dev/newscatcher-sdks/tree/main/v3/python#readme)
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
 
 - [Requirements](#requirements)
@@ -62,15 +61,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install newscatcherapi-python-sdk==6.0.2
+pip install newscatcherapi-python-sdk==6.0.3
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from pprint import pprint
 from newscatcherapi_client import Newscatcher, ApiException
@@ -115,14 +114,16 @@
         ner_name="string_example",
         title_sentiment_min=3.14,
         title_sentiment_max=3.14,
         content_sentiment_min=3.14,
         content_sentiment_max=3.14,
         iptc_tags=None,
         not_iptc_tags=None,
+        iab_tags=None,
+        not_iab_tags=None,
     )
     print(get_response)
 except ApiException as e:
     print("Exception when calling AuthorsApi.get: %s\n" % e)
     pprint(e.body)
     if e.status == 422:
         pprint(e.body["detail"])
@@ -183,14 +184,16 @@
             ner_name="string_example",
             title_sentiment_min=3.14,
             title_sentiment_max=3.14,
             content_sentiment_min=3.14,
             content_sentiment_max=3.14,
             iptc_tags=None,
             not_iptc_tags=None,
+            iab_tags=None,
+            not_iab_tags=None,
         )
         print(get_response)
     except ApiException as e:
         print("Exception when calling AuthorsApi.get: %s\n" % e)
         pprint(e.body)
         if e.status == 422:
             pprint(e.body["detail"])
@@ -251,14 +254,16 @@
         ner_name="string_example",
         title_sentiment_min=3.14,
         title_sentiment_max=3.14,
         content_sentiment_min=3.14,
         content_sentiment_max=3.14,
         iptc_tags=None,
         not_iptc_tags=None,
+        iab_tags=None,
+        not_iab_tags=None,
     )
     pprint(get_response.body)
     pprint(get_response.headers)
     pprint(get_response.status)
     pprint(get_response.round_trip_time)
 except ApiException as e:
     print("Exception when calling AuthorsApi.get: %s\n" % e)
@@ -314,14 +319,16 @@
     ner_name="string_example",
     title_sentiment_min=3.14,
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
+    iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### author_name: `str`<a id="author_name-str"></a>
 
@@ -395,14 +402,18 @@
 
 ##### content_sentiment_max: `Union[int, float]`<a id="content_sentiment_max-unionint-float"></a>
 
 ##### iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
+##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`AuthorsGetResponse`](./newscatcherapi_client/pydantic/authors_get_response.py)
 
 #### 🌐 Endpoint<a id="🌐-endpoint"></a>
 
 `/api/authors` `get`
@@ -452,14 +463,16 @@
     ner_name="string_example",
     title_sentiment_min=3.14,
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
+    iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### author_name: `str`<a id="author_name-str"></a>
 
@@ -533,14 +546,18 @@
 
 ##### content_sentiment_max: `Union[int, float]`<a id="content_sentiment_max-unionint-float"></a>
 
 ##### iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
+##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`AuthorSearchRequest`](./newscatcherapi_client/type/author_search_request.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`AuthorsPostResponse`](./newscatcherapi_client/pydantic/authors_post_response.py)
 
@@ -593,14 +610,16 @@
     misc_entity_name="string_example",
     title_sentiment_min=3.14,
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
+    iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### when: `str`<a id="when-str"></a>
 
@@ -672,14 +691,18 @@
 
 ##### content_sentiment_max: `Union[int, float]`<a id="content_sentiment_max-unionint-float"></a>
 
 ##### iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
+##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`LatestHeadlinesGetResponse`](./newscatcherapi_client/pydantic/latest_headlines_get_response.py)
 
 #### 🌐 Endpoint<a id="🌐-endpoint"></a>
 
 `/api/latest_headlines` `get`
@@ -729,14 +752,16 @@
     misc_entity_name="string_example",
     title_sentiment_min=3.14,
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
+    iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### when: `str`<a id="when-str"></a>
 
@@ -808,14 +833,18 @@
 
 ##### content_sentiment_max: `Union[int, float]`<a id="content_sentiment_max-unionint-float"></a>
 
 ##### iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
+##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`LatestHeadlinesRequest`](./newscatcherapi_client/type/latest_headlines_request.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`LatestHeadlinesPostResponse`](./newscatcherapi_client/pydantic/latest_headlines_post_response.py)
 
@@ -877,14 +906,15 @@
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
     source_name=None,
     iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### q: `str`<a id="q-str"></a>
 
@@ -976,14 +1006,16 @@
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### source_name: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="source_name-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
+
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`SearchGetResponse`](./newscatcherapi_client/pydantic/search_get_response.py)
 
 #### 🌐 Endpoint<a id="🌐-endpoint"></a>
 
 `/api/search` `get`
@@ -1042,14 +1074,15 @@
     title_sentiment_max=3.14,
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
     source_name=None,
     iab_tags=None,
+    not_iab_tags=None,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### q: `str`<a id="q-str"></a>
 
@@ -1141,14 +1174,16 @@
 
 ##### not_iptc_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iptc_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### source_name: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="source_name-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
+##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`SearchRequest`](./newscatcherapi_client/type/search_request.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`SearchPostResponse`](./newscatcherapi_client/pydantic/search_post_response.py)
```

