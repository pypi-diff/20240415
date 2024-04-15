# Comparing `tmp/airbyte_source_slack-0.4.1.tar.gz` & `tmp/airbyte_source_slack-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_slack-0.4.1.tar", max compression
+gzip compressed data, was "airbyte_source_slack-1.0.0.tar", max compression
```

## Comparing `airbyte_source_slack-0.4.1.tar` & `airbyte_source_slack-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,19 @@
--rw-r--r--   0        0        0     4478 2024-03-28 22:30:58.329734 airbyte_source_slack-0.4.1/README.md
--rw-r--r--   0        0        0      754 2024-03-28 22:34:05.791304 airbyte_source_slack-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       59 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/__init__.py
--rw-r--r--   0        0        0      227 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/run.py
--rw-r--r--   0        0        0      232 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/schemas/channel_members.json
--rw-r--r--   0        0        0     5316 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/schemas/channel_messages.json
--rw-r--r--   0        0        0     2348 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/schemas/channels.json
--rw-r--r--   0        0        0     2549 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/schemas/threads.json
--rw-r--r--   0        0        0     3288 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/schemas/users.json
--rw-r--r--   0        0        0    18222 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/source.py
--rw-r--r--   0        0        0     5335 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/spec.json
--rw-r--r--   0        0        0      833 2024-03-28 22:30:58.337734 airbyte_source_slack-0.4.1/source_slack/utils.py
--rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 airbyte_source_slack-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4478 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/README.md
+-rw-r--r--   0        0        0      775 2024-04-15 16:08:24.400759 airbyte_source_slack-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/components/__init__.py
+-rw-r--r--   0        0        0      660 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/components/channel_members_extractor.py
+-rw-r--r--   0        0        0     5080 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/components/join_channels.py
+-rw-r--r--   0        0        0     2883 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/config_migrations.py
+-rw-r--r--   0        0        0     7900 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/manifest.yaml
+-rw-r--r--   0        0        0      344 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/run.py
+-rw-r--r--   0        0        0      232 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/schemas/channel_members.json
+-rw-r--r--   0        0        0     5316 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/schemas/channel_messages.json
+-rw-r--r--   0        0        0     2348 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/schemas/channels.json
+-rw-r--r--   0        0        0     2549 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/schemas/threads.json
+-rw-r--r--   0        0        0     3288 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/schemas/users.json
+-rw-r--r--   0        0        0     2365 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/source.py
+-rw-r--r--   0        0        0     5326 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/spec.json
+-rw-r--r--   0        0        0    12505 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/streams.py
+-rw-r--r--   0        0        0      835 2024-04-15 13:48:02.000000 airbyte_source_slack-1.0.0/source_slack/utils.py
+-rw-r--r--   0        0        0     5253 1970-01-01 00:00:00.000000 airbyte_source_slack-1.0.0/PKG-INFO
```

### Comparing `airbyte_source_slack-0.4.1/README.md` & `airbyte_source_slack-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-0.4.1/pyproject.toml` & `airbyte_source_slack-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.4.1"
+version = "1.0.0"
 name = "airbyte-source-slack"
 description = "Source implementation for Slack."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -20,14 +20,15 @@
     { include = "source_slack" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 pendulum = "==2.1.2"
 airbyte-cdk = "^0"
+freezegun = "^1.4.0"
 
 [tool.poetry.scripts]
 source-slack = "source_slack.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_slack-0.4.1/source_slack/schemas/channel_messages.json` & `airbyte_source_slack-1.0.0/source_slack/schemas/channel_messages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-0.4.1/source_slack/schemas/channels.json` & `airbyte_source_slack-1.0.0/source_slack/schemas/channels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-0.4.1/source_slack/schemas/threads.json` & `airbyte_source_slack-1.0.0/source_slack/schemas/threads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-0.4.1/source_slack/schemas/users.json` & `airbyte_source_slack-1.0.0/source_slack/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-0.4.1/source_slack/source.py` & `airbyte_source_slack-1.0.0/source_slack/streams.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 from abc import ABC, abstractmethod
-from typing import Any, Iterable, List, Mapping, MutableMapping, Optional, Tuple
+from typing import Any, Iterable, List, Mapping, MutableMapping, Optional
 
 import pendulum
 import requests
-from airbyte_cdk import AirbyteLogger
 from airbyte_cdk.models import SyncMode
-from airbyte_cdk.sources import AbstractSource
-from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.sources.streams.http import HttpStream, HttpSubStream
-from airbyte_cdk.sources.streams.http.requests_native_auth import TokenAuthenticator
 from pendulum import DateTime
 
+from .components.join_channels import JoinChannelsStream
 from .utils import chunk_date_range
 
 
 class SlackStream(HttpStream, ABC):
     url_base = "https://slack.com/api/"
     primary_key = "id"
     page_size = 1000
@@ -78,49 +75,14 @@
     def data_field(self) -> str:
         """The name of the field in the response which contains the data"""
 
     def should_retry(self, response: requests.Response) -> bool:
         return response.status_code == requests.codes.REQUEST_TIMEOUT or super().should_retry(response)
 
 
-class JoinChannelsStream(HttpStream):
-    """
-    This class is a special stream which joins channels because the Slack API only returns messages from channels this bot is in.
-    Its responses should only be logged for debugging reasons, not read as records.
-    """
-
-    url_base = "https://slack.com/api/"
-    http_method = "POST"
-    primary_key = "id"
-
-    def __init__(self, channel_filter: List[str] = None, **kwargs):
-        self.channel_filter = channel_filter or []
-        super().__init__(**kwargs)
-
-    def parse_response(self, response: requests.Response, stream_slice: Mapping[str, Any] = None, **kwargs) -> Iterable:
-        """
-        Override to simply indicate that the specific channel was joined successfully.
-        This method should not return any data, but should return an empty iterable.
-        """
-        self.logger.info(f"Successfully joined channel: {stream_slice['channel_name']}")
-        return []
-
-    def next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
-        """
-        The pagination is not applicable to this Service Stream.
-        """
-        return None
-
-    def path(self, **kwargs) -> str:
-        return "conversations.join"
-
-    def request_body_json(self, stream_slice: Mapping = None, **kwargs) -> Optional[Mapping]:
-        return {"channel": stream_slice["channel"]}
-
-
 class ChanneledStream(SlackStream, ABC):
     """Slack stream with channel filter"""
 
     def __init__(self, channel_filter: List[str] = [], join_channels: bool = False, **kwargs):
         self.channel_filter = channel_filter
         self.join_channels = join_channels
         self.kwargs = kwargs
@@ -180,44 +142,14 @@
                     stream_slice=self.make_join_channel_slice(channel),
                 )
             # reading the channel data
             self.logger.info(f"Reading the channel: `{channel.get('name')}`")
             yield channel
 
 
