# Comparing `tmp/reseval-0.1.0.tar.gz` & `tmp/reseval-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reseval-0.1.0.tar", last modified: Thu Jul 20 13:28:10 2023, max compression
+gzip compressed data, was "reseval-0.1.1.tar", last modified: Mon Aug  7 19:18:18 2023, max compression
```

## Comparing `reseval-0.1.0.tar` & `reseval-0.1.1.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.869796 reseval-0.1.0/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1078 2023-04-02 16:25:40.000000 reseval-0.1.0/LICENSE
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12286 2023-07-20 13:28:10.869796 reseval-0.1.0/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    11894 2023-07-20 13:26:17.000000 reseval-0.1.0/README.md
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.841796 reseval-0.1.0/reseval/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      534 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1218 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/__main__.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.841796 reseval-0.1.0/reseval/app/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       21 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/app/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1306 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/app/heroku.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.841796 reseval-0.1.0/reseval/assets/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       15 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/Procfile
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)  1156816 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/package-lock.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      826 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/package.json
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/public/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1951 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/public/favicon.ico
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1725 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/public/index.html
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      315 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/public/manifest.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       67 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/public/robots.txt
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/src/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      221 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/App.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2722 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/Survey.js
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/src/components/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      925 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Audio.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      386 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/components/Button.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      460 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Image.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      446 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/components/Markdown.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2578 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Media.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1509 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/MediaRadioButtonGroup.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4720 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/MediaSliderGroup.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1236 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/RadioButtonGroup.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      975 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Text.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      881 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/Video.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2500 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/components/WordSelection.js
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/src/css/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3102 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/css/components.css
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      350 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/css/index.css
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      594 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/index.js
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.845796 reseval-0.1.0/reseval/assets/client/src/json/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        0 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/json/.gitkeep
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.849796 reseval-0.1.0/reseval/assets/client/src/pages/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      807 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/pages/EndPage.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2714 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/pages/FeedbackPage.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10151 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/pages/QualificationPage.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3720 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/pages/TaskPage.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      539 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/pages/WelcomePage.js
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.849796 reseval-0.1.0/reseval/assets/client/src/questions/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      235 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/questions/FreeResponse.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1393 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/questions/ListeningTest.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1208 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/questions/MultipleChoice.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1021 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/src/questions/Question.js
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.849796 reseval-0.1.0/reseval/assets/client/src/test/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2186 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/AB.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2834 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/ABX.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1994 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/MOS.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2818 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/MUSHRA.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1967 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/client/src/test/WordSelect.js
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      100 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/client/static.json
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/listening_test/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones4_0.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones4_1.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones4_2.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones4_3.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones5_0.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones5_1.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones5_2.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones5_3.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones6_0.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones6_1.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones6_2.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones6_3.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones7_0.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones7_1.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones7_2.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones7_3.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones8_0.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones8_1.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones8_2.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/listening_test/tones8_3.wav
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   147781 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/package-lock.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      848 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/package.json
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.837796 reseval-0.1.0/reseval/assets/server/
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/server/db/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      925 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/server/db/index.ts
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/server/db/queries/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      142 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/db/queries/conditions.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      101 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/db/queries/files.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1077 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/server/db/queries/participants.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      324 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/db/queries/responses.ts
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/server/routes/
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/assets/server/routes/api/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      484 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/routes/api/conditions.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      475 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/routes/api/files.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      439 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/server/routes/api/index.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1361 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/assets/server/routes/api/participants.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      641 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/routes/api/responses.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      157 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server/routes/index.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      744 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/server.ts
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1054 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/survey.xml
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10895 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/assets/tsconfig.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2900 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/constants.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/convert/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/convert/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      697 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/convert/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3706 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/convert/audio.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2777 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/convert/image.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2187 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.861796 reseval-0.1.0/reseval/create/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       25 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/create/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      936 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/create/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5138 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/create/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/credentials/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/credentials/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1039 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/credentials/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2526 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/credentials/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/crowdsource/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       40 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/crowdsource/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5776 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/crowdsource/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12696 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/crowdsource/mturk.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/database/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       83 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3616 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/aws.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10207 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      884 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/database/download.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      925 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/heroku.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1940 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/database/localhost.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/destroy/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/destroy/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      799 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/destroy/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1602 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/destroy/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      270 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/error.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/extend/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/extend/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      986 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/extend/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1922 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/extend/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      731 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/filter.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2708 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/load.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/monitor/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/monitor/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      797 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/monitor/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5241 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/monitor/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1219 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/npm.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/pay/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/pay/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      541 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/pay/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      374 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/pay/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2870 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/plot.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      244 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/random.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.865796 reseval-0.1.0/reseval/results/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/results/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      754 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/results/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2481 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/results/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.869796 reseval-0.1.0/reseval/server/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       79 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     8144 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/aws.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1901 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3737 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/heroku.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2003 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/server/local.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1620 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/stats.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.869796 reseval-0.1.0/reseval/storage/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       59 2023-04-02 16:25:40.000000 reseval-0.1.0/reseval/storage/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5015 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/storage/aws.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1425 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/storage/client.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1401 2023-06-02 19:25:32.000000 reseval-0.1.0/reseval/storage/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.869796 reseval-0.1.0/reseval/test/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      166 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1552 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/ab.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      675 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/abx.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4016 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/base.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      615 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4103 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/mos.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3018 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/mushra.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2013 2023-07-20 13:26:17.000000 reseval-0.1.0/reseval/test/wordselect.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-20 13:28:10.841796 reseval-0.1.0/reseval.egg-info/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12286 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4936 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/SOURCES.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/dependency_links.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      185 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/requires.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        8 2023-07-20 13:28:10.000000 reseval-0.1.0/reseval.egg-info/top_level.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-07-20 13:28:10.869796 reseval-0.1.0/setup.cfg
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1571 2023-07-20 13:27:25.000000 reseval-0.1.0/setup.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.400667 reseval-0.1.1/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1078 2023-07-24 17:24:30.000000 reseval-0.1.1/LICENSE
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12995 2023-08-07 19:18:18.400667 reseval-0.1.1/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12603 2023-07-24 17:24:30.000000 reseval-0.1.1/README.md
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.380667 reseval-0.1.1/reseval/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      534 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1218 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/__main__.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.380667 reseval-0.1.1/reseval/app/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       21 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/app/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1306 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/app/heroku.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.380667 reseval-0.1.1/reseval/assets/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       15 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/Procfile
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.380667 reseval-0.1.1/reseval/assets/client/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)  1156816 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/package-lock.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      826 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/package.json
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.384667 reseval-0.1.1/reseval/assets/client/public/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1951 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/public/favicon.ico
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1725 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/public/index.html
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      315 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/public/manifest.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       67 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/public/robots.txt
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.384667 reseval-0.1.1/reseval/assets/client/src/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      221 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/App.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2722 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/Survey.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.384667 reseval-0.1.1/reseval/assets/client/src/components/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      925 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/Audio.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      386 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/Button.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      460 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/Image.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      446 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/Markdown.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2578 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/Media.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1509 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/MediaRadioButtonGroup.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4720 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/MediaSliderGroup.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1236 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/RadioButtonGroup.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      975 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/Text.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      881 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/Video.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2500 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/components/WordSelection.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.384667 reseval-0.1.1/reseval/assets/client/src/css/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3102 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/css/components.css
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      350 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/css/index.css
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      594 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/index.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.384667 reseval-0.1.1/reseval/assets/client/src/json/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        0 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/json/.gitkeep
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.384667 reseval-0.1.1/reseval/assets/client/src/pages/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      807 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/pages/EndPage.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2714 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/pages/FeedbackPage.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10151 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/pages/QualificationPage.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3720 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/pages/TaskPage.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      539 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/pages/WelcomePage.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.384667 reseval-0.1.1/reseval/assets/client/src/questions/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      235 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/questions/FreeResponse.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1393 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/questions/ListeningTest.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1208 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/questions/MultipleChoice.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1021 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/questions/Question.js
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.384667 reseval-0.1.1/reseval/assets/client/src/test/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2186 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/test/AB.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2834 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/test/ABX.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1994 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/test/MOS.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2818 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/test/MUSHRA.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1967 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/src/test/WordSelect.js
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      100 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/client/static.json
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.392667 reseval-0.1.1/reseval/assets/listening_test/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones4_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones4_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones4_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones4_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones5_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones5_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones5_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones5_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones6_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones6_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones6_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones6_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones7_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones7_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones7_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones7_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones8_0.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones8_1.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones8_2.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   352828 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/listening_test/tones8_3.wav
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   147781 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/package-lock.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      848 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/package.json
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.376667 reseval-0.1.1/reseval/assets/server/
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/assets/server/db/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      925 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/db/index.ts
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/assets/server/db/queries/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      142 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/db/queries/conditions.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      101 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/db/queries/files.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1077 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/db/queries/participants.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      324 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/db/queries/responses.ts
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/assets/server/routes/
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/assets/server/routes/api/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      484 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/routes/api/conditions.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      475 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/routes/api/files.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      439 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/routes/api/index.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1361 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/routes/api/participants.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      641 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/routes/api/responses.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      157 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server/routes/index.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      744 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/server.ts
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1054 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/survey.xml
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10895 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/assets/tsconfig.json
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2900 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/constants.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/convert/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/convert/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      697 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/convert/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3706 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/convert/audio.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2777 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/convert/image.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2187 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/create/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       25 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/create/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      936 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/create/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5138 2023-08-07 19:14:25.000000 reseval-0.1.1/reseval/create/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/credentials/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/credentials/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1039 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/credentials/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2526 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/credentials/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/crowdsource/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       40 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/crowdsource/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5776 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/crowdsource/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12696 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/crowdsource/mturk.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/database/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       83 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/database/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3617 2023-08-07 18:24:05.000000 reseval-0.1.1/reseval/database/aws.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10207 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/database/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      884 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/database/download.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      925 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/database/heroku.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1940 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/database/localhost.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/destroy/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/destroy/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      799 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/destroy/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1602 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/destroy/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      270 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/error.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/extend/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/extend/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      986 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/extend/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1922 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/extend/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      731 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/filter.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2708 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/load.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/monitor/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/monitor/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      797 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/monitor/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5241 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/monitor/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1219 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/npm.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/pay/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/pay/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      541 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/pay/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      374 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/pay/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2870 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/plot.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      244 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/random.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.396667 reseval-0.1.1/reseval/results/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/results/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      754 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/results/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2481 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/results/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.400667 reseval-0.1.1/reseval/server/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       79 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/server/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     8138 2023-08-07 19:09:28.000000 reseval-0.1.1/reseval/server/aws.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1901 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/server/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3737 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/server/heroku.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2003 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/server/local.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1620 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/stats.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.400667 reseval-0.1.1/reseval/storage/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       59 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/storage/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5015 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/storage/aws.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1425 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/storage/client.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1401 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/storage/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.400667 reseval-0.1.1/reseval/test/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      166 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/test/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1552 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/test/ab.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      675 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/test/abx.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4016 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/test/base.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      615 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/test/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4103 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/test/mos.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3018 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/test/mushra.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2013 2023-07-24 17:24:30.000000 reseval-0.1.1/reseval/test/wordselect.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-08-07 19:18:18.380667 reseval-0.1.1/reseval.egg-info/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    12995 2023-08-07 19:18:18.000000 reseval-0.1.1/reseval.egg-info/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4936 2023-08-07 19:18:18.000000 reseval-0.1.1/reseval.egg-info/SOURCES.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-08-07 19:18:18.000000 reseval-0.1.1/reseval.egg-info/dependency_links.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      185 2023-08-07 19:18:18.000000 reseval-0.1.1/reseval.egg-info/requires.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        8 2023-08-07 19:18:18.000000 reseval-0.1.1/reseval.egg-info/top_level.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-08-07 19:18:18.400667 reseval-0.1.1/setup.cfg
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1571 2023-08-07 19:17:32.000000 reseval-0.1.1/setup.py
```

### Comparing `reseval-0.1.0/LICENSE` & `reseval-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/PKG-INFO` & `reseval-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-Metadata-Version: 2.1
-Name: reseval
-Version: 0.1.0
-Summary: Reproducible Subjective Evaluation
-Home-page: https://github.com/reseval/reseval
-Author: Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo
-Author-email: maxrmorrison@gmail.com
-Keywords: annotation,audio,ab,abx,crowdsourcing,evaluation,image,mos,mushra,speech,subjective
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<h1 align="center">Reproducible Subjective Evaluation (ReSEval)</h1>
+<div align="center">
 
