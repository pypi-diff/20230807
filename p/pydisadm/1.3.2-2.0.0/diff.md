# Comparing `tmp/pydisadm-1.3.2.tar.gz` & `tmp/pydisadm-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.3.2.tar", max compression
+gzip compressed data, was "pydisadm-2.0.0.tar", max compression
```

## Comparing `pydisadm-1.3.2.tar` & `pydisadm-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,34 @@
--rw-r--r--   0        0        0     2936 2023-07-03 15:50:19.086236 pydisadm-1.3.2/README.md
--rw-r--r--   0        0        0      111 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/__init__.py
--rw-r--r--   0        0        0     1130 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/__main__.py
--rw-r--r--   0        0        0     1540 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     7714 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0     2649 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/bot/update_adm_modal.py
--rw-r--r--   0        0        0      702 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/bot/utils.py
--rw-r--r--   0        0        0     1535 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/configuration.py
--rw-r--r--   0        0        0     8044 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0        0 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/data/__init__.py
--rw-r--r--   0        0        0   368313 2023-07-03 15:50:19.086236 pydisadm-1.3.2/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-07-03 15:50:19.090237 pydisadm-1.3.2/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      607 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0     1085 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0     1294 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     3814 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/services/database.py
--rw-r--r--   0        0        0     1543 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/services/esi.py
--rw-r--r--   0        0        0      484 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/utils/adm_utils.py
--rw-r--r--   0        0        0      472 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      623 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      193 2023-07-03 15:50:19.106237 pydisadm-1.3.2/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      953 2023-07-03 15:50:46.794593 pydisadm-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 pydisadm-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3763 2023-08-07 04:45:06.181514 pydisadm-2.0.0/README.md
+-rw-r--r--   0        0        0      142 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1232 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/__init__.py
+-rw-r--r--   0        0        0     1546 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     7747 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0     2649 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/update_adm_modal.py
+-rw-r--r--   0        0        0      702 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0     2388 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/configuration.py
+-rw-r--r--   0        0        0        0 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/controller/__init__.py
+-rw-r--r--   0        0        0     8071 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 04:45:06.181514 pydisadm-2.0.0/pydisadm/data/__init__.py
+-rw-r--r--   0        0        0   368313 2023-08-07 04:45:06.185514 pydisadm-2.0.0/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-08-07 04:45:06.185514 pydisadm-2.0.0/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0        0 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/loader/__init__.py
+-rw-r--r--   0        0        0      607 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0        0 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/runnable/__init__.py
+-rw-r--r--   0        0        0     1330 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0        0 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/__init__.py
+-rw-r--r--   0        0        0      896 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/common.py
+-rw-r--r--   0        0        0     1137 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/database.py
+-rw-r--r--   0        0        0     3520 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/database_mysql.py
+-rw-r--r--   0        0        0     3152 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/database_sqlite.py
+-rw-r--r--   0        0        0     1543 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      580 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/services/factory.py
+-rw-r--r--   0        0        0        0 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/__init__.py
+-rw-r--r--   0        0        0      484 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/adm_utils.py
+-rw-r--r--   0        0        0      472 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-08-07 04:45:06.201514 pydisadm-2.0.0/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      999 2023-08-07 04:45:37.409736 pydisadm-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4757 1970-01-01 00:00:00.000000 pydisadm-2.0.0/PKG-INFO
```

### Comparing `pydisadm-1.3.2/README.md` & `pydisadm-2.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -7,19 +7,28 @@
 
 This is a discord bot which will collect alliance system ADM's daily and provide commands to display them in a convenient tier list.
 
 ## ⚡ Quick Start
 
 ### From PyPI
 ```shell
-# 1. Set up environment
+# 1. Set up environment (pick option)
+
+# 1.1 With exported variables:
 export DISCORD_TOKEN=your-token-here
 export DISCORD_CHANNEL=your-channel-here
+export DISCORD_GUILD_ID=your-guild-id
 export DISCORD_APP_ID=your-app-id-here
 export ALLIANCE_ID=your-alliance-id-here
+export DB_SERVICE=sqlite
+export DB_CONNECTION_STRING=adm-data.sqlite
+export DB_KEEP_ADM_DAYS=7
+
+# 1.2 With .env file:
+cp .env.example .env
 
 # 2. Install package from PyPI
 pip install pydisadm
 
 # 3. Run Bot
 python -m pydisadm
 ```
