# Comparing `tmp/matrix_gptbot-0.3.6.tar.gz` & `tmp/matrix_gptbot-0.3.7.tar.gz`

## Comparing `matrix_gptbot-0.3.6.tar` & `matrix_gptbot-0.3.7.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/.gitlab-ci.yml
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/CHANGELOG.md
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/config.dist.ini
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/gptbot-pantalaimon.service
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/gptbot.service
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/pantalaimon.example.conf
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/pantalaimon_first_login.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/.vscode/launch.json
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/__init__.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/__main__.py
--rw-r--r--   0        0        0   190295 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/assets/logo.png
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/invite.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/join.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/message.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/roommember.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/sync.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/test.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/callbacks/test_response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/__init__.py
--rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/bot.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/dict.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/logging.py
--rw-r--r--   0        0        0    25750 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/openai.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/trackingmore.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/classes/wolframalpha.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/__init__.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/botinfo.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/calculate.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/chat.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/classify.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/coin.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/custom.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/dice.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/help.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/ignoreolder.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/imagine.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/newroom.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/parcel.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/privacy.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/roomsettings.py
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/space.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/stats.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/systemmessage.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/tts.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/commands/unknown.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/__init__.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_1.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_2.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_3.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_4.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_5.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_6.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_7.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/migrations/migration_8.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/__init__.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/base.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/datetime.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/dice.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/geocode.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/imagedescription.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/imagine.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/newroom.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/weather.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/webrequest.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/websearch.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/src/gptbot/tools/wikipedia.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/LICENSE
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/README.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    10910 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/CHANGELOG.md
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/config.dist.ini
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/gptbot-pantalaimon.service
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/gptbot.service
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/pantalaimon.example.conf
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/pantalaimon_first_login.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/.forgejo/workflows/release.yml
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/.vscode/launch.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/__main__.py
+-rw-r--r--   0        0        0   190295 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/assets/logo.png
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/callbacks/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/callbacks/invite.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/callbacks/join.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/callbacks/message.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/callbacks/roommember.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/callbacks/sync.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/callbacks/test.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/callbacks/test_response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/classes/__init__.py
+-rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/classes/bot.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/classes/dict.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/classes/logging.py
+-rw-r--r--   0        0        0    25750 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/classes/openai.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/classes/trackingmore.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/classes/wolframalpha.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/__init__.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/botinfo.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/calculate.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/chat.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/classify.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/coin.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/custom.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/dice.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/help.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/ignoreolder.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/imagine.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/newroom.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/parcel.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/privacy.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/roomsettings.py
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/space.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/stats.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/systemmessage.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/tts.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/commands/unknown.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/migrations/__init__.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/migrations/migration_1.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/migrations/migration_2.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/migrations/migration_3.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/migrations/migration_4.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/migrations/migration_5.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/migrations/migration_6.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/migrations/migration_7.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/migrations/migration_8.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/__init__.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/base.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/datetime.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/dice.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/geocode.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/imagedescription.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/imagine.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/newroom.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/weather.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/webrequest.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/websearch.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/src/gptbot/tools/wikipedia.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/LICENSE
+-rw-r--r--   0        0        0     8507 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/README.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 matrix_gptbot-0.3.7/PKG-INFO
```

### Comparing `matrix_gptbot-0.3.6/CHANGELOG.md` & `matrix_gptbot-0.3.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/config.dist.ini` & `matrix_gptbot-0.3.7/config.dist.ini`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/__main__.py` & `matrix_gptbot-0.3.7/src/gptbot/__main__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/assets/logo.png` & `matrix_gptbot-0.3.7/src/gptbot/assets/logo.png`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/callbacks/__init__.py` & `matrix_gptbot-0.3.7/src/gptbot/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/callbacks/join.py` & `matrix_gptbot-0.3.7/src/gptbot/callbacks/join.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/callbacks/message.py` & `matrix_gptbot-0.3.7/src/gptbot/callbacks/message.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/classes/bot.py` & `matrix_gptbot-0.3.7/src/gptbot/classes/bot.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/classes/logging.py` & `matrix_gptbot-0.3.7/src/gptbot/classes/logging.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/classes/openai.py` & `matrix_gptbot-0.3.7/src/gptbot/classes/openai.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/classes/trackingmore.py` & `matrix_gptbot-0.3.7/src/gptbot/classes/trackingmore.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/classes/wolframalpha.py` & `matrix_gptbot-0.3.7/src/gptbot/classes/wolframalpha.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/__init__.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/botinfo.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/botinfo.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/calculate.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/calculate.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/classify.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/classify.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/dice.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/dice.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/help.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/help.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/imagine.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/imagine.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/newroom.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/newroom.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/parcel.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/parcel.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/privacy.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/privacy.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/roomsettings.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/roomsettings.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/space.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/space.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/stats.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/stats.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/systemmessage.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/systemmessage.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/commands/tts.py` & `matrix_gptbot-0.3.7/src/gptbot/commands/tts.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/migrations/__init__.py` & `matrix_gptbot-0.3.7/src/gptbot/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_1.py` & `matrix_gptbot-0.3.7/src/gptbot/migrations/migration_1.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_3.py` & `matrix_gptbot-0.3.7/src/gptbot/migrations/migration_3.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_5.py` & `matrix_gptbot-0.3.7/src/gptbot/migrations/migration_5.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_6.py` & `matrix_gptbot-0.3.7/src/gptbot/migrations/migration_6.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_7.py` & `matrix_gptbot-0.3.7/src/gptbot/migrations/migration_7.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/migrations/migration_8.py` & `matrix_gptbot-0.3.7/src/gptbot/migrations/migration_8.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/tools/base.py` & `matrix_gptbot-0.3.7/src/gptbot/tools/base.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/tools/dice.py` & `matrix_gptbot-0.3.7/src/gptbot/tools/dice.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/tools/geocode.py` & `matrix_gptbot-0.3.7/src/gptbot/tools/geocode.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/tools/imagine.py` & `matrix_gptbot-0.3.7/src/gptbot/tools/imagine.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/tools/newroom.py` & `matrix_gptbot-0.3.7/src/gptbot/tools/newroom.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/tools/weather.py` & `matrix_gptbot-0.3.7/src/gptbot/tools/weather.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/tools/webrequest.py` & `matrix_gptbot-0.3.7/src/gptbot/tools/webrequest.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/tools/websearch.py` & `matrix_gptbot-0.3.7/src/gptbot/tools/websearch.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/src/gptbot/tools/wikipedia.py` & `matrix_gptbot-0.3.7/src/gptbot/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/LICENSE` & `matrix_gptbot-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix_gptbot-0.3.6/README.md` & `matrix_gptbot-0.3.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # GPTbot
 
