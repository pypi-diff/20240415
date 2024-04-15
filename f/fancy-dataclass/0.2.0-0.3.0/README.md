# Comparing `tmp/fancy_dataclass-0.2.0.tar.gz` & `tmp/fancy_dataclass-0.3.0.tar.gz`

## Comparing `fancy_dataclass-0.2.0.tar` & `fancy_dataclass-0.3.0.tar`

### file list

```diff
@@ -1,352 +1,363 @@
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/TODO.md
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass.json
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/ruff.toml
--rwxr-xr-x   0        0        0      118 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/summarize.sh
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/.lock
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/CACHEDIR.TAG
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/pyvenv.cfg
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/activate
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/activate.bat
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/activate.csh
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/activate.fish
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/activate.nu
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/activate.ps1
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/activate_this.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/deactivate.bat
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/pydoc.bat
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/python -> /Users/jerm/.pyenv/versions/3.11.0/bin/python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/bin/python3.11 -> python
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/_virtualenv.py
--rw-r--r--   0        0        0   117599 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/INSTALLER
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/METADATA
--rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/WHEEL
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/top_level.txt
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/__init__.py
--rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/config.py
--rw-r--r--   0        0        0    16663 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py
--rw-r--r--   0        0        0    15970 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/direct_url.json
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/events.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/exc.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/inspection.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/py.typed
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/schema.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/types.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/__init__.py
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/aioodbc.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/asyncio.py
--rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/pyodbc.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/__init__.py
--rwxr-xr-x   0        0        0   273374 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.cpython-311-darwin.so
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.pyx
--rwxr-xr-x   0        0        0   125312 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.cpython-311-darwin.so
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pxd
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pyx
--rwxr-xr-x   0        0        0   104925 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.cpython-311-darwin.so
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.pyx
--rwxr-xr-x   0        0        0   107806 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.cpython-311-darwin.so
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.pyx
--rwxr-xr-x   0        0        0   125335 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.cpython-311-darwin.so
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.pyx
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/_typing.py
--rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/__init__.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/aioodbc.py
--rw-r--r--   0        0        0   132301 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/base.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/information_schema.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/json.py
--rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/provision.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pymssql.py
--rw-r--r--   0        0        0    27056 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pyodbc.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/__init__.py
--rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/aiomysql.py
--rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/asyncmy.py
--rw-r--r--   0        0        0   120850 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/base.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/cymysql.py
--rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/dml.py
--rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/enumerated.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/expression.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/json.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadb.py
--rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadbconnector.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqlconnector.py
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqldb.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/provision.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pymysql.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pyodbc.py
--rw-r--r--   0        0        0    22822 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reflection.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reserved_words.py
--rw-r--r--   0        0        0    24343 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/types.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/__init__.py
--rw-r--r--   0        0        0   118246 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/base.py
--rw-r--r--   0        0        0    55566 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/cx_oracle.py
--rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/dictionary.py
--rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/oracledb.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/provision.py
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/types.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/__init__.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/_psycopg_common.py
--rw-r--r--   0        0        0    13734 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/array.py
--rw-r--r--   0        0        0    40240 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/asyncpg.py
--rw-r--r--   0        0        0   178989 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/base.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/dml.py
--rw-r--r--   0        0        0    16262 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ext.py
--rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/hstore.py
--rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/json.py
--rw-r--r--   0        0        0    17594 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/named_types.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/operators.py
--rw-r--r--   0        0        0    18640 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg8000.py
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg_catalog.py
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/provision.py
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg.py
--rw-r--r--   0        0        0    31607 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2cffi.py
--rw-r--r--   0        0        0    32949 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ranges.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/types.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/__init__.py
--rw-r--r--   0        0        0    12305 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/aiosqlite.py
--rw-r--r--   0        0        0    96794 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/base.py
--rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/dml.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/json.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/provision.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlcipher.py
--rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlite.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/__init__.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_processors.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_row.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_util.py
--rw-r--r--   0        0        0   123050 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/base.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/characteristics.py
--rw-r--r--   0        0        0    33206 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/create.py
--rw-r--r--   0        0        0    76314 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/cursor.py
--rw-r--r--   0        0        0    83993 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/default.py
--rw-r--r--   0        0        0    37381 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/events.py
--rw-r--r--   0        0        0   112832 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/interfaces.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/mock.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/processors.py
--rw-r--r--   0        0        0    75127 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/reflection.py
--rw-r--r--   0        0        0    77603 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/result.py
--rw-r--r--   0        0        0    12032 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/row.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/strategies.py
--rw-r--r--   0        0        0    30784 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/url.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/util.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/api.py
--rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/attr.py
--rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/base.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/legacy.py
--rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/registry.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/__init__.py
--rw-r--r--   0        0        0    65771 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/associationproxy.py
--rw-r--r--   0        0        0    61576 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/automap.py
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/baked.py
--rw-r--r--   0        0        0    20391 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/compiler.py
--rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/horizontal_shard.py
--rw-r--r--   0        0        0    52432 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/hybrid.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/indexable.py
--rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/instrumentation.py
--rw-r--r--   0        0        0    37355 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mutable.py
--rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/orderinglist.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/serializer.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/__init__.py
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/base.py
--rw-r--r--   0        0        0    48190 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/engine.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/exc.py
--rw-r--r--   0        0        0    30409 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/result.py
--rw-r--r--   0        0        0    52597 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/scoping.py
--rw-r--r--   0        0        0    63092 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/session.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/__init__.py
--rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/extensions.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/__init__.py
--rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/apply.py
--rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/decl_class.py
--rw-r--r--   0        0        0    19369 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/infer.py
--rw-r--r--   0        0        0    10479 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/names.py
--rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/plugin.py
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/util.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/future/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/future/engine.py
--rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/__init__.py
--rw-r--r--   0        0        0    99461 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_orm_constructors.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_typing.py
--rw-r--r--   0        0        0    92535 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/attributes.py
--rw-r--r--   0        0        0    27466 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/base.py
--rw-r--r--   0        0        0    70022 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/bulk_persistence.py
--rw-r--r--   0        0        0    17958 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/clsregistry.py
--rw-r--r--   0        0        0    52179 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/collections.py
--rw-r--r--   0        0        0   112001 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/context.py
--rw-r--r--   0        0        0    63674 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_api.py
--rw-r--r--   0        0        0    81601 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_base.py
--rw-r--r--   0        0        0    47631 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dependency.py
--rw-r--r--   0        0        0    37180 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/descriptor_props.py
--rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dynamic.py
--rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/evaluator.py
--rw-r--r--   0        0        0   127703 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/events.py
--rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/exc.py
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/identity.py
--rw-r--r--   0        0        0    24321 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/instrumentation.py
--rw-r--r--   0        0        0    48502 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/interfaces.py
--rw-r--r--   0        0        0    57537 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/loading.py
--rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapped_collection.py
--rw-r--r--   0        0        0   171059 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapper.py
--rw-r--r--   0        0        0    25850 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/path_registry.py
--rw-r--r--   0        0        0    61701 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/persistence.py
--rw-r--r--   0        0        0    29294 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/properties.py
--rw-r--r--   0        0        0   117596 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/query.py
--rw-r--r--   0        0        0   128644 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/relationships.py
--rw-r--r--   0        0        0    78677 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/scoping.py
--rw-r--r--   0        0        0   193181 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/session.py
--rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state.py
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py
--rw-r--r--   0        0        0   114206 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategies.py
--rw-r--r--   0        0        0    84563 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategy_options.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/sync.py
--rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/unitofwork.py
--rw-r--r--   0        0        0    80660 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/util.py
--rw-r--r--   0        0        0    22305 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/writeonly.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/__init__.py
--rw-r--r--   0        0        0    52236 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/base.py
--rw-r--r--   0        0        0    13147 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/events.py
--rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/impl.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/__init__.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_dml_constructors.py
--rw-r--r--   0        0        0    62587 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_elements_constructors.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_orm_types.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_py_util.py
--rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_selectable_constructors.py
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_typing.py
--rw-r--r--   0        0        0    18245 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/annotation.py
--rw-r--r--   0        0        0    73797 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/base.py
--rw-r--r--   0        0        0    33668 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/cache_key.py
--rw-r--r--   0        0        0    40493 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/coercions.py
--rw-r--r--   0        0        0   274503 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/compiler.py
--rw-r--r--   0        0        0    56521 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/crud.py
--rw-r--r--   0        0        0    45602 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/ddl.py
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/default_comparator.py
--rw-r--r--   0        0        0    65614 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/dml.py
--rw-r--r--   0        0        0   173693 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/elements.py
--rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/events.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/expression.py
--rw-r--r--   0        0        0    63689 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/functions.py
--rw-r--r--   0        0        0    49292 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/lambdas.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/naming.py
--rw-r--r--   0        0        0    75935 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/operators.py
--rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/roles.py
--rw-r--r--   0        0        0   228317 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/schema.py
--rw-r--r--   0        0        0   232848 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/selectable.py
--rw-r--r--   0        0        0   126076 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/sqltypes.py
--rw-r--r--   0        0        0    33589 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/traversals.py
--rw-r--r--   0        0        0    83208 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/type_api.py
--rw-r--r--   0        0        0    48077 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/util.py
--rw-r--r--   0        0        0    36317 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/visitors.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/__init__.py
--rw-r--r--   0        0        0    31439 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertions.py
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertsql.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/asyncio.py
--rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/config.py
--rw-r--r--   0        0        0    13481 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/engines.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/entities.py
--rw-r--r--   0        0        0    12460 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/exclusions.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/pickleable.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/profiling.py
--rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/provision.py
--rw-r--r--   0        0        0    51817 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/requirements.py
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/schema.py
--rw-r--r--   0        0        0    14080 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/util.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/warnings.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/__init__.py
--rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/base.py
--rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/mypy.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/orm.py
--rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/sql.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/__init__.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/bootstrap.py
--rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/plugin_base.py
--rw-r--r--   0        0        0    27656 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/pytestplugin.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/__init__.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_cte.py
--rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_ddl.py
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_deprecations.py
--rw-r--r--   0        0        0    22923 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_dialect.py
--rw-r--r--   0        0        0    18824 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_insert.py
--rw-r--r--   0        0        0   106466 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_reflection.py
--rw-r--r--   0        0        0    15937 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_results.py
--rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_rowcount.py
--rw-r--r--   0        0        0    58574 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_select.py
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_sequence.py
--rw-r--r--   0        0        0    65677 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_types.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_unicode_ddl.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_update_delete.py
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/__init__.py
--rw-r--r--   0        0        0    20063 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_collections.py
--rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_concurrency_py3k.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_has_cy.py
--rw-r--r--   0        0        0    16714 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_py_collections.py
--rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/compat.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/concurrency.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/deprecations.py
--rw-r--r--   0        0        0    64957 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/preloaded.py
--rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/queue.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/tool_support.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/topological.py
--rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/typing.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/WHEEL
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/docs/LICENSE.txt
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/docs/cli.md
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/docs/json.md
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/docs/sql.md
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/docs/subprocess.md
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass/__init__.py
--rw-r--r--   0        0        0    14543 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass/cli.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass/config.py
--rw-r--r--   0        0        0    15960 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass/dict.py
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass/json.py
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass/mixin.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass/sql.py
--rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass/subprocess.py
--rw-r--r--   0        0        0    17262 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/fancy_dataclass/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/tests/test_cli.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/tests/test_dict.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/tests/test_inheritance.py
--rw-r--r--   0        0        0    18368 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/tests/test_json.py
--rw-r--r--   0        0        0    10619 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/tests/test_mixin.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/tests/test_sql.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/tests/test_subprocess.py
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/.gitignore
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/docs/README.md
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 fancy_dataclass-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/TODO.md
+-rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass.json
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/loc-summary.txt
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/ruff.toml
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/summarize.sh
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/website_config.toml
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/CACHEDIR.TAG
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.bat
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate_this.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/deactivate.bat
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/pydoc.bat
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/python -> /Users/jerm/.pyenv/versions/3.11.0/bin/python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/python3.11 -> python
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0   117599 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/METADATA
+-rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/WHEEL
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/top_level.txt
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/__init__.py
+-rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/config.py
+-rw-r--r--   0        0        0    16663 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py
+-rw-r--r--   0        0        0    15970 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/direct_url.json
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/events.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/exc.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/inspection.py
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/py.typed
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/schema.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/types.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/__init__.py
+-rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/aioodbc.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/asyncio.py
+-rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/pyodbc.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/__init__.py
+-rwxr-xr-x   0        0        0   273374 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.cpython-311-darwin.so
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.pyx
+-rwxr-xr-x   0        0        0   125312 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.cpython-311-darwin.so
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pxd
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pyx
+-rwxr-xr-x   0        0        0   104925 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.cpython-311-darwin.so
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.pyx
+-rwxr-xr-x   0        0        0   107806 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.cpython-311-darwin.so
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.pyx
+-rwxr-xr-x   0        0        0   125335 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.cpython-311-darwin.so
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.pyx
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/_typing.py
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/aioodbc.py
+-rw-r--r--   0        0        0   132301 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/base.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/information_schema.py
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/json.py
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/provision.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pymssql.py
+-rw-r--r--   0        0        0    27056 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pyodbc.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/__init__.py
+-rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/aiomysql.py
+-rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/asyncmy.py
+-rw-r--r--   0        0        0   120850 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/base.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/cymysql.py
+-rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/dml.py
+-rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/enumerated.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/expression.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/json.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadb.py
+-rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadbconnector.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqlconnector.py
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqldb.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/provision.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pymysql.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pyodbc.py
+-rw-r--r--   0        0        0    22822 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reflection.py
+-rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reserved_words.py
+-rw-r--r--   0        0        0    24343 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/types.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/__init__.py
+-rw-r--r--   0        0        0   118246 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/base.py
+-rw-r--r--   0        0        0    55566 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/cx_oracle.py
+-rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/dictionary.py
+-rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/oracledb.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/provision.py
+-rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/types.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/__init__.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/_psycopg_common.py
+-rw-r--r--   0        0        0    13734 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/array.py
+-rw-r--r--   0        0        0    40240 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/asyncpg.py
+-rw-r--r--   0        0        0   178989 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/base.py
+-rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/dml.py
+-rw-r--r--   0        0        0    16262 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ext.py
+-rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/hstore.py
+-rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/json.py
+-rw-r--r--   0        0        0    17594 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/named_types.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/operators.py
+-rw-r--r--   0        0        0    18640 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg8000.py
+-rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg_catalog.py
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/provision.py
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg.py
+-rw-r--r--   0        0        0    31607 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2cffi.py
+-rw-r--r--   0        0        0    32949 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ranges.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/types.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/__init__.py
+-rw-r--r--   0        0        0    12305 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/aiosqlite.py
+-rw-r--r--   0        0        0    96794 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/base.py
+-rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/dml.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/json.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/provision.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlcipher.py
+-rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlite.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/__init__.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_processors.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_row.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_util.py
+-rw-r--r--   0        0        0   123050 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/base.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/characteristics.py
+-rw-r--r--   0        0        0    33206 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/create.py
+-rw-r--r--   0        0        0    76314 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/cursor.py
+-rw-r--r--   0        0        0    83993 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/default.py
+-rw-r--r--   0        0        0    37381 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/events.py
+-rw-r--r--   0        0        0   112832 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/interfaces.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/mock.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/processors.py
+-rw-r--r--   0        0        0    75127 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/reflection.py
+-rw-r--r--   0        0        0    77603 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/result.py
+-rw-r--r--   0        0        0    12032 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/row.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/strategies.py
+-rw-r--r--   0        0        0    30784 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/url.py
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/util.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/api.py
+-rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/attr.py
+-rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/base.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/legacy.py
+-rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/registry.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/__init__.py
+-rw-r--r--   0        0        0    65771 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/associationproxy.py
+-rw-r--r--   0        0        0    61576 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/automap.py
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/baked.py
+-rw-r--r--   0        0        0    20391 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/compiler.py
+-rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/horizontal_shard.py
+-rw-r--r--   0        0        0    52432 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/hybrid.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/indexable.py
+-rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/instrumentation.py
+-rw-r--r--   0        0        0    37355 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mutable.py
+-rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/orderinglist.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/serializer.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/__init__.py
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/base.py
+-rw-r--r--   0        0        0    48190 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/engine.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/exc.py
+-rw-r--r--   0        0        0    30409 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/result.py
+-rw-r--r--   0        0        0    52597 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/scoping.py
+-rw-r--r--   0        0        0    63092 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/session.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/__init__.py
+-rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/extensions.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/__init__.py
+-rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/apply.py
+-rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/decl_class.py
+-rw-r--r--   0        0        0    19369 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/infer.py
+-rw-r--r--   0        0        0    10479 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/names.py
+-rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/plugin.py
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/util.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/future/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/future/engine.py
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/__init__.py
+-rw-r--r--   0        0        0    99461 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_orm_constructors.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_typing.py
+-rw-r--r--   0        0        0    92535 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/attributes.py
+-rw-r--r--   0        0        0    27466 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/base.py
+-rw-r--r--   0        0        0    70022 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/bulk_persistence.py
+-rw-r--r--   0        0        0    17958 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/clsregistry.py
+-rw-r--r--   0        0        0    52179 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/collections.py
+-rw-r--r--   0        0        0   112001 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/context.py
+-rw-r--r--   0        0        0    63674 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_api.py
+-rw-r--r--   0        0        0    81601 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_base.py
+-rw-r--r--   0        0        0    47631 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dependency.py
+-rw-r--r--   0        0        0    37180 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/descriptor_props.py
+-rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dynamic.py
+-rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/evaluator.py
+-rw-r--r--   0        0        0   127703 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/events.py
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/exc.py
+-rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/identity.py
+-rw-r--r--   0        0        0    24321 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/instrumentation.py
+-rw-r--r--   0        0        0    48502 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/interfaces.py
+-rw-r--r--   0        0        0    57537 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/loading.py
+-rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapped_collection.py
+-rw-r--r--   0        0        0   171059 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapper.py
+-rw-r--r--   0        0        0    25850 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/path_registry.py
+-rw-r--r--   0        0        0    61701 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/persistence.py
+-rw-r--r--   0        0        0    29294 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/properties.py
+-rw-r--r--   0        0        0   117596 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/query.py
+-rw-r--r--   0        0        0   128644 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/relationships.py
+-rw-r--r--   0        0        0    78677 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/scoping.py
+-rw-r--r--   0        0        0   193181 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/session.py
+-rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state.py
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py
+-rw-r--r--   0        0        0   114206 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategies.py
+-rw-r--r--   0        0        0    84563 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategy_options.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/sync.py
+-rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/unitofwork.py
+-rw-r--r--   0        0        0    80660 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/util.py
+-rw-r--r--   0        0        0    22305 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/writeonly.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/__init__.py
+-rw-r--r--   0        0        0    52236 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/base.py
+-rw-r--r--   0        0        0    13147 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/events.py
+-rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/impl.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/__init__.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_dml_constructors.py
+-rw-r--r--   0        0        0    62587 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_elements_constructors.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_orm_types.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_py_util.py
+-rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_selectable_constructors.py
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_typing.py
+-rw-r--r--   0        0        0    18245 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/annotation.py
+-rw-r--r--   0        0        0    73797 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/base.py
+-rw-r--r--   0        0        0    33668 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/cache_key.py
+-rw-r--r--   0        0        0    40493 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/coercions.py
+-rw-r--r--   0        0        0   274503 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/compiler.py
+-rw-r--r--   0        0        0    56521 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/crud.py
+-rw-r--r--   0        0        0    45602 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/ddl.py
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/default_comparator.py
+-rw-r--r--   0        0        0    65614 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/dml.py
+-rw-r--r--   0        0        0   173693 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/elements.py
+-rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/events.py
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/expression.py
+-rw-r--r--   0        0        0    63689 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/functions.py
+-rw-r--r--   0        0        0    49292 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/lambdas.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/naming.py
+-rw-r--r--   0        0        0    75935 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/operators.py
+-rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/roles.py
+-rw-r--r--   0        0        0   228317 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/schema.py
+-rw-r--r--   0        0        0   232848 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/selectable.py
+-rw-r--r--   0        0        0   126076 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/sqltypes.py
+-rw-r--r--   0        0        0    33589 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/traversals.py
+-rw-r--r--   0        0        0    83208 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/type_api.py
+-rw-r--r--   0        0        0    48077 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/util.py
+-rw-r--r--   0        0        0    36317 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/visitors.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/__init__.py
+-rw-r--r--   0        0        0    31439 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertions.py
+-rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertsql.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/asyncio.py
+-rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/config.py
+-rw-r--r--   0        0        0    13481 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/engines.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/entities.py
+-rw-r--r--   0        0        0    12460 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/exclusions.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/pickleable.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/profiling.py
+-rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/provision.py
+-rw-r--r--   0        0        0    51817 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/requirements.py
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/schema.py
+-rw-r--r--   0        0        0    14080 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/util.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/warnings.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/__init__.py
+-rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/base.py
+-rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/mypy.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/orm.py
+-rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/sql.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/__init__.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/bootstrap.py
+-rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/plugin_base.py
+-rw-r--r--   0        0        0    27656 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/pytestplugin.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/__init__.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_cte.py
+-rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_ddl.py
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_deprecations.py
+-rw-r--r--   0        0        0    22923 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_dialect.py
+-rw-r--r--   0        0        0    18824 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_insert.py
+-rw-r--r--   0        0        0   106466 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_reflection.py
+-rw-r--r--   0        0        0    15937 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_results.py
+-rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_rowcount.py
+-rw-r--r--   0        0        0    58574 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_select.py
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_sequence.py
+-rw-r--r--   0        0        0    65677 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_types.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_unicode_ddl.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_update_delete.py
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/__init__.py
+-rw-r--r--   0        0        0    20063 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_collections.py
+-rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_concurrency_py3k.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_has_cy.py
+-rw-r--r--   0        0        0    16714 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_py_collections.py
+-rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/compat.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/concurrency.py
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/deprecations.py
+-rw-r--r--   0        0        0    64957 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/preloaded.py
+-rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/queue.py
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/tool_support.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/topological.py
+-rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/typing.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/LICENSE.txt
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/cli.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/config.md
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/json.md
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/sql.md
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/subprocess.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/toml.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/__init__.py
+-rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/cli.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/config.py
+-rw-r--r--   0        0        0    16986 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/dict.py
+-rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/json.py
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/mixin.py
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/serialize.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/sql.py
+-rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/subprocess.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/toml.py
+-rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_config.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_dict.py
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_inheritance.py
+-rw-r--r--   0        0        0    10619 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_mixin.py
+-rw-r--r--   0        0        0    24866 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_serializable.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_sql.py
+-rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_subprocess.py
+-rw-r--r--   0        0        0    11567 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/workflows/mypy.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/workflows/ruff.yml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.gitignore
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/README.md
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/PKG-INFO
```

