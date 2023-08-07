# Comparing `tmp/disposable-email-domains-0.0.92.tar.gz` & `tmp/disposable-email-domains-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disposable-email-domains-0.0.92.tar", last modified: Wed Jul 19 03:33:27 2023, max compression
+gzip compressed data, was "disposable-email-domains-0.0.93.tar", last modified: Mon Aug  7 02:36:15 2023, max compression
```

## Comparing `disposable-email-domains-0.0.92.tar` & `disposable-email-domains-0.0.93.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:33:27.427237 disposable-email-domains-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-19 03:33:27.427237 disposable-email-domains-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:33:27.427237 disposable-email-domains-0.0.92/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/bin/check_for_differences
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/bin/parse_source_data
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/bin/prerelease
--rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/bin/release
--rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/bin/update
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:33:27.427237 disposable-email-domains-0.0.92/disposable_email_domains/
--rw-r--r--   0 runner    (1001) docker     (123)    74503 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/disposable_email_domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/disposable_email_domains/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:33:27.427237 disposable-email-domains-0.0.92/disposable_email_domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-19 03:33:27.000000 disposable-email-domains-0.0.92/disposable_email_domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-19 03:33:27.000000 disposable-email-domains-0.0.92/disposable_email_domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:33:27.000000 disposable-email-domains-0.0.92/disposable_email_domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 03:33:27.000000 disposable-email-domains-0.0.92/disposable_email_domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-19 03:33:27.000000 disposable-email-domains-0.0.92/disposable_email_domains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 03:33:27.427237 disposable-email-domains-0.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:33:27.427237 disposable-email-domains-0.0.92/source_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/source_data/allowlist.conf
--rw-r--r--   0 runner    (1001) docker     (123)    46180 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/source_data/disposable_email_blocklist.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:33:27.427237 disposable-email-domains-0.0.92/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/tests/test_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-19 03:33:14.000000 disposable-email-domains-0.0.92/tests/test_blocklist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:36:15.596926 disposable-email-domains-0.0.93/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-07 02:36:15.596926 disposable-email-domains-0.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:36:15.592926 disposable-email-domains-0.0.93/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/bin/check_for_differences
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/bin/parse_source_data
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/bin/prerelease
+-rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/bin/release
+-rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/bin/update
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:36:15.596926 disposable-email-domains-0.0.93/disposable_email_domains/
+-rw-r--r--   0 runner    (1001) docker     (123)    75059 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/disposable_email_domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/disposable_email_domains/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:36:15.596926 disposable-email-domains-0.0.93/disposable_email_domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-07 02:36:15.000000 disposable-email-domains-0.0.93/disposable_email_domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-07 02:36:15.000000 disposable-email-domains-0.0.93/disposable_email_domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 02:36:15.000000 disposable-email-domains-0.0.93/disposable_email_domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 02:36:15.000000 disposable-email-domains-0.0.93/disposable_email_domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 02:36:15.000000 disposable-email-domains-0.0.93/disposable_email_domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-07 02:36:15.596926 disposable-email-domains-0.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:36:15.596926 disposable-email-domains-0.0.93/source_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/source_data/allowlist.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    46529 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/source_data/disposable_email_blocklist.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:36:15.596926 disposable-email-domains-0.0.93/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/tests/test_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-07 02:36:03.000000 disposable-email-domains-0.0.93/tests/test_blocklist.py
```

### Comparing `disposable-email-domains-0.0.92/LICENSE.txt` & `disposable-email-domains-0.0.93/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.92/PKG-INFO` & `disposable-email-domains-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disposable-email-domains
-Version: 0.0.92
+Version: 0.0.93
 Summary: A set of disposable email domains
 Home-page: https://github.com/disposable-email-domains/disposable-email-domains
 Author: Dustin Ingram
 Author-email: github@dustingram.com
 License: MIT
 Keywords: disposable email domains blocklist
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `disposable-email-domains-0.0.92/README.md` & `disposable-email-domains-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.92/bin/check_for_differences` & `disposable-email-domains-0.0.93/bin/check_for_differences`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.92/bin/parse_source_data` & `disposable-email-domains-0.0.93/bin/parse_source_data`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.92/disposable_email_domains/__init__.py` & `disposable-email-domains-0.0.93/disposable_email_domains/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     'internet-e-mail.com',
     'internet-mail.org',
     'internetemails.net',
     'internetmailing.net',
     'jetemail.net',
     'justemail.net',
     'letterboxes.org',
+    'liamekaens.com',
     'mail-central.com',
     'mail-page.com',
     'mail2world.com',
     'mailandftp.com',
     'mailas.com',
     'mailbolt.com',
     'mailc.net',
@@ -145,14 +146,15 @@
     'sent.at',
     'sent.com',
     'shitposting.agency',
     'shitware.nl',
     'sibmail.com',
     'sneakemail.com',
     'snkmail.com',
+    'snkml.com',
     'spamcannon.com',
     'spamcannon.net',
     'spamgourmet.com',
     'spamgourmet.net',
     'spamgourmet.org',
     'speedpost.net',
     'speedymail.org',
@@ -758,14 +760,15 @@
     'chalupaurybnicku.cz',
     'chammy.info',
     'chasefreedomactivate.com',
     'chatich.com',
     'cheaphub.net',
     'cheatmail.de',
     'chenbot.email',
+    'chewydonut.com',
     'chibakenma.ml',
     'chickenkiller.com',
     'chielo.com',
     'childsavetrust.org',
     'chilkat.com',
     'chinamkm.com',
     'chithinh.com',
@@ -1641,14 +1644,15 @@
     'hulapla.de',
     'humaility.com',
     'hungpackage.com',
     'hushmail.cf',
     'huskion.net',
     'hvastudiesucces.nl',
     'hwsye.net',
+    'hypenated-domain.com',
     'i2pmail.org',
     'i6.cloudns.cc',
     'iaoss.com',
     'ibnuh.bz',
     'icantbelieveineedtoexplainthisshit.com',
     'icemail.club',
     'ichigo.me',
@@ -1707,14 +1711,15 @@
     'indomaed.pw',
     'indomina.cf',
     'indoserver.stream',
     'indosukses.press',
     'ineec.net',
     'infocom.zp.ua',
     'inggo.org',
+    'inkiny.com',
     'inkomail.com',
     'inmynetwork.tk',
     'inoutmail.de',
     'inoutmail.eu',
     'inoutmail.info',
     'inoutmail.net',
     'inpwa.com',
@@ -1755,14 +1760,15 @@
     'isosq.com',
     'istii.ro',
     'isukrainestillacountry.com',
     'it7.ovh',
     'italy-mail.com',
     'itcompu.com',
     'itfast.net',
+    'itsjiff.com',
     'itunesgiftcodegenerator.com',
     'iubridge.com',
     'iuemail.men',
     'iwi.net',
     'ixaks.com',
     'ixx.io',
     'j-p.us',
@@ -1849,14 +1855,15 @@
     'kino-100.ru',
     'kiois.com',
     'kismail.ru',
     'kisstwink.com',
     'kitnastar.com',
     'kjkszpjcompany.com',
     'kkmail.be',
+    'kkoup.com',
     'kksm.be',
     'klassmaster.com',
     'klassmaster.net',
     'klick-tipp.us',
     'klipschx12.com',
     'kloap.com',
     'kludgemush.com',
@@ -1942,14 +1949,15 @@
     'liamcyrus.com',
     'lifebyfood.com',
     'lifetimefriends.info',
     'lifetotech.com',
     'ligsb.com',
     'lillemap.net',
     'lilo.me',
+    'lilspam.com',
     'lindenbaumjapan.com',
     'link2mail.net',
     'linkedintuts2016.pw',
     'linshiyouxiang.net',
     'linuxmail.so',
     'litedrop.com',
     'liveradio.tk',
@@ -2034,14 +2042,15 @@
     'mail666.ru',
     'mail7.io',
     'mail707.com',
     'mail72.com',
     'mailapp.top',
     'mailback.com',
     'mailbidon.com',
+    'mailbiscuit.com',
     'mailbiz.biz',
     'mailblocks.com',
     'mailbox.in.ua',
     'mailbox52.ga',
     'mailbox80.biz',
     'mailbox82.biz',
     'mailbox87.de',
@@ -2243,14 +2252,15 @@
     'misterpinball.de',
     'miucce.com',
     'mji.ro',
     'mjj.edu.ge',
     'mjukglass.nu',
     'mkpfilm.com',
     'ml8.ca',
+    'mliok.com',
     'mm.my',
     'mm5.se',
     'mnode.me',
     'moakt.cc',
     'moakt.co',
     'moakt.com',
     'moakt.ws',
@@ -2362,14 +2372,15 @@
     'nada.ltd',
     'nagi.be',
     'nakedtruth.biz',
     'nanonym.ch',
     'naslazhdai.ru',
     'nationalgardeningclub.com',
     'nawmin.info',
+    'naymedia.com',
     'nbzmr.com',
     'negated.com',
     'neko2.net',
     'nekochan.fr',
     'neomailbox.com',
     'neotlozhniy-zaim.ru',
     'nepwk.com',
@@ -2579,14 +2590,15 @@
     'pinehill-seattle.org',
     'pingir.com',
     'pipemail.space',
     'pisls.com',
     'pitaniezdorovie.ru',
     'pivo-bar.ru',
     'pixiil.com',
+    'pizzajunk.com',
     'pjjkp.com',
     'placebomail10.com',
     'pleasenoham.org',
     'plexfirm.com',
     'plexolan.de',
     'plhk.ru',
     'ploae.com',
@@ -2682,14 +2694,15 @@
     'qtum-ico.com',
     'quadrafit.com',
     'quick-mail.cc',
     'quickemail.info',
     'quickinbox.com',
     'quickmail.nl',
     'quicksend.ch',
+    'quipas.com',
     'ququb.com',
     'qvy.me',
     'qwickmail.com',
     'r4nd0m.de',
     'ra3.us',
     'rabin.ca',
     'rabiot.reisen',
@@ -2709,14 +2722,15 @@
     'rbb.org',
     'rcasd.com',
     'rcpt.at',
     'rdklcrv.xyz',
     're-gister.com',
     'reality-concept.club',
     'reallymymail.com',
+    'realquickemail.com',
     'realtyalerts.ca',
     'rebates.stream',
     'receiveee.com',
     'recipeforfailure.com',
     'recode.me',
     'reconmail.com',
     'recyclemail.dk',
@@ -2831,14 +2845,15 @@
     'services391.com',
     'sexforswingers.com',
     'sexical.com',
     'sexyalwasmi.top',
     'shadap.org',
     'shalar.net',
     'sharedmailbox.org',
+    'sharkfaces.com',
     'sharklasers.com',
     'shchiba.uk',
     'sheryli.com',
     'shhmail.com',
     'shhuut.org',
     'shieldedmail.com',
     'shieldemail.com',
@@ -2861,14 +2876,15 @@
     'shut.ws',
     'siberpay.com',
     'sidelka-mytischi.ru',
     'siftportal.ru',
     'sify.com',
     'sika3.com',
     'sikux.com',
+    'silenceofthespam.com',
     'siliwangi.ga',
     'silvercoin.life',
     'sim-simka.ru',
     'simaenaga.com',
     'simpleitsecurity.info',
     'sin.cl',
     'sinaite.net',
@@ -2905,20 +2921,22 @@
     'smarttalent.pw',
     'smashmail.de',
     'smellfear.com',
     'smellrear.com',
     'smellypotato.tk',
     'smtp99.com',
     'smwg.info',
+    'snakebutt.com',
     'snakemail.com',
     'snapwet.com',
     'sneakmail.de',
     'snece.com',
     'social-mailer.tk',
     'socialfurry.org',
+    'sociallymediocre.com',
     'sofia.re',
     'sofimail.com',
     'sofort-mail.de',
     'sofortmail.de',
     'sofrge.com',
     'softkey-office.ru',
     'softpls.asia',
@@ -2964,14 +2982,15 @@
     'spamcorptastic.com',
     'spamcowboy.com',
     'spamcowboy.net',
     'spamcowboy.org',
     'spamday.com',
     'spamdecoy.net',
     'spamex.com',
+    'spamfellas.com',
     'spamfighter.cf',
     'spamfighter.ga',
     'spamfighter.gq',
     'spamfighter.ml',
     'spamfighter.tk',
     'spamfree.eu',
     'spamfree24.com',
@@ -2992,14 +3011,15 @@
     'spamlot.net',
     'spammer.fail',
     'spammotel.com',
     'spammy.host',
     'spamobox.com',
     'spamoff.de',
     'spamsalad.in',
+    'spamsandwich.com',
     'spamslicer.com',
     'spamsphere.com',
     'spamspot.com',
     'spamstack.net',
     'spamthis.co.uk',
     'spamthis.network',
     'spamthisplease.com',
@@ -3011,14 +3031,15 @@
     'spamwc.gq',
     'spamwc.ml',
     'speedgaus.net',
     'sperma.cf',
     'spikio.com',
     'spindl-e.com',
     'spoofmail.de',
+    'sportrid.com',
     'spr.io',
     'spritzzone.de',
     'spruzme.com',
     'spybox.de',
     'spymail.com',
     'squizzy.de',
     'squizzy.net',
@@ -3180,14 +3201,15 @@
     'thelimestones.com',
     'thembones.com.au',
     'themegreview.com',
     'themostemail.com',
     'thereddoors.online',
     'theroyalweb.club',
     'thescrappermovie.com',
+    'thespamfather.com',
     'theteastory.info',
     'thex.ro',
     'thichanthit.com',
     'thietbivanphong.asia',
     'thisisnotmyrealemail.com',
     'thismail.net',
     'thisurl.website',
@@ -3361,14 +3383,15 @@
     'undo.it',
     'unicodeworld.com',
     'unids.com',
     'unimark.org',
     'unit7lahaina.com',
     'unmail.ru',
     'uooos.com',
+    'uorak.com',
     'upliftnow.com',
     'uplipht.com',
     'uploadnolimit.com',
     'upozowac.info',
     'urfunktion.se',
     'urhen.com',
     'uroid.com',
@@ -3518,34 +3541,37 @@
     'wegwerfmail.info',
     'wegwerfmail.net',
     'wegwerfmail.org',
     'wegwerpmailadres.nl',
     'wegwrfmail.de',
     'wegwrfmail.net',
     'wegwrfmail.org',
+    'weizixu.com',
     'wekawa.com',
     'welikecookies.com',
     'wellsfargocomcardholders.com',
     'wemel.top',
     'wetrainbayarea.com',
     'wetrainbayarea.org',
     'wfgdfhj.tk',
     'wg0.com',
     'wh4f.org',
+    'whaaaaaaaaaat.com',
     'whatiaas.com',
     'whatifanalytics.com',
     'whatpaas.com',
     'whatsaas.com',
     'whiffles.org',
     'whopy.com',
     'whyspam.me',
     'wibblesmith.com',
     'wickmail.net',
     'widaryanto.info',
     'widget.gg',
+    'wiemei.com',
     'wierie.tk',
     'wifimaple.com',
     'wifioak.com',
     'wikidocuslava.ru',
     'wilemail.com',
     'willhackforfood.biz',
     'willselfdestruct.com',
```

