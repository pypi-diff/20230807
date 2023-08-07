# Comparing `tmp/aa_incursions-0.1.0a0.tar.gz` & `tmp/aa_incursions-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_incursions-0.1.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_incursions-0.2.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_incursions-0.1.0a0.tar` & `aa_incursions-0.2.0a0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/LICENSE
--rw-r--r--   0        0        0     2372 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/README.md
--rw-r--r--   0        0        0       85 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/incursions/__init__.py
--rw-r--r--   0        0        0      562 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/incursions/admin.py
--rw-r--r--   0        0        0      289 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/incursions/app_settings.py
--rw-r--r--   0        0        0      299 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/incursions/apps.py
--rw-r--r--   0        0        0      133 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/incursions/auth_hooks.py
--rw-r--r--   0        0        0     3428 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/incursions/cogs/incursions.py
--rw-r--r--   0        0        0     8651 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/incursions/helpers.py
--rw-r--r--   0        0        0     4033 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/incursions/migrations/0001_initial.py
--rw-r--r--   0        0        0     1944 2023-08-02 07:16:09.133737 aa_incursions-0.1.0a0/incursions/migrations/0002_remove_incursion_influence_and_more.py
--rw-r--r--   0        0        0        0 2023-08-02 07:16:09.158737 aa_incursions-0.1.0a0/incursions/migrations/__init__.py
--rw-r--r--   0        0        0     5899 2023-08-02 07:16:09.134737 aa_incursions-0.1.0a0/incursions/models.py
--rw-r--r--   0        0        0      795 2023-08-02 07:16:09.134737 aa_incursions-0.1.0a0/incursions/providers.py
--rw-r--r--   0        0        0     1177 2023-08-02 07:16:09.134737 aa_incursions-0.1.0a0/incursions/signals.py
--rw-r--r--   0        0        0    84246 2023-08-02 07:16:09.134737 aa_incursions-0.1.0a0/incursions/static_data.py
--rw-r--r--   0        0        0   881823 2023-08-02 07:16:09.136737 aa_incursions-0.1.0a0/incursions/swagger.json
--rw-r--r--   0        0        0     4785 2023-08-02 07:16:09.136737 aa_incursions-0.1.0a0/incursions/tasks.py
--rw-r--r--   0        0        0     1912 2023-08-02 07:16:09.136737 aa_incursions-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 aa_incursions-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-07 02:44:45.550335 aa_incursions-0.2.0a0/LICENSE
+-rw-r--r--   0        0        0     2526 2023-08-07 02:44:45.550335 aa_incursions-0.2.0a0/README.md
+-rw-r--r--   0        0        0       85 2023-08-07 02:44:45.550335 aa_incursions-0.2.0a0/incursions/__init__.py
+-rw-r--r--   0        0        0      923 2023-08-07 02:44:45.550335 aa_incursions-0.2.0a0/incursions/admin.py
+-rw-r--r--   0        0        0      289 2023-08-07 02:44:45.550335 aa_incursions-0.2.0a0/incursions/app_settings.py
+-rw-r--r--   0        0        0      299 2023-08-07 02:44:45.550335 aa_incursions-0.2.0a0/incursions/apps.py
+-rw-r--r--   0        0        0      133 2023-08-07 02:44:45.550335 aa_incursions-0.2.0a0/incursions/auth_hooks.py
+-rw-r--r--   0        0        0     4775 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/cogs/incursions.py
+-rw-r--r--   0        0        0     8658 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/helpers.py
+-rw-r--r--   0        0        0     4033 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1944 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/migrations/0002_remove_incursion_influence_and_more.py
+-rw-r--r--   0        0        0      831 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/migrations/0003_focus.py
+-rw-r--r--   0        0        0      523 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/migrations/0004_alter_focus_incursion.py
+-rw-r--r--   0        0        0        0 2023-08-07 02:44:45.575335 aa_incursions-0.2.0a0/incursions/migrations/__init__.py
+-rw-r--r--   0        0        0     6376 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/models.py
+-rw-r--r--   0        0        0      795 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/providers.py
+-rw-r--r--   0        0        0     1177 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/signals.py
+-rw-r--r--   0        0        0    84246 2023-08-07 02:44:45.551335 aa_incursions-0.2.0a0/incursions/static_data.py
+-rw-r--r--   0        0        0   881823 2023-08-07 02:44:45.553335 aa_incursions-0.2.0a0/incursions/swagger.json
+-rw-r--r--   0        0        0     4785 2023-08-07 02:44:45.554335 aa_incursions-0.2.0a0/incursions/tasks.py
+-rw-r--r--   0        0        0     1912 2023-08-07 02:44:45.554335 aa_incursions-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3914 1970-01-01 00:00:00.000000 aa_incursions-0.2.0a0/PKG-INFO
```

### Comparing `aa_incursions-0.1.0a0/LICENSE` & `aa_incursions-0.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.1.0a0/README.md` & `aa_incursions-0.2.0a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -42,17 +42,19 @@
 Configure your Auth settings (`local.py`) as follows:
 
 - Add `'incursions'` to `INSTALLED_APPS`
 - Add below lines to your settings file:
 
 ```python
 ## Settings for AA-Incursions
-CELERYBEAT_SCHEDULE['update_incursions'] = {
+# Route is Cached for 300 Seconds, if you aren't riding the Kundalini Manifest to the last minute
+# Feel free to adjust this to minute='*/5'
+CELERYBEAT_SCHEDULE['incursions_update_incursions'] = {
     'task': 'incursions.tasks.update_incursions',
-    'schedule': crontab(minute=*/1, hour='*'),
+    'schedule': crontab(minute='*/1', hour='*'),
 }
 ```
 
 ### Step 4 - Maintain Alliance Auth
 
 - Run migrations `python manage.py migrate`
 - Gather your staticfiles `python manage.py collectstatic`