@@ -41,27 +50,38 @@
 ```
 
 ## 📃 Commands
 
 - `/adm summary` - send a summary of ADM's
 - `/adm csv` - send a csv of ADM's
 - `/adm history <name>` - send a graph showing system, constellation, or region ADM over time
-- `/adm refresh` - manually refresh the data
 - `/adm update <system>` - manually update ADM for system
 - `/adm recommend` - recommend a system to raise ADM in
 
+### Maintenace
+- `/adm refresh` - manually refresh the data
+- `!adm_sync_commands` - synchronise the interactive discord commands (only required once)
+
 ## 🔧 Configuration
 Configuration is done using environment variables or `dotenv`. See `.env.example` for example configuration.
 
 - `DISCORD_TOKEN` - the token bot should use when communicating with discord.
 - `DISCORD_CHANNEL` - the channel name bot should listen too, if this is empty the bot will listen to all channels.
+- `DISCORD_GUILD_ID` - the discord server bot should be part of
 - `DISCORD_APP_ID` - the bot application ID
 - `ALLIANCE_ID` - the alliance ID for collecting ADM values, only systems owned by this alliance will be collected.
+- `DB_SERVICE` - which database to use, can be: sqlite or mysql
+- `DB_CONNECTION_STRING` - the connection string
 - `DB_KEEP_ADM_DAYS` - how many days adm history should be kept in database (default 7).
 
+### DB_CONNECTION_STRING examples
+- `sqlite` - `adm-data.sqlite` a file name
+- `mysql` - `root:root@127.0.0.1:3600/pydisadm` - a connection string (user:password@host:port/database). See [mysqlclient](https://docs.sqlalchemy.org/en/20/dialects/mysql.html#module-sqlalchemy.dialects.mysql.mysqldb) for more information
+
+
 ## 🔍 Caveats
 * The ADM data from ESI is only updated once a day, so refreshing more often than that is not necessary.
 * The database will continue to fill up with historic entries, manually inspect size and purge older entries if it's too big.
 
 ## 🚧 Development
 
 ### Environment
```

### Comparing `pydisadm-1.3.2/pydisadm/__main__.py` & `pydisadm-2.0.0/pydisadm/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,49 @@
+"""pydisadm discord adm bot"""
 #!/usr/bin/env python
 
 import signal
 import sys
 import threading
 
 from dotenv import load_dotenv
 
 from pydisadm.bot.adm_bot import AdmBot
 from pydisadm.configuration import Configuration
 from pydisadm.controller.adm_controller import AdmController
 from pydisadm.loader.static_data import update_static_data
 from pydisadm.runnable.runnable_refresh import run_auto_refresh
-from pydisadm.services.database import Database
+from pydisadm.services.factory import create_database
 
 interrupt_event = threading.Event()
 
-def signal_handler(_1, _2):
+def _signal_handler(_1, _2):
     print('Interrupted by CTRL+C')
     interrupt_event.set()
     sys.exit(0)
 
 
 def main() -> int:
+    """Application main entrypoint"""
     load_dotenv(verbose=True)
 
-    signal.signal(signal.SIGINT, signal_handler)
+    signal.signal(signal.SIGINT, _signal_handler)
 
     run_auto_refresh(interrupt_event)
 
     configuration = Configuration()
 
-    database = Database()
+    database = create_database(configuration)
 
     update_static_data(database)
 
     controller = AdmController(configuration, database)
-    
+
     controller.update_adm_data()