### Comparing `fancy_dataclass-0.2.0/.pre-commit-config.yaml` & `fancy_dataclass-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/TODO.md` & `fancy_dataclass-0.3.0/TODO.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # TODO
 
 ## v0.3.0
 
-- ConfigDataclass
-  - Handle nesting properly (updating nested ConfigDataclass should update the parent)
-  - Load from JSON/TOML
-    - Options:
-      1. Inherit from JSONDataclass/TOMLDataclass (superfluous)?
-      2. Method to load from either, which calls `from_dict` on a proxy class then `coerce_to_dataclass`?
-    - Infer file type from extension
-- TOMLDataclass
-  - `tomlkit` maintains parsed structure (incl. whitespace & comments)
-  - Let ConfigDataclass parse TOML
-- Basic usage examples in docs
+- Github Actions for automated testing
+  - Coverage badge
+  - Auto-publish when new tag is pushed (see: https://pypi.org/manage/project/fancy-dataclass/settings/publishing/)
+- Release
+  - CHANGELOG update
+  - Tag v0.3.0
+  - Check PyPI page links to Read the Docs
 
 ## v0.3.1
 
+- `DictConfig` subclass of `Config` (unstructured configs loaded from JSON/TOML)
 - documentation
   - Dataclass mixins/settings
     - For now, `dataclass` decorator is required
     - Note purpose of `flattened=True` (good for tabular data like CSV/SQL)
     - Advanced: how to handle name collisions in settings for multiple inheritance (e.g. `ArgparseDataclass`/`SubprocessDataclass`)
   - JSON
   - TOML
@@ -27,25 +24,28 @@
   - SQL
     - Primary key (default `_id`)
     - Relationships
   - Subprocess
   - Config
   - Defining new mixins (what dunders need to be set)
     - Top-level settings, field-level settings, collisions
-  - Host on GH Pages or Readthedocs
-- Github Actions for automated testing
-  - Configure as much as possible via `hatch`
-    - `ruff`, `mypy`, `pytest`, `radon`
-    - Multiple versions of Python
-  - Coverage badge
 
 ## Future
 
+- `FileSerializable`
+  - Add `save` and `load` convenience methods?
+- `TOMLDataclass`
+  - Require subclass to set `qualified_type=True`, like `JSONDataclass`?
+  - Preserve document structure via `tomlkit`
+    - NOTE: the parsed values themselves have a `_trivia` attribute storing various formatting info
+    - Use field metadata (`help`?) as comment prior to the field
+  - For `None`, serialize as commented field?
 - `TabularDataclass`? CSV/TSV/parquet/feather
   - Make `SQLDataclass` inherit from it
+  - Convert to/from `pandas` `Series` and `DataFrame`?
 - Support subparsers in `ArgparseDataclass`
 - Field metadata
   - Be strict about unknown field metadata keys? (Maybe issue warning?)
     - Might be annoying if people want to store extra metadata.
   - PEP 712 (`converter` argument for dataclass fields)
   - Allow `Annotated` as an alternative to `field.metadata`
     - Esp. with `Doc`: this could auto-populate JSON schema, argparse description
```

### Comparing `fancy_dataclass-0.2.0/fancy_dataclass.json` & `fancy_dataclass-0.3.0/fancy_dataclass.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9660511363636364%*

 * *Differences: {"'tasks'": "{'1': {'name': 'toml-dataclass', 'status': 'complete', 'total_time_worked': "*

 * *            "0.9903421058101852, 'priority': 8.0, 'first_started_time': "*

 * *            "'2024-04-13T15:22:08Z-0400', 'completed_time': '2024-04-14T15:08:13Z-0400', "*

 * *            "'lead_time': 24.67241587111111, 'cycle_time': 0.9903421058101852}, '8': {'status': "*

 * *            "'complete', 'total_time_worked': 0.01041666925925926, 'first_started_time': "*

 * *            "'2024-04-13T13:14:55Z-0400', 'completed_time': '2024-0 […]*

```diff
@@ -2,33 +2,38 @@
     "created_time": "2024-03-20T22:58:02Z-0400",
     "name": "fancy_dataclass",
     "projects": {},
     "tasks": {
         "0": {
             "completed_time": "2024-04-13T10:08:13Z-0400",
             "created_time": "2024-04-12T20:51:56Z-0400",
-            "cycle_time": 0.5473734905092593,
+            "cycle_time": 0.5473726851851852,
             "description": "Unit tests for new behavior.",
             "expected_duration": 0.0625,
             "first_started_time": "2024-04-12T21:00:00Z-0400",
             "is_overdue": false,
-            "lead_time": 0.5529753423611111,
+            "lead_time": 0.552974537037037,
             "name": "unit-tests",
             "priority": 7.0,
             "status": "complete",
-            "total_time_worked": 0.5473734905092593
+            "total_time_worked": 0.5473726851851852
         },
         "1": {
+            "completed_time": "2024-04-14T15:08:13Z-0400",
             "created_time": "2024-03-20T22:59:57Z-0400",
+            "cycle_time": 0.9903421058101852,
             "description": "Provide a toml submodule with TOMLDataclass mixin.",
             "expected_duration": 0.10416666666666667,
+            "first_started_time": "2024-04-13T15:22:08Z-0400",
             "is_overdue": false,
-            "name": "toml",
-            "status": "todo",
-            "total_time_worked": 0.0
+            "lead_time": 24.67241587111111,
+            "name": "toml-dataclass",
+            "priority": 8.0,
+            "status": "complete",
+            "total_time_worked": 0.9903421058101852
         },
         "10": {
             "completed_time": "2024-03-29T23:50:04Z-0400",
             "created_time": "2024-03-27T18:23:19Z-0400",
             "cycle_time": 2.2267824074074074,
             "description": "Implement flattening/merging of dataclasses.",
             "expected_duration": 0.16666666666666666,
@@ -53,24 +58,24 @@
             "priority": 7.0,
             "status": "complete",
             "total_time_worked": 2.354722222222222
         },
         "12": {
             "completed_time": "2024-04-13T13:08:59Z-0400",
             "created_time": "2024-04-12T20:52:37Z-0400",
-            "cycle_time": 0.08371509230324074,
+            "cycle_time": 0.08371527777777778,
             "description": "Write 1-2 sentence intro for each dataclass mixin.",
             "expected_duration": 0.020833333333333332,
             "first_started_time": "2024-04-13T11:08:26Z-0400",
             "is_overdue": false,
-            "lead_time": 0.6780341079513889,
+            "lead_time": 0.6780324074074074,
             "name": "doc-subpage-intro",
             "priority": 7.0,
             "status": "complete",
-            "total_time_worked": 0.08371509230324074
+            "total_time_worked": 0.08371527777777778
         },
         "13": {
             "completed_time": "2024-04-11T22:00:00Z-0400",
             "created_time": "2024-03-28T20:25:43Z-0400",
             "cycle_time": 10.166666666666666,
             "description": "Placeholders for mixin pages; CHANGELOG.",
             "expected_duration": 0.03125,
@@ -78,14 +83,98 @@
             "is_overdue": false,
             "lead_time": 14.065474537037037,
             "name": "basic-docs",
             "priority": 5.0,
             "status": "complete",
             "total_time_worked": 10.166666666666666
         },
+        "14": {
+            "completed_time": "2024-04-13T17:32:39Z-0400",
+            "created_time": "2024-04-13T13:31:38Z-0400",
+            "cycle_time": 0.16030777625,
+            "description": "Finish ConfigDataclass functionality.",
+            "expected_duration": 0.0625,
+            "first_started_time": "2024-04-13T13:41:48Z-0400",
+            "is_overdue": false,
+            "lead_time": 0.16737078806712963,
+            "name": "config-dataclass",
+            "priority": 9.0,
+            "status": "complete",
+            "total_time_worked": 0.16030777625
+        },
+        "15": {
+            "completed_time": "2024-04-14T15:08:05Z-0400",
+            "created_time": "2024-04-13T13:32:53Z-0400",
+            "cycle_time": 0.6798178644328703,
+            "description": "Unit tests for TOMLDataclass.",
+            "expected_duration": 0.03125,
+            "first_started_time": "2024-04-13T22:49:09Z-0400",
+            "is_overdue": false,
+            "lead_time": 1.0661049099305555,
+            "name": "test-toml",
+            "priority": 7.0,
+            "status": "complete",
+            "total_time_worked": 0.6798178644328703
+        },
+        "16": {
+            "completed_time": "2024-04-14T15:08:10Z-0400",
+            "created_time": "2024-04-13T13:33:15Z-0400",
+            "cycle_time": 1.0529555267476851,
+            "description": "Unit tests for ConfigDataclass.",
+            "expected_duration": 0.041666666666666664,
+            "first_started_time": "2024-04-13T13:51:55Z-0400",
+            "is_overdue": false,
+            "lead_time": 1.0659096260300924,
+            "name": "test-config",
+            "priority": 7.0,
+            "status": "complete",
+            "total_time_worked": 1.0529555267476851
+        },
+        "17": {
+            "completed_time": "2024-04-14T16:34:48Z-0400",
+            "created_time": "2024-04-13T13:34:20Z-0400",
+            "cycle_time": 0.046288002465277776,
+            "description": "Basic doc page for ConfigDataclass.",
+            "expected_duration": 0.03125,
+            "first_started_time": "2024-04-14T15:28:09Z-0400",
+            "is_overdue": false,
+            "lead_time": 1.125332669525463,
+            "name": "basic-doc-config",
+            "priority": 6.0,
+            "status": "complete",
+            "total_time_worked": 0.046288002465277776
+        },
+        "18": {
+            "completed_time": "2024-04-14T15:28:04Z-0400",
+            "created_time": "2024-04-13T13:34:40Z-0400",
+            "cycle_time": 0.012613337962962963,
+            "description": "Basic doc page for TOMLDataclass.",
+            "expected_duration": 0.03125,
+            "first_started_time": "2024-04-14T15:09:54Z-0400",
+            "is_overdue": false,
+            "lead_time": 1.0787444866666667,
+            "name": "basic-doc-toml",
+            "priority": 6.0,
+            "status": "complete",
+            "total_time_worked": 0.012613337962962963
+        },
+        "19": {
+            "completed_time": "2024-04-14T18:01:10Z-0400",
+            "created_time": "2024-04-13T13:35:20Z-0400",
+            "cycle_time": 0.05613431138888889,
+            "description": "Host docs on GH Pages or Readthedocs.",
+            "expected_duration": 0.041666666666666664,
+            "first_started_time": "2024-04-14T16:40:20Z-0400",
+            "is_overdue": false,
+            "lead_time": 1.1846013796990742,
+            "name": "host-docs",
+            "priority": 6.0,
+            "status": "complete",
+            "total_time_worked": 0.05613431138888889
+        },
         "2": {
             "created_time": "2024-03-20T23:01:36Z-0400",
             "description": "Documentation for configuring fancy dataclasses.",
             "expected_duration": 0.027777777777777776,
             "is_overdue": false,
             "name": "doc-config",
             "status": "todo",
@@ -133,27 +222,33 @@
             "expected_duration": 0.027777777777777776,
             "is_overdue": false,
             "name": "doc-subprocess",
             "status": "todo",
             "total_time_worked": 0.0
         },
         "8": {
+            "completed_time": "2024-04-13T13:29:55Z-0400",
             "created_time": "2024-03-20T23:03:22Z-0400",
+            "cycle_time": 0.01041666925925926,
             "description": "Upload package to PyPI.",
             "expected_duration": 0.03125,
+            "first_started_time": "2024-04-13T13:14:55Z-0400",
             "is_overdue": false,
+            "lead_time": 23.601778137986113,
             "name": "pypi",
-            "status": "todo",
-            "total_time_worked": 0.0
+            "status": "complete",
+            "total_time_worked": 0.01041666925925926
         },
         "9": {
             "created_time": "2024-03-20T23:03:50Z-0400",
             "description": "Set up Github Actions for automated linting/testing.",
             "expected_duration": 0.08333333333333333,
+            "first_started_time": "2024-04-14T18:17:55Z-0400",
             "is_overdue": false,
             "name": "gh-actions",
-            "status": "todo",
-            "total_time_worked": 0.0
+            "priority": 6.0,
+            "status": "active",
+            "total_time_worked": 0.006944463391203704
         }
     },
     "version": 0
 }
```

### Comparing `fancy_dataclass-0.2.0/mkdocs.yml` & `fancy_dataclass-0.3.0/mkdocs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 site_name: Fancy Dataclass
 site_author: Jeremy Silver
 repo_url: https://github.com/jeremander/fancy-dataclass
+edit_uri: tree/main/docs
 
 theme:
   name: material
   features:
     - navigation.footer
     - navigation.path
 
@@ -13,15 +14,14 @@
 
 plugins:
   - mkdocstrings:
       handlers:
         python:
           import:
           - https://installer.readthedocs.io/en/stable/objects.inv
-          # - https://docs.sqlalchemy.org/en/20/core/metadata.html
           options:
             filters: ["!^_[^_]", "_replace"]
   - search
   - gen-files:
       scripts:
         # see https://mkdocstrings.github.io/recipes/
         - docs/gen_ref_pages.py
@@ -36,15 +36,17 @@
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
 
 nav:
   - README.md
   - JSON conversion: json.md
+  - TOML conversion: toml.md
+  - Config management: config.md
   - SQL persistence: sql.md
   - CLI parsing: cli.md
   - Subprocess calls: subprocess.md
   # defer to gen-files + literate-nav
-  - Code Reference: reference/
+  - Code reference: reference/
 
 watch:
   - fancy_dataclass
```

### Comparing `fancy_dataclass-0.2.0/ruff.toml` & `fancy_dataclass-0.3.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/bin/activate` & `fancy_dataclass-0.3.0/.venv/bin/activate`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/bin/activate.bat` & `fancy_dataclass-0.3.0/.venv/bin/activate.bat`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/bin/activate.csh` & `fancy_dataclass-0.3.0/.venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/bin/activate.fish` & `fancy_dataclass-0.3.0/.venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/bin/activate.nu` & `fancy_dataclass-0.3.0/.venv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/bin/activate.ps1` & `fancy_dataclass-0.3.0/.venv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/bin/activate_this.py` & `fancy_dataclass-0.3.0/.venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/bin/deactivate.bat` & `fancy_dataclass-0.3.0/.venv/bin/deactivate.bat`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/bin/pydoc.bat` & `fancy_dataclass-0.3.0/.venv/bin/pydoc.bat`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/_virtualenv.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/METADATA` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/RECORD` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/config.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/config.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/RECORD` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/events.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/exc.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/exc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/inspection.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/inspection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/log.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/log.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/schema.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/schema.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/types.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/aioodbc.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/aioodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/asyncio.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/asyncio.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/pyodbc.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/pyodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.cpython-311-darwin.so` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.pyx` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.cpython-311-darwin.so` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pyx` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.cpython-311-darwin.so` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.pyx` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.cpython-311-darwin.so` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.pyx` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.cpython-311-darwin.so` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.pyx` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/_typing.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/_typing.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/aioodbc.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/aioodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/information_schema.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/information_schema.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/json.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/provision.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pymssql.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pymssql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pyodbc.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pyodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/aiomysql.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/aiomysql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/asyncmy.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/asyncmy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/cymysql.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/cymysql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/dml.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/dml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/enumerated.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/enumerated.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/expression.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/expression.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/json.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadb.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadb.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadbconnector.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadbconnector.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqlconnector.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqlconnector.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqldb.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqldb.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/provision.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pymysql.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pymysql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pyodbc.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pyodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reflection.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reflection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reserved_words.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reserved_words.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/types.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/cx_oracle.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/cx_oracle.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/dictionary.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/dictionary.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/oracledb.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/oracledb.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/provision.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/types.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/_psycopg_common.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/_psycopg_common.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/array.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/array.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/asyncpg.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/asyncpg.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/dml.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/dml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ext.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ext.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/hstore.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/hstore.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/json.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/named_types.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/named_types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/operators.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/operators.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg8000.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg8000.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg_catalog.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg_catalog.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/provision.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2cffi.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2cffi.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ranges.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ranges.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/types.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/aiosqlite.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/dml.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/dml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/json.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/provision.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlcipher.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlcipher.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlite.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlite.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_processors.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_processors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_row.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_row.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_util.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/characteristics.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/characteristics.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/create.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/create.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/cursor.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/cursor.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/default.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/default.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/events.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/interfaces.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/interfaces.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/mock.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/mock.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/processors.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/processors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/reflection.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/reflection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/result.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/result.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/row.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/row.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/url.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/url.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/util.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/api.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/api.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/attr.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/attr.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/legacy.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/legacy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/registry.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/registry.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/associationproxy.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/associationproxy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/automap.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/automap.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/baked.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/baked.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/compiler.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/compiler.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/horizontal_shard.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/horizontal_shard.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/hybrid.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/hybrid.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/indexable.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/indexable.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/instrumentation.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/instrumentation.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mutable.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mutable.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/orderinglist.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/orderinglist.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/serializer.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/serializer.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/engine.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/engine.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/exc.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/exc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/result.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/result.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/scoping.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/scoping.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/session.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/session.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/extensions.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/extensions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/apply.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/apply.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/decl_class.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/decl_class.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/infer.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/infer.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/names.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/names.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/plugin.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/plugin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/util.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/future/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/future/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_orm_constructors.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_orm_constructors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_typing.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_typing.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/attributes.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/attributes.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/bulk_persistence.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/bulk_persistence.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/clsregistry.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/clsregistry.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/collections.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/collections.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/context.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/context.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_api.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_api.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dependency.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dependency.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/descriptor_props.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/descriptor_props.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dynamic.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dynamic.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/evaluator.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/evaluator.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/events.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/exc.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/exc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/identity.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/identity.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/instrumentation.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/instrumentation.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/interfaces.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/interfaces.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/loading.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/loading.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapped_collection.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapped_collection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapper.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapper.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/path_registry.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/path_registry.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/persistence.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/persistence.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/properties.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/properties.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/query.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/query.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/relationships.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/relationships.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/scoping.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/scoping.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/session.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/session.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategies.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategies.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategy_options.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategy_options.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/sync.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/sync.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/unitofwork.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/unitofwork.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/util.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/writeonly.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/writeonly.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/events.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/impl.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/impl.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_dml_constructors.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_dml_constructors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_elements_constructors.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_elements_constructors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_orm_types.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_orm_types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_py_util.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_py_util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_selectable_constructors.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_selectable_constructors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_typing.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_typing.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/annotation.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/annotation.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/cache_key.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/cache_key.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/coercions.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/coercions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/compiler.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/compiler.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/crud.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/crud.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/ddl.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/ddl.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/default_comparator.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/default_comparator.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/dml.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/dml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/elements.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/elements.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/events.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/expression.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/expression.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/functions.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/functions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/lambdas.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/lambdas.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/naming.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/naming.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/operators.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/operators.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/roles.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/roles.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/schema.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/schema.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/selectable.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/sqltypes.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/sqltypes.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/traversals.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/traversals.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/type_api.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/type_api.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/util.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/visitors.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/visitors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertions.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertsql.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertsql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/asyncio.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/asyncio.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/config.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/config.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/engines.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/engines.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/entities.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/entities.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/exclusions.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/exclusions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/pickleable.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/pickleable.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/profiling.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/profiling.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/provision.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/requirements.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/requirements.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/schema.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/schema.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/util.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/warnings.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/warnings.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/mypy.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/mypy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/orm.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/orm.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/sql.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/bootstrap.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/bootstrap.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/plugin_base.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/pytestplugin.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_cte.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_cte.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_ddl.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_ddl.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_deprecations.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_dialect.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_dialect.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_insert.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_insert.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_reflection.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_reflection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_results.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_results.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_rowcount.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_rowcount.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_select.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_select.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_sequence.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_sequence.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_types.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_unicode_ddl.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_unicode_ddl.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_update_delete.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_update_delete.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/__init__.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_collections.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_collections.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_concurrency_py3k.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_concurrency_py3k.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_has_cy.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_has_cy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_py_collections.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_py_collections.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/compat.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/compat.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/concurrency.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/concurrency.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/deprecations.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/deprecations.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/preloaded.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/preloaded.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/queue.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/queue.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/tool_support.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/tool_support.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/topological.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/topological.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/typing.py` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/typing.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD` & `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/docs/CHANGELOG.md` & `fancy_dataclass-0.3.0/docs/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,24 @@
     - Removed
     - Fixed
     - Security
 -->
 
 ## [Unreleased]
 
+### Added
+
+- `TOMLDataclass` for saving/loading TOML via [`tomlkit`](https://tomlkit.readthedocs.io/en/latest/)
+    - Support for loading TOML configurations in `ConfigDataclass`
+- `FileSerializable` and `DictFileSerializableDataclass` mixins to factor out shared functionality between JSON/TOML serialization
+
 ## [0.2.0]
 
+2024-04-13
+
 ### Added
 
 - `ConfigDataclass` mixin for global configurations
 - Customization of `DataclassMixin`:
     - `DataclassMixinSettings` for mixin class configuration
     - `FieldSettings` for field-specific settings
     - `__post_dataclass_wrap__` hook to customize behavior after `dataclass` decorator is applied (e.g. validating fields at definition time)
@@ -40,14 +48,16 @@
 
 ### Fixed
 
 - More robust type handling
 
 ## [0.1.0]
 
+2022-06-06
+
 ### Added
 
 - `DataclassMixin` class providing extra dataclass features
     - `ArgparseDataclass`: command-line argument parsing
     - `CLIDataclass`: command-line argument parsing and `main` function
     - `DictDataclass`: conversion to/from Python dict
     - `JSONDataclass`: conversion to/from JSON
```

#### html2text {}

```diff
@@ -1,24 +1,28 @@
 # Changelog All notable changes to this project will be documented in this
 file. The format is based on [Keep a Changelog](https://keepachangelog.com/en/
 1.1.0/), and this project attempts to adhere to [Semantic Versioning](https://
-semver.org/spec/v2.0.0.html). ## [Unreleased] ## [0.2.0] ### Added -
-`ConfigDataclass` mixin for global configurations - Customization of
+semver.org/spec/v2.0.0.html). ## [Unreleased] ### Added - `TOMLDataclass` for
+saving/loading TOML via [`tomlkit`](https://tomlkit.readthedocs.io/en/latest/
+) - Support for loading TOML configurations in `ConfigDataclass` -
+`FileSerializable` and `DictFileSerializableDataclass` mixins to factor out
+shared functionality between JSON/TOML serialization ## [0.2.0] 2024-04-13 ###
+Added - `ConfigDataclass` mixin for global configurations - Customization of
 `DataclassMixin`: - `DataclassMixinSettings` for mixin class configuration -
 `FieldSettings` for field-specific settings - `__post_dataclass_wrap__` hook to
 customize behavior after `dataclass` decorator is applied (e.g. validating
 fields at definition time) - Documentation - [Reference pages](README.md) via
 [`mkdocs-material`](https://squidfunk.github.io/mkdocs-material) and
 [`mkdocstrings`](https://mkdocstrings.github.io) - Basic usage examples for
 main mixin classes - [CHANGELOG](#changelog) - Linting via [`ruff`](https://
 docs.astral.sh/ruff/) - Unit tests - Over 90% code coverage, via [`pytest-cov`]
 (https://pytest-cov.readthedocs.io/en/latest/readme.html) ### Changed - Build
 via [`hatch`](https://github.com/pypa/hatch) - Better flattened/nested
-dataclass conversions ### Fixed - More robust type handling ## [0.1.0] ###
-Added - `DataclassMixin` class providing extra dataclass features -
+dataclass conversions ### Fixed - More robust type handling ## [0.1.0] 2022-06-
+06 ### Added - `DataclassMixin` class providing extra dataclass features -
 `ArgparseDataclass`: command-line argument parsing - `CLIDataclass`: command-
 line argument parsing and `main` function - `DictDataclass`: conversion to/from
 Python dict - `JSONDataclass`: conversion to/from JSON - `SQLDataclass`: SQL
 persistence via `sqlalchemy` - `SubprocessDataclass`: call out to another
 program via `subprocess` [unreleased]: https://github.com/jeremander/fancy-
 dataclass/compare/v0.2.0...HEAD [0.2.0]: https://github.com/jeremander/fancy-
 dataclass/releases/tag/v0.2.0 [0.1.0]: https://github.com/jeremander/fancy-
```

### Comparing `fancy_dataclass-0.2.0/docs/LICENSE.txt` & `fancy_dataclass-0.3.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/docs/cli.md` & `fancy_dataclass-0.3.0/docs/cli.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/docs/gen_ref_pages.py` & `fancy_dataclass-0.3.0/docs/gen_ref_pages.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 nav = mkdocs_gen_files.Nav()
 
 PKG_NAME = 'fancy_dataclass'
 PKG_DIR = Path(PKG_NAME)
 REF_DIR = Path('reference')
 
-# TODO: add config, toml, etc.
-REF_MODULES = ['cli', 'dict', 'json', 'mixin', 'sql', 'subprocess', 'utils']
+REF_MODULES = ['cli', 'config', 'dict', 'json', 'mixin', 'serialize', 'sql', 'subprocess', 'toml', 'utils']
 
 for mod_name in REF_MODULES:
     path = PKG_DIR / f'{mod_name}.py'
     module_path = path.relative_to(PKG_DIR).with_suffix('')
     doc_path = path.relative_to(PKG_DIR).with_suffix('.md')
     full_doc_path = REF_DIR / doc_path
     parts = tuple(module_path.parts)
```

### Comparing `fancy_dataclass-0.2.0/docs/json.md` & `fancy_dataclass-0.3.0/docs/json.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!-- markdownlint-disable MD052 -->
 
 The [`JSONDataclass`][fancy_dataclass.json.JSONDataclass] mixin provides automatic conversion to and from [JSON](https://en.wikipedia.org/wiki/JSON).
 
-- [`to_dict`][fancy_dataclass.dict.DictDataclass.to_dict] / [`from_dict`][fancy_dataclass.dict.DictDataclass.from_dict] convert to and from Python dicts (ensuring values are JSON serializable).
+- [`to_dict`][fancy_dataclass.dict.DictDataclass.to_dict] / [`from_dict`][fancy_dataclass.dict.DictDataclass.from_dict] convert to and from Python dicts.
 - [`to_json`][fancy_dataclass.json.JSONSerializable.to_json] / [`from_json`][fancy_dataclass.json.JSONSerializable.from_json] convert to and from JSON file-like objects.
 - [`to_json_string`][fancy_dataclass.json.JSONSerializable.to_json_string] / [`from_json_string`][fancy_dataclass.json.JSONSerializable.from_json_string] convert to and from JSON strings.
 
 ## Usage Example
 
 Define a `JSONDataclass`.
 
@@ -92,14 +92,15 @@
 <!--
 - Inherits from `DictDataclass`
 - Suppressing defaults
 - Other settings (`store_type`, `qualified_type`)
 - `JSONBaseDataclass` providing `qualified_type=True`
 - kwargs get passed to `json.dump`
 - `strict` argument in `from_dict`
+- Override `_json_encoder`, `_json_key_decoder`
 -->
 
 ### Notes
 
 - `JSONDataclass` is configured to use the default JSON settings provided by Python's standard [`json`](https://docs.python.org/3/library/json.html) library. This allows out-of-range float values like `nan` and `inf` to be represented as `NaN` and `Infinity`, which are not strictly part of the JSON standard. To disallow these values, you can pass `allow_nan=False` when calling `to_json` or `to_json_string`, which will raise a `ValueError` if such values occur.
 
 <style>
```

### Comparing `fancy_dataclass-0.2.0/docs/sql.md` & `fancy_dataclass-0.3.0/docs/sql.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/docs/subprocess.md` & `fancy_dataclass-0.3.0/docs/subprocess.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 
 ## Usage Example
 
 Define a `SubprocessDataclass` to delegate calls to command-line programs within Python.
 
 ```python
 from dataclasses import dataclass, field
-from typing import ClassVar
 
 from fancy_dataclass.subprocess import SubprocessDataclass
 
 
 @dataclass
-class ListDir(SubprocessDataclass, exec='ls'):
+class ListDir(SubprocessDataclass, exec='ls'):  # specify program to run
     """Lists directory contents."""
     # list in long form
     long: bool = field(default=False, metadata={'args': '-l'})
     # list in reverse order
     reverse: bool = field(default=False, metadata={'args': '-r'})
     # sort by time
     time: bool = field(default=False, metadata={'args': '-t'})
```

### Comparing `fancy_dataclass-0.2.0/fancy_dataclass/cli.py` & `fancy_dataclass-0.3.0/fancy_dataclass/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import MISSING, dataclass, fields
 from enum import IntEnum
 from typing import Any, Callable, ClassVar, Dict, List, Literal, Optional, Sequence, Type, TypeVar, Union, get_args, get_origin
 
 from typing_extensions import Self
 
 from fancy_dataclass.mixin import DataclassMixin, FieldSettings
-from fancy_dataclass.utils import check_dataclass, issubclass_safe
+from fancy_dataclass.utils import check_dataclass, issubclass_safe, type_is_optional
 
 
 T = TypeVar('T')
 
 
 @dataclass
 class ArgparseDataclassFieldSettings(FieldSettings):
@@ -133,15 +133,15 @@
             field.type.configure_parser(parser)
             return
         # determine the type of the parser argument for the field
         tp = field.metadata.get('type', field.type)
         action = field.metadata.get('action', 'store')
         origin_type = get_origin(tp)
         if origin_type is not None:  # compound type
-            if (origin_type == Union) and (getattr(tp, '_name', None) == 'Optional'):
+            if type_is_optional(tp):
                 kwargs['default'] = None
             if origin_type == ClassVar:  # by default, exclude ClassVars from the parser
                 return
             tp_args = get_args(tp)
             if tp_args:  # extract the first wrapped type (should handle List/Optional/Union)
                 tp = tp_args[0]
                 if origin_type == Literal:  # literal options will become choices
```

### Comparing `fancy_dataclass-0.2.0/fancy_dataclass/config.py` & `fancy_dataclass-0.3.0/fancy_dataclass/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,107 @@
 from contextlib import contextmanager
+from copy import deepcopy
+from dataclasses import is_dataclass, make_dataclass
 from pathlib import Path
-from typing import ClassVar, Iterator, Optional
+from typing import ClassVar, Iterator, Optional, Type
 
 from typing_extensions import Self
 
 from fancy_dataclass.dict import DictDataclass
-from fancy_dataclass.utils import AnyPath
+from fancy_dataclass.mixin import DataclassMixin
+from fancy_dataclass.serialize import FileSerializable
+from fancy_dataclass.utils import AnyPath, coerce_to_dataclass, dataclass_type_map, get_dataclass_fields
 
 
 class Config:
     """Base class for a collection of configurations.
 
-    This uses the Singleton pattern by storing a class attribute with the current configurations, which can be retrieved or updated by the user."""
+    This uses a quasi-Singleton pattern by storing a class attribute with the current global configurations, which can be retrieved or updated by the user."""
 
     _config: ClassVar[Optional[Self]] = None
 
     @classmethod
     def get_config(cls) -> Optional[Self]:
-        """Gets the current global configuration."""
-        return cls._config  # type: ignore[return-value]
+        """Gets a copy of the current global configuration.
+
+        Returns:
+            Global configuration object (`None` if not set)"""
+        return deepcopy(cls._config)  # type: ignore[return-value]
 
     @classmethod
     def _set_config(cls, config: Optional[Self]) -> None:
         """Sets the global configuration to a given value."""
         # NOTE: this is private to avoid confusion with update_config
         cls._config = config
 
     @classmethod
     def clear_config(cls) -> None:
         """Clears the global configuration by setting it to `None`."""
         cls._set_config(None)
 
     def update_config(self) -> None:
-        """Updates the global configuration, setting it equal to this value."""
+        """Updates the global configuration, setting it equal to this object."""
         type(self)._set_config(self)
 
     @contextmanager
     def configure(self) -> Iterator[None]:
-        """Context manager which temporarily updates the global configuration with this value."""
+        """Context manager which temporarily updates the global configuration with this object."""
         try:
             orig_config = type(self).get_config()
             self.update_config()
             yield
         finally:
             type(self)._set_config(orig_config)
 
 
-class ConfigDataclass(Config, DictDataclass):
+class ConfigDataclass(Config, DictDataclass, suppress_defaults=False):
     """A dataclass representing a collection of configurations.
 
     The configurations can be loaded from a file, the type of which will be inferred from its extension.
     Supported file types are:
-        - JSON
+
+    - JSON
+    - TOML
     """
 
+    @staticmethod
+    def _wrap_config_dataclass(mixin_cls: Type[DataclassMixin], cls: Type['ConfigDataclass']) -> Type[DataclassMixin]:
+        """Recursively wraps a DataclassMixin class around a ConfigDataclass so that nested dataclass fields inherit from the same mixin."""
+        def _wrap(tp: type) -> type:
+            if is_dataclass(tp):
+                wrapped_cls = mixin_cls.wrap_dataclass(tp)
+                field_data = [(fld.name, fld.type, fld) for fld in get_dataclass_fields(tp, include_classvars=True)]
+                return make_dataclass(tp.__name__, field_data, bases=wrapped_cls.__bases__)
+            return tp
+        return _wrap(dataclass_type_map(cls, _wrap))  # type: ignore[arg-type]
+
+    @classmethod
+    def _get_dataclass_type_for_extension(cls, ext: str) -> Type[FileSerializable]:
+        ext_lower = ext.lower()
+        if ext_lower == '.json':
+            from fancy_dataclass.json import JSONDataclass
+            return JSONDataclass
+        elif ext_lower == '.toml':
+            from fancy_dataclass.toml import TOMLDataclass
+            return TOMLDataclass
+        else:
+            raise ValueError(f'unknown config file extension {ext!r}')
+
     @classmethod
     def load_config(cls, path: AnyPath) -> Self:
         """Loads configurations from a file and sets them to be the global configurations for this class.
 
+        Args:
+            path: File from which to load configurations
+
         Returns:
-            The newly loaded global configuration"""
+            The newly loaded global configurations"""
         p = Path(path)
         ext = p.suffix
         if not ext:
             raise ValueError(f'filename {p} has no extension')
-        if ext == '.json':
-            from fancy_dataclass.json import JSONDataclass
-            new_cls = JSONDataclass.wrap_dataclass(cls)
-            with open(path) as f:
-                cfg: Self = cls.from_dict(new_cls.from_json(f).to_dict())
-        else:
-            raise ValueError(f'unknown config file extension {ext!r}')
+        tp = cls._get_dataclass_type_for_extension(ext)
+        new_cls: Type[FileSerializable] = ConfigDataclass._wrap_config_dataclass(tp, cls)  # type: ignore
+        with open(path) as f:
+            cfg: Self = coerce_to_dataclass(cls, new_cls._from_file(f))
         cfg.update_config()
         return cfg
```

### Comparing `fancy_dataclass-0.2.0/fancy_dataclass/dict.py` & `fancy_dataclass-0.3.0/fancy_dataclass/dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,57 @@
+from abc import ABC, abstractmethod
 from copy import copy
 import dataclasses
-from dataclasses import dataclass
+from dataclasses import Field, dataclass
 from functools import partial
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Iterable, Literal, Optional, Type, TypeVar, Union, _TypedDictMeta, get_args, get_origin  # type: ignore[attr-defined]
 
 from typing_extensions import Self, _AnnotatedAlias
 
 from fancy_dataclass.mixin import DataclassMixin, DataclassMixinSettings, FieldSettings
-from fancy_dataclass.utils import TypeConversionError, _flatten_dataclass, check_dataclass, fully_qualified_class_name, issubclass_safe, obj_class_name, safe_dict_insert
+from fancy_dataclass.utils import TypeConversionError, _flatten_dataclass, check_dataclass, fully_qualified_class_name, issubclass_safe, obj_class_name, safe_dict_insert, type_is_optional
 
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
 
 T = TypeVar('T', bound=DataclassMixin)
 D = TypeVar('D', bound='DataclassInstance')
 
 AnyDict = Dict[str, Any]
 
 
+class DictConvertible(ABC):
+    """Mixin class enabling conversion of an object to/from a Python dict.
+
+    Subclasses should override `to_dict` and `from_dict` to implement the conversion."""
+
+    @abstractmethod
+    def to_dict(self, **kwargs: Any) -> AnyDict:
+        """Converts an object to a dict.
+
+        Args:
+            kwargs: Keyword arguments
+
+        Returns:
+            A Python dict"""
+
+    @classmethod
+    @abstractmethod
+    def from_dict(cls, d: AnyDict, **kwargs: Any) -> Self:
+        """Constructs an object from a dictionary of (attribute, value) pairs.
+
+        Args:
+            d: Dict to convert into an object
+            kwargs: Keyword arguments
+
+        Returns:
+            Converted object of this class"""
+
+
 @dataclass
 class DictDataclassSettings(DataclassMixinSettings):
     """Class-level settings for the [`DictDataclass`][fancy_dataclass.dict.DictDataclass] mixin.
 
     Subclasses of `DictDataclass` may set the following boolean flags as keyword arguments during inheritance:
 
     - `suppress_defaults`: suppress default values in its dict
@@ -217,15 +246,15 @@
             elif origin_type == tuple:
                 subtypes = args
                 if subtypes[-1] == Ellipsis:  # treat it like a list
                     subtype = subtypes[0]
                     return tuple(convert_val(subtype, elt) for elt in val)
                 return tuple(convert_val(subtype, elt) for (subtype, elt) in zip(args, val))
             elif origin_type == Union:
-                if getattr(tp, '_name', None) == 'Optional':
+                if type_is_optional(tp):
                     assert len(args) == 2
                     assert args[1] is type(None)
                     args = args[::-1]  # check None first
                 for subtype in args:
                     try:
                         # NB: will resolve to the first valid type in the Union
                         return convert_val(subtype, val)
@@ -239,43 +268,50 @@
                 return cls._from_dict_value_convertible(origin_type, val, strict)
             elif issubclass_safe(origin_type, Iterable):  # arbitrary iterable
                 subtype = args[0]
                 return type(val)(convert_val(subtype, elt) for elt in val)
         raise err()
 
     @classmethod
+    def _get_missing_value(cls, fld: Field) -> Any:  # type: ignore[type-arg]
+        raise ValueError(f'{fld.name!r} field is required')
+
+    @classmethod
     def _dataclass_args_from_dict(cls, d: AnyDict, strict: bool = False) -> AnyDict:
         """Given a dict of arguments, performs type conversion and/or validity checking, then returns a new dict that can be passed to the class's constructor."""
         check_dataclass(cls)
         kwargs = {}
         bases = cls.mro()
         fields = dataclasses.fields(cls)  # type: ignore[arg-type]
         if strict:  # check there are no extraneous fields
             field_names = {field.name for field in fields}
             for key in d:
                 if (key not in field_names):
                     raise ValueError(f'{key!r} is not a valid field for {cls.__name__}')
-        for field in fields:
-            if not field.init:  # suppress fields where init=False
+        for fld in fields:
+            if not fld.init:  # suppress fields where init=False
                 continue
-            if field.name in d:
+            if fld.name in d:
                 # field may be defined in the dataclass itself or one of its ancestor dataclasses
                 for base in bases:
                     try:
-                        field_type = base.__annotations__[field.name]
-                        kwargs[field.name] = cls._from_dict_value(field_type, d[field.name], strict=strict)
+                        field_type = base.__annotations__[fld.name]
+                        kwargs[fld.name] = cls._from_dict_value(field_type, d[fld.name], strict=strict)
                         break
                     except (AttributeError, KeyError):
                         pass
                 else:
-                    raise ValueError(f'could not locate field {field.name!r}')
-            elif field.default == dataclasses.MISSING:
-                if field.default_factory == dataclasses.MISSING:
-                    raise ValueError(f'{field.name!r} field is required')
-                kwargs[field.name] = field.default_factory()
+                    raise ValueError(f'could not locate field {fld.name!r}')
+            elif fld.default == dataclasses.MISSING:
+                if fld.default_factory == dataclasses.MISSING:
+                    val = cls._get_missing_value(fld)
+                else:
+                    val = fld.default_factory()
+                    # raise ValueError(f'{fld.name!r} field is required')
+                kwargs[fld.name] = val
         return kwargs
 
     @classmethod
     def from_dict(cls, d: AnyDict, **kwargs: Any) -> Self:
         """Constructs an object from a dictionary of fields.
 
         This may also perform some basic type/validity checking.
```

### Comparing `fancy_dataclass-0.2.0/fancy_dataclass/mixin.py` & `fancy_dataclass-0.3.0/fancy_dataclass/mixin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/fancy_dataclass/sql.py` & `fancy_dataclass-0.3.0/fancy_dataclass/sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/fancy_dataclass/subprocess.py` & `fancy_dataclass-0.3.0/fancy_dataclass/subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         if not executable:
             raise ValueError(f'no executable identified for use with {obj_class_name(self)} instance')
         args = [executable]
         for fld in fields(self):  # type: ignore[arg-type]
             args += [arg for arg in self.get_arg(fld.name, suppress_defaults = suppress_defaults) if arg]
         return args
 
-    def run_subprocess(self, **kwargs: Any) -> subprocess.CompletedProcess[Union[str, bytes]]:
+    def run_subprocess(self, **kwargs: Any) -> subprocess.CompletedProcess:  # type: ignore[type-arg]
         """Executes the full subprocess command corresponding to the dataclass parameters.
 
         Args:
             kwargs: Keyword arguments passed to `subprocess.run`
 
         Returns:
             `CompletedProcess` object produced by `subprocess.run`
```

### Comparing `fancy_dataclass-0.2.0/fancy_dataclass/utils.py` & `fancy_dataclass-0.3.0/fancy_dataclass/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from copy import copy
 import dataclasses
 from dataclasses import Field, dataclass, is_dataclass, make_dataclass
 from functools import lru_cache
 import importlib
 from pathlib import Path
 import re
-from typing import TYPE_CHECKING, Any, Callable, Dict, ForwardRef, Generic, Iterator, List, Optional, Sequence, Set, Tuple, Type, TypeVar, Union, get_args, get_origin, get_type_hints
+from typing import TYPE_CHECKING, Any, BinaryIO, Callable, Dict, ForwardRef, Generic, Iterable, Iterator, List, Optional, Sequence, Set, TextIO, Tuple, Type, TypeVar, Union, get_args, get_origin, get_type_hints
 
 from typing_extensions import TypeGuard
 
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
 
 
 T = TypeVar('T')
 U = TypeVar('U')
 
+AnyIO = Union[BinaryIO, TextIO]
 Constructor = Callable[[Any], Any]
-AnyPath = str | Path
+AnyPath = Union[str, Path]
 RecordPath = Tuple[str, ...]
 
 # maximum depth when traversing the fields of a dataclass
 MAX_DATACLASS_DEPTH = 100
 
 
 class TypeConversionError(ValueError):
@@ -40,14 +41,26 @@
             val: value to convert"""
         self.tp = tp
         self.val = val
         tp_name = re.sub("'>$", '', re.sub(r"^<\w+ '", '', str(tp)))
         super().__init__(f'could not convert {val!r} to type {tp_name!r}')
 
 
+def type_is_optional(tp: type) -> bool:
+    """Determines if a type is an Optional type.
+
+    Args:
+        tp: Type to check
+
+    Returns:
+        True if the type is Optional"""
+    origin_type = get_origin(tp)
+    args = get_args(tp)
+    return (origin_type == Union) and (len(args) == 2) and (type(None) in args)
+
 def safe_dict_insert(d: Dict[Any, Any], key: str, val: Any) -> None:
     """Inserts a (key, value) pair into a dict, if the key is not already present.
 
     Args:
         d: Dict to modify
         key: Key to insert
         val: Value to insert
@@ -228,16 +241,67 @@
 
     Args:
         cls: Target dataclass type
         obj: Object to coerce
 
     Returns:
         A new object of the desired type, coerced from the input object"""
-    d = {fld.name: getattr(obj, fld.name) for fld in dataclasses.fields(cls) if hasattr(obj, fld.name)}  # type: ignore[arg-type]
-    return cls(**d)
+    kwargs = {}
+    for fld in dataclasses.fields(cls):  # type: ignore[arg-type]
+        if hasattr(obj, fld.name):
+            val = getattr(obj, fld.name)
+            if is_dataclass(fld.type):
+                val = coerce_to_dataclass(fld.type, val)
+            else:
+                origin_type = get_origin(fld.type)
+                if origin_type and issubclass_safe(origin_type, Iterable):
+                    if issubclass(origin_type, dict):
+                        (_, val_type) = get_args(origin_type)
+                        if is_dataclass(val_type):
+                            val = type(val)({key: coerce_to_dataclass(val_type, elt) for (key, elt) in val.items()})
+                    elif issubclass(origin_type, tuple):
+                        val = type(val)(coerce_to_dataclass(tp, elt) if is_dataclass(tp) else elt for (tp, elt) in zip(get_args(fld.type), val))
+                    else:
+                        (elt_type,) = get_args(fld.type)
+                        if is_dataclass(elt_type):
+                            val = type(val)(coerce_to_dataclass(elt_type, elt) for elt in val)
+            kwargs[fld.name] = val
+    return cls(**kwargs)
+
+def dataclass_type_map(cls: Type['DataclassInstance'], func: Callable[[type], type]) -> Type['DataclassInstance']:
+    """Applies a type function to all dataclass field types, recursively through container types.
+
+    Args:
+        cls: Target dataclass type to manipulate
+        func: Function to map onto basic (non-container) field types
+
+    Returns:
+        A new dataclass type whose field types have been mapped by the function"""
+    def _map_func(tp: type) -> type:
+        return func(dataclass_type_map(tp, func)) if is_dataclass(tp) else func(tp)
+    # for Py3.8 compatibility, can only subscript typing classes
+    container_type_map: Dict[type, type] = {dict: Dict, tuple: Tuple, list: List}  # type: ignore[dict-item]
+    field_data = []
+    for fld in get_dataclass_fields(cls, include_classvars=True):
+        new_fld = copy(fld)
+        origin_type = get_origin(fld.type)
+        if origin_type and issubclass_safe(origin_type, Iterable):
+            otype = container_type_map.get(origin_type, origin_type)
+            if issubclass(origin_type, dict):
+                (key_type, val_type) = get_args(origin_type)
+                tp = otype[key_type, _map_func(val_type)]
+            elif issubclass(origin_type, tuple):
+                tp = otype[tuple([_map_func(elt_type) for elt_type in get_args(fld.type)])]
+            else:
+                (elt_type,) = get_args(fld.type)
+                tp = otype[_map_func(elt_type)]
+        else:
+            tp = _map_func(fld.type)
+        field_data.append((fld.name, tp, new_fld))
+    return make_dataclass(cls.__name__, field_data, bases=cls.__bases__)
 
 
 ##############
 # FLATTENING #
 ##############
 
 def traverse_dataclass(cls: type) -> Iterator[Tuple[RecordPath, Field]]:  # type: ignore[type-arg]
@@ -252,36 +316,35 @@
 
     Returns:
         Generator of (name, field) pairs, where each field is a `dataclasses.Field` object
 
     Raises:
         TypeError: if the type cannot be traversed"""
     def _make_optional(fld: Field) -> Field:  # type: ignore[type-arg]
-        new_fld = Field
-        new_fld = copy(fld)  # type: ignore[assignment]
+        new_fld = copy(fld)
         new_fld.type = Optional[fld.type]  # type: ignore
-        new_fld.default = None  # type: ignore
-        return new_fld  # type: ignore[return-value]
+        new_fld.default = None
+        return new_fld
     def _traverse(prefix: RecordPath, tp: type) -> Iterator[Tuple[RecordPath, Field]]:  # type: ignore[type-arg]
         if len(prefix) > MAX_DATACLASS_DEPTH:
-            raise TypeError(f'Type recursion exceeds depth {MAX_DATACLASS_DEPTH}')
+            raise TypeError(f'type recursion exceeds depth {MAX_DATACLASS_DEPTH}')
         for fld in get_dataclass_fields(tp, include_classvars=True):
             fld_type = get_type_hints(tp)[fld.name] if isinstance(fld.type, str) else fld.type
             if fld_type is tp:  # prevent infinite recursion
-                raise TypeError('Type cannot contain a member field of its own type')
+                raise TypeError('type cannot contain a member field of its own type')
             path = prefix + (fld.name,)
             origin = get_origin(fld_type)
             is_union = origin is Union
             if is_union:
                 args = get_args(fld_type)
                 # if optional, use the wrapped type, otherwise error
                 base_types = []
                 for arg in args:
                     if isinstance(arg, ForwardRef):
-                        raise TypeError('Type cannot contain a ForwardRef')
+                        raise TypeError('type cannot contain a ForwardRef')
                     base_types.append(arg)
             else:
                 base_types = [fld_type]
             if any(not is_dataclass(base_type) for base_type in base_types):
                 if is_union:
                     fld = _make_optional(fld)
                 yield (path, fld)
```

### Comparing `fancy_dataclass-0.2.0/tests/test_cli.py` & `fancy_dataclass-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/tests/test_dict.py` & `fancy_dataclass-0.3.0/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/tests/test_inheritance.py` & `fancy_dataclass-0.3.0/tests/test_inheritance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dataclasses import dataclass
+from datetime import datetime
 
 import pytest
 
-from fancy_dataclass import ArgparseDataclass, ConfigDataclass, DictDataclass, JSONBaseDataclass, JSONDataclass, SQLDataclass
+from fancy_dataclass import ArgparseDataclass, ConfigDataclass, DictDataclass, JSONBaseDataclass, JSONDataclass, SQLDataclass, TOMLDataclass
 from fancy_dataclass.dict import DictDataclassSettings
 
 
-DEFAULT_MIXINS = [JSONBaseDataclass, ArgparseDataclass, ConfigDataclass, SQLDataclass]
+DEFAULT_MIXINS = [JSONBaseDataclass, ArgparseDataclass, ConfigDataclass, SQLDataclass, TOMLDataclass]
 
 
 def test_multiple_inheritance():
     """Tests inheritance from multiple DataclassMixins."""
     @dataclass
     class MyDC1(ArgparseDataclass, JSONDataclass):
         x: int
@@ -66,7 +67,25 @@
     MyDC1 = DictDataclass.wrap_dataclass(MyDC)
     # this works because JSONDataclass is not a subclass of MyDC1
     MyDC2 = JSONDataclass.wrap_dataclass(MyDC1)
     assert issubclass(MyDC2, DictDataclass)
     assert issubclass(MyDC2, JSONDataclass)
     assert issubclass(MyDC2, MyDC1)
     assert MyDC2 is not MyDC1
+
+def test_json_toml():
+    """Tests inheritance from both JSONDataclass and TOMLDataclass."""
+    dt = datetime.strptime('2024-01-01', '%Y-%m-%d')
+    json_str = '{"dt": "2024-01-01T00:00:00"}'
+    toml_str = 'dt = 2024-01-01T00:00:00\n'
+    @dataclass
+    class JSONTOMLDC(JSONDataclass, TOMLDataclass):
+        dt: datetime
+    @dataclass
+    class TOMLJSONDC(TOMLDataclass, JSONDataclass):
+        dt: datetime
+    obj1 = JSONTOMLDC(dt)
+    obj2 = TOMLJSONDC(dt)
+    for obj in [obj1, obj2]:
+        assert isinstance(obj.to_dict()['dt'], datetime)
+        assert obj.to_json_string() == json_str
+        assert obj.to_toml_string() == toml_str
```

### Comparing `fancy_dataclass-0.2.0/tests/test_mixin.py` & `fancy_dataclass-0.3.0/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/tests/test_sql.py` & `fancy_dataclass-0.3.0/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.2.0/tests/test_subprocess.py` & `fancy_dataclass-0.3.0/tests/test_subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 import re
-import sys
 from typing import ClassVar
 
 import pytest
 
 from fancy_dataclass.cli import ArgparseDataclass, ArgparseDataclassFieldSettings
 from fancy_dataclass.dict import DictDataclass
 from fancy_dataclass.subprocess import SubprocessDataclass, SubprocessDataclassFieldSettings
@@ -36,15 +35,15 @@
     dc2 = DC2(required_string='positional_arg', input_file='my_input', output_file='my_output', choice='a', optional='default', flag=True, extra_items=[], x=7, y=3.14, pair=(0,0), ignored_value='ignored', prog = prog)
     assert dc2.args() == [prog, 'positional_arg', '-i', 'my_input', '-o', 'my_output', '--choice', 'a', '--optional', 'default', '--flag', '-x', '7', '-y', '3.14', '--pair', '0', '0']
     assert dc2.args(suppress_defaults=True) == [prog, 'positional_arg', '-i', 'my_input', '-o', 'my_output', '--flag']
     # create a script to run the CLIDataclass
     dc1 = coerce_to_dataclass(DC1, dc2)
     cwd = str(Path(__file__).parent)
     with open(prog, 'w') as f:
-        print(f"""#!{sys.executable}
+        print(f"""#!/usr/bin/env python3
 import sys
 sys.path.insert(0, {cwd!r})
 from test_cli import DC1
 DC1.main()""", file=f)
     Path(prog).chmod(0o770)
     # call the script with subprocess
     res = dc2.run_subprocess(capture_output=True, text=True)
```

### Comparing `fancy_dataclass-0.2.0/tests/test_utils.py` & `fancy_dataclass-0.3.0/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 from dataclasses import dataclass, is_dataclass
 from typing import Any, ClassVar, Dict, List, Optional, Sequence, Union
 
 import pytest
 from pytest import param
 
-from fancy_dataclass.utils import _flatten_dataclass, _is_instance, get_dataclass_fields, merge_dataclasses, traverse_dataclass
+from fancy_dataclass.utils import _flatten_dataclass, _is_instance, get_dataclass_fields, merge_dataclasses, traverse_dataclass, type_is_optional
 
 
+@pytest.mark.parametrize(['tp', 'is_optional'], [
+    (int, False),
+    (Optional[int], True),
+    (Optional[Optional[int]], True),
+    (Union[int, Optional[float]], False),
+    (Union[Optional[float], int], False),
+    (Optional[type(None)], False),  # Optional[NoneType] -> NoneType
+    (List[Optional[int]], False),
+])
+def test_type_is_optional(tp, is_optional):
+    assert type_is_optional(tp) == is_optional
+
 @pytest.mark.parametrize(['obj', 'tp', 'output'], [
     (1, int, True),
     ('a', int, False),
     (None, int, False),
     (None, type(None), True),
     (1, type(None), False),
     (1, Any, True),
@@ -170,18 +182,18 @@
     param(W({'c1': C(1), 'c2': C(2)}), ['w'], id='dict of dataclasses'),
     param(X(1), ['x', 'y'], id='class var'),
 ]
 
 DC_FLATTEN_INVALID_PARAMS = [
     (G, "duplicate key 'g1'"),
     (P, "duplicate key 'g1'"),
-    (R, 'Type cannot contain a member field of its own type'),
-    (S, 'Type cannot contain a ForwardRef'),
-    (T, 'Type recursion exceeds depth'),
-    (U, 'Type recursion exceeds depth'),
+    (R, 'type cannot contain a member field of its own type'),
+    (S, 'type cannot contain a ForwardRef'),
+    (T, 'type recursion exceeds depth'),
+    (U, 'type recursion exceeds depth'),
 ]
 
 class TestFlatten:
 
     def test_traverse(self):
         """Tests depth-first traversal of dataclass fields."""
         def get_names(cls):
@@ -199,23 +211,23 @@
         assert get_names(G) == ['g1', 'g2.g1', 'g2.g2']
         assert get_names(J) == ['j']
         assert next(traverse_dataclass(J))[1].type == Optional[int]
         assert get_names(K) == ['k']
         assert get_names(M) == ['m', 'm.k']
         assert get_names(N) == ['n.j', 'n.k']
         assert get_names(P) == ['p', 'p.g1', 'p.g2.g1', 'p.g2.g2']
-        assert all('typing.Optional' in str(fld.type) for (_, fld) in traverse_dataclass(P))
+        assert all(type_is_optional(fld.type) for (_, fld) in traverse_dataclass(P))
         assert get_names(Q) == ['q', 'q.g1', 'q.g2']
-        with pytest.raises(TypeError, match='Type cannot contain a member field of its own type'):
+        with pytest.raises(TypeError, match='type cannot contain a member field of its own type'):
             _ = get_names(R)
-        with pytest.raises(TypeError, match='Type cannot contain a ForwardRef'):
+        with pytest.raises(TypeError, match='type cannot contain a ForwardRef'):
             _ = get_names(S)
-        with pytest.raises(TypeError, match='Type recursion exceeds depth'):
+        with pytest.raises(TypeError, match='type recursion exceeds depth'):
             _ = get_names(T)
-        with pytest.raises(TypeError, match='Type recursion exceeds depth'):
+        with pytest.raises(TypeError, match='type recursion exceeds depth'):
             _ = get_names(U)
         assert get_names(V) == ['v']
         assert get_names(W) == ['w']
         assert get_names(X) == ['x', 'y']
 
     @pytest.mark.parametrize(['obj', 'flat_fields'], DC_FLATTEN_VALID_PARAMS)
     def test_flatten_valid(self, obj, flat_fields):
```

### Comparing `fancy_dataclass-0.2.0/pyproject.toml` & `fancy_dataclass-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fancy-dataclass"
 dynamic = ["version"]
-description = "Enhance dataclasses with additional features."
+description = "Spiff up your dataclasses with additional features."
 readme = "docs/README.md"
 requires-python = ">=3.8"
 license = "MIT"
-keywords = ["dataclass", "cli", "orm", "serialize", "json"]
+keywords = ["dataclass", "cli", "config", "orm", "serialize", "json", "toml"]
 authors = [
   { name = "Jeremy Silver", email = "jeremys@nessiness.com" }
 ]
 classifiers = [
   "Programming Language :: Python"
 ]
 dependencies = [
   "sqlalchemy >= 2.0",
+  "tomlkit >= 0.11",
   "typing_extensions"
 ]
 
 [project.urls]
-Documentation = "https://github.com/jeremander/fancy-dataclass#readme"
+# Documentation = "https://github.com/jeremander/fancy-dataclass#readme"
+Documentation = "https://fancy-dataclass.readthedocs.io"
 Issues = "https://github.com/jeremander/fancy-dataclass/issues"
 Source = "https://github.com/jeremander/fancy-dataclass"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["TODO.txt"]
 
 [tool.hatch.version]
@@ -41,44 +43,48 @@
   "mkdocstrings-python",
   "mkdocs-literate-nav",
 ]
 
 [tool.hatch.envs.doc.scripts]
 build = "mkdocs build --clean --strict"
 serve = "mkdocs serve"
-deploy = "mkdocs gh-deploy"
+# deploy = "mkdocs gh-deploy"
+deploy = "mkdocs build --site-dir $READTHEDOCS_OUTPUT/html"
 
 [tool.hatch.envs.lint]
 dependencies = [
   "mypy>=1.0",
+  "numpy",
+  "pytest",
+  "radon",
   "ruff>=0.3",
-  "vermin"
+  "vermin",
 ]
 
 [tool.hatch.envs.lint.scripts]
-run-mypy = "mypy --install-types --non-interactive {args:fancy_dataclass tests}"
 run-ruff = "ruff check"
-run-vermin = "vermin {args:--eval-annotations --no-tips --exclude 'tests.test_json.StrEnum' fancy_dataclass}"
-all = ["run-ruff", "run-vermin", "run-mypy"]
+run-vermin = "vermin {args:-t=3.8- --eval-annotations --no-tips --violations --exclude 'tests.test_serializable.StrEnum' fancy_dataclass}"
+run-mypy = "mypy --install-types --non-interactive {args:fancy_dataclass tests}"
+run-loc-summary = "./summarize.sh"
+all = ["run-ruff", "run-vermin", "run-mypy", "run-loc-summary"]
 
 [tool.hatch.envs.test]
 dependencies = [
     "numpy",
     "pytest",
     "pytest-cov",
-    "pytest-stub"
 ]
 
 [tool.hatch.envs.test.scripts]
 test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
+test-debug = "pytest --pdb {args:tests}"
 cov-report = ["- coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
 
-[[tool.hatch.envs.all.matrix]]
+[[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.publish.index]
 disable = true
 
 [tool.coverage.run]
 source_pkgs = ["fancy_dataclass", "tests"]
@@ -109,24 +115,28 @@
 disable_error_code = ["arg-type", "attr-defined", "call-arg", "comparison-overlap", "no-redef", "no-untyped-call", "no-untyped-def", "type-arg"]
 
 [[tool.mypy.overrides]]
 module = "tests.test_cli"
 disable_error_code = ["assignment"]
 
 [[tool.mypy.overrides]]
-module = "tests.test_json"
-disable_error_code = ["assignment", "misc"]
+module = "tests.test_config"
+disable_error_code = ["misc", "union-attr"]
 
 [[tool.mypy.overrides]]
 module = "tests.test_inheritance"
 disable_error_code = ["assignment", "misc"]
 
 [[tool.mypy.overrides]]
 module = "tests.test_mixin"
 disable_error_code = ["assignment", "call-overload", "has-type", "misc", "union-attr"]
 
 [[tool.mypy.overrides]]
+module = "tests.test_serializable"
+disable_error_code = ["assignment", "misc"]
+
+[[tool.mypy.overrides]]
 module = "tests.test_subprocess"
 disable_error_code = ["assignment", "misc"]
 
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=fancy_dataclass"
```

### Comparing `fancy_dataclass-0.2.0/docs/README.md` & `fancy_dataclass-0.3.0/docs/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 ## Introduction
 
 Python 3.7 introduced the `dataclasses` module which lets you write "statically typed" classes using the type hinting mechanism.
 
 By inspecting dataclasses' type annotations, it is possible to endow them with special powers that help cut down on boilerplate code in a wide variety of domains, such as:
 
-- *JSON conversion*: serialize dataclasses to JSON and vice versa
+- *JSON/TOML conversion*: convert dataclasses to JSON/TOML files and vice versa
+- *Configuration management*: store global configurations and use them anywhere in your program
 - *SQL persistence*: define a SQL table, and save/load objects from a database
 - *CLI parsing*: parse command-line arguments and store their values in a dataclass, then use them to execute your main program logic
 - *Subprocess calls*: generate command-line arguments to be passed to another program
 
 `fancy_dataclass` borrows ideas from other excellent libraries such as [`marshmallow`](https://marshmallow.readthedocs.io/en/stable/), [`pydantic`](https://docs.pydantic.dev/latest), and [`argparse_dataclass`](https://github.com/mivade/argparse_dataclass), but it aims to be as lightweight as possible in terms of its dependencies and learning curve.
 
 ## How to install
 
-```pip install fancy_dataclass```
+```pip install fancy-dataclass```
 
 Requires Python 3.8 or higher.
 
 ## Example
 
 **Regular dataclass**
 
@@ -67,15 +68,16 @@
     "cycling"
   ]
 }
 ```
 
 ## Documentation
 
-The documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material).
-<!-- TODO: "...and is hosted by ..." -->
+Read the official documentation [here](https://fancy-dataclass.readthedocs.io).
+
+The documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) and is hosted by [Read the Docs](https://readthedocs.org).
 
 View the Changelog [here](CHANGELOG.md).
 
 ## License
 
 This library is distributed under the terms of the [MIT](LICENSE.txt) license.
```

### Comparing `fancy_dataclass-0.2.0/PKG-INFO` & `fancy_dataclass-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.3
 Name: fancy-dataclass
-Version: 0.2.0
-Summary: Enhance dataclasses with additional features.
-Project-URL: Documentation, https://github.com/jeremander/fancy-dataclass#readme
+Version: 0.3.0
+Summary: Spiff up your dataclasses with additional features.
+Project-URL: Documentation, https://fancy-dataclass.readthedocs.io
 Project-URL: Issues, https://github.com/jeremander/fancy-dataclass/issues
 Project-URL: Source, https://github.com/jeremander/fancy-dataclass
 Author-email: Jeremy Silver <jeremys@nessiness.com>
 License-Expression: MIT
-Keywords: cli,dataclass,json,orm,serialize
+Keywords: cli,config,dataclass,json,orm,serialize,toml
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Requires-Dist: sqlalchemy>=2.0
+Requires-Dist: tomlkit>=0.11
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # Basics
 
 🤵🏻‍♂️ ***Fancy Dataclass***: A library to spiff up your dataclasses with extra features.
 
 ## Introduction
 
 Python 3.7 introduced the `dataclasses` module which lets you write "statically typed" classes using the type hinting mechanism.
 
 By inspecting dataclasses' type annotations, it is possible to endow them with special powers that help cut down on boilerplate code in a wide variety of domains, such as:
 
-- *JSON conversion*: serialize dataclasses to JSON and vice versa
+- *JSON/TOML conversion*: convert dataclasses to JSON/TOML files and vice versa
+- *Configuration management*: store global configurations and use them anywhere in your program
 - *SQL persistence*: define a SQL table, and save/load objects from a database
 - *CLI parsing*: parse command-line arguments and store their values in a dataclass, then use them to execute your main program logic
 - *Subprocess calls*: generate command-line arguments to be passed to another program
 
 `fancy_dataclass` borrows ideas from other excellent libraries such as [`marshmallow`](https://marshmallow.readthedocs.io/en/stable/), [`pydantic`](https://docs.pydantic.dev/latest), and [`argparse_dataclass`](https://github.com/mivade/argparse_dataclass), but it aims to be as lightweight as possible in terms of its dependencies and learning curve.
 
 ## How to install
 
-```pip install fancy_dataclass```
+```pip install fancy-dataclass```
 
 Requires Python 3.8 or higher.
 
 ## Example
 
 **Regular dataclass**
 
@@ -83,15 +85,16 @@
     "cycling"
   ]
 }
 ```
 
 ## Documentation
 
-The documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material).
-<!-- TODO: "...and is hosted by ..." -->
+Read the official documentation [here](https://fancy-dataclass.readthedocs.io).
+
+The documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) and is hosted by [Read the Docs](https://readthedocs.org).
 
 View the Changelog [here](CHANGELOG.md).
 
 ## License
 
 This library is distributed under the terms of the [MIT](LICENSE.txt) license.
```