```

### Comparing `aa_incursions-0.1.0a0/incursions/cogs/incursions.py` & `aa_incursions-0.2.0a0/incursions/cogs/incursions.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from discord.embeds import Embed
 from discord.ext import commands
 from eveuniverse.models import EveConstellation, EveRegion, EveSolarSystem
 
 from django.conf import settings
 
 from incursions import __version__
-from incursions.models import Incursion
+from incursions.models import Focus, Incursion
 
 logger = logging.getLogger(__name__)
 
 
 class Incursions(commands.Cog):
     """
     Drifter Wormhole Mapping and Management
@@ -31,16 +31,16 @@
 
     async def search_constellations(self, ctx: AutocompleteContext):
         return list(EveConstellation.objects.filter(name__icontains=ctx.value).values_list('name', flat=True)[:10])
 
     async def search_regions(self, ctx: AutocompleteContext):
         return list(EveRegion.objects.filter(name__icontains=ctx.value).values_list('name', flat=True)[:10])
 
-    async def search_incursion(self, ctx: AutocompleteContext):
-        return list(Incursion.objects.filter(name__icontains=ctx.value).values_list('name', flat=True)[:10])
+    async def search_incursion_active(self, ctx: AutocompleteContext):
+        return list(Incursion.objects.exclude(state=Incursion.States.ENDED).filter(constellation__name__icontains=ctx.value).values_list('constellation__name', flat=True)[:10])
 
     @incursion_commands.command(name="about", description="About the Incursion Bot", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     async def about(self, ctx):
         """
         All about the bot
         """
         embed = Embed(title="AA Incursions")
@@ -54,34 +54,57 @@
         )
 
         return await ctx.respond(embed=embed)
 
     @incursion_commands.command(name="focus", description="Get information on the current focus", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     async def focus(
         self, ctx,
-        constellation=Option(str, "Constellation", autocomplete=search_constellations),
     ):
-        return await ctx.respond("Not Yet Implemented")
+        incursion_obj = Focus.get_solo().incursion
+        incursion_detail_string = f"""
+            {incursion_obj.constellation.name} ({incursion_obj.state})
+            Established: {incursion_obj.established_timestamp}
+            Mobilized: {incursion_obj.mobilizing_timestamp}
+            Withdrawing:{incursion_obj.withdrawing_timestamp}
+            Boss Spotted: {incursion_obj.has_boss}
+            Influence: {incursion_obj.influence}
+            """
+        return await ctx.respond(incursion_detail_string)
 
     @incursion_commands.command(name="set_focus", description="Set the current Focus", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     async def focus_set(
         self, ctx,
-        constellation=Option(str, "Constellation", autocomplete=search_constellations),
+        incursion=Option(str, "Constellation", autocomplete=search_incursion_active),
     ):
-        return await ctx.respond("Not Yet Implemented")
+        focus = Focus.get_solo()
+        focus.incursion_id = Incursion.objects.exclude(state=Incursion.States.ENDED).get(constellation__name__icontains=incursion)
+        focus.save()
+        return await ctx.respond("Focus Set")
 
     @incursion_commands.command(name="incursions", description="List active incursions", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     async def incursions(
         self, ctx,
     ):
-        return await ctx.respond("Not Yet Implemented")
+        incursion_string = ""
+        for incursion in Incursion.objects.exclude(state=Incursion.States.ENDED):
+            incursion_string += f"\n{incursion.constellation.name}"
+        return await ctx.respond(incursion_string)
 
     @incursion_commands.command(name="incursion_detail", description="Status of a specific incursion", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     async def incursion_detail(
         self, ctx,
-        incursion=Option(str, "Constellation", autocomplete=search_constellations),
+        incursion=Option(str, "Constellation", autocomplete=search_incursion_active),
     ):
-        return await ctx.respond("Not Yet Implemented")
+        incursion_obj = Incursion.objects.exclude(state=Incursion.States.ENDED).get(constellation__name__icontains=incursion)
+        incursion_detail_string = f"""
+            {incursion_obj.constellation.name} ({incursion_obj.state})
+            Established: {incursion_obj.established_timestamp}
+            Mobilized: {incursion_obj.mobilizing_timestamp}
+            Withdrawing:{incursion_obj.withdrawing_timestamp}
+            Boss Spotted: {incursion_obj.has_boss}
+            Influence: {incursion_obj.influence}
+            """
+        return await ctx.respond(incursion_detail_string)
 
 
 def setup(bot):
     bot.add_cog(Incursions(bot))
```

### Comparing `aa_incursions-0.1.0a0/incursions/helpers.py` & `aa_incursions-0.2.0a0/incursions/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,27 +81,27 @@
 
 
 def embed_mobilizing(incursion: Incursion) -> Embed:
     embed = embed_base()
     embed.colour = Colour.yellow()
     embed.title = f"Mobilizing {incursion.security_string}: {incursion.constellation.name}"
     embed.add_field(name="Estimated Withdrawing Time",
-                    value=f"<t:{ int((incursion.established_timestamp + timedelta(days=2)).timestamp()) }:R>", inline=False)
+                    value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=2)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Estimated Despawn Time",
-                    value=f"<t:{ int((incursion.established_timestamp + timedelta(days=3)).timestamp()) }:R>", inline=False)
+                    value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=3)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Max Spawn Stats",
                     value=f'''
                         {incursion.mobilizing_timestamp - incursion.established_timestamp}
-                        {(incursion.mobilizing_timestamp - incursion.established_timestamp)+ timedelta(days=5)} Unused
-                        {(incursion.mobilizing_timestamp - incursion.established_timestamp) / timedelta(days=5)}% total possible `established` time used")
+                        {(incursion.mobilizing_timestamp - incursion.established_timestamp) - timedelta(days=5)} Unused
+                        {(incursion.mobilizing_timestamp - incursion.established_timestamp) / timedelta(days=5) - 100:.3f}% total possible `established` time used")
                     ''')
     embed.add_field(name="Estimated Respawn Window Opens",
-                    value=f"<t:{ int((incursion.established_timestamp + timedelta(days=3, hours=12)).timestamp()) }:R>", inline=False)
+                    value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=3, hours=12)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Estimated Respawn Window Closes",
-                    value=f"<t:{ int((incursion.established_timestamp + timedelta(days=3, hours=36)).timestamp()) }:R>", inline=False)
+                    value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=3, hours=36)).timestamp()) }:R>", inline=False)
     return embed
 
     # Spawn Mobilizing!
     # Estimated Withdrawing Time
     # Friday, 23 June 2023 21:37 (in a day)
     # Estimated Despawn Time
     # Saturday, 24 June 2023 21:37 (in 2 days)
@@ -117,19 +117,19 @@
 
 
 def embed_withdrawing(incursion: Incursion) -> Embed:
     embed = embed_base()
     embed.colour = Colour.red()
     embed.title = f"Withdrawing {incursion.security_string}: {incursion.constellation.name}"
     embed.add_field(name="Despawn Before",
-                    value=f"<t:{ int((incursion.established_timestamp + timedelta(days=1)).timestamp()) }:R>", inline=False)
+                    value=f"<t:{ int((incursion.withdrawing_timestamp + timedelta(days=1)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Estimated Respawn Window Opens",
-                    value=f"<t:{ int((incursion.established_timestamp + timedelta(days=1, hours=12)).timestamp()) }:R>", inline=False)
+                    value=f"<t:{ int((incursion.withdrawing_timestamp + timedelta(days=1, hours=12)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Estimated Respawn Window Closes",
-                    value=f"<t:{ int((incursion.established_timestamp + timedelta(days=1, hours=36)).timestamp()) }:R>", inline=False)
+                    value=f"<t:{ int((incursion.withdrawing_timestamp + timedelta(days=1, hours=36)).timestamp()) }:R>", inline=False)
     return embed
 
     # Spawn Withdrawing!
     # Despawn Before
     # Saturday, 24 June 2023 21:40 (2 days ago)
     # Saturday, June 24, 2023 11:40 (Eve Time)
     # Estimated Respawn Window Opens
```

### Comparing `aa_incursions-0.1.0a0/incursions/migrations/0001_initial.py` & `aa_incursions-0.2.0a0/incursions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.1.0a0/incursions/migrations/0002_remove_incursion_influence_and_more.py` & `aa_incursions-0.2.0a0/incursions/migrations/0002_remove_incursion_influence_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.1.0a0/incursions/models.py` & `aa_incursions-0.2.0a0/incursions/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -150,7 +150,25 @@
     class Meta:
         """
         Meta definitions
         """
         default_permissions = ()
         verbose_name = "AA Incursions Settings"
         verbose_name_plural = "AA Incursions Settings"
+
+
+class Focus(SingletonModel):
+    incursion = models.ForeignKey(Incursion, verbose_name=_("Current Focus"), on_delete=models.CASCADE, blank=True, null=True)
+
+    def __str__(self):
+        try:
+            return f"Current Focus: {self.incursion}"
+        except Exception:
+            return "No Focus Set"
+
+    class Meta:
+        """
+        Meta definitions
+        """
+        default_permissions = ()
+        verbose_name = "Focus"
+        verbose_name_plural = "Focus"
```

### Comparing `aa_incursions-0.1.0a0/incursions/providers.py` & `aa_incursions-0.2.0a0/incursions/providers.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.1.0a0/incursions/signals.py` & `aa_incursions-0.2.0a0/incursions/signals.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.1.0a0/incursions/static_data.py` & `aa_incursions-0.2.0a0/incursions/static_data.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.1.0a0/incursions/swagger.json` & `aa_incursions-0.2.0a0/incursions/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.1.0a0/incursions/tasks.py` & `aa_incursions-0.2.0a0/incursions/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.1.0a0/pyproject.toml` & `aa_incursions-0.2.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.1.0a0/PKG-INFO` & `aa_incursions-0.2.0a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_incursions
-Version: 0.1.0a0
+Version: 0.2.0a0
 Summary: AllianceAuth Incursion Tools
 Keywords: allianceauth,eveonline
 Author-email: Joel Falknau <joel.falknau@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Celery
@@ -74,17 +74,19 @@
 Configure your Auth settings (`local.py`) as follows:
 
 - Add `'incursions'` to `INSTALLED_APPS`
 - Add below lines to your settings file:
 
 ```python
 ## Settings for AA-Incursions
-CELERYBEAT_SCHEDULE['update_incursions'] = {
+# Route is Cached for 300 Seconds, if you aren't riding the Kundalini Manifest to the last minute
+# Feel free to adjust this to minute='*/5'
+CELERYBEAT_SCHEDULE['incursions_update_incursions'] = {
     'task': 'incursions.tasks.update_incursions',
-    'schedule': crontab(minute=*/1, hour='*'),
+    'schedule': crontab(minute='*/1', hour='*'),
 }
 ```
 
 ### Step 4 - Maintain Alliance Auth
 
 - Run migrations `python manage.py migrate`
 - Gather your staticfiles `python manage.py collectstatic`
```