-    controller.purge_adm_records(configuration.db_keep_adm_days)
+    controller.purge_adm_records(configuration.database['keep_adm_days'])
 
     bot = AdmBot(configuration, controller)
     bot.setup_cogs()
     bot.run()
 
     interrupt_event.set()
```

### Comparing `pydisadm-1.3.2/pydisadm/bot/adm_bot.py` & `pydisadm-2.0.0/pydisadm/bot/adm_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def __init__(self, configuration: Configuration, controller: AdmController):
         self.configuration = configuration
         self.controller = controller
 
         intents = create_intents()
         self.bot = commands.Bot(
-            application_id=configuration.discord_app_id,
+            application_id=configuration.discord['app_id'],
             command_prefix='!',
             intents=intents,
             help_command=None
         )
 
     async def setup_cogs_async(self):
         """Asynchronously setup cogs"""
@@ -43,8 +43,8 @@
 
     def sync_commands(self):
         """Synchronize command tree"""
         return asyncio.run(self.sync_commands_async())
 
     def run(self):
         """Run the bot, this function is blocking"""
-        self.bot.run(self.configuration.discord_token)
+        self.bot.run(self.configuration.discord['token'])
```

### Comparing `pydisadm-1.3.2/pydisadm/bot/adm_cog.py` & `pydisadm-2.0.0/pydisadm/bot/adm_cog.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             await interaction.followup.send(f"Couldn't update ADM for {system_name} to {adm}")
         else:
             await interaction.followup.send(f"Manually updated {system_name} ADM to {adm}")
 
     @app_commands.command(description='Recommend where to raise ADM')
     async def recommend(self, interaction: discord.Interaction):
         """Command recommending which system to raise ADMs"""
-        if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
+        if not check_allowed_channel(interaction.channel, self.configuration.discord['channel']):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await interaction.response.defer()
 
         recommended_system = self.controller.get_recommended_system()
 
@@ -80,72 +80,73 @@
         region = recommended_system['regionName']
 
         await interaction.followup.send(f'🦀 `{system} in {region}`', tts=True)
 
     @app_commands.command(description='Posts a summary of all system ADM levels')
     async def summary(self, interaction: discord.Interaction):
         """Command posting a summary of ADMs"""
-        if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
+        if not check_allowed_channel(interaction.channel, self.configuration.discord['channel']):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await self.send_tier_list_summary(interaction)
 
     @app_commands.command(description='Posts a CSV file of all system ADM levels')
     async def csv(self, interaction: discord.Interaction):
         """Command posting a CSV file of ADMs"""
-        if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
+        if not check_allowed_channel(interaction.channel, self.configuration.discord['channel']):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await interaction.response.defer(thinking=True)
 
         file_name = "adm_summary.csv"
         if self.controller.create_spreadsheet(file_name):
             await interaction.followup.send(file=discord.File(file_name), content='ADM Spreadsheet')
             self.controller.delete_file(file_name)
 
     @app_commands.command(description='Post a graph of system ADM.')
     @app_commands.describe(where='The system, constellation, or region to graph.')
     async def history(self, interaction: discord.Interaction, where: str):
         """Command posting a graph of ADM history"""
-        if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
+        if not check_allowed_channel(interaction.channel, self.configuration.discord['channel']):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await self.send_system_graph(interaction, where)
 
     @app_commands.command(description='Manually refresh all ADM data.')
     async def refresh(self, interaction: discord.Interaction):
         """Command to manually refresh ADM data"""
-        if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
+        if not check_allowed_channel(interaction.channel, self.configuration.discord['channel']):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await interaction.response.defer(thinking=True)
         self.controller.update_adm_data()
         await interaction.followup.send("ADM data manually refreshed 🦀")
 
     @app_commands.command(description='Manually update ADM of system.')
     @app_commands.describe(system_name='Which system to update ADM')
     async def update(self, interaction: discord.Interaction, system_name: str):
         """Command to manually update ADM for system"""