### Comparing `disposable-email-domains-0.0.92/disposable_email_domains.egg-info/PKG-INFO` & `disposable-email-domains-0.0.93/disposable_email_domains.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disposable-email-domains
-Version: 0.0.92
+Version: 0.0.93
 Summary: A set of disposable email domains
 Home-page: https://github.com/disposable-email-domains/disposable-email-domains
 Author: Dustin Ingram
 Author-email: github@dustingram.com
 License: MIT
 Keywords: disposable email domains blocklist
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `disposable-email-domains-0.0.92/disposable_email_domains.egg-info/SOURCES.txt` & `disposable-email-domains-0.0.93/disposable_email_domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.92/setup.py` & `disposable-email-domains-0.0.93/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-__version__ = "0.0.92"
+__version__ = "0.0.93"
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="disposable-email-domains",
     version=__version__,
```

### Comparing `disposable-email-domains-0.0.92/source_data/allowlist.conf` & `disposable-email-domains-0.0.93/source_data/allowlist.conf`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 internet-e-mail.com
 internet-mail.org
 internetemails.net
 internetmailing.net
 jetemail.net
 justemail.net
 letterboxes.org
+liamekaens.com
 mail-central.com
 mail-page.com
 mail2world.com
 mailandftp.com
 mailas.com
 mailbolt.com
 mailc.net