-# Reproducible Subjective Evaluation (ReSEval)
 [![PyPI](https://img.shields.io/pypi/v/reseval.svg)](https://pypi.python.org/pypi/reseval)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![Downloads](https://pepy.tech/badge/reseval)](https://pepy.tech/project/reseval)
 
+</div>
+
 ReSEval is a framework for quickly building subjective evaluation and
 annotation tasks that are deployed on crowdworker platforms like
 [Amazon Mechanical Turk](https://www.mturk.com/). ReSEval currently supports
 A/B, ABX, MOS, MUSHRA, and Word Selection tests on audio, image, text, and video data.
 
 <h3 align="center">
     While our code is free to use, performing crowdsourced subjective
@@ -82,33 +75,33 @@
 
 ## Installation
 
 First, install the Python module. ReSEval requires Python 3.9 or higher.
 
 `pip install reseval`
 
-Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 17.4.0 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
+Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 18.16.1 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
 
 ```
 # Linux or OS X
 sudo npm install -g n
-sudo n 17.4.0
+sudo n 18.16.1
 
 # Windows
 # Must be run with administrator privileges
-nvm install 17.4.0
-nvm use 17.4.0
+nvm install 18.16.1
+nvm use 18.16.1
 ```
 
 **Note** - You must restart your terminal after changing versions of node for the change to take effect
 
 ### Deploying locally
 
 To be able to preview your subjective evaluation locally, you must
-[setup a local MySQL database](https://dev.mysql.com/doc/mysql-getting-started/en/)
+[setup a local MySQL database server](https://dev.mysql.com/doc/mysql-getting-started/en/)
 and obtain a username and password. The default username is `root`.
 
 Run the following to store the username and password in
 `reseval.CACHE / '.env'`.
 
 ```
 python -m reseval.credentials \
@@ -257,14 +250,16 @@
 <p align="center">
     <img src="docs/images/aws-00.png" width="400" alt="AWS API key instructions">
     <img src="docs/images/aws-01.png" width="400" alt="AWS API key instructions">
 </p>
 
 Note that this gives you a root access key. You can alternatively use the Identity & Access Management (IAM) system to setup more restrictive permissions for a user.
 
+If you have never used AWS Elastic Beanstalk, one more step is required. Elastic Beanstalk instances created from Python (as opposed to the AWS console) do not instantiate the default instance profile IAM role. The solution is to either create (and then delete) an Elastic Beanstalk instance from the console, or to create the required IAM role manually. The IAM role is called `aws-elasticbeanstalk-ec2-role` and contains three permissions: (1) `AWSElasticBeanstalkWebTier`, (2) `AWSElasticBeanstalkMulticontainerDocker`, and (3) `AWSElasticBeanstalkWorkerTier`.
+
 
 ### Amazon Mechanical Turk
 
 Follow the instructions [here](https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/SetUp.html) for setting up MTurk and connecting it to your AWS account.
 
 
 ### Heroku (Optional if you don't want to use AWS)
@@ -282,17 +277,21 @@
 ## Usage
 
 Once you have your configuration file and a properly formatted directory of evaluation files, you are ready to deploy a subjective evaluation. Example configuration files and corresponding evaluation files can be found in `examples/`.
 
 If you are not deploying locally, add your API keys.
 
 ```
+# AWS credentials
 python -m reseval.credentials \
     --aws_api_key <aws_api_key> \
-    --aws_api_secret_key <aws_api_secret_key> \
+    --aws_api_secret_key <aws_api_secret_key>
+
+# (Optional) Heroku credentials
+python -m reseval.credentials \
     --heroku_api_key <heroku_api_key>
 ```
 
  API keys are saved in `reseval.CACHE / '.keys'`. The `.keys` file is used to set local environment variables and is not pushed to GitHub or uploaded to any remote storage.
 
 
 ### Command-line interface
```

### Comparing `reseval-0.1.0/README.md` & `reseval-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,28 @@
-# Reproducible Subjective Evaluation (ReSEval)
+Metadata-Version: 2.1
+Name: reseval
+Version: 0.1.1
+Summary: Reproducible Subjective Evaluation
+Home-page: https://github.com/reseval/reseval
+Author: Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo
+Author-email: maxrmorrison@gmail.com
+Keywords: annotation,audio,ab,abx,crowdsourcing,evaluation,image,mos,mushra,speech,subjective
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">Reproducible Subjective Evaluation (ReSEval)</h1>
+<div align="center">
+
 [![PyPI](https://img.shields.io/pypi/v/reseval.svg)](https://pypi.python.org/pypi/reseval)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![Downloads](https://pepy.tech/badge/reseval)](https://pepy.tech/project/reseval)
 
+</div>
+
 ReSEval is a framework for quickly building subjective evaluation and
 annotation tasks that are deployed on crowdworker platforms like
 [Amazon Mechanical Turk](https://www.mturk.com/). ReSEval currently supports
 A/B, ABX, MOS, MUSHRA, and Word Selection tests on audio, image, text, and video data.
 
 <h3 align="center">
     While our code is free to use, performing crowdsourced subjective
@@ -71,33 +86,33 @@
 
 ## Installation
 
 First, install the Python module. ReSEval requires Python 3.9 or higher.
 
 `pip install reseval`
 
-Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 17.4.0 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
+Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 18.16.1 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
 
 ```
 # Linux or OS X
 sudo npm install -g n
-sudo n 17.4.0
+sudo n 18.16.1
 
 # Windows
 # Must be run with administrator privileges
-nvm install 17.4.0
-nvm use 17.4.0
+nvm install 18.16.1
+nvm use 18.16.1
 ```
 
 **Note** - You must restart your terminal after changing versions of node for the change to take effect
 
 ### Deploying locally
 
 To be able to preview your subjective evaluation locally, you must
-[setup a local MySQL database](https://dev.mysql.com/doc/mysql-getting-started/en/)
+[setup a local MySQL database server](https://dev.mysql.com/doc/mysql-getting-started/en/)
 and obtain a username and password. The default username is `root`.
 
 Run the following to store the username and password in
 `reseval.CACHE / '.env'`.
 
 ```
 python -m reseval.credentials \
@@ -246,14 +261,16 @@
 <p align="center">
     <img src="docs/images/aws-00.png" width="400" alt="AWS API key instructions">
     <img src="docs/images/aws-01.png" width="400" alt="AWS API key instructions">
 </p>
 
 Note that this gives you a root access key. You can alternatively use the Identity & Access Management (IAM) system to setup more restrictive permissions for a user.
 
+If you have never used AWS Elastic Beanstalk, one more step is required. Elastic Beanstalk instances created from Python (as opposed to the AWS console) do not instantiate the default instance profile IAM role. The solution is to either create (and then delete) an Elastic Beanstalk instance from the console, or to create the required IAM role manually. The IAM role is called `aws-elasticbeanstalk-ec2-role` and contains three permissions: (1) `AWSElasticBeanstalkWebTier`, (2) `AWSElasticBeanstalkMulticontainerDocker`, and (3) `AWSElasticBeanstalkWorkerTier`.
+
 
 ### Amazon Mechanical Turk
 
 Follow the instructions [here](https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/SetUp.html) for setting up MTurk and connecting it to your AWS account.
 
 
 ### Heroku (Optional if you don't want to use AWS)
@@ -271,17 +288,21 @@
 ## Usage
 
 Once you have your configuration file and a properly formatted directory of evaluation files, you are ready to deploy a subjective evaluation. Example configuration files and corresponding evaluation files can be found in `examples/`.
 
 If you are not deploying locally, add your API keys.
 
 ```
+# AWS credentials
 python -m reseval.credentials \
     --aws_api_key <aws_api_key> \
-    --aws_api_secret_key <aws_api_secret_key> \
+    --aws_api_secret_key <aws_api_secret_key>
+
+# (Optional) Heroku credentials
+python -m reseval.credentials \
     --heroku_api_key <heroku_api_key>
 ```
 
  API keys are saved in `reseval.CACHE / '.keys'`. The `.keys` file is used to set local environment variables and is not pushed to GitHub or uploaded to any remote storage.
 
 
 ### Command-line interface
```

### Comparing `reseval-0.1.0/reseval/__init__.py` & `reseval-0.1.1/reseval/__init__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/__main__.py` & `reseval-0.1.1/reseval/__main__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/app/heroku.py` & `reseval-0.1.1/reseval/app/heroku.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/package-lock.json` & `reseval-0.1.1/reseval/assets/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/package.json` & `reseval-0.1.1/reseval/assets/client/package.json`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/public/favicon.ico` & `reseval-0.1.1/reseval/assets/client/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/public/index.html` & `reseval-0.1.1/reseval/assets/client/public/index.html`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/Survey.js` & `reseval-0.1.1/reseval/assets/client/src/Survey.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/components/Audio.js` & `reseval-0.1.1/reseval/assets/client/src/components/Audio.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/components/Media.js` & `reseval-0.1.1/reseval/assets/client/src/components/Media.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/components/MediaRadioButtonGroup.js` & `reseval-0.1.1/reseval/assets/client/src/components/MediaRadioButtonGroup.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/components/MediaSliderGroup.js` & `reseval-0.1.1/reseval/assets/client/src/components/MediaSliderGroup.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/components/RadioButtonGroup.js` & `reseval-0.1.1/reseval/assets/client/src/components/RadioButtonGroup.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/components/Text.js` & `reseval-0.1.1/reseval/assets/client/src/components/Text.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/components/Video.js` & `reseval-0.1.1/reseval/assets/client/src/components/Video.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/components/WordSelection.js` & `reseval-0.1.1/reseval/assets/client/src/components/WordSelection.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/css/components.css` & `reseval-0.1.1/reseval/assets/client/src/css/components.css`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/index.js` & `reseval-0.1.1/reseval/assets/client/src/index.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/pages/EndPage.js` & `reseval-0.1.1/reseval/assets/client/src/pages/EndPage.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/pages/FeedbackPage.js` & `reseval-0.1.1/reseval/assets/client/src/pages/FeedbackPage.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/pages/QualificationPage.js` & `reseval-0.1.1/reseval/assets/client/src/pages/QualificationPage.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/pages/TaskPage.js` & `reseval-0.1.1/reseval/assets/client/src/pages/TaskPage.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/pages/WelcomePage.js` & `reseval-0.1.1/reseval/assets/client/src/pages/WelcomePage.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/questions/ListeningTest.js` & `reseval-0.1.1/reseval/assets/client/src/questions/ListeningTest.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/questions/MultipleChoice.js` & `reseval-0.1.1/reseval/assets/client/src/questions/MultipleChoice.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/questions/Question.js` & `reseval-0.1.1/reseval/assets/client/src/questions/Question.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/test/AB.js` & `reseval-0.1.1/reseval/assets/client/src/test/AB.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/test/ABX.js` & `reseval-0.1.1/reseval/assets/client/src/test/ABX.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/test/MOS.js` & `reseval-0.1.1/reseval/assets/client/src/test/MOS.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/test/MUSHRA.js` & `reseval-0.1.1/reseval/assets/client/src/test/MUSHRA.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/client/src/test/WordSelect.js` & `reseval-0.1.1/reseval/assets/client/src/test/WordSelect.js`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones4_0.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones4_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones4_1.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones4_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones4_2.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones4_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones4_3.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones4_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones5_0.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones5_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones5_1.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones5_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones5_2.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones5_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones5_3.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones5_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones6_0.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones6_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones6_1.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones6_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones6_2.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones6_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones6_3.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones6_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones7_0.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones7_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones7_1.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones7_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones7_2.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones7_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones7_3.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones7_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones8_0.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones8_0.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones8_1.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones8_1.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones8_2.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones8_2.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/listening_test/tones8_3.wav` & `reseval-0.1.1/reseval/assets/listening_test/tones8_3.wav`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/package-lock.json` & `reseval-0.1.1/reseval/assets/package-lock.json`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/package.json` & `reseval-0.1.1/reseval/assets/package.json`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/server/db/index.ts` & `reseval-0.1.1/reseval/assets/server/db/index.ts`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/server/db/queries/participants.ts` & `reseval-0.1.1/reseval/assets/server/db/queries/participants.ts`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/server/routes/api/participants.ts` & `reseval-0.1.1/reseval/assets/server/routes/api/participants.ts`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/server/routes/api/responses.ts` & `reseval-0.1.1/reseval/assets/server/routes/api/responses.ts`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/server.ts` & `reseval-0.1.1/reseval/assets/server.ts`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/survey.xml` & `reseval-0.1.1/reseval/assets/survey.xml`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/assets/tsconfig.json` & `reseval-0.1.1/reseval/assets/tsconfig.json`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/constants.py` & `reseval-0.1.1/reseval/constants.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/convert/__main__.py` & `reseval-0.1.1/reseval/convert/__main__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/convert/audio.py` & `reseval-0.1.1/reseval/convert/audio.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/convert/image.py` & `reseval-0.1.1/reseval/convert/image.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/core.py` & `reseval-0.1.1/reseval/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/create/__main__.py` & `reseval-0.1.1/reseval/create/__main__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/create/core.py` & `reseval-0.1.1/reseval/create/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/credentials/__main__.py` & `reseval-0.1.1/reseval/credentials/__main__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/credentials/core.py` & `reseval-0.1.1/reseval/credentials/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/crowdsource/core.py` & `reseval-0.1.1/reseval/crowdsource/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/crowdsource/mturk.py` & `reseval-0.1.1/reseval/crowdsource/mturk.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/database/aws.py` & `reseval-0.1.1/reseval/database/aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             }
         ]
     )['SecurityGroups']
     group_ids = [group['GroupId'] for group in security_groups]
 
     # Add ingress rules for local IP and MySQL
     local_ip = json.loads(
-        requests.get('https://ip.seeip.org/jsonip?').text
+        requests.get('https://api.seeip.org/jsonip?').text
     )['ip']
     for group_id in group_ids:
         client.authorize_security_group_ingress(
             GroupId=group_id,
             IpPermissions=[
                 {
                     'IpProtocol': '-1',
```

### Comparing `reseval-0.1.0/reseval/database/core.py` & `reseval-0.1.1/reseval/database/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/database/download.py` & `reseval-0.1.1/reseval/database/download.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/database/heroku.py` & `reseval-0.1.1/reseval/database/heroku.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/database/localhost.py` & `reseval-0.1.1/reseval/database/localhost.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/destroy/__main__.py` & `reseval-0.1.1/reseval/destroy/__main__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/destroy/core.py` & `reseval-0.1.1/reseval/destroy/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/extend/__main__.py` & `reseval-0.1.1/reseval/extend/__main__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/extend/core.py` & `reseval-0.1.1/reseval/extend/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/filter.py` & `reseval-0.1.1/reseval/filter.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/load.py` & `reseval-0.1.1/reseval/load.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/monitor/__main__.py` & `reseval-0.1.1/reseval/monitor/__main__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/monitor/core.py` & `reseval-0.1.1/reseval/monitor/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/npm.py` & `reseval-0.1.1/reseval/npm.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/pay/__main__.py` & `reseval-0.1.1/reseval/pay/__main__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/plot.py` & `reseval-0.1.1/reseval/plot.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/results/__main__.py` & `reseval-0.1.1/reseval/results/__main__.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/results/core.py` & `reseval-0.1.1/reseval/results/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/server/aws.py` & `reseval-0.1.1/reseval/server/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     while response['Status'].lower() != 'ready':
         time.sleep(3)
         response = client.describe_environments(
             ApplicationName=unique,
             EnvironmentNames=[unique])['Environments'][0]
 
     # Return application URL
-    return {'URL': response['EndpointURL']}
+    return {'URL': response['CNAME']}
 
 
 def destroy(name, credentials):
     """Destroy an AWS server"""
     # Get unique identifier
     unique = reseval.load.credentials_by_name(name, 'unique')['unique']
```

### Comparing `reseval-0.1.0/reseval/server/core.py` & `reseval-0.1.1/reseval/server/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/server/heroku.py` & `reseval-0.1.1/reseval/server/heroku.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/server/local.py` & `reseval-0.1.1/reseval/server/local.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/stats.py` & `reseval-0.1.1/reseval/stats.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/storage/aws.py` & `reseval-0.1.1/reseval/storage/aws.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/storage/client.py` & `reseval-0.1.1/reseval/storage/client.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/storage/core.py` & `reseval-0.1.1/reseval/storage/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/test/ab.py` & `reseval-0.1.1/reseval/test/ab.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/test/abx.py` & `reseval-0.1.1/reseval/test/abx.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/test/base.py` & `reseval-0.1.1/reseval/test/base.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/test/core.py` & `reseval-0.1.1/reseval/test/core.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/test/mos.py` & `reseval-0.1.1/reseval/test/mos.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/test/mushra.py` & `reseval-0.1.1/reseval/test/mushra.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval/test/wordselect.py` & `reseval-0.1.1/reseval/test/wordselect.py`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/reseval.egg-info/PKG-INFO` & `reseval-0.1.1/reseval.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: reseval
-Version: 0.1.0
+Version: 0.1.1
 Summary: Reproducible Subjective Evaluation
 Home-page: https://github.com/reseval/reseval
 Author: Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo
 Author-email: maxrmorrison@gmail.com
 Keywords: annotation,audio,ab,abx,crowdsourcing,evaluation,image,mos,mushra,speech,subjective
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Reproducible Subjective Evaluation (ReSEval)
+<h1 align="center">Reproducible Subjective Evaluation (ReSEval)</h1>
+<div align="center">
+
 [![PyPI](https://img.shields.io/pypi/v/reseval.svg)](https://pypi.python.org/pypi/reseval)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![Downloads](https://pepy.tech/badge/reseval)](https://pepy.tech/project/reseval)
 
+</div>
+
 ReSEval is a framework for quickly building subjective evaluation and
 annotation tasks that are deployed on crowdworker platforms like
 [Amazon Mechanical Turk](https://www.mturk.com/). ReSEval currently supports
 A/B, ABX, MOS, MUSHRA, and Word Selection tests on audio, image, text, and video data.
 
 <h3 align="center">
     While our code is free to use, performing crowdsourced subjective
@@ -82,33 +86,33 @@
 
 ## Installation
 
 First, install the Python module. ReSEval requires Python 3.9 or higher.
 
 `pip install reseval`
 
-Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 17.4.0 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
+Next, [download Node.js](https://nodejs.org/en/). You can check that your installation is correct by running `node --version`. ReSEval uses Node.js version 18.16.1 and is not guaranteed to work on all versions. If needed, Linux and OS X users can use `n` to change their version of Node.js, and Windows users can use [NVM for Windows](https://github.com/coreybutler/nvm-windows).
 
 ```
 # Linux or OS X
 sudo npm install -g n
-sudo n 17.4.0
+sudo n 18.16.1
 
 # Windows
 # Must be run with administrator privileges
-nvm install 17.4.0
-nvm use 17.4.0
+nvm install 18.16.1
+nvm use 18.16.1
 ```
 
 **Note** - You must restart your terminal after changing versions of node for the change to take effect
 
 ### Deploying locally
 
 To be able to preview your subjective evaluation locally, you must
-[setup a local MySQL database](https://dev.mysql.com/doc/mysql-getting-started/en/)
+[setup a local MySQL database server](https://dev.mysql.com/doc/mysql-getting-started/en/)
 and obtain a username and password. The default username is `root`.
 
 Run the following to store the username and password in
 `reseval.CACHE / '.env'`.
 
 ```
 python -m reseval.credentials \
@@ -257,14 +261,16 @@
 <p align="center">
     <img src="docs/images/aws-00.png" width="400" alt="AWS API key instructions">
     <img src="docs/images/aws-01.png" width="400" alt="AWS API key instructions">
 </p>
 
 Note that this gives you a root access key. You can alternatively use the Identity & Access Management (IAM) system to setup more restrictive permissions for a user.
 
+If you have never used AWS Elastic Beanstalk, one more step is required. Elastic Beanstalk instances created from Python (as opposed to the AWS console) do not instantiate the default instance profile IAM role. The solution is to either create (and then delete) an Elastic Beanstalk instance from the console, or to create the required IAM role manually. The IAM role is called `aws-elasticbeanstalk-ec2-role` and contains three permissions: (1) `AWSElasticBeanstalkWebTier`, (2) `AWSElasticBeanstalkMulticontainerDocker`, and (3) `AWSElasticBeanstalkWorkerTier`.
+
 
 ### Amazon Mechanical Turk
 
 Follow the instructions [here](https://docs.aws.amazon.com/AWSMechTurk/latest/AWSMechanicalTurkGettingStartedGuide/SetUp.html) for setting up MTurk and connecting it to your AWS account.
 
 
 ### Heroku (Optional if you don't want to use AWS)
@@ -282,17 +288,21 @@
 ## Usage
 
 Once you have your configuration file and a properly formatted directory of evaluation files, you are ready to deploy a subjective evaluation. Example configuration files and corresponding evaluation files can be found in `examples/`.
 
 If you are not deploying locally, add your API keys.
 
 ```
+# AWS credentials
 python -m reseval.credentials \
     --aws_api_key <aws_api_key> \
-    --aws_api_secret_key <aws_api_secret_key> \
+    --aws_api_secret_key <aws_api_secret_key>
+
+# (Optional) Heroku credentials
+python -m reseval.credentials \
     --heroku_api_key <heroku_api_key>
 ```
 
  API keys are saved in `reseval.CACHE / '.keys'`. The `.keys` file is used to set local environment variables and is not pushed to GitHub or uploaded to any remote storage.
 
 
 ### Command-line interface
```

### Comparing `reseval-0.1.0/reseval.egg-info/SOURCES.txt` & `reseval-0.1.1/reseval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reseval-0.1.0/setup.py` & `reseval-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         for path in assets_directory.rglob('*')]}
 
 
 # Setup
 setup(
     name='reseval',
     description='Reproducible Subjective Evaluation',
-    version='0.1.0',
+    version='0.1.1',
     author='Max Morrison, Brian Tang, Gefei Tan, Bryan Pardo',
     author_email='maxrmorrison@gmail.com',
     url='https://github.com/reseval/reseval',
     install_requires=[
         'appdirs>=1.4.4',
         'boto3>=1.21.3',
         'matplotlib>=3.5.2',
```