-        if not check_allowed_channel(interaction.channel, self.configuration.discord_channel):
+        if not check_allowed_channel(interaction.channel, self.configuration.discord['channel']):
             await interaction.response.send_message('Not allowed in this channel.', ephemeral=True)
             return
 
         await interaction.response.send_modal(UpdateAdmModal(system_name, self.controller))
 
     @commands.Cog.listener()
     async def on_ready(self):
         """cog on_ready event callback"""
         channels = text_channels_with_send_permission(self.bot)
 
         valid_channels = [
-            channel for channel in channels if channel.name == self.configuration.discord_channel]
+            channel for channel in channels if channel.name == self.configuration.discord['channel']
+        ]
 
         embed = discord.Embed(title=f'🦀 ADM Bot v{pydisadm.__version__}')
         embed.add_field(name='Summary', value='/adm summary')
         embed.add_field(name='CSV', value='/adm csv')
         embed.add_field(name='History', value='/adm history <name>')
         embed.add_field(name='Update', value='/adm update <system>')
         embed.add_field(name='Recommend', value='/adm recommend')
@@ -156,14 +157,14 @@
             await channel.send(embed=embed)
 
     @commands.command(pass_context=True)
     async def adm_sync_commands(self, ctx: Context):
         """synchronize slash commands"""
 
         if self.configuration.discord_guild_id:
-            guild = discord.Object(id=self.configuration.discord_guild_id)
+            guild = discord.Object(id=self.configuration.discord['guild_id'])
             self.bot.tree.copy_global_to(guild=guild)
             await self.bot.tree.sync(guild=guild)
         else:
             await self.bot.tree.sync()
 
         await ctx.send('Synchronized bot commands.')
```

### Comparing `pydisadm-1.3.2/pydisadm/bot/update_adm_modal.py` & `pydisadm-2.0.0/pydisadm/bot/update_adm_modal.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.2/pydisadm/bot/utils.py` & `pydisadm-2.0.0/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.2/pydisadm/controller/adm_controller.py` & `pydisadm-2.0.0/pydisadm/controller/adm_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Controller implementation for ADM operations"""
 import os
 import numpy as np
 import pandas as pd
 from tabulate import tabulate
 
 from pydisadm.configuration import Configuration
-from pydisadm.services.database import Database
+from pydisadm.services.database_sqlite import DatabaseSqlite
 from pydisadm.services.esi import sovereignty_structures
 from pydisadm.utils.adm_utils import adm_from_index
 from pydisadm.utils.plot_utils import plot_adm_history_of_systems, plot_save_to_file
 
 
 class AdmController:
     """Controller implementation for ADM operations"""
 
-    def __init__(self, configuration: Configuration, database: Database):
+    def __init__(self, configuration: Configuration, database: DatabaseSqlite):
         self.configuration = configuration
         self.database = database
 
     def generate_tier_list(self):
         """Generate a system tier list based on tier values"""
         system_adms = self.database.select_systems()
 
@@ -54,15 +54,15 @@
         ]
 
         table = tabulate(sorted_summary, showindex=False, headers='keys',
                          tablefmt='fancy_grid', numalign='left', stralign='center')
 
         generated_at = self.database.select_most_recent_row()
 
-        return (table, generated_at['created_at'][0])
+        return (table, str(generated_at['created_at'][0]))
 
     def create_history_graph(self, name, file_name):
         """Generate an ADM history graph and save to file"""
         systems_by_name = self.database.select_system_by_name(name)
 
         if plot_adm_history_of_systems(systems_by_name):
             plot_save_to_file('ADM History', file_name)
@@ -196,15 +196,15 @@
         systems = self.database.select_systems()
         systems.sort_values(by='adm', inplace=True, ascending=True)
 
         return systems.iloc[0]
 
     def update_adm_data(self):
         """Update ADM data"""
-        alliance_id = self.configuration.alliance_id
+        alliance_id = self.configuration.alliance['id']
         system_adms = self.get_system_adms(alliance_id)
 
         self.database.insert_systems(system_adms)
 
     def purge_adm_records(self, days_old: int):
         """Purge adm records more than days_old days old"""
```

### Comparing `pydisadm-1.3.2/pydisadm/data/mapConstellations.csv` & `pydisadm-2.0.0/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.2/pydisadm/data/mapRegions.csv` & `pydisadm-2.0.0/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.2/pydisadm/data/mapSolarSystems.csv` & `pydisadm-2.0.0/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.2/pydisadm/loader/datasets.py` & `pydisadm-2.0.0/pydisadm/loader/datasets.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.2/pydisadm/loader/static_data.py` & `pydisadm-2.0.0/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.2/pydisadm/runnable/runnable_refresh.py` & `pydisadm-2.0.0/pydisadm/runnable/runnable_refresh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Module for running scheduled refresh"""
 import logging
 import schedule
 
 from pydisadm.configuration import Configuration
 from pydisadm.controller.adm_controller import AdmController