@@ -144,14 +145,15 @@
 sent.at
 sent.com
 shitposting.agency
 shitware.nl
 sibmail.com
 sneakemail.com
 snkmail.com
+snkml.com
 spamcannon.com
 spamcannon.net
 spamgourmet.com
 spamgourmet.net
 spamgourmet.org
 speedpost.net
 speedymail.org
```

### Comparing `disposable-email-domains-0.0.92/source_data/disposable_email_blocklist.conf` & `disposable-email-domains-0.0.93/source_data/disposable_email_blocklist.conf`

 * *Files 0% similar despite different names*

```diff
@@ -579,14 +579,15 @@
 chalupaurybnicku.cz
 chammy.info
 chasefreedomactivate.com
 chatich.com
 cheaphub.net
 cheatmail.de
 chenbot.email
+chewydonut.com
 chibakenma.ml
 chickenkiller.com
 chielo.com
 childsavetrust.org
 chilkat.com
 chinamkm.com
 chithinh.com
@@ -1462,14 +1463,15 @@
 hulapla.de
 humaility.com
 hungpackage.com
 hushmail.cf
 huskion.net
 hvastudiesucces.nl
 hwsye.net
+hypenated-domain.com
 i2pmail.org
 i6.cloudns.cc
 iaoss.com
 ibnuh.bz
 icantbelieveineedtoexplainthisshit.com
 icemail.club
 ichigo.me
