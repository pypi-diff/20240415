# Comparing `tmp/absfuyu-3.3.2.tar.gz` & `tmp/absfuyu-3.3.3.tar.gz`

## Comparing `absfuyu-3.3.2.tar` & `absfuyu-3.3.3.tar`

### file list

```diff
@@ -1,78 +1,87 @@
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/__init__.py
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/__main__.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/core.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/everything.py
--rw-r--r--   0        0        0    12906 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/py.typed
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/sort.py
--rw-r--r--   0        0        0    13559 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/version.py
--rw-r--r--   0        0        0     8630 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/config/__init__.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/config/config.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/extensions/__init__.py
--rw-r--r--   0        0        0     5319 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/extensions/beautiful.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/extensions/dev/__init__.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/extensions/dev/password_hash.py
--rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/extensions/dev/passwordlib.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/extensions/dev/project_starter.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/extensions/dev/shutdownizer.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/extensions/extra/__init__.py
--rw-r--r--   0        0        0    31699 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/extensions/extra/data_analysis.py
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/fun/WGS.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/fun/__init__.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/fun/tarot.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/game/__init__.py
--rw-r--r--   0        0        0    10374 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/game/sudoku.py
--rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/game/tictactoe.py
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/game/tictactoe2.py
--rw-r--r--   0        0        0   101143 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/game/wordle.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/general/__init__.py
--rw-r--r--   0        0        0    17431 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/general/content.py
--rw-r--r--   0        0        0    48936 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/general/data_extension.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/general/generator.py
--rw-r--r--   0        0        0     9680 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/general/human.py
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/pkg_data/__init__.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/pkg_data/chemistry.pkl
--rw-r--r--   0        0        0    56195 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/pkg_data/tarot.pkl
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/tools/__init__.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/tools/converter.py
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/tools/keygen.py
--rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/tools/obfuscator.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/tools/stats.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/tools/web.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/util/__init__.py
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/util/api.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/util/json_method.py
--rw-r--r--   0        0        0    13788 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/util/lunar.py
--rw-r--r--   0        0        0    16627 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/util/path.py
--rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/util/performance.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/util/pkl.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 absfuyu-3.3.2/src/absfuyu/util/zipped.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/conftest.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_DictExt.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_IntNumber.py
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_ListExt.py
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_Text.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_api.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_beautiful.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_config.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_converter.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_data_analysis.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_everything.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_extensions.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_fun.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_generator.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_json_method.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_logger.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_obfuscator.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_passwordlib.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_path.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_pkg_data.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_tarot.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_util.py
--rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 absfuyu-3.3.2/tests/test_version.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 absfuyu-3.3.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 absfuyu-3.3.2/LICENSE
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 absfuyu-3.3.2/README.md
--rw-r--r--   0        0        0     5978 2020-02-02 00:00:00.000000 absfuyu-3.3.2/pyproject.toml
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 absfuyu-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 absfuyu-3.3.3/dev_requirements.txt
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 absfuyu-3.3.3/docs/Makefile
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 absfuyu-3.3.3/docs/conf.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 absfuyu-3.3.3/docs/index.rst
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 absfuyu-3.3.3/docs/info.md
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 absfuyu-3.3.3/docs/make.bat
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 absfuyu-3.3.3/docs/modules.rst
+-rw-r--r--   0        0        0    34015 2020-02-02 00:00:00.000000 absfuyu-3.3.3/images/repository-image-crop.png
+-rw-r--r--   0        0        0    37867 2020-02-02 00:00:00.000000 absfuyu-3.3.3/images/repository-image-white.png
+-rw-r--r--   0        0        0    38341 2020-02-02 00:00:00.000000 absfuyu-3.3.3/images/repository-image.png
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/__main__.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/core.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/everything.py
+-rw-r--r--   0        0        0    13135 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/py.typed
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/sort.py
+-rw-r--r--   0        0        0    14128 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/version.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/cli/__init__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/cli/color.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/cli/config_group.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/cli/do_group.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/cli/game_group.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/config/__init__.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/config/config.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/extensions/__init__.py
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/extensions/beautiful.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/extensions/dev/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/extensions/dev/password_hash.py
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/extensions/dev/passwordlib.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/extensions/dev/project_starter.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/extensions/dev/shutdownizer.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/extensions/extra/__init__.py
+-rw-r--r--   0        0        0    31695 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/extensions/extra/data_analysis.py
+-rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/fun/WGS.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/fun/__init__.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/fun/tarot.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/game/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/game/game_stat.py
+-rw-r--r--   0        0        0    10141 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/game/sudoku.py
+-rw-r--r--   0        0        0     9609 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/game/tictactoe.py
+-rw-r--r--   0        0        0   101336 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/game/wordle.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/general/__init__.py
+-rw-r--r--   0        0        0    17441 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/general/content.py
+-rw-r--r--   0        0        0    49017 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/general/data_extension.py
+-rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/general/generator.py
+-rw-r--r--   0        0        0     9720 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/general/human.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/pkg_data/__init__.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/pkg_data/chemistry.pkl
+-rw-r--r--   0        0        0    56195 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/pkg_data/tarot.pkl
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/tools/__init__.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/tools/converter.py
+-rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/tools/keygen.py
+-rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/tools/obfuscator.py
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/tools/stats.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/tools/web.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/util/__init__.py
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/util/api.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/util/json_method.py
+-rw-r--r--   0        0        0    13804 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/util/lunar.py
+-rw-r--r--   0        0        0    16620 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/util/path.py
+-rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/util/performance.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/util/pkl.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 absfuyu-3.3.3/src/absfuyu/util/zipped.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/conftest.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_beautiful.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_config.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_data_analysis.py
+-rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_data_extension.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_everything.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_extensions.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_fun.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_game.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_generator.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_logger.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_passwordlib.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_pkg_data.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_tarot.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_tools.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_util.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 absfuyu-3.3.3/tests/test_version.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 absfuyu-3.3.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 absfuyu-3.3.3/LICENSE
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 absfuyu-3.3.3/README.md
+-rw-r--r--   0        0        0     8243 2020-02-02 00:00:00.000000 absfuyu-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 absfuyu-3.3.3/PKG-INFO
```