-class ChannelMembers(ChanneledStream):
-    data_field = "members"
-    primary_key = ["member_id", "channel_id"]
-
-    def path(self, **kwargs) -> str:
-        return "conversations.members"
-
-    def request_params(self, stream_state: Mapping[str, Any], stream_slice: Mapping[str, Any] = None, **kwargs) -> MutableMapping[str, Any]:
-        params = super().request_params(stream_state=stream_state, stream_slice=stream_slice, **kwargs)
-        params["channel"] = stream_slice["channel_id"]
-        return params
-
-    def parse_response(self, response: requests.Response, stream_slice: Mapping[str, Any] = None, **kwargs) -> Iterable[Mapping]:
-        for member_id in super().parse_response(response, **kwargs):
-            # Slack just returns raw IDs as a string, so we want to put them in a "join table" format
-            yield {"member_id": member_id, "channel_id": stream_slice["channel_id"]}
-
-    def stream_slices(self, **kwargs) -> Iterable[Optional[Mapping[str, Any]]]:
-        channels_stream = Channels(authenticator=self._session.auth, channel_filter=self.channel_filter)
-        for channel_record in channels_stream.read_records(sync_mode=SyncMode.full_refresh):
-            yield {"channel_id": channel_record["id"]}
-
-
-class Users(SlackStream):
-    data_field = "members"
-
-    def path(self, **kwargs) -> str:
-        return "users.list"
-
-
 # Incremental Streams
 class IncrementalMessageStream(ChanneledStream, ABC):
     data_field = "messages"
     cursor_field = "float_ts"
     primary_key = ["channel_id", "ts"]
 
     def __init__(self, default_start_date: DateTime, end_date: Optional[DateTime] = None, **kwargs):
@@ -342,69 +274,7 @@
             self.logger.info(f"Syncing replies {message_chunk}")
             for message in messages_stream.read_records(sync_mode=SyncMode.full_refresh, stream_slice=message_chunk):
                 yield {"channel": message_chunk["channel"], self.sub_primary_key_2: message[self.sub_primary_key_2]}
                 slice_yielded = True
         if not slice_yielded:
             # yield an empty slice to checkpoint state later
             yield {}