@@ -1528,14 +1530,15 @@
 indomaed.pw
 indomina.cf
 indoserver.stream
 indosukses.press
 ineec.net
 infocom.zp.ua
 inggo.org
+inkiny.com
 inkomail.com
 inmynetwork.tk
 inoutmail.de
 inoutmail.eu
 inoutmail.info
 inoutmail.net
 inpwa.com
@@ -1576,14 +1579,15 @@
 isosq.com
 istii.ro
 isukrainestillacountry.com
 it7.ovh
 italy-mail.com
 itcompu.com
 itfast.net
+itsjiff.com
 itunesgiftcodegenerator.com
 iubridge.com
 iuemail.men
 iwi.net
 ixaks.com
 ixx.io
 j-p.us
@@ -1670,14 +1674,15 @@
 kino-100.ru
 kiois.com
 kismail.ru
 kisstwink.com
 kitnastar.com
 kjkszpjcompany.com
 kkmail.be
+kkoup.com
 kksm.be
 klassmaster.com
 klassmaster.net
 klick-tipp.us
 klipschx12.com
 kloap.com
 kludgemush.com
@@ -1763,14 +1768,15 @@
 liamcyrus.com
 lifebyfood.com
 lifetimefriends.info
 lifetotech.com
 ligsb.com
 lillemap.net
 lilo.me
