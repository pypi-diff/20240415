# Comparing `tmp/dc_prometheus-1.0.tar.gz` & `tmp/dc_prometheus-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dc_prometheus-1.0.tar", last modified: Sat Mar 16 07:08:10 2024, max compression
+gzip compressed data, was "dc_prometheus-1.1.tar", last modified: Mon Apr 15 08:53:03 2024, max compression
```

## Comparing `dc_prometheus-1.0.tar` & `dc_prometheus-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 07:08:10.695452 dc_prometheus-1.0/
--rw-rw-rw-   0        0        0     1067 2024-03-16 07:05:00.000000 dc_prometheus-1.0/LICENSE
--rw-rw-rw-   0        0        0      508 2024-03-16 07:08:10.693790 dc_prometheus-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       22 2024-03-16 06:57:52.000000 dc_prometheus-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 07:08:10.686867 dc_prometheus-1.0/dc_prometheus/
--rw-rw-rw-   0        0        0       39 2023-09-20 04:38:07.000000 dc_prometheus-1.0/dc_prometheus/__init__.py
--rw-rw-rw-   0        0        0     3649 2024-03-16 06:35:36.000000 dc_prometheus-1.0/dc_prometheus/logcog.py
-drwxrwxrwx   0        0        0        0 2024-03-16 07:08:10.692996 dc_prometheus-1.0/dc_prometheus.egg-info/
--rw-rw-rw-   0        0        0      508 2024-03-16 07:08:10.000000 dc_prometheus-1.0/dc_prometheus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-03-16 07:08:10.000000 dc_prometheus-1.0/dc_prometheus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 07:08:10.000000 dc_prometheus-1.0/dc_prometheus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-03-16 07:08:10.000000 dc_prometheus-1.0/dc_prometheus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-16 07:08:10.000000 dc_prometheus-1.0/dc_prometheus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-16 07:08:10.695452 dc_prometheus-1.0/setup.cfg
--rw-rw-rw-   0        0        0      771 2024-03-16 06:56:00.000000 dc_prometheus-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:53:03.876937 dc_prometheus-1.1/
+-rw-rw-rw-   0        0        0     1067 2024-03-16 07:05:00.000000 dc_prometheus-1.1/LICENSE
+-rw-rw-rw-   0        0        0      508 2024-04-15 08:53:03.874937 dc_prometheus-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2024-03-16 06:57:52.000000 dc_prometheus-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 08:53:03.859122 dc_prometheus-1.1/dc_prometheus/
+-rw-rw-rw-   0        0        0       39 2023-09-20 04:38:07.000000 dc_prometheus-1.1/dc_prometheus/__init__.py
+-rw-rw-rw-   0        0        0     4065 2024-04-15 08:46:36.000000 dc_prometheus-1.1/dc_prometheus/logcog.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:53:03.873937 dc_prometheus-1.1/dc_prometheus.egg-info/
+-rw-rw-rw-   0        0        0      508 2024-04-15 08:53:03.000000 dc_prometheus-1.1/dc_prometheus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-15 08:53:03.000000 dc_prometheus-1.1/dc_prometheus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:53:03.000000 dc_prometheus-1.1/dc_prometheus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-15 08:53:03.000000 dc_prometheus-1.1/dc_prometheus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 08:53:03.000000 dc_prometheus-1.1/dc_prometheus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:53:03.876937 dc_prometheus-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      773 2024-04-15 08:46:36.000000 dc_prometheus-1.1/setup.py
```

### Comparing `dc_prometheus-1.0/LICENSE` & `dc_prometheus-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dc_prometheus-1.0/dc_prometheus/logcog.py` & `dc_prometheus-1.1/dc_prometheus/logcog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from prometheus_client import start_http_server, Counter, Gauge
 from discord.ext import commands, tasks
-from discord import Interaction, InteractionType, AutoShardedClient , Status
+from discord import Interaction, InteractionType, AutoShardedClient, Status
 import psutil
 import os
 import logging