-from pydisadm.services.database import Database
+from pydisadm.services.factory import create_database
 from pydisadm.utils.thread_utils import run_threaded
 
 logger = logging.getLogger('adm_auto_refresh')
 
 def scheduler_loop(interrupt_event):
     """Scheduler main loop"""
     configuration = Configuration()
-    database = Database()
+
+    database = create_database(configuration)
 
     controller = AdmController(configuration, database)
 
     schedule.every().day.at('11:30', tz='UTC').do(refresh_job, controller, configuration)
 
     while True:
         schedule.run_pending()
@@ -26,14 +27,14 @@
 def refresh_job(controller: AdmController, configuration: Configuration):
     """Refresh adm data"""
     logger.info('updating adm data...')
     controller.update_adm_data()
     logger.info('adm data update finished')
 
     logger.info('purge old adm data...')
-    controller.purge_adm_records(configuration.db_keep_adm_days)
+    controller.purge_adm_records(configuration.database['keep_adm_days'])
     logger.info('purge finished')
 
 def run_auto_refresh(interrupt_event):
     """Run automatic adm data refresh in separate thread"""
     logger.info('starting adm data update thread')
     run_threaded(lambda: scheduler_loop(interrupt_event))
```

### Comparing `pydisadm-1.3.2/pydisadm/services/database.py` & `pydisadm-2.0.0/pydisadm/services/database_sqlite.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,34 @@
-"""Database service"""
+"""Disk database service"""
 import sqlite3
 import pandas as pd
+from pydisadm.services.common import CREATE_TABLE_ADM, CREATE_TABLE_MAP
 
-class Database:
-    """Database service implementation"""
+from pydisadm.services.database import Database
 
-    def __init__(self):
-        self.conn = sqlite3.connect('adm-data.sqlite')
+class DatabaseSqlite(Database):
+    """Disk database service implementation"""
+
+    def __init__(self, conn_string):
+        if conn_string is None:
+            conn_string = 'adm-data.sqlite'
+
+        self.conn = sqlite3.connect(conn_string)
         self.setup()
 
     def setup(self):
         """Setup database schema"""
         cur = self.conn.cursor()
-        cur.execute("""
-                        CREATE TABLE IF NOT EXISTS systems (
-                            id INTEGER PRIMARY KEY AUTOINCREMENT, 
-                            system_id INTEGER NOT NULL, 
-                            adm REAL NOT NULL, 
-                            tier TEXT NOT NULL,
-                            created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
-                        )
-                    """)
-
-        cur.execute("""
-                        CREATE TABLE IF NOT EXISTS map (
-                            solarSystemID INTEGER PRIMARY KEY NOT NULL, 
-                            constellationID INTEGER NOT NULL, 
-                            regionID INTEGER NOT NULL, 
-                            solarSystemName TEXT NOT NULL,
-                            constellationName TEXT NOT NULL,
-                            regionName TEXT NOT NULL
-                        )
-                    """)
+        cur.execute(CREATE_TABLE_ADM)
+        cur.execute(CREATE_TABLE_MAP)
         self.conn.commit()
 
     def insert_systems(self, systems):
         """Insert system ADM records"""