+lilspam.com
 lindenbaumjapan.com
 link2mail.net
 linkedintuts2016.pw
 linshiyouxiang.net
 linuxmail.so
 litedrop.com
 liveradio.tk
@@ -1855,14 +1861,15 @@
 mail666.ru
 mail7.io
 mail707.com
 mail72.com
 mailapp.top
 mailback.com
 mailbidon.com
+mailbiscuit.com
 mailbiz.biz
 mailblocks.com
 mailbox.in.ua
 mailbox52.ga
 mailbox80.biz
 mailbox82.biz
 mailbox87.de
@@ -2064,14 +2071,15 @@
 misterpinball.de
 miucce.com
 mji.ro
 mjj.edu.ge
 mjukglass.nu
 mkpfilm.com
 ml8.ca
+mliok.com
 mm.my
 mm5.se
 mnode.me
 moakt.cc
 moakt.co
 moakt.com
 moakt.ws
@@ -2183,14 +2191,15 @@
 nada.ltd
 nagi.be
 nakedtruth.biz
 nanonym.ch
 naslazhdai.ru
 nationalgardeningclub.com
 nawmin.info
+naymedia.com
 nbzmr.com
 negated.com
 neko2.net
 nekochan.fr
 neomailbox.com
 neotlozhniy-zaim.ru
 nepwk.com
@@ -2400,14 +2409,15 @@
 pinehill-seattle.org
 pingir.com
 pipemail.space
 pisls.com
 pitaniezdorovie.ru
 pivo-bar.ru
 pixiil.com
+pizzajunk.com
 pjjkp.com
 placebomail10.com
 pleasenoham.org
 plexfirm.com
 plexolan.de
 plhk.ru
 ploae.com
@@ -2503,14 +2513,15 @@
 qtum-ico.com
 quadrafit.com
 quick-mail.cc
 quickemail.info
 quickinbox.com
 quickmail.nl
 quicksend.ch
+quipas.com
 ququb.com
 qvy.me
 qwickmail.com
 r4nd0m.de
 ra3.us
 rabin.ca
 rabiot.reisen
@@ -2530,14 +2541,15 @@
 rbb.org
 rcasd.com
 rcpt.at
 rdklcrv.xyz
 re-gister.com
 reality-concept.club
 reallymymail.com