+[![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
+
 GPTbot is a simple bot that uses different APIs to generate responses to
 messages in a Matrix room.
 
 ## Features
 
 - AI-generated responses to text, image and voice messages in a Matrix room 
 (chatbot)
```

### Comparing `matrix_gptbot-0.3.6/pyproject.toml` & `matrix_gptbot-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "matrix-gptbot"
-version = "0.3.6"
+version = "0.3.7"
 
 authors = [
   { name="Kumi Mitterer", email="gptbot@kumi.email" },
 ]
 
 description = "Multifunctional Chatbot for Matrix"
 readme = "README.md"
```

### Comparing `matrix_gptbot-0.3.6/PKG-INFO` & `matrix_gptbot-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: matrix-gptbot
-Version: 0.3.6
+Version: 0.3.7
 Summary: Multifunctional Chatbot for Matrix
 Project-URL: Homepage, https://kumig.it/kumitterer/matrix-gptbot
 Project-URL: Bug Tracker, https://kumig.it/kumitterer/matrix-gptbot/issues
 Author-email: Kumi Mitterer <gptbot@kumi.email>
 License: Copyright (c) 2023 Kumi Mitterer <gptbot@kumi.email>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,32 +33,42 @@
 Requires-Dist: matrix-nio[e2e]
 Requires-Dist: pillow
 Requires-Dist: python-magic
 Requires-Dist: tiktoken
 Provides-Extra: all
 Requires-Dist: beautifulsoup4; extra == 'all'
 Requires-Dist: geopy; extra == 'all'
-Requires-Dist: matrix-gptbot[e2ee,openai,wolframalpha]; extra == 'all'
+Requires-Dist: openai>=1.2; extra == 'all'
+Requires-Dist: pantalaimon>=0.10.5; extra == 'all'
+Requires-Dist: pydub; extra == 'all'
+Requires-Dist: wolframalpha; extra == 'all'
 Provides-Extra: dev
+Requires-Dist: beautifulsoup4; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
+Requires-Dist: geopy; extra == 'dev'
 Requires-Dist: hatchling; extra == 'dev'
-Requires-Dist: matrix-gptbot[all]; extra == 'dev'
+Requires-Dist: openai>=1.2; extra == 'dev'
+Requires-Dist: pantalaimon>=0.10.5; extra == 'dev'
+Requires-Dist: pydub; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
+Requires-Dist: wolframalpha; extra == 'dev'
 Provides-Extra: e2ee
 Requires-Dist: pantalaimon>=0.10.5; extra == 'e2ee'
 Provides-Extra: openai
 Requires-Dist: openai>=1.2; extra == 'openai'
 Requires-Dist: pydub; extra == 'openai'
 Provides-Extra: wolframalpha
 Requires-Dist: wolframalpha; extra == 'wolframalpha'
 Description-Content-Type: text/markdown
 
 # GPTbot
 
+[![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
+
 GPTbot is a simple bot that uses different APIs to generate responses to
 messages in a Matrix room.
 
 ## Features
 
 - AI-generated responses to text, image and voice messages in a Matrix room 
 (chatbot)
```