-        systems.to_sql('systems', self.conn, index=False, if_exists='append')
+        systems.to_sql('adm', self.conn, index=False, if_exists='append')
 
         self.conn.commit()
 
     def insert_map_data(self, map_data):
         """Insert map data"""
         map_data.to_sql('map', self.conn, index=True, if_exists='replace')
 
@@ -49,46 +37,46 @@
     def select_system_with_name(self, system_name) -> pd.DataFrame:
         """Select system matching name"""
         return pd.read_sql_query("SELECT * FROM map WHERE solarSystemName = ?",
                                  self.conn, params=[system_name])
 
     def select_most_recent_row(self) -> pd.DataFrame:
         """Select the most recent ADM record"""
-        return pd.read_sql_query("SELECT created_at FROM systems ORDER BY created_at DESC LIMIT 1",
+        return pd.read_sql_query("SELECT created_at FROM adm ORDER BY created_at DESC LIMIT 1",
                                  self.conn)
 
     def select_systems(self) -> pd.DataFrame:
         """Select most recent record of all systems"""
         return pd.read_sql_query("""
-            SELECT t1.*, t2.solarSystemName, t2.constellationName, t2.regionName FROM systems t1 
+            SELECT t1.*, t2.solarSystemName, t2.constellationName, t2.regionName FROM adm t1 
             LEFT JOIN map t2 ON t1.system_id = t2.solarSystemID 
-            WHERE t1.created_at = (SELECT MAX(t3.created_at) FROM systems t3 WHERE t3.system_id = t1.system_id);
+            WHERE t1.created_at = (SELECT MAX(t3.created_at) FROM adm t3 WHERE t3.system_id = t1.system_id);
         """, self.conn)
 
     def select_system_by_name(self, name) -> pd.DataFrame:
         """Select systems by name"""
         sql = """
-            SELECT map.solarSystemName system_name, adm, tier, created_at FROM systems
-            INNER JOIN map ON map.solarSystemID = systems.system_id
+            SELECT map.solarSystemName system_name, adm, tier, created_at FROM adm
+            INNER JOIN map ON map.solarSystemID = adm.system_id
             WHERE map.solarSystemName=? OR map.constellationName=? OR map.regionName=? ORDER BY created_at
         """
         return pd.read_sql_query(sql, self.conn, params=[name, name, name])
 
     def select_system_history(self, system, limit) -> pd.DataFrame:
         """Select history of a single system"""
         return pd.read_sql_query("""
-            SELECT system_id, adm, tier, created_at FROM systems
-            INNER JOIN map ON map.solarSystemID = systems.system_id
+            SELECT system_id, adm, tier, created_at FROM adm
+            INNER JOIN map ON map.solarSystemID = adm.system_id
             WHERE map.solarSystemName=? ORDER BY created_at DESC LIMIT ?
         """, self.conn, params=[system, limit])
 
     def delete_system_rows(self, days_old):
         """Delete system rows older than days_old"""
         cur = self.conn.cursor()
         cur.execute(f"""
-            DELETE FROM systems 
+            DELETE FROM adm 
             WHERE id IN (
-                SELECT id FROM systems WHERE created_at < (select datetime('now', '-{days_old} day'))
+                SELECT id FROM adm WHERE created_at < (select datetime('now', '-{days_old} day'))
             )
         """)
 
         self.conn.commit()
```

### Comparing `pydisadm-1.3.2/pydisadm/services/esi.py` & `pydisadm-2.0.0/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.2/pydisadm/utils/plot_utils.py` & `pydisadm-2.0.0/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.3.2/pyproject.toml` & `pydisadm-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.3.2"
+version = "2.0.0"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
 
@@ -13,14 +13,16 @@
 schedule = "^1.2.0"
 requests = "^2.30.0"
 discord = "^2.2.3"
 python-dotenv = "^1.0.0"
 pandas = "^2.0.1"
 tabulate = "^0.9.0"
 matplotlib = "^3.7.1"
+sqlalchemy = "^2.0.19"
+mysqlclient = "^2.2.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.4"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
```

### Comparing `pydisadm-1.3.2/PKG-INFO` & `pydisadm-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.3.2
+Version: 2.0.0
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: discord (>=2.2.3,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: mysqlclient (>=2.2.0,<3.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: schedule (>=1.2.0,<2.0.0)
+Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/agelito/adm-bot
 Description-Content-Type: text/markdown
 
 # EVE ADM Bot
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/agelito/adm-bot/ci-cd.yml)](https://github.com/agelito/adm-bot/actions/workflows/ci-cd.yml)
@@ -31,19 +33,28 @@
 
 This is a discord bot which will collect alliance system ADM's daily and provide commands to display them in a convenient tier list.
 
 ## ⚡ Quick Start
 
 ### From PyPI
 ```shell
-# 1. Set up environment
+# 1. Set up environment (pick option)
+
+# 1.1 With exported variables:
 export DISCORD_TOKEN=your-token-here
 export DISCORD_CHANNEL=your-channel-here
+export DISCORD_GUILD_ID=your-guild-id
 export DISCORD_APP_ID=your-app-id-here
 export ALLIANCE_ID=your-alliance-id-here
+export DB_SERVICE=sqlite
+export DB_CONNECTION_STRING=adm-data.sqlite
+export DB_KEEP_ADM_DAYS=7
+
+# 1.2 With .env file:
+cp .env.example .env
 
 # 2. Install package from PyPI
 pip install pydisadm
 
 # 3. Run Bot
 python -m pydisadm
 ```
@@ -65,27 +76,38 @@
 ```
 
 ## 📃 Commands
 
 - `/adm summary` - send a summary of ADM's
 - `/adm csv` - send a csv of ADM's
 - `/adm history <name>` - send a graph showing system, constellation, or region ADM over time
-- `/adm refresh` - manually refresh the data
 - `/adm update <system>` - manually update ADM for system
 - `/adm recommend` - recommend a system to raise ADM in
 
+### Maintenace
+- `/adm refresh` - manually refresh the data
+- `!adm_sync_commands` - synchronise the interactive discord commands (only required once)
+
 ## 🔧 Configuration
 Configuration is done using environment variables or `dotenv`. See `.env.example` for example configuration.
 
 - `DISCORD_TOKEN` - the token bot should use when communicating with discord.
 - `DISCORD_CHANNEL` - the channel name bot should listen too, if this is empty the bot will listen to all channels.
+- `DISCORD_GUILD_ID` - the discord server bot should be part of
 - `DISCORD_APP_ID` - the bot application ID
 - `ALLIANCE_ID` - the alliance ID for collecting ADM values, only systems owned by this alliance will be collected.
+- `DB_SERVICE` - which database to use, can be: sqlite or mysql
+- `DB_CONNECTION_STRING` - the connection string
 - `DB_KEEP_ADM_DAYS` - how many days adm history should be kept in database (default 7).
 
+### DB_CONNECTION_STRING examples
+- `sqlite` - `adm-data.sqlite` a file name
+- `mysql` - `root:root@127.0.0.1:3600/pydisadm` - a connection string (user:password@host:port/database). See [mysqlclient](https://docs.sqlalchemy.org/en/20/dialects/mysql.html#module-sqlalchemy.dialects.mysql.mysqldb) for more information
+
+
 ## 🔍 Caveats
 * The ADM data from ESI is only updated once a day, so refreshing more often than that is not necessary.
 * The database will continue to fill up with historic entries, manually inspect size and purge older entries if it's too big.
 
 ## 🚧 Development
 
 ### Environment
```