-
-
-class SourceSlack(AbstractSource):
-    def _get_authenticator(self, config: Mapping[str, Any]):
-        # Added to maintain backward compatibility with previous versions
-        if "api_token" in config:
-            return TokenAuthenticator(config["api_token"])
-
-        credentials = config.get("credentials", {})
-        credentials_title = credentials.get("option_title")
-        if credentials_title == "Default OAuth2.0 authorization":
-            return TokenAuthenticator(credentials["access_token"])
-        elif credentials_title == "API Token Credentials":
-            return TokenAuthenticator(credentials["api_token"])
-        else:
-            raise Exception(f"No supported option_title: {credentials_title} specified. See spec.json for references")
-
-    def check_connection(self, logger: AirbyteLogger, config: Mapping[str, Any]) -> Tuple[bool, Optional[Any]]:
-        try:
-            authenticator = self._get_authenticator(config)
-            users_stream = Users(authenticator=authenticator)
-            next(users_stream.read_records(SyncMode.full_refresh))
-            return True, None
-        except Exception as e:
-            return (
-                False,
-                f"Got an exception while trying to set up the connection: {e}. "
-                f"Most probably, there are no users in the given Slack instance or your token is incorrect",
-            )
-
-    def streams(self, config: Mapping[str, Any]) -> List[Stream]:
-        authenticator = self._get_authenticator(config)
-        default_start_date = pendulum.parse(config["start_date"])
-        # this field is not exposed to spec, used only for testing purposes
-        end_date = config.get("end_date")
-        end_date = end_date and pendulum.parse(end_date)
-        threads_lookback_window = pendulum.Duration(days=config["lookback_window"])
-        channel_filter = config.get("channel_filter", [])
-        should_join_to_channels = config.get("join_channels")
-
-        channels = Channels(authenticator=authenticator, join_channels=should_join_to_channels, channel_filter=channel_filter)
-        streams = [
-            channels,
-            ChannelMembers(authenticator=authenticator, channel_filter=channel_filter),
-            ChannelMessages(
-                parent=channels,
-                authenticator=authenticator,
-                default_start_date=default_start_date,
-                end_date=end_date,
-                channel_filter=channel_filter,
-            ),
-            Threads(
-                authenticator=authenticator,
-                default_start_date=default_start_date,
-                end_date=end_date,
-                lookback_window=threads_lookback_window,
-                channel_filter=channel_filter,
-            ),
-            Users(authenticator=authenticator),
-        ]
-
-        return streams
```

### Comparing `airbyte_source_slack-0.4.1/source_slack/spec.json` & `airbyte_source_slack-1.0.0/source_slack/spec.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6614583333333334%*

 * *Differences: {"'advanced_auth'": "{'oauth_config_specification': "*

 * *                    "{'oauth_user_input_from_connector_config_specification': None}}",*

 * * 'delete': "['documentationUrl']"}*

```diff
@@ -42,15 +42,16 @@
                             "credentials",
                             "client_secret"
                         ],
                         "type": "string"
                     }
                 },
                 "type": "object"
-            }
+            },
+            "oauth_user_input_from_connector_config_specification": null
         },
         "predicate_key": [
             "credentials",
             "option_title"
         ],
         "predicate_value": "Default OAuth2.0 authorization"
     },
@@ -166,10 +167,9 @@
         "required": [
             "start_date",
             "lookback_window",
             "join_channels"
         ],
         "title": "Slack Spec",
         "type": "object"
-    },
-    "documentationUrl": "https://docs.airbyte.com/integrations/sources/slack"
+    }
 }
```

### Comparing `airbyte_source_slack-0.4.1/source_slack/utils.py` & `airbyte_source_slack-1.0.0/source_slack/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import Iterable, Optional
 
 import pendulum
 from pendulum import DateTime, Period
 
 
-def chunk_date_range(start_date: DateTime, interval=pendulum.duration(days=1), end_date: Optional[DateTime] = None) -> Iterable[Period]:
+def chunk_date_range(start_date: DateTime, interval=pendulum.duration(days=100), end_date: Optional[DateTime] = None) -> Iterable[Period]:
     """
     Yields a list of the beginning and ending timestamps of each day between the start date and now.
     The return value is a pendulum.period
     """
 
     end_date = end_date or pendulum.now()
     # Each stream_slice contains the beginning and ending timestamp for a 24 hour period
```

### Comparing `airbyte_source_slack-0.4.1/PKG-INFO` & `airbyte_source_slack-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: airbyte-source-slack
-Version: 0.4.1
+Version: 1.0.0
 Summary: Source implementation for Slack.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: freezegun (>=1.4.0,<2.0.0)
 Requires-Dist: pendulum (==2.1.2)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/slack
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Slack source connector
```