+realquickemail.com
 realtyalerts.ca
 rebates.stream
 receiveee.com
 recipeforfailure.com
 recode.me
 reconmail.com
 recyclemail.dk
@@ -2652,14 +2664,15 @@
 services391.com
 sexforswingers.com
 sexical.com
 sexyalwasmi.top
 shadap.org
 shalar.net
 sharedmailbox.org
+sharkfaces.com
 sharklasers.com
 shchiba.uk
 sheryli.com
 shhmail.com
 shhuut.org
 shieldedmail.com
 shieldemail.com
@@ -2682,14 +2695,15 @@
 shut.ws
 siberpay.com
 sidelka-mytischi.ru
 siftportal.ru
 sify.com
 sika3.com
 sikux.com
+silenceofthespam.com
 siliwangi.ga
 silvercoin.life
 sim-simka.ru
 simaenaga.com
 simpleitsecurity.info
 sin.cl
 sinaite.net
@@ -2726,20 +2740,22 @@
 smarttalent.pw
 smashmail.de
 smellfear.com
 smellrear.com
 smellypotato.tk
 smtp99.com
 smwg.info
+snakebutt.com
 snakemail.com
 snapwet.com
 sneakmail.de
 snece.com
 social-mailer.tk
 socialfurry.org
+sociallymediocre.com
 sofia.re
 sofimail.com
 sofort-mail.de
 sofortmail.de
 sofrge.com
 softkey-office.ru
 softpls.asia
@@ -2785,14 +2801,15 @@
 spamcorptastic.com
 spamcowboy.com
 spamcowboy.net
 spamcowboy.org
 spamday.com
 spamdecoy.net
 spamex.com
+spamfellas.com
 spamfighter.cf
 spamfighter.ga
 spamfighter.gq
 spamfighter.ml
 spamfighter.tk
 spamfree.eu
 spamfree24.com
@@ -2813,14 +2830,15 @@
 spamlot.net
 spammer.fail
 spammotel.com
 spammy.host
 spamobox.com
 spamoff.de
 spamsalad.in
+spamsandwich.com
 spamslicer.com
 spamsphere.com
 spamspot.com
 spamstack.net
 spamthis.co.uk
 spamthis.network
 spamthisplease.com
@@ -2832,14 +2850,15 @@
 spamwc.gq
 spamwc.ml
 speedgaus.net
 sperma.cf
 spikio.com
 spindl-e.com
 spoofmail.de
+sportrid.com
 spr.io
 spritzzone.de
 spruzme.com
 spybox.de
 spymail.com
 squizzy.de
 squizzy.net
@@ -3001,14 +3020,15 @@
 thelimestones.com
 thembones.com.au
 themegreview.com
 themostemail.com
 thereddoors.online
 theroyalweb.club
 thescrappermovie.com
+thespamfather.com
 theteastory.info
 thex.ro
 thichanthit.com
 thietbivanphong.asia
 thisisnotmyrealemail.com
 thismail.net
 thisurl.website
@@ -3182,14 +3202,15 @@
 undo.it
 unicodeworld.com
 unids.com
 unimark.org
 unit7lahaina.com
 unmail.ru
 uooos.com
+uorak.com
 upliftnow.com
 uplipht.com
 uploadnolimit.com
 upozowac.info
 urfunktion.se
 urhen.com
 uroid.com
@@ -3339,34 +3360,37 @@
 wegwerfmail.info
 wegwerfmail.net
 wegwerfmail.org
 wegwerpmailadres.nl
 wegwrfmail.de
 wegwrfmail.net
 wegwrfmail.org
+weizixu.com
 wekawa.com
 welikecookies.com
 wellsfargocomcardholders.com
 wemel.top
 wetrainbayarea.com
 wetrainbayarea.org
 wfgdfhj.tk
 wg0.com
 wh4f.org
+whaaaaaaaaaat.com
 whatiaas.com
 whatifanalytics.com
 whatpaas.com
 whatsaas.com
 whiffles.org
 whopy.com
 whyspam.me
 wibblesmith.com
 wickmail.net
 widaryanto.info
 widget.gg
+wiemei.com
 wierie.tk
 wifimaple.com
 wifioak.com
 wikidocuslava.ru
 wilemail.com
 willhackforfood.biz
 willselfdestruct.com
```