+
 log = logging.getLogger("prometheus")
 
 """
 需要紀錄的東西:
 1. 群組數量
 2. 成員數量
 3. 指令使用次數
@@ -20,88 +21,101 @@
 guild_count = Gauge("guild_count", "Number of guilds")
 channel_count = Gauge("channel_count", "Number of channels")
 users_count = Gauge("users_count", "Number of users")
 users_online = Gauge("users_online", "Number of users online")
 ping = Gauge("ping", "Ping to discord")
 cpu_usage = Gauge("cpu_usage", "CPU usage")
 ram_usage = Gauge("ram_usage", "RAM usage")
-command_count = Counter("command_count", "Number of commands",["command"])
+command_count = Counter("command_count", "Number of commands", ["command"])
 interaction_count = Counter(
     "interaction_count", "Number of interactions", ["type", "command"]
 )
 all_commands_count = Counter("all_commands_count", "Number of all commands")
-message_count = Counter("message_count", "Number of messages",["guild","user"])
-
+message_count = Counter("message_count", "Number of messages", ["guild", "user"])
 
 
 class logcog(commands.Cog):
-    def __init__(self, bot:commands.Bot,port:int=8000) -> None:
+    def __init__(self, bot: commands.Bot, port: int = 8000) -> None:
+        """
+        Args:
+            bot: discord bot
+            port (int, optional): prometheus server port. Defaults is 8000
+        """
         self.bot = bot
         self.running = False
         self.port = port
 
-    def run_prometheus(self):
+    def run_prometheus(self) -> None:
         try:
             start_http_server(self.port)
         except OSError:
-            log.warning(f"Port {self.port} is already in use, try {self.port+1} instead")
+            log.warning(
+                f"Port {self.port} is already in use, try {self.port+1} instead"
+            )
             self.port += 1
             self.run_prometheus()
+            return
         log.info(f"Prometheus server started on port {self.port}")
         self.running = True
 
-    def sync_all_status(self):
+    def sync_all_status(self) -> None:
         guild_count.set(len(self.bot.guilds))
         channel_count.set(len(list(self.bot.get_all_channels())))
         users_count.set(len(list(self.bot.get_all_members())))
-        users_online.set(len(list(filter(lambda m: m.status != Status.offline, self.bot.get_all_members()))))
+        users_online.set(
+            len(
+                list(
+                    filter(
+                        lambda m: m.status != Status.offline, self.bot.get_all_members()
+                    )
+                )
+            )
+        )
 
     @tasks.loop(seconds=20)
-    async def sync_sys_status(self):
+    async def sync_sys_status(self) -> None:
         ping.set(round(self.bot.latency, 1))
         cpu_usage.set(psutil.cpu_percent(3))
         ram_usage.set(psutil.Process(os.getpid()).memory_percent())
 
     @commands.Cog.listener()
-    async def on_ready(self):
+    async def on_ready(self) -> None:
         self.sync_all_status()
         self.sync_sys_status.start()
         if not self.running:
             self.run_prometheus()
 
     @commands.Cog.listener()
-    async def on_command(self, ctx):
+    async def on_command(self, ctx) -> None:
         command_count.labels(ctx.command.name).inc()
         all_commands_count.inc()
 
     @commands.Cog.listener()
-    async def on_interaction(self, interaction: Interaction):
+    async def on_interaction(self, interaction: Interaction) -> None:
         cmdname = None
         if interaction.type == InteractionType.application_command:
             cmdname = interaction.command.name
-        interaction_count.labels(
-            interaction.type.name, cmdname
-        ).inc()
+        interaction_count.labels(interaction.type.name, cmdname).inc()
         all_commands_count.inc()
 
     @commands.Cog.listener()
-    async def on_message(self, message):
+    async def on_message(self, message) -> None:
         if message.guild:
-            message_count.labels(message.guild.id,message.author.id).inc()
+            message_count.labels(message.guild.id, message.author.id).inc()
         else:
-            message_count.labels(0,message.author.id).inc()
+            message_count.labels(0, message.author.id).inc()
 
     @commands.Cog.listener()
-    async def on_guide_join(self, guild):
+    async def on_guild_join(self, guild) -> None:
         self.sync_all_status()
 
     @commands.Cog.listener()
-    async def on_guide_remove(self, guild):
+    async def on_guild_remove(self, guild) -> None:
         self.sync_all_status()
 
     @commands.Cog.listener()
-    async def on_member_join(self, member):
+    async def on_member_join(self, member) -> None:
         users_count.inc()
 
     @commands.Cog.listener()
-    async def on_member_remove(self, member):
+    async def on_member_remove(self, member) -> None:
         users_count.dec()
```

### Comparing `dc_prometheus-1.0/setup.py` & `dc_prometheus-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dc_prometheus",
-    version="1.0",
+    version="1.1",
     author='phillychi3',
     author_email='phillychi3@gmail.com',
     description='push discord bot data to prometheus',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phillychi3/dc_grafana",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",],
     packages = setuptools.find_packages(where="."),
     package_dir = {"":"."},
     python_requires=">=3.7",
     install_requires=["prometheus_client",]
-)
+)
```