### Comparing `absfuyu-3.3.2/src/absfuyu/__init__.py` & `absfuyu-3.3.3/src/absfuyu/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 -----
 - [Home page](https://pypi.org/project/absfuyu/)
 - [Documentation](https://absolutewinter.github.io/absfuyu/)
 
 USAGE
 -----
 
-Normal import: 
+Normal import:
 >>> import absfuyu
 >>> help(absfuyu)
 
-Using in cmd (`absfuyu[cli]` required): 
+Using in cmd (`absfuyu[cli]` required):
 ``$ fuyu --help``
 """
 
-
 __title__ = "absfuyu"
 __author__ = "AbsoluteWinter"
 __license__ = "MIT License"
-__version__ = "3.3.2"
+__version__ = "3.3.3"
 __all__ = [
     "core",
     "config",
     "everything",
     "extensions",
     "logger",
     "fun",
```

### Comparing `absfuyu-3.3.2/src/absfuyu/core.py` & `absfuyu-3.3.3/src/absfuyu/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,44 @@
 """
 Absfuyu: Core
 -------------
 Contain type hints and other stuffs
 
-Version: 2.1.10
-Date updated: 05/04/2024 (dd/mm/yyyy)
+Version: 2.2.0
+Date updated: 14/04/2024 (dd/mm/yyyy)
 """
 
 # Module Package
 ###########################################################################
 __all__ = [
-    # module
-    "ModulePackage",
-    "ModuleList",
     # color
-    "Color",
     "CLITextColor",
     # path
     "CORE_PATH",
     "CONFIG_PATH",
     "DATA_PATH",
 ]
 
-ModulePackage = ["all", "beautiful", "extra", "res", "full", "dev"]
-ModuleList = [
-    "config",
-    "extensions",
-    "fun",
-    "game",
-    "general",
-    "pkg_data",
-    "sort",
-    "tools",
-    "util",
-    "version",
-]
+__package_feature__ = ["beautiful", "extra", "res", "full", "dev"]
 
 
-# Library
-###########################################################################
 from pathlib import Path
 
-import colorama
-
 # import sys
 # from sys import version_info as _python_version
 
 # if sys.version_info.minor >= 10:
 #     from importlib.resources import files
 # else:
 #     try:
 #         from importlib_resources import files
 #     except:
 #         raise ImportError("Please install importlib-resources")
 
 
-# Color - colorama
-###########################################################################
-# colorama.init(autoreset=True)
-Color = {
-    "green": colorama.Fore.LIGHTGREEN_EX,
-    "GREEN": colorama.Fore.GREEN,
-    "blue": colorama.Fore.LIGHTCYAN_EX,
-    "BLUE": colorama.Fore.CYAN,
-    "red": colorama.Fore.LIGHTRED_EX,
-    "RED": colorama.Fore.RED,
-    "yellow": colorama.Fore.LIGHTYELLOW_EX,
-    "YELLOW": colorama.Fore.YELLOW,
-    "reset": colorama.Fore.RESET,
-}
-
-
 class CLITextColor:
     """Color code for text in terminal"""
 
     WHITE = "\x1b[37m"
     BLACK = "\x1b[30m"
     BLUE = "\x1b[34m"
     GRAY = "\x1b[90m"
@@ -82,20 +46,11 @@
     RED = "\x1b[91m"
     DARK_RED = "\x1b[31m"
     MAGENTA = "\x1b[35m"
     YELLOW = "\x1b[33m"
     RESET = "\x1b[39m"
 
 
-# Path
-###########################################################################
-# CORE_PATH = Path(os.path.abspath(os.path.dirname(__file__)))
 CORE_PATH = Path(__file__).parent.absolute()
 # CORE_PATH = files("absfuyu")
 CONFIG_PATH = CORE_PATH.joinpath("config", "config.json")
 DATA_PATH = CORE_PATH.joinpath("pkg_data")
-
-
-# Run
-###########################################################################
-if __name__ == "__main__":
-    print(CORE_PATH)
```

### Comparing `absfuyu-3.3.2/src/absfuyu/everything.py` & `absfuyu-3.3.3/src/absfuyu/everything.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
+# flake8: noqa
 """
 Absfuyu: Everything
 -------------------
 Everything has to offer in this package
 
 Version: 2.0.1
 Date updated: 26/11/2023 (mm/dd/yyyy)
 
 Usage:
 ------
 >>> from absfuyu import everything as ab
 """
 
-
 # Library
 ###########################################################################
-from absfuyu.core import *
 from absfuyu.config import *
+from absfuyu.core import *
+from absfuyu.extensions import *
 from absfuyu.fun import *
-from absfuyu.pkg_data import *
+from absfuyu.game import *
+from absfuyu.general import *
 from absfuyu.logger import *
+from absfuyu.pkg_data import *
 from absfuyu.sort import *
-from absfuyu.version import *
-
-from absfuyu.general import *
-from absfuyu.extensions import *
-from absfuyu.game import *
 from absfuyu.tools import *
 from absfuyu.util import *
-
+from absfuyu.version import *
 
 # Is loaded
 ###########################################################################
 __IS_EVERYTHING = True
```

### Comparing `absfuyu-3.3.2/src/absfuyu/logger.py` & `absfuyu-3.3.3/src/absfuyu/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 >>> logger.debug("This logs!")
 """
 
 # Module level
 ###########################################################################
 __all__ = [
     # logger
-    "logger", "compress_for_log",
+    "logger",
+    "compress_for_log",
     # log level
-    "LogLevel"
+    "LogLevel",
 ]
 
 
 # Library
 ###########################################################################
 import logging
 import math
@@ -35,84 +36,91 @@
 
 # Setup
 ###########################################################################
 class LogLevel:
     """
     ``logging``'s log level wrapper + custom log level
     """
+
     TRACE: int = logging.DEBUG - 5
     DEBUG: int = logging.DEBUG
     INFO: int = logging.INFO
     WARNING: int = logging.WARNING
     ERROR: int = logging.ERROR
     CRITICAL: int = logging.CRITICAL
     EXTREME: int = logging.CRITICAL + 10
 
+
 class _LogFormat:
     """Some log format styles"""
-    FULL = "[%(asctime)s] [%(process)-d] [%(module)s] [%(name)s] [%(funcName)s] [%(levelname)-s] %(message)s" # Time|ProcessID|Module|Name|Function|LogType|Message
-    SHORT = "[%(module)s] [%(name)s] [%(funcName)s] [%(levelname)-s] %(message)s" # Module|Name|Function|LogType|Message
-    CONSOLE = "%(asctime)s [%(levelname)5s] %(funcName)s:%(lineno)3d: %(message)s" # Time|LogType|Function|LineNumber|Message
-    FILE = "%(asctime)s [%(levelname)5s] %(filename)s:%(funcName)s:%(lineno)3d: %(message)s" # Time|LogType|FileName|Function|LineNumber|Message
+
+    FULL = "[%(asctime)s] [%(process)-d] [%(module)s] [%(name)s] [%(funcName)s] [%(levelname)-s] %(message)s"  # Time|ProcessID|Module|Name|Function|LogType|Message
+    SHORT = "[%(module)s] [%(name)s] [%(funcName)s] [%(levelname)-s] %(message)s"  # Module|Name|Function|LogType|Message
+    CONSOLE = "%(asctime)s [%(levelname)5s] %(funcName)s:%(lineno)3d: %(message)s"  # Time|LogType|Function|LineNumber|Message
+    FILE = "%(asctime)s [%(levelname)5s] %(filename)s:%(funcName)s:%(lineno)3d: %(message)s"  # Time|LogType|FileName|Function|LineNumber|Message
+
 
 # Create a custom logger
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
 # Create handlers
 ## Console log handler
 console_handler = logging.StreamHandler()
-console_handler.setLevel(LogLevel.TRACE) # Minimum log level
-console_handler.setFormatter(logging.Formatter(_LogFormat.CONSOLE, datefmt="%Y-%m-%d %H:%M:%S"))
+console_handler.setLevel(LogLevel.TRACE)  # Minimum log level
+console_handler.setFormatter(
+    logging.Formatter(_LogFormat.CONSOLE, datefmt="%Y-%m-%d %H:%M:%S")
+)
 logger.addHandler(console_handler)
 
 
 # Functions
 ###########################################################################
 def _compress_list_for_print(iterable: list, max_visible: Optional[int] = 5) -> str:
     """
     Compress the list to be more log-readable
-    
+
     iterable: list
     max_visible: Maximum items can be printed on screen (Minimum: 3)
     """
 
     if max_visible is None or max_visible <= 2:
         max_visible = 5
-    
+
     if len(iterable) <= max_visible:
         return str(iterable)
-    else:        
+    else:
         # logger.debug(f"Max vis: {max_visible}")
         if max_visible % 2 == 0:
-            cut_idx_1 = math.floor(max_visible/2) - 1
-            cut_idx_2 = math.floor(max_visible/2)
+            cut_idx_1 = math.floor(max_visible / 2) - 1
+            cut_idx_2 = math.floor(max_visible / 2)
         else:
-            cut_idx_1 = cut_idx_2 = math.floor(max_visible/2)
-        
+            cut_idx_1 = cut_idx_2 = math.floor(max_visible / 2)
+
         # logger.debug(f"Cut pos: {(cut_idx_1, cut_idx_2)}")
         # temp = [iterable[:cut_idx_1], ["..."], iterable[len(iterable)-cut_idx_2:]]
         # out = list(chain.from_iterable(temp))
         # out = [*iterable[:cut_idx_1], "...", *iterable[len(iterable)-cut_idx_2:]] # Version 2
-        out = f"{str(iterable[:cut_idx_1])[:-1]}, ...,{str(iterable[len(iterable)-cut_idx_2:])[1:]}" # Version 3
+        out = f"{str(iterable[:cut_idx_1])[:-1]}, ...,{str(iterable[len(iterable)-cut_idx_2:])[1:]}"  # Version 3
         # logger.debug(out)
         return f"{out} [Len: {len(iterable)}]"
 
+
 def _compress_string_for_print(text: str, max_visible: Optional[int] = 120) -> str:
     """
     Compress the string to be more log-readable
 
     text: str
     max_visible: Maximum text can be printed on screen (Minimum: 5)
     """
 
     if max_visible is None or max_visible <= 5:
         max_visible = 120
 
-    text = text.replace("\n", " ") # Remove new line
+    text = text.replace("\n", " ")  # Remove new line
     # logger.debug(text)
 
     if len(text) <= max_visible:
         return str(text)
     else:
         cut_idx = math.floor((max_visible - 3) / 2)
         temp = f"{text[:cut_idx]}...{text[len(text)-cut_idx:]}"
@@ -128,116 +136,129 @@
     :returns: Compressed log output
     :rtype: str
     """
 
     if isinstance(object_, list):
         return _compress_list_for_print(object_, max_visible)
 
-    elif isinstance(object_, set) or isinstance(object_, tuple):
+    elif isinstance(object_, (set, tuple)):
         return _compress_list_for_print(list(object_), max_visible)
 
     elif isinstance(object_, dict):
         temp = [{k: v} for k, v in object_.items()]
         return _compress_list_for_print(temp, max_visible)
 
     elif isinstance(object_, str):
         return _compress_string_for_print(object_, max_visible)
 
     else:
         try:
             return _compress_string_for_print(str(object_), max_visible)
-        except:
+        except Exception:
             return object_  # type: ignore
 
 
 # Class
 ###########################################################################
 class _CustomLogger:
     """
     Custom logger [W.I.P]
-    
-    Create a custom logger 
+
+    Create a custom logger
     *Useable but maybe unstable*
     """
+
     def __init__(
-            self,
-            name: str,
-            cwd: Union[str, Path] = ".",
-            log_format: Optional[str] = None,
-            *,
-            save_log_file: bool = False,
-            separated_error_file: bool = False,
-            timed_log: bool = False,
-            date_log_format: Optional[str] = None,
-            error_log_size: int = 1_000_000 # 1 MB
-        ) -> None:
+        self,
+        name: str,
+        cwd: Union[str, Path] = ".",
+        log_format: Optional[str] = None,
+        *,
+        save_log_file: bool = False,
+        separated_error_file: bool = False,
+        timed_log: bool = False,
+        date_log_format: Optional[str] = None,
+        error_log_size: int = 1_000_000,  # 1 MB
+    ) -> None:
         """
         :param name: Custom logger name
         :param cwd: Current working directory
         :param log_format: Log format
         :param save_log_file: Save logs to log file (default: False)
         :param separated_error_file: Save error logs into a separated file (Default: False)
         :param timed_log: Split log file every day. Requirement: `save_log_file = True` (Default: False)
         :param date_log_format: Date format in log
         :param error_log_size: Error log file max size (Default: 1 MB)
         """
         self._cwd = Path(cwd)
         self.log_folder = self._cwd.joinpath("logs")
-        self.log_folder.mkdir(exist_ok=True) # Does not throw exception when folder existed
+        self.log_folder.mkdir(
+            exist_ok=True, parents=True
+        )  # Does not throw exception when folder existed
         self.name = name
         self.log_file = self.log_folder.joinpath(f"{name}.log")
 
         # Create a custom logger
         try:
             self.logger = logging.getLogger(self.name)
-        except:
+        except Exception:
             try:
                 self.logger = logging.getLogger(__name__)
-            except:
+            except Exception:
                 self.logger = logging.getLogger()
         self.logger.setLevel(logging.DEBUG)
 
         if date_log_format is None:
             _date_format = "%Y-%m-%d %H:%M:%S"
         else:
             _date_format = date_log_format
 
         ## Console log handler
         if log_format is None:
             # Time|LogType|Function|LineNumber|Message
-            _log_format = "%(asctime)s [%(levelname)5s] %(funcName)s:%(lineno)3d: %(message)s"
+            _log_format = (
+                "%(asctime)s [%(levelname)5s] %(funcName)s:%(lineno)3d: %(message)s"
+            )
         else:
             _log_format = log_format
         console_handler = logging.StreamHandler()
-        console_handler.setLevel(logging.DEBUG) # Minimum log level
-        _console_log_format = _log_format # Create formatters and add it to handlers
-        _console_formatter = logging.Formatter(_console_log_format, datefmt=_date_format)
+        console_handler.setLevel(logging.DEBUG)  # Minimum log level
+        _console_log_format = _log_format  # Create formatters and add it to handlers
+        _console_formatter = logging.Formatter(
+            _console_log_format, datefmt=_date_format
+        )
         console_handler.setFormatter(_console_formatter)
         self._console_handler = console_handler
-        self.logger.addHandler(self._console_handler) # Add handlers to the logger
+        self.logger.addHandler(self._console_handler)  # Add handlers to the logger
 
         ## Log file handler
         if save_log_file:
             if log_format is None:
                 # Time|LogType|FileName|Function|LineNumber|Message
                 _log_format = "%(asctime)s [%(levelname)5s] %(filename)s:%(funcName)s:%(lineno)3d: %(message)s"
             else:
                 _log_format = log_format
-            file_handler = logging.FileHandler(self.log_file, mode="a", encoding="utf-8")
+            file_handler = logging.FileHandler(
+                self.log_file, mode="a", encoding="utf-8"
+            )
             file_handler.setLevel(logging.DEBUG)
             _file_log_format = _log_format
             _file_formatter = logging.Formatter(_file_log_format, datefmt=_date_format)
             file_handler.setFormatter(_file_formatter)
             self._file_handler = file_handler
             self.logger.addHandler(self._file_handler)
 
             if timed_log:
                 ## Time handler (split log every day)
-                time_handler = _TRFH(self.log_folder.joinpath(f"{self.name}_timed.log"),
-                                     when="midnight", interval=1, encoding="utf-8")
+                time_handler = _TRFH(
+                    self.log_folder.joinpath(f"{self.name}_timed.log"),
+                    when="midnight",
+                    interval=1,
+                    encoding="utf-8",
+                )
                 time_handler.setLevel(logging.DEBUG)
                 time_handler.setFormatter(_file_formatter)
                 self._time_handler = time_handler
                 self.logger.addHandler(self._time_handler)
                 # |   Value  |    Type of interval   |
                 # |:--------:|:---------------------:|
                 # |     S    |        Seconds        |
@@ -250,23 +271,28 @@
         ## Error and above log handler
         if separated_error_file:
             if log_format is None:
                 # Time|LogType|FileName|Function|LineNumber|Message
                 _log_format = "%(asctime)s [%(levelname)5s] %(filename)s:%(funcName)s:%(lineno)3d: %(message)s"
             else:
                 _log_format = log_format
-            error_handler = _RFH(self.log_folder.joinpath(f"{self.name}_error.log"),
-                                 maxBytes=error_log_size, backupCount=1, encoding="utf-8")
+            error_handler = _RFH(
+                self.log_folder.joinpath(f"{self.name}_error.log"),
+                maxBytes=error_log_size,
+                backupCount=1,
+                encoding="utf-8",
+            )
             error_handler.setLevel(logging.ERROR)
             error_handler.setFormatter(_log_format)  # type: ignore
             self._error_handler = error_handler
             self.logger.addHandler(self._error_handler)
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.name})"
+
     def __repr__(self) -> str:
         return self.__str__()
 
     @staticmethod
     def _add_logging_level(
         level_name: str, level_num: int, method_name: Optional[str] = None
     ):
@@ -297,14 +323,15 @@
 
         # This method was inspired by the answers to Stack Overflow post
         # http://stackoverflow.com/q/2183233/2988730, especially
         # http://stackoverflow.com/a/13638084/2988730
         def logForLevel(self, message, *args, **kwargs):
             if self.isEnabledFor(level_num):
                 self._log(level_num, message, args, **kwargs)
+
         def logToRoot(message, *args, **kwargs):
             logging.log(level_num, message, *args, **kwargs)
 
         logging.addLevelName(level_num, level_name)
         setattr(logging, level_name, level_num)
         setattr(logging.getLoggerClass(), method_name, logForLevel)
         setattr(logging, method_name, logToRoot)
```

### Comparing `absfuyu-3.3.2/src/absfuyu/sort.py` & `absfuyu-3.3.3/src/absfuyu/sort.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/version.py` & `absfuyu-3.3.3/src/absfuyu/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,60 @@
 """
 Absfuyu: Version
 ----------------
 Package versioning module
 
-Version: 2.1.0
-Date updated: 06/04/2024 (dd/mm/yyyy)
+Version: 2.1.1
+Date updated: 14/04/2024 (dd/mm/yyyy)
 """
 
-# Module level
-###########################################################################
 __all__ = [
     # Options
     "ReleaseOption",
     "ReleaseLevel",
     # Class
     "Version",
     "Bumper",
     "PkgVersion",
 ]
 
 
-# Library
-###########################################################################
 import json
 import re
 import subprocess
 from typing import List, Tuple, TypedDict, Union
 from urllib.error import URLError
 from urllib.request import Request, urlopen
 
 from absfuyu.logger import logger
 
 
-# Class
-###########################################################################
 class ReleaseOption:
     """
     ``MAJOR``, ``MINOR``, ``PATCH``
     """
 
     MAJOR: str = "major"
     MINOR: str = "minor"
     PATCH: str = "patch"
 
-    # @staticmethod
     def all_option() -> List[str]:  # type: ignore
         """Return a list of release options"""
         return [__class__.MAJOR, __class__.MINOR, __class__.PATCH]  # type: ignore
 
 
 class ReleaseLevel:
     """
     ``FINAL``, ``DEV``, ``RC``
     """
 
     FINAL: str = "final"
     DEV: str = "dev"
     RC: str = "rc"  # Release candidate
 
-    # @staticmethod
     def all_level() -> List[str]:  # type: ignore
         """Return a list of release levels"""
         return [__class__.FINAL, __class__.DEV, __class__.RC]  # type: ignore
 
 
 class VersionDictFormat(TypedDict):
     """
@@ -116,15 +108,19 @@
     def __str__(self) -> str:
         return self.version
 
     def __repr__(self) -> str:
         if self.release_level.startswith(ReleaseLevel.FINAL):
             return f"{self.__class__.__name__}(major={self.major}, minor={self.minor}, patch={self.patch})"
         else:
-            return f"{self.__class__.__name__}(major={self.major}, minor={self.minor}, patch={self.patch}, release_level={self.release_level}, serial={self.serial})"
+            return (
+                f"{self.__class__.__name__}("
+                f"major={self.major}, minor={self.minor}, patch={self.patch}, "
+                f"release_level={self.release_level}, serial={self.serial})"
+            )
 
     def __format__(self, format_spec: str) -> str:
         """
         Change format of an object.
         Avaiable option: ``full``
 
         Usage
@@ -181,14 +177,19 @@
             Version tuple in correct format
 
         Returns
         -------
         Version
             Version
 
+        Raises
+        ------
+        ValueError
+            Wrong tuple format
+
 
         Example:
         --------
         >>> test = Version.from_tuple((1, 0, 0))
         >>> test.version
         1.0.0
         """
@@ -199,14 +200,41 @@
         elif len(iterable) == 3:
             return cls(iterable[0], iterable[1], iterable[2])  # major.minor.patch only
         else:
             raise ValueError("iterable must have len of 5 or 3")
 
     @classmethod
     def from_str(cls, version_string: str):
+        """
+        Convert to ``Version`` from a ``str``
+
+        Parameters
+        ----------
+        version_string : str
+            | Version str in correct format
+            | ``<major>.<minor>.<patch>``
+            | ``<major>.<minor>.<patch>.<release level><serial>``
+
+        Returns
+        -------
+        Version
+            Version
+
+        Raises
+        ------
+        ValueError
+            Wrong version_string format
+
+
+        Example:
+        --------
+        >>> test = Version.from_str("1.0.0")
+        >>> test.version
+        1.0.0
+        """
         short_ver_pattern = re.compile(r"\b(\d)+\.(\d+)\.(\d+)\b")
         long_ver_pattern = re.compile(r"\b(\d)+\.(\d+)\.(\d+)\.(dev|rc|final)(\d+)\b")
         ver = version_string.lower().strip()
 
         long_ver = re.search(long_ver_pattern, ver)
         if long_ver:
             return cls.from_tuple(long_ver.groups())  # type: ignore
@@ -252,28 +280,25 @@
 class Bumper(Version):
     """Version bumper"""
 
     def _bump_ver(self, release_option: str) -> None:
         """
         Bumping major, minor, patch
         """
-        logger.debug(f"Before: {self.version}")
 
         if release_option.startswith(ReleaseOption.MAJOR):
             self.major += 1
             self.minor = 0
             self.patch = 0
         elif release_option.startswith(ReleaseOption.MINOR):
             self.minor += 1
             self.patch = 0
         else:
             self.patch += 1
 
-        logger.debug(f"After: {self.version}")
-
     def bump(
         self, *, option: str = ReleaseOption.PATCH, channel: str = ReleaseLevel.FINAL
     ) -> None:
         """
         Bump current version (internally)
 
         Parameters
@@ -294,18 +319,18 @@
         1.0.0
         >>> test.bump()
         >>> test.version
         1.0.1
         """
         # Check conditions - use default values if fail
         if option not in ReleaseOption.all_option():
-            logger.debug(ReleaseOption.all_option())
+            logger.warning(f"Available option: {ReleaseOption.all_option()}")
             option = ReleaseOption.PATCH
         if channel not in ReleaseLevel.all_level():
-            logger.debug(ReleaseLevel.all_level())
+            logger.warning(f"Available level: {ReleaseLevel.all_level()}")
             channel = ReleaseLevel.FINAL
         logger.debug(f"Target: {option} {channel}")
 
         # Bump ver
         if channel.startswith(ReleaseLevel.FINAL):  # Final release level
             if self.release_level in [
                 ReleaseLevel.RC,
@@ -358,27 +383,35 @@
         except URLError as e:
             if hasattr(e, "reason"):
                 logger.error("Failed to reach server.")
                 logger.error("Reason: ", e.reason)
             elif hasattr(e, "code"):
                 logger.error("The server couldn't fulfill the request.")
                 logger.error("Error code: ", e.code)
-        except:
+        except Exception:
             logger.error("Fetch failed!")
         else:
             return response.read().decode()
 
     def _get_latest_version_legacy(self) -> str:
         """
         Load data from PyPI's RSS -- OLD
         """
         rss = f"https://pypi.org/rss/project/{self.package_name}/releases.xml"
         xml_file: str = self._fetch_data_from_server(rss)
-        ver = xml_file[xml_file.find("<item>") : xml_file.find("</item>")]  # First item
-        version = ver[ver.find("<title>") + len("<title>") : ver.find("</title>")]
+        ver = xml_file[
+            xml_file.find("<item>") : xml_file.find(
+                "</item>"
+            )  # noqa: E203
+        ]  # First item
+        version = ver[
+            ver.find("<title>") + len("<title>") : ver.find(
+                "</title>"
+            )  # noqa: E203
+        ]
         return version
 
     def _load_data_from_json(self, json_link: str) -> dict:
         """
         Load data from api then convert to json
         """
         json_file: str = self._fetch_data_from_server(json_link)
@@ -410,15 +443,15 @@
 
         :param force_update: Auto update the package when run (Default: ``False``)
         :type force_update: bool
         """
 
         try:
             latest = self._get_latest_version()
-        except:
+        except Exception:
             latest = self._get_latest_version_legacy()
 
         try:
             import importlib
 
             _pk = importlib.__import__(self.package_name)
             current: str = _pk.__version__
@@ -430,15 +463,15 @@
         if current == latest:
             print(f"You are using the latest version ({latest})")
         else:
             if force_update:
                 print(f"Newer version ({latest}) available. Upgrading...")
                 try:
                     self._get_update()
-                except:
+                except Exception:
                     print(
                         f"""
                     Unable to perform update.
                     Please update manually with:
                     pip install -U {self.package_name}=={latest}
                     """
                     )
```

### Comparing `absfuyu-3.3.2/src/absfuyu/config/__init__.py` & `absfuyu-3.3.3/src/absfuyu/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,16 +225,16 @@
         # Get setting
         setting = self._get_setting(name)
         setting_value: bool = setting.value
 
         # Change value
         try:
             self.change_setting(name, not setting_value)
-        except:
-            raise SystemExit("This setting is not type: bool")
+        except Exception:
+            raise SystemExit("This setting is not type: bool")  # noqa: B904
 
     def add_setting(self, name: str, value: Any, default: Any, help_: str = "") -> None:
         """
         Add ``Setting`` if not exist
 
         Parameters
         ----------
@@ -262,15 +262,15 @@
 
         Parameters
         ----------
         name : str
             Name of the setting
         """
         name = name.strip().lower().replace(" ", _SPACE_REPLACE)
-        self.settings = [x for x in self.settings if not x.name == name]
+        self.settings = [x for x in self.settings if x.name != name]
         self.save()
 
     def welcome(self) -> None:
         """Run first-run script (if any)"""
         self.change_setting("first-run", False)
```

### Comparing `absfuyu-3.3.2/src/absfuyu/config/config.json` & `absfuyu-3.3.3/src/absfuyu/config/config.json`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/extensions/beautiful.py` & `absfuyu-3.3.3/src/absfuyu/extensions/beautiful.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 ------------------
 A decorator that makes output more beautiful
 
 Version: 1.0.2
 Date updated: 24/11/2023 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     "beautiful_output",
     "print",
     "demo",
 ]
@@ -38,15 +37,15 @@
 
     if ABSFUYU_CONFIG._get_setting("auto-install-extra").value:
         __cmd: str = "python -m pip install -U absfuyu[beautiful]".split()
         from subprocess import run as __run
 
         __run(__cmd)
     else:
-        raise SystemExit("This feature is in absfuyu[beautiful] package")
+        raise SystemExit("This feature is in absfuyu[beautiful] package")  # noqa: B904
 else:
     BEAUTIFUL_MODE = True
 
 
 # Function
 ###########################################################################
 def beautiful_output(
```

### Comparing `absfuyu-3.3.2/src/absfuyu/extensions/dev/__init__.py` & `absfuyu-3.3.3/src/absfuyu/extensions/dev/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # type: ignore
+# flake8: noqa
+
 """
 Absfuyu: Development
 --------------------
 Some stuffs that are not ready to use yet.
 Use at your own risk, everything is subject to change
 
 Version: 2.0.0
```

### Comparing `absfuyu-3.3.2/src/absfuyu/extensions/dev/password_hash.py` & `absfuyu-3.3.3/src/absfuyu/extensions/dev/password_hash.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # type: ignore
+# flake8: noqa
+
 # Library
 ##############################################################
 import hashlib as __hash
 import os as __os
 from typing import Dict as __Dict
 from typing import NewType as __NewType
 from typing import TypeVar as __TypeVar
```

### Comparing `absfuyu-3.3.2/src/absfuyu/extensions/dev/passwordlib.py` & `absfuyu-3.3.3/src/absfuyu/extensions/dev/passwordlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # type: ignore
+# flake8: noqa
+
 """
 Absfuyu: Passwordlib
 --------------------
 Password library
 
 Version: 1.0.0dev1
 Date updated: 30/11/2023 (dd/mm/yyyy)
 """
 
-
 # Library
 ###########################################################################
 # from collections import namedtuple
 import hashlib
 import os
 import random
 import re
-from typing import Dict, List, Optional, Union
+from typing import List, Optional
 
 from absfuyu_res import DATA
 
 from absfuyu.general.data_extension import DictExt, Text
 from absfuyu.general.generator import Charset, Generator
 from absfuyu.logger import logger
 from absfuyu.util import set_min
@@ -234,15 +235,15 @@
         Myomectomies7-Sully4-Torpedomen7-Netful2-Begaud8
         """
 
         def convert_func(value: str):
             if first_letter_cap:
                 value = value.title()
             if include_number:
-                value += str(random.choice(range(0, 10)))
+                value += str(random.choice(range(10)))
             return value
 
         if not block_divider:
             block_divider = "-"
 
         return block_divider.join(
             [convert_func(random.choice(self.words)) for _ in range(num_of_blocks)]
```

### Comparing `absfuyu-3.3.2/src/absfuyu/extensions/dev/project_starter.py` & `absfuyu-3.3.3/src/absfuyu/extensions/dev/project_starter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # type: ignore
+# flake8: noqa
+
 """
 Absfuyu: Project starter
 ------------------------
 
 Version: 1.0.0dev1
 Date updated: 01/12/2023 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["get_parser"]
 
 
 # Library
 ###########################################################################
```

### Comparing `absfuyu-3.3.2/src/absfuyu/extensions/dev/shutdownizer.py` & `absfuyu-3.3.3/src/absfuyu/extensions/dev/shutdownizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # type: ignore
+# flake8: noqa
+
 """
 Absfuyu: Shutdownizer
 ---------------------
 This shutdowns
 
 Version: 1.0.0dev
 Date updated: 27/11/2023 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["ShutDownizer"]
 
 
 # Library
 ###########################################################################
```

### Comparing `absfuyu-3.3.2/src/absfuyu/extensions/extra/__init__.py` & `absfuyu-3.3.3/src/absfuyu/extensions/extra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,11 @@
 # Library
 ###########################################################################
 
 
 # Function
 ###########################################################################
 
-
 # Run
 ###########################################################################
 if __name__ == "__main__":
     pass
```

### Comparing `absfuyu-3.3.2/src/absfuyu/extensions/extra/data_analysis.py` & `absfuyu-3.3.3/src/absfuyu/extensions/extra/data_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 ------------------------------
 Extension for ``pd.DataFrame``
 
 Version: 2.1.3
 Date updated: 20/03/2024 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = [
     # Function
     "compare_2_list",
     # Support
     "CityData",
@@ -36,17 +35,17 @@
 # import matplotlib.pyplot as plt
 # from scipy import stats
 # from dateutil.relativedelta import relativedelta
 import numpy as np
 import pandas as pd
 from deprecated import deprecated
 from deprecated.sphinx import deprecated as sphinx_deprecated
-from deprecated.sphinx import versionadded, versionchanged
+from deprecated.sphinx import versionadded
 
-from absfuyu.logger import logger  # type: ignore
+from absfuyu.logger import logger
 from absfuyu.util import set_min, set_min_max
 
 
 # Function
 ###########################################################################
 @deprecated(reason="Not needed", version="3.1.0")
 @sphinx_deprecated(reason="Not needed", version="3.1.0")
@@ -470,15 +469,15 @@
         -------
         DataAnalystDataFrame
             Modified DataFrame
         """
         for column in columns:
             try:
                 self.drop(columns=[column], inplace=True)
-            except:
+            except Exception:
                 logger.debug(f"{column} column does not exist")
                 # pass
         return self
 
     # Drop right-most columns
     def drop_rightmost(self, num_of_cols: int = 1):
         """
@@ -736,15 +735,15 @@
         Returns
         -------
         DataAnalystDataFrame
             Modified DataFrame
         """
         try:
             self[column_name] = self[column_name].fillna(fill)
-        except:
+        except Exception:
             self.add_blank_column(column_name, fill_when_not_exist)
         return self
 
     # Split DataFrame
     def split_na(self, by_column: str) -> SplittedDF:
         """
         Split DataFrame into 2 parts:
@@ -805,15 +804,15 @@
             Modified DataFrame
         """
         # Clean
         try:
             self[destination_column] = self[
                 destination_column
             ].str.strip()  # Remove trailing space
-        except:
+        except Exception:
             pass
 
         # Logic
         col_df = self.show_distribution(destination_column)
 
         # Rename
         if top is not None:
```

### Comparing `absfuyu-3.3.2/src/absfuyu/fun/WGS.py` & `absfuyu-3.3.3/src/absfuyu/fun/WGS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# flake8: noqa
 """
 Absfuyu: WGS
 ------------
 Wolf's Gravestone
 
 - This module is not affiliated with miHoYo/Hoyoverse.
 - Genshin Impact, game content and materials are trademarks and copyrights of miHoYo/Hoyoverse.
@@ -11,15 +12,14 @@
 
 Usage:
 ------
 >>> test = WGS()
 >>> print(test.pixel_art())
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["WGS"]
 
 
 # Library
 ###########################################################################
```

### Comparing `absfuyu-3.3.2/src/absfuyu/fun/__init__.py` & `absfuyu-3.3.3/src/absfuyu/fun/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     Get random activity from ``boredapi`` website
 
     :rtype: str
     """
     try:
         api = APIRequest("https://www.boredapi.com/api/activity")
         return api.fetch_data_only().json()["activity"]  # type: ignore
-    except:
+    except Exception:
         return "FAILED"
 
 
 def force_shutdown():
     """Force the computer to shutdown"""
     # Get operating system
     os_name = sys.platform
```

### Comparing `absfuyu-3.3.2/src/absfuyu/fun/tarot.py` & `absfuyu-3.3.3/src/absfuyu/fun/tarot.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/game/__init__.py` & `absfuyu-3.3.3/src/absfuyu/game/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,166 +1,168 @@
-# type: ignore
 """
 Absfuyu: Game
 -------------
 Contain some game that can be played on terminal
 
-Version: 1.0.2
-Date updated: 24/11/2023 (mm/dd/yyyy)
+Version: 1.1.0
+Date updated: 14/04/2024 (mm/dd/yyyy)
 """
 
-
-# Module Package
-###########################################################################
 __all__ = [
     "game_escapeLoop",
     "game_RockPaperScissors",
 ]
 
 
-# Library
-###########################################################################
-from random import choice as __randChoice
+import random
+import time
+
+from .game_stat import GameStats
+
+# Escape loop
+_ESCAPE_LOOP_GAME_MSG = """\
+Are you sure about this?
+Don't leave me =((
+I can't believe you did this to me!
+Are you very much sure?
+I'll be sad. Pick again please.
+I still don't believe you.
+Choose again.
+You actually have to answer the correct keyword
+I think you need to choose again.
+Last chance!
+Okay okay, i believe you ;)
+Almost there.
+I can do this all day
+So close!
+You can't escape from me.
+How are you still here, just to suffer?
+Never gonna give you up
+Never gonna let you down
+"""
 
 
-# Default games
-###########################################################################
 def game_escapeLoop() -> None:
     """Try to escape the infinite loop"""
 
     init = True
     welcome_messages = [
         "Congrats! You are now stuck inside an infinite loop.",
         "Do you want to escape this loop?",
     ]
 
-    num1 = __randChoice([2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])
-    num2 = __randChoice([2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])
+    num1 = random.choice(range(2, 13))
+    num2 = random.choice(range(2, 13))
     hidden_answer = str(num1 * num2)
 
-    game_messages = [
-        "Are you sure about this?",
-        "Don't leave me =((",
-        "I can't believe you did this to me!",
-        "Are you very much sure?",
-        "I'll be sad. Pick again please.",
-        "I still don't believe you.",
-        "Choose again.",
-        "You actually have to answer the correct keyword",
-        "I think you need to choose again.",
-        "Last chance!",
-        "Okay okay, i believe you ;)",
-        "Almost there.",
-        "I can do this all day",
-        "So close!",
-        "You can't escape from me.",
-        "How are you still here, just to suffer?",
-        "Never gonna give you up",
-        "Never gonna let you down",
+    gm_msg = {x for x in _ESCAPE_LOOP_GAME_MSG.splitlines() if len(x) > 0}
+    game_messages = list(gm_msg) + [
         f"Hint 01: The keyword is: {num1}",
-        f"Hint 02: *{num2}",
+        f"Hint 02: {num2}",
     ]
 
     congrats_messages = ["Congratulation! You've escaped."]
 
+    start_time = time.time()
     while True:
         # Welcome
         if init:
             for x in welcome_messages:
                 print(x)
             answer = str(input())
             init = False
 
         # Random text
-        mess = __randChoice(game_messages)
+        mess = random.choice(game_messages)
         print(mess)
 
         # Condition check
         answer = str(input())
         if answer == hidden_answer:
             for x in congrats_messages:
                 print(x)
+            stop_time = time.time()
             break
-    pass
+    print(f"= Escaped in {stop_time-start_time:,.2f}s =")
 
 
-def game_RockPaperScissors(hard_mode=False):
+# Rock Paper Scissors
+def game_RockPaperScissors(hard_mode: bool = False) -> GameStats:
     """
     Rock Paper Scissors
 
     :param hard_mode: The bot only win or draw (Default: ``False``)
     :type hard_mode: bool
     """
 
-    state_dict = {0: "rock", 1: "paper", 2: "scissors"}
+    state_dict = {"0": "rock", "1": "paper", "2": "scissors"}
 
     init = True
 
     end_message = "end"
 
     welcome_messages = [
         "Welcome to Rock Paper Scissors",
         f"Type '{end_message}' to end",
     ]
 
     game_messages = [
         "Pick one option to begin:",
+        " ".join([f"{k}={v}" for k, v in state_dict.items()]),
     ]
 
-    game_summary = {"Win": 0, "Draw": 0, "Lose": 0}
+    game_summary = GameStats()
 
     while True:
         # Welcome
         if init:
             for x in welcome_messages:
                 print(x)
             init = False
 
         # Game start
         print("")
         for x in game_messages:
             print(x)
-        print(state_dict)
 
         # Player's choice
-        answer = input()
+        answer = input().strip().lower()
 
         # Condition check
         if answer == end_message:
             print(game_summary)
             break
 
         elif answer not in ["0", "1", "2"]:
             print("Invalid option. Choose again!")
 
         else:
             # Calculation
-            answer = int(answer)
             if hard_mode:
-                if answer == 0:
-                    game_choice = __randChoice([0, 1])
-                if answer == 1:
-                    game_choice = __randChoice([1, 2])
-                if answer == 2:
-                    game_choice = __randChoice([0, 2])
+                if answer == "0":
+                    game_choice = random.choice(["0", "1"])
+                if answer == "1":
+                    game_choice = random.choice(["1", "2"])
+                if answer == "2":
+                    game_choice = random.choice(["0", "2"])
             else:
-                game_choice = __randChoice([0, 1, 2])
+                game_choice = random.choice(["0", "1", "2"])
             print(f"You picked: {state_dict[answer]}")
             print(f"BOT picked: {state_dict[game_choice]}")
 
-            if answer == 2 and game_choice == 0:
+            if answer == "2" and game_choice == "0":
                 print("You Lose!")
-                game_summary["Lose"] += 1
-            elif answer == 0 and game_choice == 2:
+                game_summary.update_score("lose")
+            elif answer == "0" and game_choice == "2":
                 print("You Win!")
-                game_summary["Win"] += 1
+                game_summary.update_score("win")
             elif answer == game_choice:
                 print("Draw Match!")
-                game_summary["Draw"] += 1
+                game_summary.update_score("draw")
             elif answer > game_choice:
                 print("You Win!")
-                game_summary["Win"] += 1
+                game_summary.update_score("win")
             else:
                 print("You Lose!")
-                game_summary["Lose"] += 1
+                game_summary.update_score("lose")
 
     return game_summary
```

### Comparing `absfuyu-3.3.2/src/absfuyu/game/sudoku.py` & `absfuyu-3.3.3/src/absfuyu/game/sudoku.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,48 +8,41 @@
 
 Credit:
 -------
 - [Hardest sudoku](https://www.telegraph.co.uk/news/science/science-news/9359579/Worlds-hardest-sudoku-can-you-crack-it.html)
 - [Solve algo](https://www.techwithtim.net/tutorials/python-programming/sudoku-solver-backtracking/)
 """
 
-
-# Module level
-###########################################################################
 __all__ = ["Sudoku"]
 
 
-# Library
-###########################################################################
-from typing import List, Tuple
+from typing import List, Literal, Tuple
 
 
-# Class
-###########################################################################
 class Sudoku:
     def __init__(self, sudoku_data: List[List[int]]) -> None:
         self.data = sudoku_data
         # self._original = sudoku_data # Make backup
         self._row_len = len(self.data)
         self._col_len = len(self.data[0])
         # self.solved = None
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.export_to_string()})"
 
     def __repr__(self) -> str:
         return self.__str__()
 
-    def export_to_string(self, *, style: str = "dot") -> str:
+    def export_to_string(self, *, style: Literal["dot", "zero"] = "dot") -> str:
         """
         Export Sudoku data to string form
 
         Parameters
         ----------
-        style : str
+        style : Literal["dot", "zero"]
             - "zero": ``0`` is ``0``
             - "dot": ``0`` is ``.``
 
         Returns
         -------
         str
             Sudoku string
@@ -282,15 +275,15 @@
          \u2503  4 3 8  \u2503  5 2 6  \u2503  9 1 7  \u2503
          \u2503  7 9 6  \u2503  3 1 8  \u2503  4 5 2  \u2503
          \u2516\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u251A
         """
         self._solve()
         # self.solved = self.data
         # self.data = self._original
-        return __class__(self.data)  # type: ignore
+        return self.__class__(self.data)
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     test = Sudoku.hardest_sudoku()
     print(test.solve().to_board_form())
```

### Comparing `absfuyu-3.3.2/src/absfuyu/game/tictactoe.py` & `absfuyu-3.3.3/src/absfuyu/general/content.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,561 +1,565 @@
-# type: ignore
 """
-Game: Tic Tac Toe
------------------
-
-Version: 1.0.3
-Date update: 24/11/2023 (mm/dd/yyyy)
+Absfuyu: Content
+----------------
+Handle .txt file
+
+Version: 1.2.6
+Date updated: 05/04/2024 (dd/mm/yyyy)
+
+Usage:
+------
+>>> from absfuyu.general.content import ContentLoader
 """
 
+# Module level
+###########################################################################
+__all__ = ["ContentLoader", "Content", "LoadedContent"]
 
-# Library
-##############################################################
-import random as __random
-import time as __time
-from typing import List as __List
-from typing import Optional as __Optional
-
-from absfuyu import core as __core
-from absfuyu.game.tictactoe2 import GameMode
-
-# Tic Tac Toe
-##############################################################
-
-# GAME SETTING
-X = "X"
-O = "O"
-BLANK = " "
-POS_SPLIT = ","
-END_BREAK = "END"
-__C = __core.Color
-
-
-# FUNCTIONS
-def __test_case_3x3(num: int = 0):
-    case = {
-        1: [[X,X,X],
-            [BLANK,BLANK,BLANK],
-            [BLANK,BLANK,BLANK]],
-        2: [[BLANK,BLANK,BLANK],
-            [X,X,X],
-            [BLANK,BLANK,BLANK]],
-        3: [[BLANK,BLANK,BLANK],
-            [BLANK,BLANK,BLANK],    
-            [X,X,X]],
-        4: [[X,BLANK,BLANK],
-            [X,BLANK,BLANK],
-            [X,BLANK,BLANK]],
-        5: [[BLANK,X,BLANK],
-            [BLANK,X,BLANK],
-            [BLANK,X,BLANK]],
-        6: [[BLANK,BLANK,X],
-            [BLANK,BLANK,X],
-            [BLANK,BLANK,X]],
-        7: [[X,BLANK,BLANK],
-            [BLANK,X,BLANK],
-            [BLANK,BLANK,X]],
-        8: [[BLANK,BLANK,X],
-            [BLANK,X,BLANK],
-            [X,BLANK,BLANK]],
-    }
-    try:
-        import numpy as np
-        for k, v in case.items():
-            case[k] = np.array(v)
-    except:
-        pass
-    
-    if num < 1:
-        return case
-    return case[num]
-
-
-def __gen_board(row_size: int, col_size: int, content: str = BLANK):
-    """
-    Generate board game (with or without `numpy`)
-
-    Parameter:
-    ---
-    row_size : int
-        Number of rows
-
-    col_size : int
-        Number of columns
-
-    content : str
-        What should be filled inside the board
-    
-    Return:
-    ---
-    Game board
-    """
-    
-    try:
-        import numpy as np
-    except:
-        np = None
-    
-    if np is None:
-        board = [[BLANK for _ in range(row_size)] for _ in range(col_size)]
-    else:
-        board = np.full((row_size, col_size), content)
-    return board
-
-def __check_state(table):
-    """
-    Check game winning state
-    
-    Parameter:
-    ---
-    table : numpy.ndarray | list[list[str]]
-        Game board
-    
-    Return:
-    ---
-    X | O | BLANK
-    """
-
-    # Data
-    nrow, ncol = len(table), len(table[0])
-
-    # Check rows
-    for row in range(nrow):
-        if len(set(table[row])) == 1:
-            # return list(set(table[row]))[0]
-            key = list(set(table[row]))[0]
-            return {"key": key, "location": "row", "pos": row} # modified
-
-    # Check cols
-    for col in range(ncol):
-        temp = [table[row][col] for row in range(nrow)]
-        if len(set(temp)) == 1:
-            # return list(set(temp))[0]
-            key = list(set(temp))[0]
-            return {"key": key, "location": "col", "pos": col} # modified
-    
-    # Check diagonal
-    diag1 = [table[i][i] for i in range(len(table))]
-    if len(set(diag1)) == 1:
-        # return list(set(diag1))[0]
-        key = list(set(diag1))[0]
-        return {"key": key, "location": "diag", "pos": 1} # modified
-    
-    diag2 = [table[i][len(table)-i-1] for i in range(len(table))]
-    if len(set(diag2)) == 1:
-        # return list(set(diag2))[0]
-        key = list(set(diag2))[0]
-        return {"key": key, "location": "diag", "pos": 2} # modified
-    
-    # Else
-    # return BLANK
-    return {"key": BLANK}
-
-def __print_board(table):
-    """
-    Print Tic Tac Toe board
-
-    Parameter:
-    ---
-    table : numpy.ndarray | list[list[str]]
-        Game board
-    """
-    nrow, ncol = len(table), len(table[0])
-    length = len(table)
-    print(f"{'+---'*length}+")
-    for row in range(nrow):
-        for col in range(ncol):
-            print(f"| {table[row][col]} ", end="")
-        print(f"|\n{'+---'*length}+")
 
-def __win_hightlight(table):
-    """
-    Hight light the win by removing other placed key
-
-    Parameter:
-    ---
-    table : numpy.ndarray | list[list[str]]
-        Game board
-    """
-
-    # Get detailed information
-    detail = __check_state(table)
-    loc = detail["location"]
-    loc_line = detail["pos"]
-
-    # Make new board
-    board = __gen_board(len(table), len(table[0]))
-
-    # Fill in the hightlighted content
-    if loc.startswith("col"):
-        for i in range(len(board)):
-            board[i][loc_line] = detail['key']
-    elif loc.startswith("row"):
-        for i in range(len(board)):
-            board[loc_line][i] = detail['key']
-    else:
-        if loc_line == 1:
-            for i in range(len(board)):
-                board[i][i] = detail['key']
+# Library
+###########################################################################
+import json
+import random
+import re
+from collections import Counter
+from itertools import chain
+from pathlib import Path
+from typing import List, Optional
+
+from unidecode import unidecode
+
+from absfuyu.logger import logger
+
+
+# Class
+###########################################################################
+class Content:
+    """
+    Contain data
+
+    Data format: list[str, list[str]]
+        where: ``str: data``; ``list[str]: data tags``
+    """
+
+    def __init__(self, data: list) -> None:
+        self.data: str = str(data[0])
+        self.tag: list = data[1]
+        # logger.debug(self.__dict__)
+
+    def __str__(self) -> str:
+        # return f"{self.data} | {self.tag}"
+        return str(self.data)
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def unidecoded(self) -> "Content":
+        """
+        Convert data through ``unidecode`` package
+
+        Returns
+        -------
+        Content
+            ``unidecoded`` Content
+        """
+        return self.__class__([unidecode(self.data), list(map(unidecode, self.tag))])
+
+    def to_text(self) -> str:
+        """
+        Convert back into text
+
+        Returns
+        -------
+        str
+            Text
+        """
+        # hard code
+        tags = ",".join(self.tag)
+        return f"{self.data}|{tags}"
+
+    def short_form(self, separator: str = ",") -> str:
+        """
+        Short form show only first item when separated by ``separator``
+
+        Parameters
+        ----------
+        separator : str
+            Default: ``","``
+
+        Returns
+        -------
+        str
+            Short form
+        """
+        if not separator.startswith(","):
+            logger.debug(f"Separated symbol: {separator}")
+        return self.data.split(separator)[0]
+
+    def handle_address(
+        self, address_separator: str = ",", *, first_item_not_address: bool = True
+    ) -> "Content":
+        """
+        Handle ``self.data`` as address and then update the address into ``self.tag``
+
+        Parameters
+        ----------
+        address_separator : str
+            | Split the address by which character
+            | (Default: ``","``)
+
+        first_item_not_address : bool
+            Set to ``False`` when ``<splited data>[0]`` is not part of an address
+
+        Returns
+        -------
+        Content
+            Handled Content
+
+
+        Example:
+        --------
+        >>> test = "Shop A, 22 ABC Street, DEF District, GHI City"
+        >>> # After handle_address()
+        ["Shop A", "22 ABC Street", "DEF District", "GHI City"]
+
+        >>> # After handle_address(first_item_not_address = False)
+        ["22 ABC Street", "DEF District", "GHI City"]
+        """
+        if first_item_not_address:
+            temp = self.data.split(address_separator)
         else:
-            for i in range(len(board)):
-                board[i][len(board)-i-1] = detail['key']
-    
-    # Output
-    return board
-
-def __is_blank(table, pos: __List[int]):
-    """Check if current slot is filled"""
-    return table[pos[0]][pos[1]] == BLANK
-
-def __convert_bot_output(pos: __List[int]):
-    """
-    Turn to real pos by:
-    - +1 to row and col
-    - convert into str
-    """
-    for i in range(len(pos)):
-        pos[i] = str(int(pos[i])+1)
-    return pos
-
-def __generate_surround_move(table, pos: __List[int]):
-    """
-    Generate all surrounding move of a position
-    """
-    surround_move = [
-        [pos[0]-1, pos[1]], # Up pos
-        [pos[0]+1, pos[1]], # Down pos
-        [pos[0], pos[1]-1], # Left pos
-        [pos[0], pos[1]+1], # Right pos
-        [pos[0]-1, pos[1]-1], # Up left pos
-        [pos[0]-1, pos[1]+1], # Up right pos
-        [pos[0]+1, pos[1]-1], # Down left pos
-        [pos[0]+1, pos[1]+1], # Down right pos
-    ]
-    surround_move = {
-        "U": [pos[0]-1, pos[1]], # Up pos
-        "D": [pos[0]+1, pos[1]], # Down pos
-        "L": [pos[0], pos[1]-1], # Left pos
-        "R": [pos[0], pos[1]+1], # Right pos
-        "UL": [pos[0]-1, pos[1]-1], # Up left pos
-        "UR": [pos[0]-1, pos[1]+1], # Up right pos
-        "DL": [pos[0]+1, pos[1]-1], # Down left pos
-        "DR": [pos[0]+1, pos[1]+1], # Down right pos
-    }
-    # Remove value outside of board
-    # output = []
-    # for x in surround_move:
-    #     condition = [
-    #         x[0] < 0 or x[1] < 0,
-    #         x[0] >= len(table) or x[1] >= len(table)
-    #     ]
-    #     if any(condition):
-    #         continue
-    #     output.append(x)
-    # return output
-    for k, v in surround_move.items():
-        condition = [
-            v[0] < 0 or v[1] < 0,
-            v[0] >= len(table) or v[1] >= len(table)
-        ]
-        if any(condition):
-            surround_move.pop(k)
-            continue
-        # output.append(x)
-    return surround_move
-
-def __generate_random_move(table):
-    """
-    Generate a random move from board game
-    """
-    while True:
-        output = [
-            __random.randint(0, len(table)-1),
-            __random.randint(0, len(table)-1)
-        ]
-        if __is_blank(table, output):
-            break
-    return __convert_bot_output(output)
-
-def __bot_move(table, pos: __List[int] = None, debug: bool = False):
-    """
-    Calculate position to place for BOT
-
-    Parameters:
-    ---
-    table : numpy.ndarray | list[list[str]]
-        Game board
-    
-    pos : list[int]
-        previous move
-    """
-
-    if debug:
-        print("Init Data:")
-        print(table)
-        print(pos)
-        # print(opponent)
-
-    if pos is None:
-        return __generate_random_move(table)
-
-    # Smart move: position that around previous game move
-    valid_move = __generate_surround_move(table, pos)
-    valid_move = list(valid_move.values())
-    if debug:
-        print("Smart move:")
-        print(valid_move)
-    
-    # Filtered smart move: take only the placable position
-    filtered_move = []
-    for x in valid_move:
-        if __is_blank(table, x):
-            filtered_move.append(x)
-        # else:
-        #     opponent = table[pos[0], pos[1]]
-        #     if table[x[0], x[1]] == opponent:
-        #         temp = __generate_surround_move(table, x)
-        #         for v in temp:
-        #             if __is_blank(table, v):
-        #                 filtered_move.append(v)
-                # print(temp)
-
-    
-    if debug:
-        print("Filtered move:")
-        print(filtered_move)
-    
-    if not filtered_move:
-        # If invalid then return a random move
-        return __generate_random_move(table)
-    
-    # else
-    while True:
-        rand_move = __random.choice(filtered_move)
-        if any([
-            rand_move[0] < 0,
-            rand_move[0] >= len(table),
-            rand_move[1] < 0,
-            rand_move[1] >= len(table)
-        ]):
-            continue
-        
-        if __is_blank(table, rand_move):
-            rand_move = __convert_bot_output(rand_move)
-            if debug:
-                print("Chosen smart move:")
-                print(rand_move)
-            break
-    
-    # print(rand_move)
-    return rand_move
-
-def bot_ttt(table, pos: __List[int] = None):
-    """Smart bot i guess"""
-    free_slots = []
-    for i in range(len(table)):
-        for j in range(len(table[0])):
-            if table[i][j] == BLANK:
-                free_slots.append([i, j])
-    if not free_slots:
-        return None
-    
-    if pos is not None:
-        sur = __generate_surround_move(table, pos)
-        print(sur)
-
-        counter = []
-        for k, v in sur.items():
-            if table[v[0]][v[1]] == table[pos[0]][pos[1]]:
-                try:
-                    if k == "R": counter.append(sur["L"])
-                except: pass
-                try:
-                    if k == "L": counter.append(sur["R"])
-                except: pass
-                try:
-                    if k == "U": counter.append(sur["D"])
-                except: pass
-                try:
-                    if k == "D": counter.append(sur["U"])
-                except: pass
-                try:
-                    if k == "UL": counter.append(sur["DR"])
-                except: pass
-                try:
-                    if k == "UR": counter.append(sur["DL"])
-                except: pass
-                try:
-                    if k == "DL": counter.append(sur["UR"])
-                except: pass
-                try:
-                    if k == "DR": counter.append(sur["UL"])
-                except: pass
-
-        if not counter:
-            pass
-
-    return free_slots
-
-def game_tictactoe(
-        size: int = 3,
-        mode: str = GameMode.ONE_V_BOT,
-        smarter_bot: bool = False,
-        board_game: __Optional[bool] = True,
-        bot_time: float = 0,
-        show_stats: bool = False,
-    ):
-    """
-    Tic Tac Toe
+            logger.debug(
+                f"First item ({self.data.split(address_separator)[0]}) is not part of an address"
+            )
+            temp = self.data.split(address_separator)[1:]
+
+        new_tag = [x.strip().lower() for x in temp]
+        logger.debug(f"Current tags: {self.tag}")
+        logger.debug(f"New tags: {new_tag}")
+        self.tag = list(set(self.tag + new_tag))
+        logger.debug(f"Final tags: {self.tag} Len: {len(self.tag)}")
+
+        return self.__class__([self.data, self.tag])
+
+
+class LoadedContent(List[Content]):
+    """
+    Contain list of ``Content``
+    """
+
+    def __str__(self) -> str:
+        # return f"{self.__class__.__name__} - Total: {len(self)}"
+        return f"{self.__class__.__name__}({[x.data for x in self]})"
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def apply(self, func) -> "LoadedContent":
+        """
+        Apply function to each entry
+
+        :param func: Callable function
+        :type func: Callable
+        :rtype: LoadedContent
+        """
+        return self.__class__(func(x.data) for x in self)
+
+    @classmethod
+    def load_from_json(cls, file: Path) -> "LoadedContent":
+        """
+        Use this method to load data from ``.json`` file from ``to_json()`` method
+
+        Parameters
+        ----------
+        file : Path
+            Path to ``.json`` file
+
+        Returns
+        -------
+        LoadedContent
+            Loaded content from ``.json`` file
+        """
+        with open(file) as json_file:
+            parsed_json: dict = json.load(json_file)
+        out = [Content(list(x.values())) for x in parsed_json]
+        return cls(out)
+
+    @property
+    def tags(self) -> list:
+        """A list contains all available tag"""
+        temp = chain.from_iterable([x.tag for x in self])
+        out = list(set(temp))
+        logger.debug(f"Found {len(out)} {'tags' if len(out) > 1 else 'tag'}")
+        return sorted(out)
+
+    def tag_count(self) -> Counter:
+        """
+        Count number of tags
+
+        :rtype: Counter
+        """
+        temp = chain.from_iterable([x.tag for x in self])
+        logger.debug(temp)
+        return Counter(temp)
+
+    def filter(self, tag: str) -> "LoadedContent":
+        """
+        Filter out entry with ``tag``
+
+        :param tag: Tag to filter
+        :type tag: str
+        :rtype: LoadedContent
+        """
+        tag = tag.strip().lower()
+        logger.debug(f"Tag: {tag}")
+        if tag not in self.tags:
+            # tag = random.choice(self.tags)
+            # logger.debug(f"Tag not exist, changing to a random tag... {tag}")
+            logger.warning(f'"{tag}" tag does not exist')
+            _avail_tag = ", ".join(list(dict(self.tag_count().most_common(5)).keys()))
+            raise ValueError(
+                f"Available tags: {_avail_tag},..."
+                f"\nMore tag at: `{self.__class__.__name__}.tags`"
+            )
+        return self.__class__([x for x in self if tag in x.tag])
+
+    def find(self, keyword: str) -> "LoadedContent":
+        """
+        Return all entries that include ``keyword``
+
+        :param keyword: Keyword to find
+        :type keyword: str
+        :rtype: LoadedContent
+        """
+        temp = self.__class__(
+            [x for x in self if x.data.lower().find(keyword.lower()) >= 0]
+        )
+        if temp:
+            logger.debug(f"Found {len(temp)} {'entries' if len(temp) > 1 else 'entry'}")
+        else:
+            logger.debug("No result")
+        return temp
 
-    Parameters
-    ----------
-    size : int
-        board size
-
-    mode : str
-        "1v1": Player vs player
-        "1v0": Player vs BOT
-        "0v0": BOT vs BOT
-    
-    smarter_bot : bool
-        W.I.P
-        New bot's behaviour
-    
-    board_game : True | False | None
-        True: draw board
-        False: print array
-        None: no board or array
-
-    bot_time : float
-        time sleep between each bot move
-        [Default: 0]
-    
-    show_stats : bool
-        Print current game stats
-        [Default: False]
-    
-    Returns
-    ------
-    dict
-        Game stats
-    """
+    def short_form(self, separator: str = ",") -> List[str]:
+        """
+        Shows only first item when separated by ``separator`` of ``Content.data``
+
+        Parameters
+        ----------
+        separator : str
+            Default: ``","``
+
+        Returns
+        -------
+        list[str]
+            Short form
+        """
+        return [x.short_form(separator) for x in self]
+
+    def pick_one(self, tag: Optional[str] = None) -> Content:
+        """
+        Pick a random entry
+
+        Parameters
+        ----------
+        tag : str | None
+            Pick a random entry with ``tag``
+            (Default: None)
+
+        Returns
+        -------
+        Content
+            Random entry
+        """
+        if tag:
+            temp = self.filter(tag)
+            logger.debug(f"Tag: {tag}")
+            return random.choice(temp)
+        return random.choice(self)
+
+    def handle_address(
+        self, address_separator: str = ",", *, first_item_not_address: bool = True
+    ) -> "LoadedContent":
+        """
+        Execute ``Content.handle_address()`` on every ``self.data`` of ``Content``
+
+        Parameters
+        ----------
+        address_separator : str
+            | Split the address by which character
+            | (Default: ``","``)
+
+        first_item_not_address : bool
+            Set to ``False`` when ``<splited data>[0]`` is not part of an address
+
+        Returns
+        -------
+        LoadedContent
+            Handled Content
+
+
+        Example:
+        --------
+        >>> test = "Shop A, 22 ABC Street, DEF District, GHI City"
+        >>> # After handle_address()
+        ["Shop A", "22 ABC Street", "DEF District", "GHI City"]
+
+        >>> # After handle_address(first_item_not_address = False)
+        ["22 ABC Street", "DEF District", "GHI City"]
+        """
+        return self.__class__(
+            [
+                x.handle_address(
+                    address_separator=address_separator,
+                    first_item_not_address=first_item_not_address,
+                )
+                for x in self
+            ]
+        )
+
+    def to_json(self, no_accent: bool = False) -> str:
+        """
+        Convert data into ``.json`` file
+
+        Parameters
+        ----------
+        no_accent : bool
+            | when ``True``: convert the data through ``unidecode`` package
+            | (Default: ``False``)
+
+        Returns
+        -------
+        str
+            Data
+        """
+        if no_accent:
+            out = [x.unidecoded().__dict__ for x in self]
+        else:
+            out = [x.__dict__ for x in self]
+        logger.debug(out)
+        return json.dumps(out, indent=2)
+
+    def to_text(self, no_accent: bool = False) -> str:
+        """
+        Convert data into ``.txt`` file
+
+        Parameters
+        ----------
+        no_accent : bool
+            | when ``True``: convert the data through ``unidecode`` package
+            | (Default: ``False``)
+
+        Returns
+        -------
+        str
+            Data
+        """
+        if no_accent:
+            out = [x.unidecoded().to_text() for x in self]
+        else:
+            out = [x.to_text() for x in self]
+        logger.debug(out)
+        return "\n".join(out)
+
+
+class ContentLoader:
+    """
+    This load data from ``.txt`` file
+
+    Content format:
+    ``<content><split_symbol><tags separated by <tag_separate_symbol>>``
+    """
+
+    def __init__(
+        self,
+        file_path: Path,
+        characteristic_detect: bool = True,
+        tag_dictionary: Optional[dict] = None,
+        *,
+        comment_symbol: str = "#",
+        split_symbol: str = "|",
+        tag_separate_symbol: str = ",",
+    ) -> None:
+        """
+        Parameters
+        ----------
+        file_path : str
+            file location/file to load
+
+        characteristic_detect : bool
+            detect whether the content is long, short, or a question
+            (default: ``True``)
+
+        tag_dict : dict
+            custom tag pattern
+            format: ``{"keyword": "tag",...}``
+            example: ``{"apple": "fruit", "orange": "fruit"}``
+
+        comment_symbol : str
+            symbol that `ContentLoader` will ignore
+            (default: ``"#"``)
+
+        split_symbol : str
+            symbol that `ContentLoader` will split content and tags
+            (default: ``"|"``)
+
+        tag_separate_symbol : str
+            symbol that `ContentLoader` will split between tags
+            (default: ``","``)
+        """
+        # file
+        self.file = Path(file_path)
+
+        # characteristic detect
+        self.characteristic_detect: bool = characteristic_detect
+
+        # tag dictionary
+        if tag_dictionary is None:
+            # logger.debug("No tag patern available")
+            self.tag_dictionary: dict = dict()
+        else:
+            logger.debug(
+                f"Tag pattern available: "
+                f"{len(tag_dictionary)} {'entries' if len(tag_dictionary) > 1 else 'entry'} "
+                f"({len(set(tag_dictionary.values()))} unique "
+                f"{'tags' if len(set(tag_dictionary.values())) > 1 else 'tag'})"
+            )
+            self.tag_dictionary = tag_dictionary
+
+        # symbol stuff
+        assert (
+            comment_symbol != split_symbol
+        ), "comment_symbol and split_symbol should have different values"
+        assert (
+            tag_separate_symbol != split_symbol
+        ), "tag_separate_symbol and split_symbol should have different values"
+        self.comment_symbol: str = comment_symbol
+        self.split_symbol: str = split_symbol
+        self.tag_separate_symbol: str = tag_separate_symbol
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}({self.__dict__})"
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def content_format(self) -> str:
+        """
+        Shows current content format
+
+        Returns
+        -------
+        str
+            Current content format
+
+
+        Example:
+        --------
+        >>> ContentLoader(".").content_format()
+        # This line will be ignored
+        <content> | <tag1>, <tag2>
+        """
+        out = (
+            f"{self.comment_symbol} This line will be ignored\n"
+            f"<content> {self.split_symbol} "
+            f"<tag1>{self.tag_separate_symbol} <tag2>"
+        )
+        return out
+
+    def load(self) -> list:
+        """
+        Load content from ``self.file``
+
+        Returns
+        -------
+        list
+            List of content
+        """
+        with open(self.file, "r", encoding="utf-8") as data:
+            logger.debug("Loading data...")
+            dat = []
+            check = []
+
+            for i, x in enumerate(data.readlines()):
+                x = x.strip()
+                if x.startswith(self.comment_symbol) or len(x) == 0:
+                    continue  # skip comment and empty lines
+                logger.debug(
+                    f"### Loop {i+1} #####################################################################"
+                )
+
+                temp = x.split(self.split_symbol)
+                if len(temp) != 2:
+                    logger.debug(f"Split len: {len(temp)}")
+                    logger.warning(
+                        f"The current entry is missing data or tag: {x[:20]}..."
+                    )
+
+                temp[0] = temp[0].strip()
+                if temp[0].lower() not in check:
+                    check.append(temp[0].lower())  # check for dupes
+
+                    # tag
+                    additional_tags = []
+                    for k, v in self.tag_dictionary.items():
+                        key = k.strip().lower()
+                        val = temp[0].lower()
+                        regex_pattern = f"[^a-zA-Z0-9]({key})[^a-zA-Z0-9]|^({key})[^a-zA-Z0-9]|[^a-zA-Z0-9]({key})$"
+                        if re.search(regex_pattern, val) is not None or val.startswith(
+                            key
+                        ):
+                            # regex has a bug (or idk if it's a bug or not) that
+                            # doesn't recognise when there is only one word in the sentence
+                            # therefore use `val.startswith(key)` to fix
+                            additional_tags.append(v.strip().lower())
+
+                    if self.characteristic_detect:
+                        long_short = (120, 20)  # setting
+                        if len(temp[0]) > long_short[0]:
+                            additional_tags.append("long")
+                        if len(temp[0]) < long_short[1]:
+                            additional_tags.append("short")
+                        if temp[0][-1].startswith("?"):
+                            additional_tags.append("question")
+                    if additional_tags:
+                        logger.debug(f"Additional tags: {additional_tags}")
+
+                    try:
+                        tags = [
+                            tag.strip() for tag in temp[1].strip().lower().split(",")
+                        ]  # separate and strip tags
+                        logger.debug(f"Tags: {tags}")
+                    except Exception:
+                        logger.warning("No tag found in the original string")
+                        if additional_tags:
+                            tags = additional_tags
+                        else:
+                            tags = ["unspecified"]
+                            logger.debug('Assigned "unspecified" tag')
+
+                    tags.extend(additional_tags)
+                    final_tags = list(set(tags))
+                    logger.debug(f"Final tags: {final_tags} Len: {len(final_tags)}")
 
-    # Init game
-    board = __gen_board(size, size)
-    filled = 0
-    current_player = X
-    # state = __check_state(board)
-    state = __check_state(board)["key"]
-    BOT = False
-    BOT2 = False
-
-    # Welcome message
-    if board_game is not None:
-        print(f"""\
-{__C['GREEN']}Welcome to Tic Tac Toe!
-
-{__C['YELLOW']}Rules: Match lines vertically, horizontally or diagonally
-{__C['YELLOW']}{X} goes first, then {O}
-{__C['RED']}Type '{END_BREAK}' to end the game{__C['reset']}""")
-    else:
-        print("Tic Tac Toe")
-
-    # Check gamemode
-    game_mode = [
-        "1v1", # Player vs player
-        "1v0", # Player vs BOT
-        "0v0" # BOT vs BOT
-    ]
-    if mode not in game_mode:
-        mode = game_mode[1] # Force vs BOT
-    if mode.startswith("1v0"):
-        BOT = True
-    if mode.startswith("0v0"):
-        BOT = True
-        BOT2 = True
-    
-    # Game
-    if board_game:
-        __print_board(board)
-    elif board_game is None:
-        pass
-    else:
-        print(board)
-
-    place_pos = None
-    while state == BLANK and filled < size**2:
-        if board_game is not None:
-            print(f"{__C['BLUE']}{current_player}'s turn:{__C['reset']}")
-        
-        try: # Error handling
-            if (BOT and current_player == O) or BOT2:
-                if smarter_bot:
-                    move = __bot_move(board, place_pos)
+                    dat.append([temp[0], final_tags])  # add everything
                 else:
-                    move = __generate_random_move(board)
-                str_move = POS_SPLIT.join(move)
-                move = str_move
-
-            else:
-                move = input(f"Place {__C['BLUE']}{current_player}{__C['reset']} at {__C['BLUE']}<row{POS_SPLIT}col>:{__C['reset']} ")
-            
-            if move.upper() == END_BREAK: # Failsafe
-                print(f"{__C['RED']}Game ended{__C['reset']}")
-                break
-            
-            move = move.split(POS_SPLIT)
-            row = int(move[0])
-            col = int(move[1])
-            place_pos = [row-1, col-1]
-
-            if __is_blank(board, place_pos):
-                board[place_pos[0]][place_pos[1]] = current_player
-                filled += 1
-            
-            else: # User and BOT error
-                if board_game is not None:
-                    print(f"{__C['RED']}Invalid move, please try again{__C['reset']}")
-                continue
-        
-        except: # User error
-            if board_game is not None:
-                print(f"{__C['RED']}Invalid move, please try again{__C['reset']}")
-            continue
-        
-        state = __check_state(board)["key"]
-        if board_game:
-            __print_board(board)
-        elif board_game is None:
-            pass
-        else:
-            print(board)
+                    logger.debug(f"Found duplicates, {x} removed")
 
-        # state = __check_state(board)
-        if state != BLANK:
-            print(f"{__C['GREEN']}{state} WON!{__C['reset']}")
-            if board_game:
-                __print_board(__win_hightlight(board))
-            break
-
-        # Change turn
-        if BOT2: # BOT delay
-            __time.sleep(bot_time)
-        
-        if current_player == X:
-            current_player = O
-        else:
-            current_player = X
+        return dat
 
-    if state == BLANK and filled == size**2:
-        print(f"{__C['YELLOW']}Draw Match!{__C['reset']}")
-    
-    # Game stats
-    game_stats = {
-        "Total move": filled,
-        "Win by": None if state==BLANK else state,
-    }
-    if show_stats:
-        print(f"{__C['BLUE']}GAME STATS:{__C['reset']}")
-        for k, v in game_stats.items():
-            print(f"{__C['YELLOW']}{k}: {v}{__C['reset']}")
-    return game_stats
+    def load_content(self) -> LoadedContent:
+        """
+        Load data into a list of ``Content``
+
+        Returns
+        -------
+        LoadedContent
+            Loaded content
+        """
+        return LoadedContent(map(Content, self.load()))
+
+
+# Run
+###########################################################################
+if __name__ == "__main__":
+    logger.setLevel(10)
```

### Comparing `absfuyu-3.3.2/src/absfuyu/game/tictactoe2.py` & `absfuyu-3.3.3/src/absfuyu/game/tictactoe.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,26 @@
 Game: Tic Tac Toe
 -----------------
 
 Version: 2.0.3
 Date updated: 05/04/2024 (mm/dd/yyyy)
 """
 
-# Module level
-###########################################################################
 __all__ = ["TicTacToe", "GameMode"]
 
 
-# Library
-###########################################################################
-# from collections import namedtuple
 import random
 import time
-from typing import Dict, List, Literal, NamedTuple, Union
+from typing import List, Literal, NamedTuple
 
 from absfuyu.core import CLITextColor
 
-# Class
-###########################################################################
 BoardGame = List[List[str]]
 
 
-# Pos = namedtuple("Pos", ["row", "col"])  # Position
 class Pos(NamedTuple):
     """Position"""
 
     row: int
     col: int
 
 
@@ -71,15 +63,15 @@
 
         # Board size
         self.row_size = game_size
         self.col_size = game_size
 
         # Game setting
         self.X = x
-        self.O = o
+        self.O = o  # noqa: E741
         self.BLANK = blank
         self.POS_SPLIT = position_split_symbol
         self.END_BREAK = end_break_word
         self.welcome_message = welcome_message
 
         # Init board
         self.board = self._gen_board()
@@ -294,15 +286,15 @@
 
                 else:  # User and BOT error
                     print(
                         f"{CLITextColor.RED}Invalid move, please try again{CLITextColor.RESET}"
                     )
                     continue
 
-            except:  # User error
+            except Exception:  # User error
                 print(
                     f"{CLITextColor.RED}Invalid move, please try again{CLITextColor.RESET}"
                 )
                 continue
 
             state = self._check_state().key
             self._print_board(self.board)
@@ -318,13 +310,7 @@
             if current_player == self.X:
                 current_player = self.O
             else:
                 current_player = self.X
 
         if state == self.BLANK and filled == self.row_size**2:
             print(f"{CLITextColor.YELLOW}Draw Match!{CLITextColor.RESET}")
-
-
-# Run
-###########################################################################
-if __name__ == "__main__":
-    pass
```

### Comparing `absfuyu-3.3.2/src/absfuyu/game/wordle.py` & `absfuyu-3.3.3/src/absfuyu/game/wordle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 """
 Game: Wordle Solver
 -------------------
 
-Version: 1.1.3
-Date updated: 05/04/2024 (dd/mm/yyyy)
+Version: 1.1.4
+Date updated: 14/04/2024 (dd/mm/yyyy)
 
 Usage:
 ------
->>> Wordle.solve()
+>>> Wordle().solve()
 
 Credit:
 -------
 - [Code](https://www.inspiredpython.com/article/solving-wordle-puzzles-with-basic-python)
 - [Words](https://raw.githubusercontent.com/dwyl/english-words/master/words_dictionary.json)
 """
 
-# Library
-###########################################################################
+__all__ = ["Wordle"]
+
 import operator
 import string
 from collections import Counter
 from itertools import chain
+from typing import List, Set, Tuple
 
 import requests
 
-from absfuyu.logger import logger
-
-# Settings
-###########################################################################
 OFFLINE_WORDS = """\
 aahed,aalii,aargh,aaron,abaca,abaci,aback,abada,abaff,abaft,abaka,abama,abamp,aband,abase,abash,abask,abate,abaue,abave,abaze,abbas,abbes,abbey,abbie,abbot,abdal,abdat,abdom,abeam,abear,abede,abele,abend,aberr,abets,abhor,abide,abidi,abies,abilo,abime,abkar,abler,ables,ablet,ablow,abmho,abner,abnet,abode,abody,abohm,aboil,aboma,aboon,abord,abort,abote,about,above,abram,abray,abret,abrim,abrin,abris,abrus,absee,absey,absis,absit,abstr,abuna,abune,abura,abuse,abush,abuta,abuts,abuzz,abwab,abyes,abysm,abyss,acale,acana,acapu,acara,acari,acast,acate,accel,accoy,accra,accts,accum,accur,accus,acedy,acerb,aceta,achar,ached,achen,acher,aches,achoo,achor,acids,acidy,acier,acies,acing,acini,ackee,acker,ackey,aclys,acmes,acmic,acned,acnes,acock,acoin,acold,acoma,acone,acool,acorn,acost,acoup,acrab,acred,acres,acrid,acroa,acron,acrux,acryl,acted,actin,acton,actor,actos,actus,acuan,acute,acyls,adage,adagy,adams,adapa,adapt,adati,adaty,adawe,adawn,adays,adcon,addax,addda,added,adder,addie,addio,addis,addle,addnl,adead,adeem,adeep,adela,adeps,adept,adfix,adiel,adieu,adion,adios,adits,adjag,adlai,adlay,adlet,adman,admen,admin,admit,admix,admov,admrx,adnex,adobe,adobo,adolf,adopt,adore,adorn,adown,adoxa,adoxy,adoze,adpao,adrad,adret,adrip,adrop,adrue,adsum,adult,adunc,adure,adusk,adust,adyta,adzer,adzes,aecia,aedes,aeger,aegir,aegis,aegle,aeons,aequi,aeric,aerie,aeron,aesir,aesop,aetat,aevia,aevum,aface,afara,afars,afear,affix,afgod,afifi,afire,aflat,afley,aflow,afoam,afoot,afore,afoul,afray,afret,afric,afrit,afros,after,agada,agade,again,agama,agami,agamy,agape,agars,agasp,agast,agata,agate,agaty,agave,agaze,agena,agend,agene,agent,agers,agete,agger,aggie,aggro,aggry,aggur,aghan,aghas,agiel,agile,aging,agios,agism,agist,aglee,aglet,agley,aglow,agmas,agnat,agnel,agnes,agnus,agoge,agoho,agone,agons,agony,agora,agrah,agral,agree,agria,agric,agrin,agrom,agron,agsam,agues,aguey,agura,agush,agust,ahead,aheap,ahems,ahind,ahint,ahmed,ahmet,ahold,aholt,ahong,ahsan,ahull,ahunt,ahura,ahush,ahwal,aided,aider,aides,aiery,aiger,aigre,ailed,ailie,aillt,aimak,aimed,aimee,aimer,ainee,ainoi,ainus,aioli,airan,aired,airer,airns,airth,airts,aisle,aitch,aitis,aiver,aiwan,aizle,ajaja,ajari,ajava,ajhar,ajiva,ajuga,akala,akali,akasa,akebi,akees,akeki,akela,akene,aking,akkad,aknee,aknow,akpek,akron,akule,akund,alack,alada,alain,alaki,alala,alamo,aland,alane,alang,alani,alans,alant,alapa,alarm,alary,alate,alawi,alban,albas,albee,albin,album,albus,albyn,alcae,alces,alcid,alcor,alday,aldea,alden,alder,aldim,aldol,aldus,aleak,
 aleck,alecs,alefs,aleft,alenu,aleph,alert,aleut,alfas,alfet,alfin,alfur,algae,algal,algas,algic,algid,algin,algol,algor,algum,alhet,alias,alibi,alice,alick,alida,alids,alien,aliet,alife,alifs,align,alike,alima,aline,alish,aliso,alisp,alist,alite,ality,alive,aliya,alkes,alkin,alkyd,alkyl,allah,allan,allay,allen,aller,alley,allez,allie,allis,allod,alloo,allot,allow,alloy,allyl,almah,alman,almas,almeh,almes,almon,almud,almug,alnus,alody,aloed,aloes,aloft,alogy,aloha,aloid,aloin,alois,aloma,alone,along,aloof,alosa,alose,aloud,alout,alowe,alpax,alpen,alpha,alpid,altar,alter,altho,altin,altos,altun,altus,aluco,alula,alums,alure,aluta,alvah,alvan,alvar,alvia,alvin,alvus,alway,amaas,amadi,amaga,amahs,amain,amala,amalg,amang,amani,amant,amapa,amara,amass,amate,amati,amaut,amaze,amban,ambar,ambas,ambay,amber,ambit,amble,ambon,ambos,ambry,ameba,ameed,ameen,ameer,amelu,amend,amene,amens,ament,amess,amhar,amias,amice,amici,amide,amido,amids,amies,amiga,amigo,amine,amini,amino,amins,amire,amirs,amish,amiss,amita,amity,amlet,amman,ammer,ammos,amnia,amnic,amoke,amoks,amole,among,amora,amort,amour,amove,amowt,amper,amphi,ample,amply,ampul,ampyx,amrit,amsel,amuck,amula,amuse,amuze,amvis,amylo,amyls,amzel,anabo,anack,anama,anana,anasa,ancha,ancle,ancon,ancor,ancre,andes,andia,andor,andre,anear,anele,anend,anent,angas,angel,anger,angia,angie,angka,angle,anglo,angor,angry,angst,angus,anhyd,aniba,anice,anigh,anile,anils,anima,anime,animi,animo,anion,anise,anita,anjan,anjou,ankee,anker,ankhs,ankle,ankou,ankus,anlas,anlet,anlia,anmia,annal,annam,annas,annat,annet,annex,annie,anniv,annot,annoy,annul,annum,annus,anoas,anode,anoia,anoil,anole,anoli,anomy,anorn,anour,anous,anova,ansae,ansar,ansel,anser,antae,antal,antar,antas,anted,antes,antic,antiq,antis,anton,antra,antre,antsy,antum,anura,anury,anvil,anzac,aoife,aorta,aotea,aotes,aotus,aouad,apace,apaid,apair,apama,apart,apass,apast,apeak,apeek,apers,apert,aperu,apery,aphid,aphis,aphra,apian,apiin,apili,apina,aping,apiol,apios,apish,apism,apium,apnea,apoda,apods,apoop,aport,apout,appal,appar,appay,appel,appet,apple,apply,appmt,appro,apptd,appui,apres,april,apron,apses,apsid,apsis,aptal,apter,aptly,aquae,aquas,araba,arabs,araby,araca,arace,arach,arado,arage,arain,arake,araks,aramu,arank,arara,araru,arase,arati,araua,arawa,arber,arbor,arcae,arced,arces,archd,arche,archt,archy,arcos,arcus,ardea,ardeb,arder,ardor,ardri,aread,areae,areal,arean,arear,areas,areca,areek,areel,arefy,areic,arena,arend,areng,arent,arere,arest,arete,argal,argan,argas,argel,argid,argil,
 argin,argle,argol,argon,argos,argot,argue,argus,arhar,arhat,arian,arias,ariel,aries,ariki,arils,arioi,arion,ariot,arise,arish,arist,arite,arith,arius,arjun,arkab,arkie,arles,armed,armer,armet,armil,armit,armor,arneb,arnee,arnut,aroar,arock,aroid,aroma,aroon,aroph,arose,arpen,arrah,arras,arrau,array,arret,arrgt,arrha,arrie,arris,arrow,arroz,arses,arsis,arsle,arson,arsyl,artal,artar,artel,arter,artha,artic,artie,artly,artou,artsy,artus,aruac,aruke,arulo,arums,arupa,arusa,arval,arvel,arvos,aryan,aryls,arzan,arzun,asale,asana,asaph,asarh,ascan,ascii,ascon,ascot,ascry,ascus,asdic,asgmt,ashed,ashen,asher,ashes,ashet,ashir,ashot,ashur,asian,aside,askar,asked,asker,askew,askip,askoi,askos,aslop,asoak,asoka,aspca,aspen,asper,aspic,aspis,assai,assam,assay,asses,asset,assis,assoc,assot,astay,astel,aster,astir,astor,astre,astur,asuri,asway,aswim,asyla,asyle,async,atake,atame,atavi,ataxy,ateba,atees,atelo,ately,athar,athel,atilt,atimy,ating,atlas,atlee,atman,atmas,atmid,atmos,atnah,atoke,atole,atoll,atoms,atomy,atone,atony,atopy,atour,atren,atria,atrip,attal,attar,atter,attic,attid,attle,attry,atule,atune,atwin,atypy,aubin,aucan,aucht,audad,audio,audit,aueto,augen,auger,auget,aught,augur,aulae,aulas,aulic,auloi,aulos,aumil,aunts,aunty,aurae,aural,aurar,auras,aurei,aures,auric,aurin,aurir,auris,aurum,auryl,autem,autor,autos,autre,auxil,auxin,avahi,avail,avale,avant,avars,avast,avell,avena,avens,aveny,avera,avern,avers,avert,avery,avgas,avian,avick,aview,avile,avine,avion,aviso,avoid,avoir,avoke,avoue,avour,avowe,avows,awabi,awacs,awaft,await,awake,awald,awalt,awane,award,aware,awarn,awash,awave,aways,awber,aweek,aweel,awest,aweto,awful,awhet,awhir,awide,awing,awink,awiwi,awkly,awned,awner,awoke,awols,awork,axels,axers,axial,axile,axils,axine,axing,axiom,axion,axite,axled,axles,axman,axmen,axoid,axone,axons,ayahs,ayelp,ayens,ayins,aylet,ayllu,ayond,ayont,ayous,ayuyu,azans,azide,azido,azine,azlon,azoch,azofy,azoic,azole,azons,azote,azoth,azoxy,aztec,azure,azury,azyme,
 baaed,baals,babai,babas,babby,babel,babes,babis,babka,bable,baboo,babua,babul,babus,bacao,bacca,baccy,bache,bacin,bacis,backs,backy,bacon,badan,baddy,badge,badju,badly,badon,baffs,baffy,bafta,bagdi,bagel,bagge,baggy,bagie,bagio,bagle,bagne,bagre,bahai,baham,bahan,bahar,bahay,bahoe,bahoo,bahts,bahur,bahut,baign,baile,bailo,bails,baioc,bairn,baith,baits,baiza,baize,bajan,bajau,bajra,bajri,bakal,baked,baken,baker,bakes,bakie,bakli,bakra,balai,balak,balan,balao,balas,balat,balau,balds,baldy,baled,balei,baler,bales,balks,balky,balli,ballo,balls,bally,balms,balmy,balon,baloo,balor,balow,balsa,balti,balun,balut,balza,bamah,banak,banal,banat,banba,banca,banco,banda,bande,bandh,bandi,bando,bands,bandy,baned,banes,banff,banga,bange,bangs,bangy,bania,banig,banjo,banks,banky,banns,bantu,banty,banus,banya,barad,barat,barba,barbe,barbs,barbu,barde,bardo,bards,bardy,bared,barer,bares,baret,barff,barfs,barfy,barge,bargh,baria,baric,barid,barie,barih,baris,barit,barks,barky,barly,barms,barmy,barns,barny,baroi,baron,barra,barre,barry,barse,barth,barye,basad,basal,basan,basat,based,baser,bases,basic,basil,basin,basis,baske,basks,bason,basos,bassa,bassi,basso,bassy,basta,baste,basti,basto,basts,basyl,batad,batak,batan,batch,batea,bated,batel,bater,bates,bathe,baths,batik,batis,baton,batta,batts,battu,batty,batwa,baubo,bauch,bauds,bauge,bauld,baulk,baume,bauno,baure,bauta,bavin,bawds,bawdy,bawke,bawls,bawly,bawra,bawty,bayal,bayed,bayok,bayou,bazar,bazoo,beach,beads,beady,beaks,beaky,beala,beams,beamy,beano,beans,beant,beany,beard,bearm,bears,beast,beata,beath,beati,beats,beaus,beaut,beaux,bebar,bebat,bebay,bebed,bebog,bebop,becap,becco,beche,becks,becky,becry,becut,bedad,beday,bedel,beden,bedew,bedim,bedin,bedip,bedog,bedot,bedub,bedur,bedye,beech,beedi,beefs,beefy,beele,beent,beeps,beers,beery,beest,beeth,beets,beety,beeve,befan,befit,befog,befop,befur,begad,began,begar,begat,begay,begem,beget,begin,begob,begod,begot,begum,begun,begut,behap,behav,behen,behew,beice,beige,beigy,beild,being,beira,beisa,bejan,bejel,bejig,bekah,bekko,belah,belam,belap,belar,belat,belay,belch,belee,belga,belie,belis,bella,belle,belli,bello,bells,belly,below,belts,belue,belve,bemad,beman,bemar,bemas,bemat,bemba,bemix,bemol,bemud,benab,bench,benda,bends,bendy,benes,benet,benic,benim,benin,benjy,benne,benni,benny,bensh,bents,benty,benzo,beode,bepat,bepaw,bepen,bepun,berat,beray,beret,bergh,bergs,bergy,berme,berms,berne,berob,beroe,berri,berry,berth,berun,beryl,beryx,besan,besee,beset,besew,besin,besit,besom,besot,bespy,besra,
 bessi,bessy,bests,betag,betas,betel,betes,beths,betis,beton,betso,betsy,betta,betty,bevel,bever,bevil,bevor,bevue,bevvy,bewet,bewig,bewit,bewry,bezan,bezel,bezil,bezzi,bezzo,bhaga,bhalu,bhang,bhara,bhava,bhili,bhima,bhoot,bhuts,biabo,biali,bialy,bibbs,bibby,bibio,bible,bicep,bices,bichy,bidar,biddy,bided,bider,bides,bidet,bidri,bidry,bield,biens,biers,bifer,biffs,biffy,bifid,bigae,bigam,bigas,biggy,bigha,bight,bigly,bigot,bihai,biham,bijou,biked,biker,bikes,bikie,bikol,bilbi,bilbo,bilby,bilch,biles,bilge,bilgy,bilic,bilin,bilio,bilks,billa,bills,billy,bilos,bilsh,bimah,bimas,bimbo,binal,bindi,binds,bines,binge,bingo,bingy,binit,binna,binny,bints,biome,biont,biose,biota,biped,bipod,birch,birde,birds,birdy,birks,birky,birle,birls,birma,birne,birny,biron,birri,birrs,birse,birsy,birth,bises,biset,bisie,bisks,bisme,bison,bisso,bisti,bitch,bited,biter,bites,bitis,bitsy,bitte,bitts,bitty,biune,bivvy,bixin,bizel,bizen,bizes,bizet,blabs,black,blade,blady,blaff,blahs,blain,blair,blake,blame,blams,blanc,bland,blank,blare,blart,blase,blash,blast,blate,blats,blawn,blaws,blayk,blaze,blazy,bleak,blear,bleat,blebs,bleck,bleed,bleep,blend,blenk,blens,blent,blere,bless,blest,blets,blibe,blick,blier,blimp,blimy,blind,blini,blink,bliny,blips,blirt,bliss,blist,blite,blitz,blizz,bloat,blobs,block,blocs,bloke,blond,blood,bloom,bloop,blore,blote,blots,blout,blown,blows,blowy,blued,bluer,blues,bluet,bluey,bluff,blume,blunk,blunt,blurb,blurs,blurt,blush,blype,board,boars,boart,boast,boats,bobac,bobby,bobet,bobol,bocal,bocca,bocce,bocci,boche,bocks,bocoy,boded,boden,boder,bodes,bodge,bodhi,bodle,boers,boffo,boffs,bogan,boget,bogey,boggy,bogie,bogle,bogue,bogum,bogus,bohea,bohor,boiko,boils,boily,boing,boise,boist,boite,bokom,bokos,bolag,bolar,bolas,boldo,boldu,boled,boles,bolis,bolls,bolly,bolos,bolti,bolts,bolty,bolus,bombe,bombo,bombs,bomos,bonav,bonbo,bonce,bonds,boned,boner,bones,boney,bongo,bongs,bonks,bonne,bonny,bonos,bonum,bonus,bonze,boobs,booby,boodh,boody,booed,books,booky,booly,booms,boomy,boone,boong,boonk,boons,boors,boort,boose,boost,boosy,booth,boots,booty,booze,boozy,borak,boral,boran,boras,borax,bored,boree,borel,borer,bores,borgh,boric,borid,boris,borne,boron,borts,borty,bortz,boryl,bosch,boser,bosey,bosks,bosky,bosom,boson,bossa,bossy,bosun,botan,botas,botch,botel,bothy,botry,botte,botts,bottu,bouch,boucl,bouet,bouge,bough,boule,boult,bound,bourd,bourg,bourn,bourr,bouse,bousy,bouto,bouts,bovey,bovid,bovld,bowed,bowel,bower,bowet,bowge,bowie,bowla,bowle,bowls,bowly,bowne,bowse,boxed,boxen,
 boxer,boxes,boxty,boyar,boyau,boyce,boyer,boyla,boyos,bozal,bozos,bozze,braca,brace,brach,brack,bract,brads,braes,bragi,brags,brahm,braid,brail,brain,brake,braky,brame,brand,brank,brans,brant,brash,brass,brast,brats,brava,brave,bravi,bravo,brawl,brawn,braws,braxy,braye,brays,braza,braze,bread,break,bream,breba,breck,brede,bredi,breed,breek,brees,breme,brens,brent,brerd,brere,brest,breth,brett,breva,breve,brevi,brews,brian,briar,bribe,brick,bride,brief,brier,bries,brigs,brike,brill,brims,brine,bring,brink,brins,briny,brios,brisa,brise,brisk,briss,brist,brite,brith,brits,britt,briza,brizz,broad,broch,brock,brogh,broid,broil,broke,broll,broma,brome,bromo,bronc,bronk,bronx,brood,brook,brool,broom,broon,broos,brose,brosy,broth,brott,browd,brown,brows,brubu,bruce,bruet,brugh,bruin,bruit,bruja,brujo,bruke,brule,brume,brune,bruno,brunt,brush,brusk,bruta,brute,bruzz,bryan,bryce,bryon,bryum,btise,buaze,bubal,bubas,bubba,bubby,bubos,bucca,bucco,buchu,bucko,bucks,bucku,bucky,buddh,buddy,budge,budgy,bueno,buffa,buffe,buffi,buffo,buffs,buffy,bugan,buggy,bught,bugle,bugre,buhls,buhrs,buick,build,built,buist,bukat,bulak,bulbs,bulby,bulge,bulgy,bulks,bulky,bulla,bulls,bully,bulse,bumbo,bumfs,bumph,bumps,bumpy,bunce,bunch,bunco,bunda,bundh,bunds,bundt,bundu,bundy,bunga,bungo,bungs,bungy,bunko,bunks,bunns,bunny,bunts,bunty,bunya,buoys,buran,burao,buras,burbs,burds,burel,buret,burez,burga,burge,burgh,burgs,burin,burka,burke,burls,burly,burma,burns,burnt,burny,buroo,burps,burro,burrs,burry,bursa,burse,burst,burut,burys,busby,bused,buses,bushi,bushy,busks,busky,bussu,bussy,busti,busto,busts,busty,butat,butch,butea,buteo,butic,butin,butle,butsu,butte,butts,butty,butut,butyl,butyn,butyr,buxom,buxus,buyer,buzzy,bwana,byard,bylaw,bynin,byous,byres,byrls,byron,byrri,bysen,byssi,bytes,byway,
@@ -78,129 +75,142 @@
 wrack,wramp,wrang,wraps,wrapt,wrast,wrath,wrawl,wreak,wreat,wreck,wrens,wrest,wrick,wride,wried,wrier,wries,wring,wrist,write,writh,writs,wrive,wroke,wrong,wroot,wrote,wroth,wrung,wryer,wryly,wudge,wunna,wurly,wurst,wuzzy,wyled,wyles,wynds,wynne,wynns,wyson,wysty,wyted,wytes,wyver,
 xebec,xenia,xenic,xenon,xenos,xenyl,xeres,xeric,xerox,xerus,xicak,xinca,xoana,xurel,xviii,xxiii,xylan,xylem,xylia,xylic,xylol,xylon,xylyl,xyrid,xyris,xysti,xysts,
 yabbi,yabby,yaboo,yacal,yacca,yacht,yacks,yadim,yaffs,yager,yagis,yagua,yahan,yahoo,yaird,yajna,yakan,yakin,yakka,yakut,yalla,yamel,yamen,yameo,yampa,yamph,yamun,yanan,yangs,yanks,yanky,yaply,yapok,yapon,yappy,yaqui,yarak,yaray,yards,yarer,yarke,yarly,yarns,yarry,yarth,yasht,yasna,yauds,yauld,yaups,yawed,yawey,yawls,yawns,yawny,yawps,yazoo,yclad,yeans,yeara,yeard,yearn,years,yeast,yecch,yechs,yechy,yeech,yeggs,yelek,yelks,yells,yelps,yemen,yenta,yente,yeply,yerba,yerga,yerks,yerth,yerva,yeses,yesso,yesty,yetis,yetts,yeuks,yeuky,yeven,yezdi,yezzy,yfere,ygapo,yield,yikes,yills,yince,yinst,yipes,yirds,yirrs,yirth,ylems,yobbo,yocco,yocks,yodel,yodhs,yodle,yogas,yogee,yoghs,yogic,yogin,yogis,yoick,yojan,yoked,yokel,yoker,yokes,yolks,yolky,yomer,yomim,yomin,yomud,yonic,yonis,yores,youff,young,youre,yourn,yours,yourt,youse,youth,youve,youze,yoven,yowed,yowes,yowie,yowls,yquem,ytter,yuans,yucca,yucch,yuchi,yucks,yucky,yugas,yukon,yulan,yules,yuman,yummy,yunca,yupon,yurak,yurok,yurta,yurts,yuruk,
 zabra,zabti,zaire,zakah,zakat,zaman,zambo,zamia,zande,zante,zanza,zanze,zapas,zapus,zaque,zarfs,zaxes,zayat,zayin,zazen,zeals,zebec,zebra,zebub,zebus,zeins,zeism,zeiss,zeist,zemmi,zemni,zendo,zerda,zerma,zeros,zests,zesty,zetas,zhmud,ziara,zibet,ziega,ziffs,zigan,zihar,zilch,zilla,zills,zimbi,zimme,zimmi,zimmy,zinco,zincs,zincy,zineb,zings,zingy,zinke,zinky,zippy,zirai,zirak,ziram,zitis,zizel,zizia,zizit,zlote,zloty,zmudz,zoaea,zocco,zoeae,zoeal,zoeas,zogan,zohak,zoism,zoist,zokor,zolle,zombi,zonal,zonar,zonda,zoned,zoner,zones,zonic,zonta,zooid,zooks,zooms,zoona,zoons,zooty,zoque,zoril,zoris,zorro,zosma,zowie,zucco,zudda,zulus,zunis,zygal,zygon,zymes,zymic,zymin
 """
 
 
-# Class
-###########################################################################
 class Wordle:
     """
     Wordle class
 
     Use: ``Wordle.solve()``
     """
-    def __init__(
-            self,
-            *,
-            green: str = "G",
-            yellow: str = "Y",
-            gray: str = "?"
-        ) -> None:
+
+    def __init__(self, *, green: str = "G", yellow: str = "Y", gray: str = "?") -> None:
         # Setting
         self._ALLOWABLE_CHARACTERS = set(string.ascii_letters)
         self._ALLOWED_ATTEMPTS = 6
         self._WORD_LENGTH = 5
 
-        self._WORDS = set(OFFLINE_WORDS.replace("\n", "").split(","))
+        self._WORDS: List[str] = list(set(OFFLINE_WORDS.replace("\n", "").split(",")))
 
         self._LETTER_COUNTER = Counter(chain.from_iterable(self._WORDS))
 
         self._LETTER_FREQUENCY = {
             character: value / sum(self._LETTER_COUNTER.values())
             for character, value in self._LETTER_COUNTER.items()
         }
 
         # Notation
         self._GREEN = green
         self._YELLOW = yellow
         self._GRAY = gray
 
     def __str__(self) -> str:
-        return self.__class__.__name__
+        return self.__repr__()
 
     def __repr__(self) -> str:
-        return self.__str__()
+        return self.__class__.__name__
 
     def update_words(self) -> None:
         """
         Try to fetch words list from online source
         """
         try:
             dict_link = "https://raw.githubusercontent.com/dwyl/english-words/master/words_dictionary.json"
             res = requests.get(dict_link)
-            word_list = list(res.json().keys())
-            logger.debug(word_list)
-            self._WORDS = {
-                word.lower()
-                for word in word_list
-                if len(word) == self._WORD_LENGTH and set(word) < self._ALLOWABLE_CHARACTERS 
-            }
-        except:
+            word_list: list[str] = list(res.json().keys())
+            self._WORDS = list(
+                {
+                    word.lower()
+                    for word in word_list
+                    if len(word) == self._WORD_LENGTH
+                    and set(word) < self._ALLOWABLE_CHARACTERS
+                }
+            )
+        except Exception:
             pass
 
     # Logic
-    def _calculate_word_commonality(self, word):
+    def _calculate_word_commonality(self, word: str) -> float:
         score = 0.0
         for char in word:
             score += self._LETTER_FREQUENCY[char]
         return score / (self._WORD_LENGTH - len(set(word)) + 1)
 
-    def _sort_by_word_commonality(self):
+    def _sort_by_word_commonality(self) -> List[Tuple[str, float]]:
         sort_by = operator.itemgetter(1)
         return sorted(
             [(word, self._calculate_word_commonality(word)) for word in self._WORDS],
             key=sort_by,
             reverse=True,
         )
 
-    def _display_word_table(self, word_commonalities):
-        for (word, freq) in word_commonalities:
+    def _display_word_table(self, word_commonalities: List[Tuple[str, float]]) -> None:
+        for word, freq in word_commonalities:
             print(f"{word:<10} | {freq:<5.2}")
 
-    def _input_word(self):
+    def _input_word(self) -> str:
         while True:
             word = input("Input the word you entered> ")
             if len(word) == self._WORD_LENGTH and word.lower() in self._WORDS:
                 break
         return word.lower()
 
-    def _input_response(self):
+    def _input_response(self) -> str:
         print("Type the color-coded reply from Wordle:")
         print(f"  {self._GREEN} for Green")
         print(f"  {self._YELLOW} for Yellow")
         print(f"  {self._GRAY} for Gray")
         while True:
             response = input("Response from Wordle> ")
-            if len(response) == self._WORD_LENGTH and set(response) <= {self._GREEN, self._YELLOW, self._GRAY}:
+            if len(response) == self._WORD_LENGTH and set(response) <= {
+                self._GREEN,
+                self._YELLOW,
+                self._GRAY,
+            }:
                 break
             else:
                 print(f"Error - invalid answer {response}")
+        if response == self._GREEN * 5:  # Win
+            return "win"
         return response
 
-    def _match_word_vector(self, word, word_vector):
+    def _match_word_vector(self, word: str, word_vector: List[Set[str]]) -> bool:
         assert len(word) == len(word_vector)
         for letter, v_letter in zip(word, word_vector):
             if letter not in v_letter:
                 return False
         return True
 
-    def _match(self, word_vector, possible_words):
-        return [word for word in possible_words if self._match_word_vector(word, word_vector)]
+    def _match(
+        self, word_vector: List[Set[str]], possible_words: List[str]
+    ) -> List[str]:
+        return [
+            word
+            for word in possible_words
+            if self._match_word_vector(word, word_vector)
+        ]
 
     # Main
     def solve(self) -> None:
         """Solve Wordle"""
         word_vector = [set(string.ascii_lowercase) for _ in range(self._WORD_LENGTH)]
+
         for attempt in range(1, self._ALLOWED_ATTEMPTS + 1):
             print(f"Attempt {attempt} with {len(self._WORDS)} possible words")
             self._display_word_table(self._sort_by_word_commonality()[:15])
             word = self._input_word()
+
             response = self._input_response()
+            if response == "win":
+                print("You Won!")
+                break
+
             for idx, letter in enumerate(response):
                 if letter == self._GREEN:
                     word_vector[idx] = {word[idx]}
                 elif letter == self._YELLOW:
                     try:
                         word_vector[idx].remove(word[idx])
                     except KeyError:
@@ -213,10 +223,9 @@
                             pass
             self._WORDS = self._match(word_vector, self._WORDS)
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
-    logger.setLevel(10) # DEBUG
     test = Wordle()
     test.solve()
```

### Comparing `absfuyu-3.3.2/src/absfuyu/general/__init__.py` & `absfuyu-3.3.3/src/absfuyu/general/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     Update attribute through dict
     """
 
     def __init__(self, data: Optional[Dict[Any, Any]] = None) -> None:
         try:
             self.__dict__.update(data)  # type: ignore
-        except:
+        except Exception:
             pass
 
     def __str__(self) -> str:
         class_name = self.__class__.__name__
         return f"{class_name}({self.__dict__})"
 
     def __repr__(self) -> str:
```

### Comparing `absfuyu-3.3.2/src/absfuyu/general/content.py` & `absfuyu-3.3.3/src/absfuyu/util/path.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,565 +1,563 @@
 """
-Absfuyu: Content
-----------------
-Handle .txt file
-
-Version: 1.2.6
-Date updated: 05/04/2024 (dd/mm/yyyy)
-
-Usage:
-------
->>> from absfuyu.general.content import ContentLoader
+Absfuyu: Path
+-------------
+Path related
+
+Version: 1.6.5
+Date updated: 10/04/2024 (dd/mm/yyyy)
+
+Feature:
+--------
+- Directory
+- SaveFileAs
 """
 
 # Module level
 ###########################################################################
-__all__ = ["ContentLoader", "Content", "LoadedContent"]
+__all__ = [
+    # Main
+    "Directory",
+    "SaveFileAs",
+    # Support
+    "FileOrFolderWithModificationTime",
+    "DirectoryInfo",
+]
 
 
 # Library
 ###########################################################################
-import json
-import random
+import os
 import re
-from collections import Counter
-from itertools import chain
+import shutil
+from datetime import datetime
+from functools import partial
 from pathlib import Path
-from typing import List, Optional
+from typing import Any, List, Literal, NamedTuple, Optional, Union
 
-from unidecode import unidecode
+from deprecated.sphinx import versionadded
 
-from absfuyu.logger import logger
+from absfuyu.logger import LogLevel, logger
 
 
-# Class
+# Support Class
 ###########################################################################
-class Content:
+@versionadded(version="3.3.0")
+class FileOrFolderWithModificationTime(NamedTuple):
     """
-    Contain data
+    File or Folder with modification time
 
-    Data format: list[str, list[str]]
-        where: ``str: data``; ``list[str]: data tags``
+    :param path: Original path
+    :param modification_time: Modification time
     """
 
-    def __init__(self, data: list) -> None:
-        self.data: str = str(data[0])
-        self.tag: list = data[1]
-        # logger.debug(self.__dict__)
+    path: Path
+    modification_time: datetime
+
+
+@versionadded(version="3.3.0")
+class DirectoryInfo(NamedTuple):
+    """Information of a directory"""
+
+    files: int
+    folders: int
+    creation_time: datetime
+    modification_time: datetime
+
+
+# Class - Directory | version 3.4.0: Remake Directory into modular class
+###########################################################################
+class DirectoryBase:
+    def __init__(
+        self,
+        source_path: Union[str, Path],
+        create_if_not_exist: bool = False,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        source_path : str | Path
+            Source folder
+
+        create_if_not_exist : bool
+            Create directory when not exist
+            (Default: ``False``)
+        """
+        self.source_path = Path(source_path)
+        if create_if_not_exist:
+            if not self.source_path.exists():
+                self.source_path.mkdir(exist_ok=True, parents=True)
 
     def __str__(self) -> str:
-        # return f"{self.data} | {self.tag}"
-        return str(self.data)
+        return self.source_path.__str__()
 
     def __repr__(self) -> str:
-        return self.__str__()
+        return f"{self.__class__.__name__}({self.source_path})"
 
-    def unidecoded(self) -> "Content":
+    def __format__(self, __format_spec: str) -> str:
         """
-        Convert data through ``unidecode`` package
+        Change format of an object.
+        Avaiable option: ``info``
 
-        Returns
-        -------
-        Content
-            ``unidecoded`` Content
+        Usage
+        -----
+        >>> print(f"{<object>:<format_spec>}")
+        >>> print(<object>.__format__(<format_spec>))
+        >>> print(format(<object>, <format_spec>))
         """
-        return self.__class__([unidecode(self.data), list(map(unidecode, self.tag))])
+        # Show quick info
+        if __format_spec.lower().startswith("info"):
+            return self.quick_info().__repr__()
 
-    def to_text(self) -> str:
+        # No format spec
+        return self.__repr__()
+
+    # Everything
+    @property
+    @versionadded(version="3.3.0")
+    def everything(self) -> List[Path]:
         """
-        Convert back into text
+        Every folders and files in this Directory
+        """
+        return list(x for x in self.source_path.glob("**/*"))
 
-        Returns
-        -------
-        str
-            Text
+    @versionadded(version="3.3.0")
+    def _every_folder(self) -> List[Path]:
+        """
+        Every folders in this Directory
         """
-        # hard code
-        tags = ",".join(self.tag)
-        return f"{self.data}|{tags}"
+        return list(x for x in self.source_path.glob("**/*") if x.is_dir())
 
-    def short_form(self, separator: str = ",") -> str:
+    @versionadded(version="3.3.0")
+    def _every_file(self) -> List[Path]:
         """
-        Short form show only first item when separated by ``separator``
+        Every folders in this Directory
+        """
+        return list(x for x in self.source_path.glob("**/*") if x.is_file())
 
-        Parameters
-        ----------
-        separator : str
-            Default: ``","``
+    # Quick information
+    @versionadded(version="3.3.0")
+    def quick_info(self) -> DirectoryInfo:
+        """
+        Quick information about this Directory
 
-        Returns
-        -------
-        str
-            Short form
+        :rtype: DirectoryInfo
         """
-        if not separator.startswith(","):
-            logger.debug(f"Separated symbol: {separator}")
-        return self.data.split(separator)[0]
+        source_stat: os.stat_result = self.source_path.stat()
+        out = DirectoryInfo(
+            files=len(self._every_file()),
+            folders=len(self._every_folder()),
+            creation_time=datetime.fromtimestamp(source_stat.st_ctime),
+            modification_time=datetime.fromtimestamp(source_stat.st_mtime),
+        )
+        return out
 
-    def handle_address(
-        self, address_separator: str = ",", *, first_item_not_address: bool = True
-    ) -> "Content":
+
+class DirectoryBasicOperation(DirectoryBase):
+    # Rename
+    def rename(self, new_name: str) -> None:
         """
-        Handle ``self.data`` as address and then update the address into ``self.tag``
+        Rename directory
 
         Parameters
         ----------
-        address_separator : str
-            | Split the address by which character
-            | (Default: ``","``)
-
-        first_item_not_address : bool
-            Set to ``False`` when ``<splited data>[0]`` is not part of an address
+        new_name : str
+            Name only (not the entire path)
+        """
+        try:
+            logger.debug(f"Renaming to {new_name}...")
+            self.source_path.rename(self.source_path.with_name(new_name))
+            logger.debug(f"Renaming to {new_name}...DONE")
+        except Exception as e:
+            logger.error(e)
+        # return self.source_path
 
-        Returns
-        -------
-        Content
-            Handled Content
+    # Copy
+    def copy(self, dst: Path) -> None:
+        """
+        Copy entire directory
 
+        Parameters
+        ----------
+        dst : Path
+            Destination
+        """
+        logger.debug(f"Copying to {dst}...")
+        try:
+            try:
+                shutil.copytree(self.source_path, Path(dst), dirs_exist_ok=True)
+            except Exception:
+                shutil.copytree(self.source_path, Path(dst))
+            logger.debug(f"Copying to {dst}...DONE")
+        except Exception as e:
+            logger.error(e)
 
-        Example:
-        --------
-        >>> test = "Shop A, 22 ABC Street, DEF District, GHI City"
-        >>> # After handle_address()
-        ["Shop A", "22 ABC Street", "DEF District", "GHI City"]
-
-        >>> # After handle_address(first_item_not_address = False)
-        ["22 ABC Street", "DEF District", "GHI City"]
-        """
-        if first_item_not_address:
-            temp = self.data.split(address_separator)
-        else:
-            logger.debug(
-                f"First item ({self.data.split(address_separator)[0]}) is not part of an address"
-            )
-            temp = self.data.split(address_separator)[1:]
+    # Move
+    def move(self, dst: Path, content_only: bool = False) -> None:
+        """
+        Move entire directory
 
-        new_tag = [x.strip().lower() for x in temp]
-        logger.debug(f"Current tags: {self.tag}")
-        logger.debug(f"New tags: {new_tag}")
-        self.tag = list(set(self.tag + new_tag))
-        logger.debug(f"Final tags: {self.tag} Len: {len(self.tag)}")
+        Parameters
+        ----------
+        dst : Path
+            Destination
 
-        return self.__class__([self.data, self.tag])
+        content_only : bool
+            Only move content inside the folder (Default: ``False``; Move entire folder)
+        """
+        try:
+            logger.debug(f"Moving to {dst}...")
+            if content_only:
+                for x in self.source_path.iterdir():
+                    shutil.move(x, Path(dst))
+            else:
+                shutil.move(self.source_path, Path(dst))
+            logger.debug(f"Moving to {dst}...DONE")
+
+        except shutil.Error as e:  # File already exists
+            logger.error(e)
+            logger.debug("Overwriting file...")
+            if content_only:
+                for x in self.source_path.iterdir():
+                    shutil.move(x, Path(dst).joinpath(x.name))
+            else:
+                shutil.move(self.source_path, Path(dst))
+            logger.debug("Overwriting file...DONE")
+
+    # Delete folder
+    def _mtime_folder(self) -> List[FileOrFolderWithModificationTime]:
+        """
+        Get modification time of file/folder (first level only)
+        """
+        return [
+            FileOrFolderWithModificationTime(
+                path, datetime.fromtimestamp(path.stat().st_mtime)
+            )
+            for path in self.source_path.glob("*")
+        ]
 
+    @staticmethod
+    def _delete_files(list_of_files: List[Path]) -> None:
+        """
+        Delete files/folders
+        """
+        for x in list_of_files:
+            x = Path(x).absolute()
+            logger.debug(f"Removing {x}...")
+            try:
+                if x.is_dir():
+                    shutil.rmtree(x)
+                else:
+                    x.unlink()
+                logger.debug(f"Removing {x}...SUCCEED")
+            except Exception:
+                logger.error(f"Removing {x}...FAILED")
+
+    @staticmethod
+    def _date_filter(
+        value: FileOrFolderWithModificationTime,
+        period: Literal["Y", "M", "D"] = "Y",
+    ) -> bool:
+        """
+        Filter out file with current Year|Month|Day
+        """
+        data = {
+            "Y": value.modification_time.year,
+            "M": value.modification_time.month,
+            "D": value.modification_time.day,
+        }
+        now = datetime.now()
+        ntime = {"Y": now.year, "M": now.month, "D": now.day}
+        return data[period] != ntime[period]
 
-class LoadedContent(List[Content]):
-    """
-    Contain list of ``Content``
-    """
+    def delete(
+        self,
+        entire: bool = False,
+        *,
+        based_on_time: bool = False,
+        keep: Literal["Y", "M", "D"] = "Y",
+    ) -> None:
+        """
+        Deletes everything
 
-    def __str__(self) -> str:
-        # return f"{self.__class__.__name__} - Total: {len(self)}"
-        return f"{self.__class__.__name__}({[x.data for x in self]})"
+        Parameters
+        ----------
+        entire : bool
+            | ``True``: Deletes the folder itself
+            | ``False``: Deletes content inside only
+            | (Default: ``False``)
 
-    def __repr__(self) -> str:
-        return self.__str__()
+        based_on_time : bool
+            | ``True``: Deletes everything except ``keep`` period
+            | ``False``: Works normal
+            | (Default: ``False``)
 
-    def apply(self, func) -> "LoadedContent":
+        keep : Literal["Y", "M", "D"]
+            Delete all file except current ``Year`` | ``Month`` | ``Day``
         """
-        Apply function to each entry
+        try:
+            logger.info(f"Removing {self.source_path}...")
 
-        :param func: Callable function
-        :type func: Callable
-        :rtype: LoadedContent
-        """
-        return self.__class__(func(x.data) for x in self)
+            if entire:
+                shutil.rmtree(self.source_path)
+            else:
+                if based_on_time:
+                    filter_func = partial(self._date_filter, period=keep)
+                    # self._delete_files([x[0] for x in filter(filter_func, self._mtime_folder())])
+                    self._delete_files(
+                        [x.path for x in filter(filter_func, self._mtime_folder())]
+                    )
+                else:
+                    self._delete_files(
+                        map(lambda x: x.path, self._mtime_folder())  # type: ignore
+                    )
 
-    @classmethod
-    def load_from_json(cls, file: Path) -> "LoadedContent":
+            logger.info(f"Removing {self.source_path}...SUCCEED")
+        except Exception as e:
+            logger.error(f"Removing {self.source_path}...FAILED\n{e}")
+
+    # Zip
+    def compress(self, *, format: str = "zip") -> Union[Path, None]:
         """
-        Use this method to load data from ``.json`` file from ``to_json()`` method
+        Compress the directory (Default: Create ``.zip`` file)
 
         Parameters
         ----------
-        file : Path
-            Path to ``.json`` file
+        format : Literal["zip", "tar", "gztar", "bztar", "xztar"]
+            - ``zip``: ZIP file (if the ``zlib`` module is available).
+            - ``tar``: Uncompressed tar file. Uses POSIX.1-2001 pax format for new archives.
+            - ``gztar``: gzip'ed tar-file (if the ``zlib`` module is available).
+            - ``bztar``: bzip2'ed tar-file (if the ``bz2`` module is available).
+            - ``xztar``: xz'ed tar-file (if the ``lzma`` module is available).
 
         Returns
         -------
-        LoadedContent
-            Loaded content from ``.json`` file
-        """
-        with open(file) as json_file:
-            parsed_json: dict = json.load(json_file)
-        out = [Content(list(x.values())) for x in parsed_json]
-        return cls(out)
-
-    @property
-    def tags(self) -> list:
-        """A list contains all available tag"""
-        temp = chain.from_iterable([x.tag for x in self])
-        out = list(set(temp))
-        logger.debug(f"Found {len(out)} {'tags' if len(out) > 1 else 'tag'}")
-        return sorted(out)
-
-    def tag_count(self) -> Counter:
-        """
-        Count number of tags
-
-        :rtype: Counter
-        """
-        temp = chain.from_iterable([x.tag for x in self])
-        logger.debug(temp)
-        return Counter(temp)
-
-    def filter(self, tag: str) -> "LoadedContent":
-        """
-        Filter out entry with ``tag``
-
-        :param tag: Tag to filter
-        :type tag: str
-        :rtype: LoadedContent
-        """
-        tag = tag.strip().lower()
-        logger.debug(f"Tag: {tag}")
-        if tag not in self.tags:
-            # tag = random.choice(self.tags)
-            # logger.debug(f"Tag not exist, changing to a random tag... {tag}")
-            logger.warning(f'"{tag}" tag does not exist')
-            _avail_tag = ", ".join(list(dict(self.tag_count().most_common(5)).keys()))
-            raise ValueError(
-                f"Available tags: {_avail_tag},..."
-                f"\nMore tag at: `{self.__class__.__name__}.tags`"
+        Path
+            Compressed path
+        None
+            When fail to compress
+        """
+        logger.debug(f"Zipping {self.source_path}...")
+        try:
+            # zip_name = self.source_path.parent.joinpath(self.source_path.name).__str__()
+            # shutil.make_archive(zip_name, format=format, root_dir=self.source_path)
+            zip_path = shutil.make_archive(
+                self.source_path.__str__(), format=format, root_dir=self.source_path
             )
-        return self.__class__([x for x in self if tag in x.tag])
+            logger.debug(f"Zipping {self.source_path}...DONE")
+            logger.debug(f"Path: {zip_path}")
+            return Path(zip_path)
+        except Exception as e:
+            logger.error(f"Zipping {self.source_path}...FAILED\n{e}")
+            return None
 
-    def find(self, keyword: str) -> "LoadedContent":
-        """
-        Return all entries that include ``keyword``
 
-        :param keyword: Keyword to find
-        :type keyword: str
-        :rtype: LoadedContent
-        """
-        temp = self.__class__(
-            [x for x in self if x.data.lower().find(keyword.lower()) >= 0]
-        )
-        if temp:
-            logger.debug(f"Found {len(temp)} {'entries' if len(temp) > 1 else 'entry'}")
-        else:
-            logger.debug("No result")
-        return temp
+class DirectoryTree(DirectoryBase):
+    pass
+
+
+class Directory(DirectoryBasicOperation, DirectoryTree):
+    """
+    Some shortcuts for directory
+
+    - list_structure
+    - delete, rename, copy, move
+    - zip
+    - quick_info
+    """
 
-    def short_form(self, separator: str = ",") -> List[str]:
+    # Directory structure
+    def _list_dir(self, *ignore: str) -> List[Path]:
         """
-        Shows only first item when separated by ``separator`` of ``Content.data``
+        List all directories and files
 
         Parameters
         ----------
-        separator : str
-            Default: ``","``
-
-        Returns
-        -------
-        list[str]
-            Short form
+        ignore : str
+            List of pattern to ignore. Example: "__pycache__", ".pyc"
         """
-        return [x.short_form(separator) for x in self]
+        logger.debug(f"Base folder: {self.source_path.name}")
 
-    def pick_one(self, tag: Optional[str] = None) -> Content:
+        list_of_path = self.source_path.glob("**/*")
+
+        # No ignore rules
+        if len(ignore) == 0:  # No ignore pattern
+            return [path.relative_to(self.source_path) for path in list_of_path]
+
+        # With ignore rules
+        # ignore_pattern = "|".join(ignore)
+        ignore_pattern = re.compile("|".join(ignore))
+        logger.debug(f"Ignore pattern: {ignore_pattern}")
+        return [
+            path.relative_to(self.source_path)
+            for path in list_of_path
+            if re.search(ignore_pattern, path.name) is None
+        ]
+
+    @staticmethod
+    @versionadded(version="3.3.0")
+    def _split_dir(list_of_path: List[Path]) -> List[List[str]]:
         """
-        Pick a random entry
+        Split pathname by ``os.sep``
 
         Parameters
         ----------
-        tag : str | None
-            Pick a random entry with ``tag``
-            (Default: None)
+        list_of_path : list[Path]
+            List of Path
 
         Returns
         -------
-        Content
-            Random entry
+        list[list[str]]
+            List of splitted dir
+
+
+        Example:
+        --------
+        >>> test = [Path(test_root/test_not_root), ...]
+        >>> Directory._split_dir(test)
+        [[test_root, test_not_root], [...]...]
         """
-        if tag:
-            temp = self.filter(tag)
-            logger.debug(f"Tag: {tag}")
-            return random.choice(temp)
-        return random.choice(self)
 
-    def handle_address(
-        self, address_separator: str = ",", *, first_item_not_address: bool = True
-    ) -> "LoadedContent":
+        return sorted([str(path).split(os.sep) for path in list_of_path])
+
+    def _separate_dir_and_files(
+        self,
+        list_of_path: List[Path],
+        *,
+        tab_symbol: Optional[str] = None,
+        sub_dir_symbol: Optional[str] = None,
+    ) -> List[str]:
         """
-        Execute ``Content.handle_address()`` on every ``self.data`` of ``Content``
+        Separate dir and file and transform into folder structure
 
         Parameters
         ----------
-        address_separator : str
-            | Split the address by which character
-            | (Default: ``","``)
+        list_of_path : list[Path]
+            List of paths
 
-        first_item_not_address : bool
-            Set to ``False`` when ``<splited data>[0]`` is not part of an address
+        tab_symbol : str | None
+            Tab symbol
+            (Default: ``"\\t"``)
+
+        sub_dir_symbol : str | None
+            Sub-directory symbol
+            (Default: ``"|-- "``)
 
         Returns
         -------
-        LoadedContent
-            Handled Content
+        list[str]
+            Folder structure ready to print
+        """
+        # Check for tab and sub-dir symbol
+        if not tab_symbol:
+            tab_symbol = "\t"
+        if not sub_dir_symbol:
+            sub_dir_symbol = "|-- "
 
+        temp: List[List[str]] = self._split_dir(list_of_path)
 
-        Example:
-        --------
-        >>> test = "Shop A, 22 ABC Street, DEF District, GHI City"
-        >>> # After handle_address()
-        ["Shop A", "22 ABC Street", "DEF District", "GHI City"]
-
-        >>> # After handle_address(first_item_not_address = False)
-        ["22 ABC Street", "DEF District", "GHI City"]
-        """
-        return self.__class__(
-            [
-                x.handle_address(
-                    address_separator=address_separator,
-                    first_item_not_address=first_item_not_address,
-                )
-                for x in self
-            ]
-        )
+        return [  # Returns n-tab space with sub-dir-symbol for the last item in x
+            f"{tab_symbol * (len(x) - 1)}{sub_dir_symbol}{x[-1]}" for x in temp
+        ]
 
-    def to_json(self, no_accent: bool = False) -> str:
+    def list_structure(self, *ignore: str) -> str:
         """
-        Convert data into ``.json`` file
+        List folder structure
 
         Parameters
         ----------
-        no_accent : bool
-            | when ``True``: convert the data through ``unidecode`` package
-            | (Default: ``False``)
+        ignore : str
+            Tuple contains patterns to ignore
 
         Returns
         -------
         str
-            Data
-        """
-        if no_accent:
-            out = [x.unidecoded().__dict__ for x in self]
-        else:
-            out = [x.__dict__ for x in self]
-        logger.debug(out)
-        return json.dumps(out, indent=2)
+            Directory structure
+
 
-    def to_text(self, no_accent: bool = False) -> str:
+        Example (For typical python library):
+        -------------------------------------
+        >>> test = Directory(<source path>)
+        >>> test.list_structure(
+                "__pycache__",
+                ".pyc",
+                "__init__",
+                "__main__",
+            )
+        ...
         """
-        Convert data into ``.txt`` file
+        temp: List[Path] = self._list_dir(*ignore)
+        out: List[str] = self._separate_dir_and_files(temp)
+        return "\n".join(out)  # Join the list
 
-        Parameters
-        ----------
-        no_accent : bool
-            | when ``True``: convert the data through ``unidecode`` package
-            | (Default: ``False``)
+    def list_structure_pkg(self) -> str:
+        """
+        List folder structure of a typical python package
 
         Returns
         -------
         str
-            Data
+            Directory structure
         """
-        if no_accent:
-            out = [x.unidecoded().to_text() for x in self]
-        else:
-            out = [x.to_text() for x in self]
-        logger.debug(out)
-        return "\n".join(out)
+        return self.list_structure("__pycache__", ".pyc")
 
 
-class ContentLoader:
-    """
-    This load data from ``.txt`` file
-
-    Content format:
-    ``<content><split_symbol><tags separated by <tag_separate_symbol>>``
-    """
+# Class - SaveFileAs
+###########################################################################
+class SaveFileAs:
+    """File as multiple file type"""
 
-    def __init__(
-        self,
-        file_path: Path,
-        characteristic_detect: bool = True,
-        tag_dictionary: Optional[dict] = None,
-        *,
-        comment_symbol: str = "#",
-        split_symbol: str = "|",
-        tag_separate_symbol: str = ",",
-    ) -> None:
+    def __init__(self, data: Any, *, encoding: Union[str, None] = "utf-8") -> None:
         """
-        Parameters
-        ----------
-        file_path : str
-            file location/file to load
-
-        characteristic_detect : bool
-            detect whether the content is long, short, or a question
-            (default: ``True``)
-
-        tag_dict : dict
-            custom tag pattern
-            format: ``{"keyword": "tag",...}``
-            example: ``{"apple": "fruit", "orange": "fruit"}``
-
-        comment_symbol : str
-            symbol that `ContentLoader` will ignore
-            (default: ``"#"``)
-
-        split_symbol : str
-            symbol that `ContentLoader` will split content and tags
-            (default: ``"|"``)
-
-        tag_separate_symbol : str
-            symbol that `ContentLoader` will split between tags
-            (default: ``","``)
-        """
-        # file
-        self.file = Path(file_path)
-
-        # characteristic detect
-        self.characteristic_detect: bool = characteristic_detect
-
-        # tag dictionary
-        if tag_dictionary is None:
-            # logger.debug("No tag patern available")
-            self.tag_dictionary: dict = dict()
-        else:
-            logger.debug(
-                f"Tag pattern available: "
-                f"{len(tag_dictionary)} {'entries' if len(tag_dictionary) > 1 else 'entry'} "
-                f"({len(set(tag_dictionary.values()))} unique "
-                f"{'tags' if len(set(tag_dictionary.values())) > 1 else 'tag'})"
-            )
-            self.tag_dictionary = tag_dictionary
-
-        # symbol stuff
-        assert (
-            comment_symbol != split_symbol
-        ), "comment_symbol and split_symbol should have different values"
-        assert (
-            tag_separate_symbol != split_symbol
-        ), "tag_separate_symbol and split_symbol should have different values"
-        self.comment_symbol: str = comment_symbol
-        self.split_symbol: str = split_symbol
-        self.tag_separate_symbol: str = tag_separate_symbol
+        :param encoding: Default: utf-8
+        """
+        self.data = data
+        self.encoding = encoding
 
     def __str__(self) -> str:
-        return f"{self.__class__.__name__}({self.__dict__})"
+        return f"{self.__class__.__name__}()"
 
     def __repr__(self) -> str:
         return self.__str__()
 
-    def content_format(self) -> str:
+    def to_txt(self, path: Union[str, Path]) -> None:
         """
-        Shows current content format
-
-        Returns
-        -------
-        str
-            Current content format
-
+        Save as ``.txt`` file
 
-        Example:
-        --------
-        >>> ContentLoader(".").content_format()
-        # This line will be ignored
-        <content> | <tag1>, <tag2>
-        """
-        out = (
-            f"{self.comment_symbol} This line will be ignored\n"
-            f"<content> {self.split_symbol} "
-            f"<tag1>{self.tag_separate_symbol} <tag2>"
-        )
-        return out
-
-    def load(self) -> list:
+        Parameters
+        ----------
+        path : Path
+            Save location
         """
-        Load content from ``self.file``
+        with open(path, "w", encoding=self.encoding) as file:
+            file.writelines(self.data)
 
-        Returns
-        -------
-        list
-            List of content
-        """
-        with open(self.file, "r", encoding="utf-8") as data:
-            logger.debug("Loading data...")
-            dat = []
-            check = []
-
-            for i, x in enumerate(data.readlines()):
-                x = x.strip()
-                if x.startswith(self.comment_symbol) or len(x) == 0:
-                    continue  # skip comment and empty lines
-                logger.debug(
-                    f"### Loop {i+1} #####################################################################"
-                )
-
-                temp = x.split(self.split_symbol)
-                if len(temp) != 2:
-                    logger.debug(f"Split len: {len(temp)}")
-                    logger.warning(
-                        f"The current entry is missing data or tag: {x[:20]}..."
-                    )
+    # def to_pickle(self, path: Union[str, Path]) -> None:
+    #     """
+    #     Save as .pickle file
 
-                temp[0] = temp[0].strip()
-                if temp[0].lower() not in check:
-                    check.append(temp[0].lower())  # check for dupes
-
-                    # tag
-                    additional_tags = []
-                    for k, v in self.tag_dictionary.items():
-                        key = k.strip().lower()
-                        val = temp[0].lower()
-                        regex_pattern = f"[^a-zA-Z0-9]({key})[^a-zA-Z0-9]|^({key})[^a-zA-Z0-9]|[^a-zA-Z0-9]({key})$"
-                        if re.search(regex_pattern, val) is not None or val.startswith(
-                            key
-                        ):
-                            # regex has a bug (or idk if it's a bug or not) that
-                            # doesn't recognise when there is only one word in the sentence
-                            # therefore use `val.startswith(key)` to fix
-                            additional_tags.append(v.strip().lower())
-
-                    if self.characteristic_detect:
-                        long_short = (120, 20)  # setting
-                        if len(temp[0]) > long_short[0]:
-                            additional_tags.append("long")
-                        if len(temp[0]) < long_short[1]:
-                            additional_tags.append("short")
-                        if temp[0][-1].startswith("?"):
-                            additional_tags.append("question")
-                    if additional_tags:
-                        logger.debug(f"Additional tags: {additional_tags}")
-
-                    try:
-                        tags = [
-                            tag.strip() for tag in temp[1].strip().lower().split(",")
-                        ]  # separate and strip tags
-                        logger.debug(f"Tags: {tags}")
-                    except:
-                        logger.warning("No tag found in the original string")
-                        if additional_tags:
-                            tags = additional_tags
-                        else:
-                            tags = ["unspecified"]
-                            logger.debug('Assigned "unspecified" tag')
-
-                    tags.extend(additional_tags)
-                    final_tags = list(set(tags))
-                    logger.debug(f"Final tags: {final_tags} Len: {len(final_tags)}")
+    #     :param path: Save location
+    #     """
+    #     from absfuyu.util.pkl import Pickler
+    #     Pickler.save(path, self.data)
 
-                    dat.append([temp[0], final_tags])  # add everything
-                else:
-                    logger.debug(f"Found duplicates, {x} removed")
+    # def to_json(self, path: Union[str, Path]) -> None:
+    #     """
+    #     Save as .json file
 
-        return dat
+    #     :param path: Save location
+    #     """
+    #     from absfuyu.util.json_method import JsonFile
+    #     temp = JsonFile(path, sort_keys=False)
+    #     temp.save_json()
 
-    def load_content(self) -> LoadedContent:
-        """
-        Load data into a list of ``Content``
 
-        Returns
-        -------
-        LoadedContent
-            Loaded content
-        """
-        return LoadedContent(map(Content, self.load()))
+# Dev and Test new feature before get added to the main class
+###########################################################################
+class _NewDirFeature(Directory):
+    pass
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
-    logger.setLevel(10)
+    logger.setLevel(LogLevel.DEBUG)
```

### Comparing `absfuyu-3.3.2/src/absfuyu/general/data_extension.py` & `absfuyu-3.3.3/src/absfuyu/general/data_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,15 +479,15 @@
 
         if not raw:
             temp = []
             str_len = len(hex_str)
 
             for i in range(str_len):
                 if i % 2 == 0:
-                    temp.append(f"\\x")
+                    temp.append("\\x")
                 temp.append(hex_str[i])
             return "".join(temp)
         else:
             return hex_str
 
     def random_capslock(self, probability: int = 50) -> "Text":
         """
@@ -615,15 +615,15 @@
         temp = str(self)
         if ignore_capslock:
             pattern = pattern.lower()
             temp = temp.lower()
 
         out = [
             1
-            for i in range(0, len(temp) - len(pattern) + 1)
+            for i in range(len(temp) - len(pattern) + 1)
             if temp[i : i + len(pattern)] == pattern
         ]
         return sum(out)
 
     @versionadded(version="3.3.0")
     def hapax(self, strict: bool = False) -> List[str]:
         """
@@ -927,15 +927,15 @@
             | ``True`` if a narcissistic number
             | ``False`` if not a narcissistic number
         """
         try:
             check = sum([int(x) ** len(str(self)) for x in str(self)])
             res = int(self) == check
             return res  # type: ignore
-        except:
+        except Exception:
             return False
 
     def reverse(self) -> "IntNumber":
         """
         Reverse a number. Reverse ``abs(number)`` if ``number < 0``
 
         Returns
@@ -1002,15 +1002,15 @@
         --------
         >>> test = IntNumber(102)
         >>> test.lcm(5)
         510
         """
         try:
             return self.__class__(math.lcm(self, with_number))
-        except:
+        except AttributeError:  # Python < 3.9
             return self.__class__((self * with_number) // math.gcd(self, with_number))
 
     @versionchanged(version="3.3.0", reason="Fix bug")
     def gcd(self, with_number: int) -> "IntNumber":
         """
         Greatest common divisor of ``self`` and ``with_number``
 
@@ -1374,15 +1374,15 @@
                 temp = Counter(data)
             else:
                 logger.debug(f"Freq of first {num_of_first_char} char")
                 temp = Counter([str(x)[:num_of_first_char] for x in data])
 
         try:
             times_appear = dict(sorted(temp.items()))
-        except:
+        except Exception:
             times_appear = dict(self.__class__(temp.items()).sorts())
         logger.debug(times_appear)
 
         if appear_increment:
             times_appear_increment: List[int] = list(
                 accumulate(times_appear.values(), operator.add)
             )
@@ -1638,15 +1638,15 @@
         --------
         >>> test = ListExt([["test"], ["test", "test"], ["test"]])
         >>> test.flatten()
         ['test', 'test', 'test', 'test']
         """
         try:
             return ListExt(chain(*self))
-        except:
+        except Exception:
             temp = list(map(lambda x: x if isinstance(x, list) else [x], self))
             return ListExt(chain(*temp))
 
     def numbering(self, start: int = 0) -> "ListExt":
         """
         Number the item in list
         (``enumerate`` wrapper)
@@ -1735,18 +1735,18 @@
             #     "min": min_list,
             # }
 
             # logger.debug(output)
             # return output
             return DictAnalyzeResult(max_val, min_val, max_list, min_list)
 
-        except:
+        except Exception:
             err_msg = "Value must be int or float"
             logger.error(err_msg)
-            raise ValueError(err_msg)
+            raise ValueError(err_msg)  # noqa: B904
 
     def swap_items(self) -> "DictExt":
         """
         Swap ``dict.keys()`` with ``dict.values()``
 
         Returns
         -------
```

### Comparing `absfuyu-3.3.2/src/absfuyu/general/generator.py` & `absfuyu-3.3.3/src/absfuyu/general/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         --------
         >>> Generator.generate_string(times=3)
         ['67Xfh1fv', 'iChcGz9P', 'u82fNzlm']
         """
 
         try:
             char_lst = list(charset)
-        except:
+        except Exception:
             char_lst = charset  # type: ignore # ! review this sometime
         # logger.debug(char_lst)
 
         unique_string = []
         count = 0
         logger.debug(f"Unique generated text: {unique}")
```

### Comparing `absfuyu-3.3.2/src/absfuyu/general/human.py` & `absfuyu-3.3.3/src/absfuyu/general/human.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
             When unable to get ``self.birthday``
         """
         if self.birthday is not None:
             now = datetime.now()
             # age = now - self.birthday
             try:
                 rdelta = relativedelta(now, self.birthday)
-            except:
+            except Exception:
                 date_str = self.birthday
                 if date_str is None:
                     self.birthday = datetime.now().date()
                 else:
                     for x in ["/", "-"]:
                         date_str = date_str.replace(x, "/")
                     date = datetime.strptime(date_str, "%Y/%m/%d")
@@ -235,15 +235,15 @@
         None
             When unable to get ``self.height`` and ``self.weight``
         """
         try:
             temp = self.height / 100
             bmi = self.weight / (temp * temp)
             return round(bmi, 2)
-        except:
+        except Exception:
             return None
 
     # @property
     def dir_(self) -> list:
         """
         List property
 
@@ -310,15 +310,15 @@
             Zodiac sign
 
         None
             When unable to get ``self.birthday``
         """
         try:
             return zodiac_sign(self.birthday.day, self.birthday.month)
-        except:
+        except Exception:
             return None
 
     @property
     def zodiac_sign_13(self):
         """
         Zodiac sign of ``Person`` (13 zodiac signs version)
 
@@ -328,15 +328,15 @@
             Zodiac sign
 
         None
             When unable to get ``self.birthday``
         """
         try:
             return zodiac_sign(self.birthday.day, self.birthday.month, zodiac13=True)
-        except:
+        except Exception:
             return None
 
     @property
     def numerology(self) -> int:
         """
         Numerology number of ``Person``
```

### Comparing `absfuyu-3.3.2/src/absfuyu/pkg_data/__init__.py` & `absfuyu-3.3.3/src/absfuyu/pkg_data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 ---------------------
 Load package data
 
 Version: 2.2.2
 Date updated: 30/11/2023 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["PkgData"]
 
 
 # Library
 ###########################################################################
@@ -23,16 +22,16 @@
 from typing import List, Union
 
 if _python_version.minor >= 10:
     from importlib.resources import files
 else:
     try:
         from importlib_resources import files  # type: ignore
-    except:
-        raise ImportError("Please install importlib-resources")
+    except Exception:
+        raise ImportError("Please install importlib-resources")  # noqa: B904
 
 from absfuyu.core import DATA_PATH
 from absfuyu.logger import logger
 
 # External Data
 ###########################################################################
 _EXTERNAL_DATA = {
@@ -135,15 +134,15 @@
 
             for data_name, data_link in _EXTERNAL_DATA.items():
                 logger.debug(f"Downloading {data_name}...")
                 data = APIRequest(data_link, encoding="utf-8")
                 data.fetch_data(update=True, json_cache=DATA_PATH.joinpath(data_name))
                 logger.debug(f"Downloading {data_name}...DONE")
             logger.debug("Downloading data...DONE")
-        except:
+        except Exception:
             logger.debug("Downloading data...FAILED")
 
     def clear_data(self) -> None:
         """Clear data in data list"""
         for x in self.get_data_list():
             x.unlink()
```

### Comparing `absfuyu-3.3.2/src/absfuyu/pkg_data/chemistry.pkl` & `absfuyu-3.3.3/src/absfuyu/pkg_data/chemistry.pkl`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/pkg_data/tarot.pkl` & `absfuyu-3.3.3/src/absfuyu/pkg_data/tarot.pkl`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/tools/converter.py` & `absfuyu-3.3.3/src/absfuyu/tools/converter.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/tools/keygen.py` & `absfuyu-3.3.3/src/absfuyu/tools/keygen.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,73 +7,68 @@
 
 Version: 2.0.2
 Date updated: 05/04/2024 (dd/mm/yyyy)
 """
 
 # Module level
 ###########################################################################
-__all__ = [
-    "Keygen"
-]
+__all__ = ["Keygen"]
 
 
 # Library
 ###########################################################################
 import random
 
 
 # Class
 ###########################################################################
 class Keygen:
     """Key generator"""
+
     @staticmethod
     def _is_mod7(text: str) -> bool:
         """
         Check if sum of elements in a string is divisible by 7
 
-        text: number in str type to check
+        :param text: number in str type to check
         """
-        text = str(text) # Safety convert
+        text = str(text)  # Safety convert
         try:
             res = sum(map(int, text)) % 7
             # logger.debug(f"Sum value: {res}")
             return res == 0
-        except:
-            raise ValueError("Invalid string")
+        except Exception:
+            raise ValueError("Invalid string")  # noqa: B904
 
     @staticmethod
-    def _mod7_gen(
-            num_of_digits: int,
-            *,
-            fillchar: str = "0"
-        ) -> str:
+    def _mod7_gen(num_of_digits: int, *, fillchar: str = "0") -> str:
         """
         Generate a number with desired length that is divisible by 7
 
-        Parameters:
-        ---
+        Parameters
+        ----------
         num_of_digits : int
             Length of number
 
         fillchar : str
             filled character when `len(generated number)` < `num_of_digits`
-        
-        Return:
-        ---
+
+        Returns
+        -------
         str:
             Mod7 number
         """
 
         # Init
         mod7_num: int = 0
 
         # Conditions
-        max_value = 10**num_of_digits-1
+        max_value = 10**num_of_digits - 1
         mod7_valid = False
-        invalid_digits = [0,8,9] # Invalid last digit
+        invalid_digits = [0, 8, 9]  # Invalid last digit
 
         # Loop
         while not mod7_valid:
             # Gen num
             mod7_num = random.randint(0, max_value)
 
             # Check last digit
@@ -88,92 +83,94 @@
         return str(mod7_num).rjust(num_of_digits, fillchar)
 
     @staticmethod
     def mod7_cd_key(fast: bool = False) -> str:
         """
         CD Key generator
 
-        Format: ``XXX-XXXXXXX``                              
-        
+        Format: ``XXX-XXXXXXX``
+
         Rules:
-        
+
         - Last seven digits must add to be divisible by ``7``
         - First 3 digits cannot be ``333``, ``444``,..., ``999``
         - Last digit of last seven digits cannot be ``0``, ``8`` or ``9``
-        
+
         Parameters
         ----------
         fast : bool
-            Use pre-generated key 
+            Use pre-generated key
             (Default: ``False``)
-        
+
         Returns
         -------
         str:
             Mod7 Key
         """
 
         # Fast mode: pre-generated key
         if fast:
             return "111-1111111"
 
         # PART 01
         part1_valid = False
         part1_not_valid_digits = [333, 444, 555, 666, 777, 888]
         part1: str = ""
-        while not part1_valid: # Loop check
-            part1_num = random.randint(0, 998) # Gen random int from 0 to 998
+        while not part1_valid:  # Loop check
+            part1_num = random.randint(0, 998)  # Gen random int from 0 to 998
             # part1_num = random.randint(100,300) # or just use this
             if part1_num not in part1_not_valid_digits:
-                part1 = str(part1_num).rjust(3, "0") # Convert into string
-                part1_valid = True # Break loop
+                part1 = str(part1_num).rjust(3, "0")  # Convert into string
+                part1_valid = True  # Break loop
 
         # PART 02
         part2 = __class__._mod7_gen(num_of_digits=7)  # type: ignore
 
         # OUTPUT
         return f"{part1}-{part2}"
 
     @staticmethod
     def mod7_11_digit_key(fast: bool = False) -> str:
         """
         11-digit CD Key generator
 
         Format: ``XXXX-XXXXXXX``
-        
+
         - ``XXXX``: Can be anything from ``0001`` to ``9991``. The last digit must be 3rd digit + ``1`` or ``2``. When the result is > ``9``, it overflows to ``0`` or ``1``.
         - ``XXXXXXX``: Same as CD Key
-        
+
         Parameters
         ----------
         fast : bool
-            Use pre-generated key 
+            Use pre-generated key
             (Default: ``False``)
-        
+
         Returns
         -------
         str:
             Mod7 Key
         """
 
         # Fast mode: pre-generated key
         if fast:
             return "0001-0000007"
 
         # PART 01
         part1_valid = False
         part1: str = ""
         while not part1_valid:
-            part1_1_num = random.randint(0, 999) # Random 3-digit number
-            last_digit_choice = [1, 2] # Choice for last digit
-            part1_2_num = int(str(part1_1_num)[-1]) + random.choice(last_digit_choice) # Make last digit
-            if part1_2_num > 9: # Check condition then overflow
+            part1_1_num = random.randint(0, 999)  # Random 3-digit number
+            last_digit_choice = [1, 2]  # Choice for last digit
+            part1_2_num = int(str(part1_1_num)[-1]) + random.choice(
+                last_digit_choice
+            )  # Make last digit
+            if part1_2_num > 9:  # Check condition then overflow
                 part1_2_num = int(str(part1_2_num)[-1])
-            part1_str = f"{part1_1_num}{part1_2_num}" # Concat string
-            if int(part1_str) < 9991: # Check if < 9991
+            part1_str = f"{part1_1_num}{part1_2_num}"  # Concat string
+            if int(part1_str) < 9991:  # Check if < 9991
                 part1 = part1_str.rjust(4, "0")
                 part1_valid = True
 
         # PART 02
         part2 = __class__._mod7_gen(num_of_digits=7)  # type: ignore
 
         # OUTPUT
@@ -190,17 +187,17 @@
         - ``YY``: The last two digits of the year. It can be anything from ``95`` to ``03``
         - ``0XXXXXX``: A random number that has a sum that is divisible by ``7`` and does not end with ``0``, ``8`` or ``3``.
         - ``XXXXX``: A random 5-digit number
 
         Parameters
         ----------
         fast : bool
-            Use pre-generated key 
+            Use pre-generated key
             (Default: ``False``)
-        
+
         Returns
         -------
         str:
             Mod7 Key
         """
 
         # Fast mode: pre-generated key
@@ -229,17 +226,17 @@
     def mod7_combo(fast: bool = False):
         """
         A combo that consist of CD, 11-digit, and OEM Key
 
         Parameters
         ----------
         fast : bool
-            Use pre-generated key 
+            Use pre-generated key
             (Default: ``False``)
-        
+
         Returns
         -------
         dict:
             Mod7 Key combo
         """
         out = {
             "CD Key": __class__.mod7_cd_key(fast=fast),  # type: ignore
```

### Comparing `absfuyu-3.3.2/src/absfuyu/tools/obfuscator.py` & `absfuyu-3.3.3/src/absfuyu/tools/obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/tools/stats.py` & `absfuyu-3.3.3/src/absfuyu/tools/stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
+# flake8: noqa
 """
 Absfuyu: Stats
 --------------
-List's stats
+List's stats (soon will be deprecated)
 
 Version: 2.0.3
 Date updated: 26/11/2023 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
-__all__ = [
-    "ListStats"
-]
+__all__ = ["ListStats"]
 
 
 # Library
 ###########################################################################
 import math
 from typing import List, Union
 
@@ -24,14 +22,15 @@
 from absfuyu.logger import logger
 
 
 # Class
 ###########################################################################
 class ListStats(List[Union[int, float]]):
     """Stats"""
+
     def mean(self) -> float:
         """
         Mean/Average
 
         Returns
         -------
         float
@@ -41,20 +40,20 @@
         Example:
         --------
         >>> test = ListStats([1, 2, 3, 4, 5, 6])
         >>> test.mean()
         3.5
         """
         s = sum(self)
-        return s/len(self)
+        return s / len(self)
 
     def median(self) -> Union[int, float]:
         """
         Median/Middle
-        
+
         Returns
         -------
         int | float
             Median/Middle value
 
 
         Example:
@@ -72,17 +71,17 @@
             num2 = lst[math.floor(LENGTH / 2)]
             med = (num1 + num2) / 2
             return med
 
     def mode(self) -> List[Union[int, float]]:
         """
         Mode:
-        
+
             The Mode value is the value that appears the most number of times
-        
+
         Returns
         -------
         list[int | float]
             Mode value
 
 
         Example:
@@ -102,37 +101,37 @@
                 keys.append(k)
 
         return keys
 
     def var(self) -> float:
         """
         Variance
-        
+
         Returns
         -------
         float
             Variance value
 
 
         Example:
         --------
         >>> test = ListStats([1, 2, 3, 4, 5, 6])
         >>> test.var()
         2.9166666666666665
         """
         lst = self
         MEAN = self.mean()
-        v = [(x-MEAN)**2 for x in lst]
-        out = sum(v)/len(v)
+        v = [(x - MEAN) ** 2 for x in lst]
+        out = sum(v) / len(v)
         return out
 
     def std(self) -> float:
         """
         Standard deviation
-        
+
         Returns
         -------
         float
             Standard deviation value
 
 
         Example:
@@ -147,17 +146,17 @@
     def percentile(self, percent: int = 50) -> Union[int, float]:
         """
         Percentile
 
         Parameters
         ----------
         percent : int
-            Which percentile 
+            Which percentile
             (Default: ``50``)
-        
+
         Returns
         -------
         int | float
             Percentile value
 
 
         Example:
@@ -171,15 +170,15 @@
         if idx == len(lst):
             idx -= 1
         return sorted(lst)[idx]
 
     def summary(self):
         """
         Quick summary of data
-        
+
         Returns
         -------
         dict
             Summary of data
 
 
         Example:
@@ -208,19 +207,20 @@
             "Variance": self.var(),
             "Max": max(lst),
             "Min": min(lst),
             "Percentiles": {
                 "1st Quartile": self.percentile(25),
                 "2nd Quartile": self.percentile(50),
                 "3rd Quartile": self.percentile(75),
-            }
+            },
         }
         return output
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
     logger.setLevel(10)
     from rich import print
-    test = ListStats([1,8,9,2,3,4,4])
+
+    test = ListStats([1, 8, 9, 2, 3, 4, 4])
     print(test.summary())
```

### Comparing `absfuyu-3.3.2/src/absfuyu/tools/web.py` & `absfuyu-3.3.3/src/absfuyu/tools/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
         ``BeautifulSoup`` instance
     """
     try:
         page = requests.get(link)
         soup = BeautifulSoup(page.content, "html.parser")
         logger.debug("Soup completed!")
         return soup
-    except:
+    except Exception:
         logger.error("Can't soup")
-        raise SystemExit("Something wrong")
+        raise SystemExit("Something wrong")  # noqa: B904
 
 
 def gen_random_commit_msg() -> str:
     """
     Generate random commit message
 
     Returns
```

### Comparing `absfuyu-3.3.2/src/absfuyu/util/__init__.py` & `absfuyu-3.3.3/src/absfuyu/util/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/util/api.py` & `absfuyu-3.3.3/src/absfuyu/util/api.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/util/json_method.py` & `absfuyu-3.3.3/src/absfuyu/util/json_method.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/src/absfuyu/util/lunar.py` & `absfuyu-3.3.3/src/absfuyu/util/lunar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# flake8: noqa
 """
 Absfuyu: Lunar calendar
 -----------------------
 Convert to lunar calendar
 
 Version: 1.0.2
 Date updated: 05/04/2024 (dd/mm/yyyy)
```

### Comparing `absfuyu-3.3.2/src/absfuyu/util/performance.py` & `absfuyu-3.3.3/src/absfuyu/util/performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,15 @@
         return f"{self.__class__.__name__}({self.item_to_check})"
 
     @property
     def name(self) -> Union[Any, None]:
         """``__name__`` of variable (if any)"""
         try:
             return self.item_to_check.__name__
-        except:
+        except Exception:
             return None
 
     @property
     def value(self) -> Any:
         """Value of the variable"""
         return self.item_to_check
 
@@ -305,15 +305,15 @@
         return ListNoDunder(self.item_to_check.__dir__())
 
     @property
     def source(self) -> Union[str, None]:
         """Source code of variable (if available)"""
         try:
             return getsource(self.item_to_check)
-        except:
+        except Exception:
             return None
 
     def check(self, full: bool = False) -> Dict[str, Any]:
         """
         Check the variable
 
         Parameters
```

### Comparing `absfuyu-3.3.2/src/absfuyu/util/pkl.py` & `absfuyu-3.3.3/src/absfuyu/util/pkl.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 ---------------
 ``pickle`` wrapper
 
 Version: 1.0.2
 Last update: 24/11/2023 (dd/mm/yyyy)
 """
 
-
 # Module level
 ###########################################################################
 __all__ = ["Pickler"]
 
 
 # Library
 ###########################################################################
-from pathlib import Path
 import pickle
+from pathlib import Path
 from typing import Any
 
 
 # Class
 ###########################################################################
 class Pickler:
     """Save and load pickle file"""
```

### Comparing `absfuyu-3.3.2/src/absfuyu/util/zipped.py` & `absfuyu-3.3.3/src/absfuyu/util/zipped.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,33 +51,33 @@
         Zip file/folder
 
         :param delete_after_zip: Delete source after zip (Default: ``False``)
         :type delete_after_zip: bool
         """
 
         # Zip
-        logger.debug(f"Zipping...")
+        logger.debug("Zipping...")
         if self.source_path.is_dir():  # zip entire folder
             try:
                 with zipfile.ZipFile(self.destination, "w", zipfile.ZIP_DEFLATED) as f:
                     for file in self.source_path.rglob("*"):
                         f.write(file, file.relative_to(self.source_path))
-            except:
+            except Exception:
                 logger.error("Zip failed!")
                 # shutil.make_archive(zip_file, format="zip", root_dir=zip_path) # Method 2
         else:  # zip a file
             # Implement later
             pass
 
         # Delete folder
         if delete_after_zip:
             try:
-                logger.debug(f"Deleting unused folder...")
+                logger.debug("Deleting unused folder...")
                 shutil.rmtree(self.source_path)
-                logger.debug(f"Files deleted")
+                logger.debug("Files deleted")
             except OSError as e:
                 logger.error(f"Error: {e.filename} - {e.strerror}.")
 
 
 # Run
 ###########################################################################
 if __name__ == "__main__":
```

### Comparing `absfuyu-3.3.2/tests/test_config.py` & `absfuyu-3.3.3/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,15 @@
 import pytest
 
 from absfuyu.config import ABSFUYU_CONFIG, Setting
 
 
 # Setting
 def test_from_dict():
-    test = Setting.from_dict({
-        "test": {
-            "default": False,
-            "help": "HELP",
-            "value": True
-        }
-    })
+    _ = Setting.from_dict({"test": {"default": False, "help": "HELP", "value": True}})
     assert True
 
 
 # Config
 class TestConfig:
     def test_add_and_del_setting(self) -> None:
         # Make random name
```

### Comparing `absfuyu-3.3.2/tests/test_converter.py` & `absfuyu-3.3.3/tests/test_tools.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """
-Test: Converter
+Test: Tools
 
-Version: 1.2.0
-Date updated: 22/03/2024 (dd/mm/yyyy)
+Version: 1.0.0
+Date updated: 14/04/2024 (dd/mm/yyyy)
 """
 
+import base64
+
 import pytest
 
 from absfuyu.general.generator import Charset, Generator
 from absfuyu.tools.converter import Base64EncodeDecode, Text2Chemistry
+from absfuyu.tools.obfuscator import Obfuscator
 
 
+# MARK: fixture
 @pytest.fixture
-def instance():
-    return Text2Chemistry()
+def obfuscator_instance():
+    code = "print('Hello World')"
+    return Obfuscator(code=code)
 
 
-# convert
+# MARK: converter
+@pytest.mark.abs_tools
 class TestChemistryConvert:
-    @pytest.mark.parametrize(
-        ["instance", "value", "output"],
-        [
-            (Text2Chemistry(), "jump", []),
-            (Text2Chemistry(), "queen", []),
-        ],
-    )
-    def test_convert_not_work(
-        self, instance: Text2Chemistry, value: str, output: list
-    ) -> None:
+    """absfuyu.tools.converter.Text2Chemistry"""
+
+    @pytest.mark.parametrize(["value", "output"], [("jump", []), ("queen", [])])
+    def test_convert_not_work(self, value: str, output: list) -> None:
+        instance = Text2Chemistry()
         assert instance.convert(value) == output
 
-    def test_convert(self, instance: Text2Chemistry) -> None:
+    def test_convert(self) -> None:
+        instance = Text2Chemistry()
         assert instance.convert("bakery") != []
 
 
-# base64
+@pytest.mark.abs_tools
 class TestBase64:
+    """absfuyu.tools.converter.Base64EncodeDecode"""
+
     def test_base64_encode(self) -> None:
         test = Base64EncodeDecode.encode("Hello, World!")
         assert test == "SGVsbG8sIFdvcmxkIQ=="
 
     def test_base64_decode(self) -> None:
         test = Base64EncodeDecode.decode("SGVsbG8sIFdvcmxkIQ==")
         assert test == "Hello, World!"
@@ -48,7 +52,19 @@
         """Run multiple times"""
         TIMES = 100
         test = []
         for x in Generator.generate_string(Charset.FULL, times=TIMES):
             encode = Base64EncodeDecode.encode(x)
             test.append(x == Base64EncodeDecode.decode(encode))
         assert all(test)
+
+
+# MARK: obfuscator
+@pytest.mark.abs_tools
+class TestObfuscator:
+    """absfuyu.tools.obfuscator"""
+
+    def test_convert_to_base64_decode(self) -> None:
+        assert eval(Obfuscator._convert_to_base64_decode("rot_13")) == "rot_13"
+
+    def test_obfuscate(self, obfuscator_instance: Obfuscator) -> None:
+        assert obfuscator_instance.obfuscate()
```

### Comparing `absfuyu-3.3.2/tests/test_data_analysis.py` & `absfuyu-3.3.3/tests/test_data_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,156 +1,153 @@
 """
 Test: Data Analysis
 
 Version: 1.2.0
 Date updated: 08/03/2024 (dd/mm/yyyy)
 """
 
-
 # Library
 ###########################################################################
 import random
 
 import numpy as np
 import pandas as pd
 import pytest
 
-from absfuyu.general.generator import Generator, Charset
-from absfuyu.extensions.extra.data_analysis import (
-    CityData,
-    DADF, SplittedDF
-)
-
+from absfuyu.extensions.extra.data_analysis import DADF, CityData, SplittedDF
+from absfuyu.general.generator import Charset, Generator
 
 # Test
 ###########################################################################
 SAMPLE_SIZE = 100
 sample_city_data = CityData._sample_city_data(size=SAMPLE_SIZE)
 
+
 @pytest.fixture
 def sample_df() -> DADF:
     # Number of columns generated
     num_of_cols: int = random.randint(5, 10)
     # List of column name
     col_name: list = Generator.generate_string(
-        Charset.LOWERCASE, 
-        unique=True,
-        times=num_of_cols
+        Charset.LOWERCASE, unique=True, times=num_of_cols
     )
     # Create DataFrame
     df = pd.DataFrame(
-        np.random.randn(random.randint(5, 100), num_of_cols), 
-        columns=col_name
+        np.random.randn(random.randint(5, 100), num_of_cols), columns=col_name
     )
     out = DADF(df)
     return out
 
+
 @pytest.fixture
 def sample_df_2() -> DADF:
     return DADF.sample_df()
 
+
 @pytest.fixture
 def sample_df_3():
     sample = DADF.sample_df(size=SAMPLE_SIZE)
     sample["city"] = [x.city for x in sample_city_data]
     return sample
 
 
 # Drop cols
 def test_drop_rightmost(sample_df: DADF):
     num_of_cols_drop = random.randint(1, 4)
-    
+
     num_of_cols_current = sample_df.shape[1]
     sample_df.drop_rightmost(num_of_cols_drop)
     num_of_cols_modified = sample_df.shape[1]
-    
+
     condition = (num_of_cols_current - num_of_cols_modified) == num_of_cols_drop
     assert condition
 
 
 # Add blank column
 def test_add_blank_column(sample_df: DADF):
     original_num_of_cols = sample_df.shape[1]
     sample_df.add_blank_column("new_col", 0)
     new_num_of_cols = sample_df.shape[1]
 
-    condition = (
-        (new_num_of_cols - original_num_of_cols) == 1
-        and sum(sample_df["new_col"]) == 0
-    )
+    condition = (new_num_of_cols - original_num_of_cols) == 1 and sum(
+        sample_df["new_col"]
+    ) == 0
     assert condition
 
 
 # Add date column
 def test_add_date_from_month(sample_df_2: DADF):
     sample_df_2.add_detail_date("date", mode="m")
     original_num_of_cols = sample_df_2.shape[1]
     sample_df_2.add_date_from_month("month", col_name="mod_date")
     new_num_of_cols = sample_df_2.shape[1]
-    
+
     original_month = sample_df_2["month"][0]
     modified_month = sample_df_2["mod_date"][0].month
 
     # assert original_month == modified_month
     condition = (
-        (new_num_of_cols - original_num_of_cols) == 1
-        and original_month == modified_month
-    )
+        new_num_of_cols - original_num_of_cols
+    ) == 1 and original_month == modified_month
     assert condition
 
+
 def test_add_date_column(sample_df_2: DADF):
     # Get random mode
     mode_list = ["d", "w", "m", "y"]
     test_mode = list(map(lambda x: "".join(x), Generator.combinations_range(mode_list)))
     random_mode = random.choice(test_mode)
     num_of_new_cols = len(random_mode)
-    
+
     # Convert
     original_num_of_cols = sample_df_2.shape[1]
     sample_df_2.add_detail_date("date", mode=random_mode)
     new_num_of_cols = sample_df_2.shape[1]
     assert (new_num_of_cols - original_num_of_cols) == num_of_new_cols
 
 
 # Join and split
 def test_split_df(sample_df_2: DADF):
     test = sample_df_2.split_na("missing_value")
     assert len(test) > 1
 
+
 def test_split_df_2(sample_df_2: DADF):
     test = SplittedDF.divide_dataframe(sample_df_2, "number_range")
     assert len(test) > 1
 
+
 def test_join_df(sample_df_2: DADF):
     test = sample_df_2.split_na("missing_value")
     out = test.concat()
     assert out.shape[0] == 100
 
+
 def test_join_df_2(sample_df_2: DADF):
     """This test static method"""
     test = SplittedDF.divide_dataframe(sample_df_2, "number_range")
     out = SplittedDF.concat_df(test)
     assert out.shape[0] == 100
 
 
 # Threshold filter
 def test_threshold_filter(sample_df_2: DADF):
     original_num_of_cols = sample_df_2.shape[1]
     sample_df_2.threshold_filter("number_range", 11)
     new_num_of_cols = sample_df_2.shape[1]
-    
+
     # Check new column
     assert (new_num_of_cols - original_num_of_cols) == 1
 
     # Check filler value
     test: list = sample_df_2["number_range_filtered"].unique().tolist()
     try:
         test.index("Other")
         assert True
-    except:
+    except Exception:
         pass
 
     # Check len
     test1 = sample_df_2["number_range"].unique().tolist()
     assert (len(test1) - len(test)) >= 1
```

### Comparing `absfuyu-3.3.2/tests/test_everything.py` & `absfuyu-3.3.3/tests/test_everything.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Test: Everything
 
-Version: 1.1.23
-Date updated: 11/04/2024 (dd/mm/yyyy)
+Version: 1.1.26
+Date updated: 14/04/2024 (dd/mm/yyyy)
 """
 
 # Library
 ###########################################################################
 import pytest
 
 from absfuyu import __author__, __license__, __title__, __version__
@@ -23,17 +23,15 @@
 # --- Loading test --------------------------------------------------------
 # from absfuyu.core import *
 from absfuyu.core import (
     CONFIG_PATH,
     CORE_PATH,
     DATA_PATH,
     CLITextColor,
-    Color,
-    ModuleList,
-    ModulePackage,
+    __package_feature__,
 )
 from absfuyu.extensions import is_loaded
 from absfuyu.extensions.beautiful import beautiful_output, demo  # Has rich
 from absfuyu.extensions.extra import *
 from absfuyu.extensions.extra.data_analysis import (  # Has pandas, numpy
     CityData,
     DataAnalystDataFrame,
@@ -45,17 +43,17 @@
     equalize_df,
     rename_with_dict,
     summary,
 )
 from absfuyu.fun import force_shutdown, happy_new_year, im_bored, zodiac_sign
 from absfuyu.fun.tarot import Tarot, TarotCard
 from absfuyu.fun.WGS import WGS
-from absfuyu.game import game_escapeLoop, game_RockPaperScissors
+from absfuyu.game import GameStats, game_escapeLoop, game_RockPaperScissors
 from absfuyu.game.sudoku import Sudoku
-from absfuyu.game.tictactoe import game_tictactoe
+from absfuyu.game.tictactoe import GameMode, TicTacToe
 from absfuyu.game.wordle import Wordle  # Has requests
 
 # --- Sub-package ---
 from absfuyu.general import ClassBase, Dummy
 from absfuyu.general.content import (  # Has unidecode
     Content,
     ContentLoader,
```

### Comparing `absfuyu-3.3.2/tests/test_fun.py` & `absfuyu-3.3.3/tests/test_fun.py`

 * *Files identical despite different names*

### Comparing `absfuyu-3.3.2/tests/test_generator.py` & `absfuyu-3.3.3/tests/test_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 import pytest
 
 from absfuyu.general.generator import Charset, Generator
 
 
 class TestGenerator:
+    """absfuyu.general.generator.Generator"""
+
     # Charset
     @pytest.mark.parametrize(
         ["value", "output"],
         [
             (Charset.PRODUCT_KEY, "BCDFGHJKMNPQRTVWXY2346789"),
             (Charset.DEFAULT, string.ascii_letters + string.digits),
         ],
```

### Comparing `absfuyu-3.3.2/tests/test_logger.py` & `absfuyu-3.3.3/tests/test_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Test: Logger
 
 Version: 1.0.0
 Date updated: 19/11/2023 (dd/mm/yyyy)
 """
 
-
 # Library
 ###########################################################################
 import pytest
 
 from absfuyu.logger import compress_for_log
```

### Comparing `absfuyu-3.3.2/tests/test_passwordlib.py` & `absfuyu-3.3.3/tests/test_passwordlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 Test: Passwordlib
 
 Version: 1.1.0
 Date updated: 30/11/2023 (dd/mm/yyyy)
 """
 
-
 # Library
 ###########################################################################
 from itertools import combinations_with_replacement
 
 import pytest
 
-from absfuyu.general.data_extension import Text
 from absfuyu.extensions.dev.passwordlib import Password
-
+from absfuyu.general.data_extension import Text
 
 # Test
 ###########################################################################
 # def test_generate_password():
 #     test = [password_check(Password.generate_password()) for _ in range(100)]
 #     assert all(test)
 
@@ -47,10 +45,11 @@
             ).analyze()
             for _ in range(num_of_test)
         ]
         test = list(set(map(check, test)))
         if len(test) == 1:
             out.append(test[0] == check_value)
         else:
-            assert False
+            # assert False
+            raise AssertionError()
 
     assert all(out)
```

### Comparing `absfuyu-3.3.2/tests/test_version.py` & `absfuyu-3.3.3/tests/test_version.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,59 +11,61 @@
 import pytest
 
 from absfuyu.version import Bumper, ReleaseLevel, ReleaseOption, Version
 
 
 # Version
 class TestVersion:
-
     @pytest.mark.parametrize(
         ["major", "minor", "patch", "serial"], [(1, 0, 0, 5), ("1", "0", "0", "8")]
     )
     def test_init(
         self,
         major: Union[int, str],
         minor: Union[int, str],
         patch: Union[int, str],
         serial: Union[int, str],
     ) -> None:
         try:
             _ = Version(major, minor, patch, ReleaseLevel.DEV, serial)
             assert True
-        except Exception:
-            assert False
+        except Exception as err:
+            # assert False
+            raise AssertionError(err)
 
     @pytest.mark.parametrize("data", [list(), dict(), set(), tuple()])
     def test_init_error(self, data) -> None:
         with pytest.raises(TypeError) as excinfo:
             _ = Version(data, data, data)
         assert str(excinfo.value)
 
     @pytest.mark.parametrize("tuple_", [(1, 0, 0), (1, 0, 0, "dev", 0)])
     def test_from_tuple(self, tuple_: tuple) -> None:
         try:
             _ = Version.from_tuple(tuple_)
             assert True
-        except Exception:
-            assert False
+        except Exception as err:
+            # assert False
+            raise AssertionError(err)
 
     def test_from_tuple_error(self) -> None:
         with pytest.raises(ValueError) as excinfo:
             _ = Version.from_tuple((1, 0))
         assert str(excinfo.value)
 
     @pytest.mark.parametrize(
         "str_", ["1.0.0 ", " 100.8.48", "1.5.2.dev2", "1.2.4.rc8456", "1.9.4.final2"]
     )
     def test_from_str(self, str_: str) -> None:
         try:
             _ = Version.from_str(str_)
             assert True
-        except Exception:
-            assert False
+        except Exception as err:
+            # assert False
+            raise AssertionError(err)
 
     @pytest.mark.parametrize("str_", ["1.0.0s", "5555.1.fnl5"])
     def test_from_str_error(self, str_: str) -> None:
         with pytest.raises(ValueError) as excinfo:
             _ = Version.from_str(str_)
         assert str(excinfo.value)
```

### Comparing `absfuyu-3.3.2/.gitignore` & `absfuyu-3.3.3/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -126,22 +126,20 @@
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 
+# PyPI
 .pypirc
 
 
-# VS Code
-# .vscode
+# docs
+absfuyu*.rst
 
+# VS Code
+.vscode
 tempCodeRunnerFile.py
 
-
-
-
-note.txt
-tests.py
 testing/
 .bash_profile
```

### Comparing `absfuyu-3.3.2/LICENSE` & `absfuyu-3.3.3/LICENSE`

 * *Files identical despite different names*

