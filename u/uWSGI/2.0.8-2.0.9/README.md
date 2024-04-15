# Comparing `tmp/uwsgi-2.0.8.tar.gz` & `tmp/uwsgi-2.0.9.tar.gz`

## Comparing `uwsgi-2.0.8.tar` & `uwsgi-2.0.9.tar`

### file list

```diff
@@ -1,807 +1,809 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/
--rw-rw-r--   0 root         (0) root         (0)      178 2014-10-26 04:30:44.000000 uwsgi-2.0.8/.gitignore
--rw-rw-r--   0 root         (0) root         (0)     1881 2014-10-26 04:30:44.000000 uwsgi-2.0.8/.travis.yml
--rw-rw-r--   0 root         (0) root         (0)      717 2014-10-26 04:30:44.000000 uwsgi-2.0.8/CONTRIBUTORS
--rw-rw-r--   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/INSTALL
--rw-rw-r--   0 root         (0) root         (0)    18628 2014-10-26 04:30:44.000000 uwsgi-2.0.8/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      261 2014-10-26 04:30:44.000000 uwsgi-2.0.8/Makefile
--rw-rw-r--   0 root         (0) root         (0)      148 2014-10-26 04:30:44.000000 uwsgi-2.0.8/README
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/apache2/
--rw-rw-r--   0 root         (0) root         (0)    24733 2014-10-26 04:30:44.000000 uwsgi-2.0.8/apache2/mod_Ruwsgi.c
--rw-rw-r--   0 root         (0) root         (0)    15385 2014-10-26 04:30:44.000000 uwsgi-2.0.8/apache2/mod_proxy_uwsgi.c
--rw-rw-r--   0 root         (0) root         (0)    22714 2014-10-26 04:30:44.000000 uwsgi-2.0.8/apache2/mod_uwsgi.c
--rw-rw-r--   0 root         (0) root         (0)      190 2014-10-26 04:30:44.000000 uwsgi-2.0.8/attach.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/bin/
--rw-rw-r--   0 root         (0) root         (0)      113 2014-10-26 04:30:44.000000 uwsgi-2.0.8/bin/uwsgi
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/
--rw-rw-r--   0 root         (0) root         (0)      243 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/all.ini
--rw-rw-r--   0 root         (0) root         (0)       61 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/asyncio.ini
--rw-rw-r--   0 root         (0) root         (0)      922 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/base.ini
--rw-rw-r--   0 root         (0) root         (0)       41 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/cgi.ini
--rw-rw-r--   0 root         (0) root         (0)       61 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/core.ini
--rw-rw-r--   0 root         (0) root         (0)       49 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/coroae.ini
--rw-rw-r--   0 root         (0) root         (0)      170 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/coverity.ini
--rw-rw-r--   0 root         (0) root         (0)       51 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/default.ini
--rw-rw-r--   0 root         (0) root         (0)       93 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/django.ini
--rw-rw-r--   0 root         (0) root         (0)       89 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/embedded.ini
--rw-rw-r--   0 root         (0) root         (0)       44 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/erlang.ini
--rw-rw-r--   0 root         (0) root         (0)       43 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/gccgo.ini
--rw-rw-r--   0 root         (0) root         (0)       51 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/gevent.ini
--rw-rw-r--   0 root         (0) root         (0)       47 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/glusterfs.ini
--rw-rw-r--   0 root         (0) root         (0)       44 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/gridfs.ini
--rw-rw-r--   0 root         (0) root         (0)       47 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/jwsgi.ini
--rw-rw-r--   0 root         (0) root         (0)       95 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/lib.ini
--rw-rw-r--   0 root         (0) root         (0)       41 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/lua.ini
--rw-rw-r--   0 root         (0) root         (0)       52 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/luap.ini
--rw-rw-r--   0 root         (0) root         (0)      390 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/minimal.ini
--rw-rw-r--   0 root         (0) root         (0)      128 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/modular.ini
--rw-rw-r--   0 root         (0) root         (0)       42 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/mono.ini
--rw-rw-r--   0 root         (0) root         (0)       37 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/nolang.ini
--rw-rw-r--   0 root         (0) root         (0)       70 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/package.ini
--rw-rw-r--   0 root         (0) root         (0)       41 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/php.ini
--rw-rw-r--   0 root         (0) root         (0)       45 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/plonly.ini
--rw-rw-r--   0 root         (0) root         (0)      408 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/ppa.ini
--rw-rw-r--   0 root         (0) root         (0)       42 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/psgi.ini
--rw-rw-r--   0 root         (0) root         (0)       58 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/pyerl.ini
--rw-rw-r--   0 root         (0) root         (0)       48 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/pylua.ini
--rw-rw-r--   0 root         (0) root         (0)       47 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/pyonly.ini
--rw-rw-r--   0 root         (0) root         (0)       42 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/pypy.ini
--rw-rw-r--   0 root         (0) root         (0)       45 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/pypyonly.ini
--rw-rw-r--   0 root         (0) root         (0)       86 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/pyring.ini
--rw-rw-r--   0 root         (0) root         (0)       92 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/pyuwsgi.ini
--rw-rw-r--   0 root         (0) root         (0)       42 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/rack.ini
--rw-rw-r--   0 root         (0) root         (0)       43 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/rados.ini
--rw-rw-r--   0 root         (0) root         (0)       45 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/rbonly.ini
--rw-rw-r--   0 root         (0) root         (0)       46 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/ring.ini
--rw-rw-r--   0 root         (0) root         (0)       58 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/ruby2.ini
--rw-rw-r--   0 root         (0) root         (0)       49 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/servlet.ini
--rw-rw-r--   0 root         (0) root         (0)       37 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/travis.ini
--rw-rw-r--   0 root         (0) root         (0)      432 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/unbit.ini
--rw-rw-r--   0 root         (0) root         (0)      108 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/unbitstaff.ini
--rw-rw-r--   0 root         (0) root         (0)      396 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/uwsgi.it.ini
--rw-rw-r--   0 root         (0) root         (0)       40 2014-10-26 04:30:44.000000 uwsgi-2.0.8/buildconf/v8.ini
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/
--rw-rw-r--   0 root         (0) root         (0)     3490 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/Uwsgi.pm
--rw-rw-r--   0 root         (0) root         (0)      657 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/binder.pl
--rw-rw-r--   0 root         (0) root         (0)     1629 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/centos_init_script
--rw-rw-r--   0 root         (0) root         (0)     1586 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/cgi_python.c
--rw-rw-r--   0 root         (0) root         (0)      450 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/cryptologger.rb
--rw-rw-r--   0 root         (0) root         (0)     3311 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/emperormon.ru
--rw-rw-r--   0 root         (0) root         (0)      101 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/fdconf.pl
--rw-rw-r--   0 root         (0) root         (0)     1003 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/graphite_uwsgi.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/launchd/
--rw-rw-r--   0 root         (0) root         (0)      478 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/launchd/it.unbit.uwsgi.emperor.plist
--rw-rw-r--   0 root         (0) root         (0)      544 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/launchd/it.unbit.uwsgi.plist
--rw-rw-r--   0 root         (0) root         (0)      513 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/loadapp.pl
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/pypy/
--rw-rw-r--   0 root         (0) root         (0)     1768 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/pypy/uwsgi_pypy_greenlets.py
--rw-rw-r--   0 root         (0) root         (0)      331 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/pyuwsgi.py
--rw-rw-r--   0 root         (0) root         (0)     2560 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/runuwsgi.py
--rw-rw-r--   0 root         (0) root         (0)      814 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/securesubscribe.pl
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/spoolqueue/
--rw-rw-r--   0 root         (0) root         (0)      183 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/spoolqueue/producer.py
--rw-rw-r--   0 root         (0) root         (0)      191 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/spoolqueue/tasks.py
--rw-rw-r--   0 root         (0) root         (0)      958 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/spoolqueue/tasksconsumer.py
--rw-rw-r--   0 root         (0) root         (0)      445 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/subscribe.pl
--rw-rw-r--   0 root         (0) root         (0)     4043 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/twuwsgi.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/upstart/
--rw-rw-r--   0 root         (0) root         (0)      245 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/upstart/emperor.conf
--rw-rw-r--   0 root         (0) root         (0)      344 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/upstart/uwsgi.conf
--rw-rw-r--   0 root         (0) root         (0)      245 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/upython
--rw-rw-r--   0 root         (0) root         (0)    10028 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/urack.rb
--rw-rw-r--   0 root         (0) root         (0)     4587 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/uwsgi-cache-monitor.py
--rw-rw-r--   0 root         (0) root         (0)      693 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/uwsgi.erl
--rw-rw-r--   0 root         (0) root         (0)     6765 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/uwsgi.java
--rw-rw-r--   0 root         (0) root         (0)     3563 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/uwsgi.rb
--rw-rw-r--   0 root         (0) root         (0)     1780 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/uwsgi_client.c
--rw-rw-r--   0 root         (0) root         (0)     1779 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/uwsgi_dynamic_client.c
--rw-rw-r--   0 root         (0) root         (0)     2783 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/uwsgisubscribers.ru
--rw-rw-r--   0 root         (0) root         (0)      411 2014-10-26 04:30:44.000000 uwsgi-2.0.8/contrib/xinetd_uwsgi
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/
--rw-rw-r--   0 root         (0) root         (0)    11552 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/alarm.c
--rw-rw-r--   0 root         (0) root         (0)    15214 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/async.c
--rw-rw-r--   0 root         (0) root         (0)    12177 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/buffer.c
--rw-rw-r--   0 root         (0) root         (0)    64563 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/cache.c
--rw-rw-r--   0 root         (0) root         (0)     5462 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/chunked.c
--rw-rw-r--   0 root         (0) root         (0)       14 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/clang_fake.c
--rw-rw-r--   0 root         (0) root         (0)      907 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/clock.c
--rw-rw-r--   0 root         (0) root         (0)    21879 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/config.c
--rw-rw-r--   0 root         (0) root         (0)     1601 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/cookie.c
--rw-rw-r--   0 root         (0) root         (0)     8454 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/cron.c
--rw-rw-r--   0 root         (0) root         (0)    14989 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/daemons.c
--rw-rw-r--   0 root         (0) root         (0)    62746 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/emperor.c
--rw-rw-r--   0 root         (0) root         (0)     3055 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/errors.c
--rw-rw-r--   0 root         (0) root         (0)    28826 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/event.c
--rw-rw-r--   0 root         (0) root         (0)    16778 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/exceptions.c
--rw-rw-r--   0 root         (0) root         (0)     4358 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/fifo.c
--rw-rw-r--   0 root         (0) root         (0)     4427 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/fsmon.c
--rw-rw-r--   0 root         (0) root         (0)     4713 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/gateway.c
--rw-rw-r--   0 root         (0) root         (0)     2365 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/hash.c
--rw-rw-r--   0 root         (0) root         (0)    16123 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/hooks.c
--rw-rw-r--   0 root         (0) root         (0)     2820 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/ini.c
--rw-rw-r--   0 root         (0) root         (0)    14071 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/init.c
--rw-rw-r--   0 root         (0) root         (0)    34521 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/io.c
--rw-rw-r--   0 root         (0) root         (0)     8700 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/json.c
--rw-rw-r--   0 root         (0) root         (0)    35763 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/legion.c
--rw-rw-r--   0 root         (0) root         (0)    20134 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/lock.c
--rw-rw-r--   0 root         (0) root         (0)    55355 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/logging.c
--rw-rw-r--   0 root         (0) root         (0)     3469 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/loop.c
--rw-rw-r--   0 root         (0) root         (0)    31168 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/master.c
--rw-rw-r--   0 root         (0) root         (0)    10824 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/master_checks.c
--rw-rw-r--   0 root         (0) root         (0)     7616 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/master_events.c
--rw-rw-r--   0 root         (0) root         (0)    49019 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/master_utils.c
--rw-rw-r--   0 root         (0) root         (0)    31489 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/metrics.c
--rw-rw-r--   0 root         (0) root         (0)     6147 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/mount.c
--rw-rw-r--   0 root         (0) root         (0)    11749 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/mule.c
--rw-rw-r--   0 root         (0) root         (0)     2803 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/notify.c
--rw-rw-r--   0 root         (0) root         (0)    17328 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/offload.c
--rw-rw-r--   0 root         (0) root         (0)     7702 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/plugins.c
--rw-rw-r--   0 root         (0) root         (0)     2662 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/plugins_builder.c
--rw-rw-r--   0 root         (0) root         (0)     2813 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/progress.c
--rw-rw-r--   0 root         (0) root         (0)    30720 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/protocol.c
--rw-rw-r--   0 root         (0) root         (0)     1128 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/querystring.c
--rw-rw-r--   0 root         (0) root         (0)     4452 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/queue.c
--rw-rw-r--   0 root         (0) root         (0)     7567 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/rb_timers.c
--rw-rw-r--   0 root         (0) root         (0)    20712 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/reader.c
--rw-rw-r--   0 root         (0) root         (0)     2491 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/regexp.c
--rw-rw-r--   0 root         (0) root         (0)    68920 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/routing.c
--rw-rw-r--   0 root         (0) root         (0)     5052 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/rpc.c
--rw-rw-r--   0 root         (0) root         (0)     2555 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/sendfile.c
--rw-rw-r--   0 root         (0) root         (0)     4108 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/setup_utils.c
--rw-rw-r--   0 root         (0) root         (0)    12712 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/sharedarea.c
--rw-rw-r--   0 root         (0) root         (0)    13060 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/signal.c
--rw-rw-r--   0 root         (0) root         (0)      214 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/skel.c
--rw-rw-r--   0 root         (0) root         (0)     9561 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/snmp.c
--rw-rw-r--   0 root         (0) root         (0)    50440 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/socket.c
--rw-rw-r--   0 root         (0) root         (0)    16524 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/spooler.c
--rw-rw-r--   0 root         (0) root         (0)    21462 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/ssl.c
--rw-rw-r--   0 root         (0) root         (0)    18218 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/static.c
--rw-rw-r--   0 root         (0) root         (0)    14340 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/stats.c
--rw-rw-r--   0 root         (0) root         (0)     1191 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/storage.c
--rw-rw-r--   0 root         (0) root         (0)     9867 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/strings.c
--rw-rw-r--   0 root         (0) root         (0)    30894 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/subscription.c
--rw-rw-r--   0 root         (0) root         (0)     1187 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/timebomb.c
--rw-rw-r--   0 root         (0) root         (0)     3839 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/transformations.c
--rw-rw-r--   0 root         (0) root         (0)   100692 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/utils.c
--rw-rw-r--   0 root         (0) root         (0)   210575 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/uwsgi.c
--rw-rw-r--   0 root         (0) root         (0)    13867 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/websockets.c
--rw-rw-r--   0 root         (0) root         (0)    22812 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/writer.c
--rw-rw-r--   0 root         (0) root         (0)     6491 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/xmlconf.c
--rw-rw-r--   0 root         (0) root         (0)     5035 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/yaml.c
--rw-rw-r--   0 root         (0) root         (0)     2043 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/zeus.c
--rw-rw-r--   0 root         (0) root         (0)     4420 2014-10-26 04:30:44.000000 uwsgi-2.0.8/core/zlib.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/
--rw-rw-r--   0 root         (0) root         (0)      128 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/bootstrap.py
--rw-rw-r--   0 root         (0) root         (0)       91 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/bootstrap2.py
--rw-rw-r--   0 root         (0) root         (0)      186 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/bootstrap3.py
--rw-rw-r--   0 root         (0) root         (0)       80 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/bootstrap4.py
--rw-rw-r--   0 root         (0) root         (0)       46 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/bootstrap5.py
--rw-rw-r--   0 root         (0) root         (0)      227 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/config.lua
--rw-rw-r--   0 root         (0) root         (0)      195 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/config.ru
--rw-rw-r--   0 root         (0) root         (0)      530 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/config17.ru
--rw-rw-r--   0 root         (0) root         (0)      198 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/config2.lua
--rw-rw-r--   0 root         (0) root         (0)       77 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/config2.ru
--rw-rw-r--   0 root         (0) root         (0)     1120 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/config30.ru
--rw-rw-r--   0 root         (0) root         (0)     1803 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/corostream.pl
--rw-rw-r--   0 root         (0) root         (0)       27 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/debug.ini
--rw-rw-r--   0 root         (0) root         (0)      739 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/fibers.ru
--rw-rw-r--   0 root         (0) root         (0)      125 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/fibers.yml
--rw-rw-r--   0 root         (0) root         (0)      497 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/flaskpost.py
--rw-rw-r--   0 root         (0) root         (0)      418 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/heavytest.ini
--rw-rw-r--   0 root         (0) root         (0)      530 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/heavytest.py
--rw-rw-r--   0 root         (0) root         (0)      755 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/info_uwsgi.php
--rw-rw-r--   0 root         (0) root         (0)      678 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/logic.ini
--rw-rw-r--   0 root         (0) root         (0)      389 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/mega.xml
--rw-rw-r--   0 root         (0) root         (0)      629 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/mjpeg_stream.py
--rw-rw-r--   0 root         (0) root         (0)      373 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/mojoapp.pl
--rw-rw-r--   0 root         (0) root         (0)      461 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/multi.ini
--rw-rw-r--   0 root         (0) root         (0)     1075 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/multi.xml
--rw-rw-r--   0 root         (0) root         (0)      573 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/multiapp.py
--rw-rw-r--   0 root         (0) root         (0)      424 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/protected.ini
--rw-rw-r--   0 root         (0) root         (0)      582 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/router.lua
--rw-rw-r--   0 root         (0) root         (0)      831 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/simple_app.py
--rw-rw-r--   0 root         (0) root         (0)      319 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/simple_app_wsgi2.py
--rw-rw-r--   0 root         (0) root         (0)      108 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/simple_logger.py
--rw-rw-r--   0 root         (0) root         (0)      451 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/sites.xml
--rw-rw-r--   0 root         (0) root         (0)      217 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/sputnik.ws
--rw-rw-r--   0 root         (0) root         (0)      474 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/staticfilesnmp.py
--rw-rw-r--   0 root         (0) root         (0)      757 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/taskqueue.py
--rw-rw-r--   0 root         (0) root         (0)      592 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/uwsgi.xml
--rw-rw-r--   0 root         (0) root         (0)     1882 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/uwsgirouter.py
--rw-rw-r--   0 root         (0) root         (0)      160 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/uwsgirouter2.py
--rw-rw-r--   0 root         (0) root         (0)      405 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/uwsgirouter3.py
--rw-rw-r--   0 root         (0) root         (0)      258 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/uwsgirouter4.py
--rw-rw-r--   0 root         (0) root         (0)      178 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/uwsgirouter5.py
--rw-rw-r--   0 root         (0) root         (0)     1793 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/uwsgistatus.py
--rw-rw-r--   0 root         (0) root         (0)      229 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/welcome.ini
--rw-rw-r--   0 root         (0) root         (0)     3232 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/welcome.py
--rw-rw-r--   0 root         (0) root         (0)     1074 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/welcome3.py
--rw-rw-r--   0 root         (0) root         (0)      235 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/werkzeug.js
--rw-rw-r--   0 root         (0) root         (0)      533 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/werkzeug.yml
--rw-rw-r--   0 root         (0) root         (0)      193 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/werkzeug_strict.yml
--rw-rw-r--   0 root         (0) root         (0)     3600 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/xmlindex-html.xsl
--rw-rw-r--   0 root         (0) root         (0)      530 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/xmlindex.ini
--rw-rw-r--   0 root         (0) root         (0)      212 2014-10-26 04:30:44.000000 uwsgi-2.0.8/examples/zmqgevent.ini
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/ext/
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/ext/uwsgi/
--rw-rw-r--   0 root         (0) root         (0)      641 2014-10-26 04:30:44.000000 uwsgi-2.0.8/ext/uwsgi/extconf.rb
--rw-rw-r--   0 root         (0) root         (0)      551 2014-10-26 04:30:44.000000 uwsgi-2.0.8/install.sh
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/lib/
--rw-rw-r--   0 root         (0) root         (0)     6341 2014-10-26 04:30:44.000000 uwsgi-2.0.8/lib/linux_ns.c
--rw-rw-r--   0 root         (0) root         (0)    10633 2014-10-26 04:30:44.000000 uwsgi-2.0.8/lib/netlink.c
--rw-rw-r--   0 root         (0) root         (0)      644 2014-10-26 04:30:44.000000 uwsgi-2.0.8/lib/sun_fixes.c
--rw-rw-r--   0 root         (0) root         (0)     5971 2014-10-26 04:30:44.000000 uwsgi-2.0.8/logo_uWSGI.png
--rw-rw-r--   0 root         (0) root         (0)     4142 2014-10-26 04:30:44.000000 uwsgi-2.0.8/logo_uWSGI.svg
--rw-rw-r--   0 root         (0) root         (0)      665 2014-10-26 04:30:44.000000 uwsgi-2.0.8/mongrel2-uwsgi.conf
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/airbrake/
--rw-rw-r--   0 root         (0) root         (0)     8660 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/airbrake/airbrake_plugin.c
--rw-rw-r--   0 root         (0) root         (0)      184 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/airbrake/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_curl/
--rw-rw-r--   0 root         (0) root         (0)     7686 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_curl/alarm_curl_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       95 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_curl/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_speech/
--rw-rw-r--   0 root         (0) root         (0)     1313 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_speech/alarm_speech.m
--rw-rw-r--   0 root         (0) root         (0)      237 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_speech/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_xmpp/
--rw-rw-r--   0 root         (0) root         (0)      745 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_xmpp/alarm_xmpp_plugin.c
--rw-rw-r--   0 root         (0) root         (0)     4504 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_xmpp/gloox.cc
--rw-rw-r--   0 root         (0) root         (0)      108 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/alarm_xmpp/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/asyncio/
--rw-rw-r--   0 root         (0) root         (0)    11947 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/asyncio/asyncio.c
--rw-rw-r--   0 root         (0) root         (0)      193 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/asyncio/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cache/
--rw-rw-r--   0 root         (0) root         (0)    11738 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cache/cache.c
--rw-rw-r--   0 root         (0) root         (0)       71 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cache/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/carbon/
--rw-rw-r--   0 root         (0) root         (0)    15243 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/carbon/carbon.c
--rw-rw-r--   0 root         (0) root         (0)       73 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/carbon/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cgi/
--rw-rw-r--   0 root         (0) root         (0)    27579 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cgi/cgi_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       72 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cgi/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cheaper_backlog2/
--rw-rw-r--   0 root         (0) root         (0)     2192 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cheaper_backlog2/cheaper_backlog2.c
--rw-rw-r--   0 root         (0) root         (0)       92 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cheaper_backlog2/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cheaper_busyness/
--rw-rw-r--   0 root         (0) root         (0)    18536 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cheaper_busyness/cheaper_busyness.c
--rw-rw-r--   0 root         (0) root         (0)       92 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cheaper_busyness/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/clock_monotonic/
--rw-rw-r--   0 root         (0) root         (0)      730 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/clock_monotonic/clock_monotonic.c
--rw-rw-r--   0 root         (0) root         (0)       96 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/clock_monotonic/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/clock_realtime/
--rw-rw-r--   0 root         (0) root         (0)      718 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/clock_realtime/clock_realtime.c
--rw-rw-r--   0 root         (0) root         (0)       94 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/clock_realtime/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/corerouter/
--rw-rw-r--   0 root         (0) root         (0)    33769 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/corerouter/corerouter.c
--rw-rw-r--   0 root         (0) root         (0)    12636 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/corerouter/cr.h
--rw-rw-r--   0 root         (0) root         (0)     8368 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/corerouter/cr_common.c
--rw-rw-r--   0 root         (0) root         (0)     6044 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/corerouter/cr_map.c
--rw-rw-r--   0 root         (0) root         (0)      104 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/corerouter/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/coroae/
--rw-rw-r--   0 root         (0) root         (0)    10245 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/coroae/coroae.c
--rw-rw-r--   0 root         (0) root         (0)      588 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/coroae/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cplusplus/
--rw-rw-r--   0 root         (0) root         (0)     1365 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cplusplus/base.cc
--rw-rw-r--   0 root         (0) root         (0)      405 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cplusplus/plugin.c
--rw-rw-r--   0 root         (0) root         (0)       96 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/cplusplus/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/curl_cron/
--rw-rw-r--   0 root         (0) root         (0)     2862 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/curl_cron/curl_cron.c
--rw-rw-r--   0 root         (0) root         (0)       86 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/curl_cron/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/dumbloop/
--rw-rw-r--   0 root         (0) root         (0)     2274 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/dumbloop/dumb.c
--rw-rw-r--   0 root         (0) root         (0)       72 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/dumbloop/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/dummy/
--rw-rw-r--   0 root         (0) root         (0)      254 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/dummy/dummy.c
--rw-rw-r--   0 root         (0) root         (0)       71 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/dummy/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/echo/
--rw-rw-r--   0 root         (0) root         (0)      321 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/echo/echo_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       75 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/echo/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_amqp/
--rw-rw-r--   0 root         (0) root         (0)    17237 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_amqp/amqp.c
--rw-rw-r--   0 root         (0) root         (0)     3239 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_amqp/emperor_amqp.c
--rw-rw-r--   0 root         (0) root         (0)       92 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_amqp/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_mongodb/
--rw-rw-r--   0 root         (0) root         (0)     5411 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_mongodb/emperor_mongodb.cc
--rw-rw-r--   0 root         (0) root         (0)      619 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_mongodb/plugin.c
--rw-rw-r--   0 root         (0) root         (0)      316 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_mongodb/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_pg/
--rw-rw-r--   0 root         (0) root         (0)     2896 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_pg/emperor_pg.c
--rw-rw-r--   0 root         (0) root         (0)      330 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_pg/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_zeromq/
--rw-rw-r--   0 root         (0) root         (0)     5962 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_zeromq/emperor_zeromq.c
--rw-rw-r--   0 root         (0) root         (0)       96 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/emperor_zeromq/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/example/
--rw-rw-r--   0 root         (0) root         (0)      827 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/example/example_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       81 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/example/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/exception_log/
--rw-rw-r--   0 root         (0) root         (0)     3483 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/exception_log/exception_log.c
--rw-rw-r--   0 root         (0) root         (0)       86 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/exception_log/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/fastrouter/
--rw-rw-r--   0 root         (0) root         (0)    12001 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/fastrouter/fastrouter.c
--rw-rw-r--   0 root         (0) root         (0)      108 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/fastrouter/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/fiber/
--rw-rw-r--   0 root         (0) root         (0)     2516 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/fiber/fiber.c
--rw-rw-r--   0 root         (0) root         (0)     1255 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/fiber/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/forkptyrouter/
--rw-rw-r--   0 root         (0) root         (0)     9753 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/forkptyrouter/forkptyrouter.c
--rw-rw-r--   0 root         (0) root         (0)      113 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/forkptyrouter/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gccgo/
--rw-rw-r--   0 root         (0) root         (0)    13843 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gccgo/gccgo_plugin.c
--rw-rw-r--   0 root         (0) root         (0)     4336 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gccgo/uwsgi.go
--rw-rw-r--   0 root         (0) root         (0)      389 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gccgo/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/geoip/
--rw-rw-r--   0 root         (0) root         (0)     4141 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/geoip/geoip.c
--rw-rw-r--   0 root         (0) root         (0)       81 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/geoip/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gevent/
--rw-rw-r--   0 root         (0) root         (0)    17210 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gevent/gevent.c
--rw-rw-r--   0 root         (0) root         (0)     2404 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gevent/gevent.h
--rw-rw-r--   0 root         (0) root         (0)     3879 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gevent/hooks.c
--rw-rw-r--   0 root         (0) root         (0)      200 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gevent/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/glusterfs/
--rw-rw-r--   0 root         (0) root         (0)     9098 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/glusterfs/glusterfs.c
--rw-rw-r--   0 root         (0) root         (0)      221 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/glusterfs/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/graylog2/
--rw-rw-r--   0 root         (0) root         (0)     2438 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/graylog2/graylog2_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       88 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/graylog2/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/greenlet/
--rw-rw-r--   0 root         (0) root         (0)     4384 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/greenlet/greenlet.c
--rw-rw-r--   0 root         (0) root         (0)      195 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/greenlet/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gridfs/
--rw-rw-r--   0 root         (0) root         (0)     9353 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gridfs/gridfs.cc
--rw-rw-r--   0 root         (0) root         (0)      719 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gridfs/plugin.c
--rw-rw-r--   0 root         (0) root         (0)      360 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/gridfs/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/http/
--rw-rw-r--   0 root         (0) root         (0)     4230 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/http/common.h
--rw-rw-r--   0 root         (0) root         (0)    35321 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/http/http.c
--rw-rw-r--   0 root         (0) root         (0)    14280 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/http/https.c
--rw-rw-r--   0 root         (0) root         (0)     5676 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/http/keepalive.c
--rw-rw-r--   0 root         (0) root         (0)    22858 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/http/spdy3.c
--rw-rw-r--   0 root         (0) root         (0)    12685 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/http/spdy3.h
--rw-rw-r--   0 root         (0) root         (0)      127 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/http/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/jvm/
--rw-rw-r--   0 root         (0) root         (0)     3420 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/jvm/jvm.h
--rw-rw-r--   0 root         (0) root         (0)    42889 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/jvm/jvm_plugin.c
--rw-rw-r--   0 root         (0) root         (0)     1543 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/jvm/uwsgi.java
--rw-rw-r--   0 root         (0) root         (0)     3069 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/jvm/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/jwsgi/
--rw-rw-r--   0 root         (0) root         (0)     5364 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/jwsgi/jwsgi_plugin.c
--rw-rw-r--   0 root         (0) root         (0)      298 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/jwsgi/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ldap/
--rw-rw-r--   0 root         (0) root         (0)    15137 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ldap/ldap.c
--rw-rw-r--   0 root         (0) root         (0)       77 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ldap/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/legion_cache_fetch/
--rw-rw-r--   0 root         (0) root         (0)     1938 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/legion_cache_fetch/legion_cache_fetch.c
--rw-rw-r--   0 root         (0) root         (0)      100 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/legion_cache_fetch/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/libffi/
--rw-rw-r--   0 root         (0) root         (0)     1830 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/libffi/libffi.c
--rw-rw-r--   0 root         (0) root         (0)       70 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/libffi/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/libtcc/
--rw-rw-r--   0 root         (0) root         (0)     1315 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/libtcc/libtcc.c
--rw-rw-r--   0 root         (0) root         (0)       70 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/libtcc/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logcrypto/
--rw-rw-r--   0 root         (0) root         (0)     5282 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logcrypto/logcrypto.c
--rw-rw-r--   0 root         (0) root         (0)       78 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logcrypto/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logfile/
--rw-rw-r--   0 root         (0) root         (0)     2169 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logfile/logfile.c
--rw-rw-r--   0 root         (0) root         (0)       74 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logfile/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logpipe/
--rw-rw-r--   0 root         (0) root         (0)     1186 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logpipe/logpipe.c
--rw-rw-r--   0 root         (0) root         (0)       74 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logpipe/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logsocket/
--rw-rw-r--   0 root         (0) root         (0)     1590 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logsocket/logsocket_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       85 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logsocket/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logzmq/
--rw-rw-r--   0 root         (0) root         (0)     1743 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logzmq/plugin.c
--rw-rw-r--   0 root         (0) root         (0)       80 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/logzmq/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/lua/
--rw-rw-r--   0 root         (0) root         (0)    27053 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/lua/lua_plugin.c
--rw-rw-r--   0 root         (0) root         (0)      726 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/lua/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/matheval/
--rw-rw-r--   0 root         (0) root         (0)     1860 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/matheval/math.c
--rw-rw-r--   0 root         (0) root         (0)       84 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/matheval/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mongodb/
--rw-rw-r--   0 root         (0) root         (0)      172 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mongodb/plugin.c
--rw-rw-r--   0 root         (0) root         (0)      195 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mongodb/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mongodblog/
--rw-rw-r--   0 root         (0) root         (0)     4063 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mongodblog/mongodblog_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       87 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mongodblog/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mongrel2/
--rw-rw-r--   0 root         (0) root         (0)    22912 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mongrel2/mongrel2.c
--rw-rw-r--   0 root         (0) root         (0)       84 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mongrel2/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mono/
--rw-rw-r--   0 root         (0) root         (0)    22699 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mono/mono_plugin.c
--rw-rw-r--   0 root         (0) root         (0)     5011 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mono/uwsgi.cs
--rw-rw-r--   0 root         (0) root         (0)      595 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/mono/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/msgpack/
--rw-rw-r--   0 root         (0) root         (0)    12175 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/msgpack/msgpack.c
--rw-rw-r--   0 root         (0) root         (0)       67 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/msgpack/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/nagios/
--rw-rw-r--   0 root         (0) root         (0)     1622 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/nagios/nagios.c
--rw-rw-r--   0 root         (0) root         (0)       73 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/nagios/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/notfound/
--rw-rw-r--   0 root         (0) root         (0)      740 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/notfound/notfound.c
--rw-rw-r--   0 root         (0) root         (0)       76 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/notfound/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/objc_gc/
--rw-rw-r--   0 root         (0) root         (0)       82 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/objc_gc/objc_gc.m
--rw-rw-r--   0 root         (0) root         (0)       78 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/objc_gc/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pam/
--rw-rw-r--   0 root         (0) root         (0)     1604 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pam/pam.c
--rw-rw-r--   0 root         (0) root         (0)       73 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pam/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/php/
--rw-rw-r--   0 root         (0) root         (0)      215 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/php/common.h
--rw-rw-r--   0 root         (0) root         (0)    27317 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/php/php_plugin.c
--rw-rw-r--   0 root         (0) root         (0)      983 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/php/session.c
--rw-rw-r--   0 root         (0) root         (0)      728 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/php/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ping/
--rw-rw-r--   0 root         (0) root         (0)     1972 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ping/ping_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       74 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ping/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/psgi/
--rw-rw-r--   0 root         (0) root         (0)     2152 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/psgi/psgi.h
--rw-rw-r--   0 root         (0) root         (0)    15114 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/psgi/psgi_loader.c
--rw-rw-r--   0 root         (0) root         (0)    25070 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/psgi/psgi_plugin.c
--rw-rw-r--   0 root         (0) root         (0)     5493 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/psgi/psgi_response.c
--rw-rw-r--   0 root         (0) root         (0)    19742 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/psgi/uwsgi_plmodule.c
--rw-rw-r--   0 root         (0) root         (0)      436 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/psgi/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pty/
--rw-rw-r--   0 root         (0) root         (0)     9807 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pty/pty.c
--rw-rw-r--   0 root         (0) root         (0)      171 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pty/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pypy/
--rw-rw-r--   0 root         (0) root         (0)     1469 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pypy/README
--rw-rw-r--   0 root         (0) root         (0)    10968 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pypy/pypy_plugin.c
--rw-rw-r--   0 root         (0) root         (0)    28863 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pypy/pypy_setup.py
--rw-rw-r--   0 root         (0) root         (0)      249 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pypy/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/
--rw-rw-r--   0 root         (0) root         (0)      761 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/gil.c
--rw-rw-r--   0 root         (0) root         (0)     2185 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/profiler.c
--rw-rw-r--   0 root         (0) root         (0)     9413 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/pump_subhandler.c
--rw-rw-r--   0 root         (0) root         (0)    21847 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/pyloader.c
--rw-rw-r--   0 root         (0) root         (0)    54488 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/python_plugin.c
--rw-rw-r--   0 root         (0) root         (0)     9897 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/pyutils.c
--rw-rw-r--   0 root         (0) root         (0)     2440 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/raw.c
--rw-rw-r--   0 root         (0) root         (0)    22860 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/symimporter.c
--rw-rw-r--   0 root         (0) root         (0)     8155 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/tracebacker.c
--rw-rw-r--   0 root         (0) root         (0)    94381 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/uwsgi_pymodule.c
--rw-rw-r--   0 root         (0) root         (0)     8913 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/uwsgi_python.h
--rw-rw-r--   0 root         (0) root         (0)     2657 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/uwsgiplugin.py
--rw-rw-r--   0 root         (0) root         (0)     6789 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/web3_subhandler.c
--rw-rw-r--   0 root         (0) root         (0)    14122 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/wsgi_handlers.c
--rw-rw-r--   0 root         (0) root         (0)     4976 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/wsgi_headers.c
--rw-rw-r--   0 root         (0) root         (0)    11275 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/python/wsgi_subhandler.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pyuwsgi/
--rw-rw-r--   0 root         (0) root         (0)     1660 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pyuwsgi/pyuwsgi.c
--rw-rw-r--   0 root         (0) root         (0)      243 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/pyuwsgi/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rack/
--rw-rw-r--   0 root         (0) root         (0)    34133 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rack/rack_api.c
--rw-rw-r--   0 root         (0) root         (0)    37245 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rack/rack_plugin.c
--rw-rw-r--   0 root         (0) root         (0)      963 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rack/uwsgi_rack.h
--rw-rw-r--   0 root         (0) root         (0)     3183 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rack/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rados/
--rw-rw-r--   0 root         (0) root         (0)    18779 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rados/rados.c
--rw-rw-r--   0 root         (0) root         (0)       89 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rados/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rawrouter/
--rw-rw-r--   0 root         (0) root         (0)     9998 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rawrouter/rawrouter.c
--rw-rw-r--   0 root         (0) root         (0)      106 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rawrouter/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rbthreads/
--rw-rw-r--   0 root         (0) root         (0)     6321 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rbthreads/rbthreads.c
--rw-rw-r--   0 root         (0) root         (0)     1263 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rbthreads/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/redislog/
--rw-rw-r--   0 root         (0) root         (0)     3839 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/redislog/redislog_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       83 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/redislog/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ring/
--rw-rw-r--   0 root         (0) root         (0)    14609 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ring/ring_plugin.c
--rw-rw-r--   0 root         (0) root         (0)      642 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ring/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_access/
--rw-rw-r--   0 root         (0) root         (0)     2109 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_access/router_access.c
--rw-rw-r--   0 root         (0) root         (0)      111 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_access/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_basicauth/
--rw-rw-r--   0 root         (0) root         (0)     5126 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_basicauth/router_basicauth.c
--rw-rw-r--   0 root         (0) root         (0)      217 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_basicauth/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_cache/
--rw-rw-r--   0 root         (0) root         (0)    20078 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_cache/router_cache.c
--rw-rw-r--   0 root         (0) root         (0)       84 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_cache/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_expires/
--rw-rw-r--   0 root         (0) root         (0)     3266 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_expires/expires.c
--rw-rw-r--   0 root         (0) root         (0)       81 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_expires/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_hash/
--rw-rw-r--   0 root         (0) root         (0)     3759 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_hash/router_hash.c
--rw-rw-r--   0 root         (0) root         (0)       82 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_hash/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_http/
--rw-rw-r--   0 root         (0) root         (0)     4594 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_http/router_http.c
--rw-rw-r--   0 root         (0) root         (0)       82 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_http/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_memcached/
--rw-rw-r--   0 root         (0) root         (0)    11224 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_memcached/router_memcached.c
--rw-rw-r--   0 root         (0) root         (0)       92 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_memcached/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_metrics/
--rw-rw-r--   0 root         (0) root         (0)     4102 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_metrics/plugin.c
--rw-rw-r--   0 root         (0) root         (0)       80 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_metrics/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_radius/
--rw-rw-r--   0 root         (0) root         (0)     8199 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_radius/radius.c
--rw-rw-r--   0 root         (0) root         (0)       79 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_radius/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_redirect/
--rw-rw-r--   0 root         (0) root         (0)     2580 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_redirect/router_redirect.c
--rw-rw-r--   0 root         (0) root         (0)       90 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_redirect/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_redis/
--rw-rw-r--   0 root         (0) root         (0)    11248 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_redis/router_redis.c
--rw-rw-r--   0 root         (0) root         (0)       84 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_redis/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_rewrite/
--rw-rw-r--   0 root         (0) root         (0)     2684 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_rewrite/router_rewrite.c
--rw-rw-r--   0 root         (0) root         (0)       88 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_rewrite/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_spnego/
--rw-rw-r--   0 root         (0) root         (0)     7877 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_spnego/router_spnego.c
--rw-rw-r--   0 root         (0) root         (0)      217 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_spnego/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_static/
--rw-rw-r--   0 root         (0) root         (0)    11016 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_static/router_static.c
--rw-rw-r--   0 root         (0) root         (0)       86 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_static/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_uwsgi/
--rw-rw-r--   0 root         (0) root         (0)     5147 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_uwsgi/router_uwsgi.c
--rw-rw-r--   0 root         (0) root         (0)       84 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_uwsgi/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_xmldir/
--rw-rw-r--   0 root         (0) root         (0)     6212 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_xmldir/router_xmldir.c
--rw-rw-r--   0 root         (0) root         (0)       85 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/router_xmldir/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rpc/
--rw-rw-r--   0 root         (0) root         (0)    21047 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rpc/rpc_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       73 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rpc/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rrdtool/
--rw-rw-r--   0 root         (0) root         (0)     4827 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rrdtool/rrdtool.c
--rw-rw-r--   0 root         (0) root         (0)       75 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rrdtool/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rsyslog/
--rw-rw-r--   0 root         (0) root         (0)     2941 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rsyslog/rsyslog_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       81 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/rsyslog/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ruby19/
--rw-rw-r--   0 root         (0) root         (0)     1868 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ruby19/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/servlet/
--rw-rw-r--   0 root         (0) root         (0)     2577 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/servlet/servlet_plugin.c
--rw-rw-r--   0 root         (0) root         (0)    12278 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/servlet/uwsgi_servlet.java
--rw-rw-r--   0 root         (0) root         (0)      327 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/servlet/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/signal/
--rw-rw-r--   0 root         (0) root         (0)      639 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/signal/signal_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       80 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/signal/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/spooler/
--rw-rw-r--   0 root         (0) root         (0)     1622 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/spooler/spooler_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       81 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/spooler/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/sqlite3/
--rw-rw-r--   0 root         (0) root         (0)     2221 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/sqlite3/plugin.c
--rw-rw-r--   0 root         (0) root         (0)       85 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/sqlite3/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ssi/
--rw-rw-r--   0 root         (0) root         (0)    12876 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ssi/ssi.c
--rw-rw-r--   0 root         (0) root         (0)       66 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ssi/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/sslrouter/
--rw-rw-r--   0 root         (0) root         (0)    14303 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/sslrouter/sslrouter.c
--rw-rw-r--   0 root         (0) root         (0)      106 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/sslrouter/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stackless/
--rw-rw-r--   0 root         (0) root         (0)     2917 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stackless/stackless.c
--rw-rw-r--   0 root         (0) root         (0)      197 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stackless/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_file/
--rw-rw-r--   0 root         (0) root         (0)     1988 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_file/plugin.c
--rw-rw-r--   0 root         (0) root         (0)       84 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_file/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_mongodb/
--rw-rw-r--   0 root         (0) root         (0)      372 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_mongodb/plugin.c
--rw-rw-r--   0 root         (0) root         (0)     1713 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_mongodb/stats_pusher_mongodb.cc
--rw-rw-r--   0 root         (0) root         (0)      326 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_mongodb/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_socket/
--rw-rw-r--   0 root         (0) root         (0)     3092 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_socket/plugin.c
--rw-rw-r--   0 root         (0) root         (0)       86 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_socket/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_statsd/
--rw-rw-r--   0 root         (0) root         (0)     3199 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_statsd/plugin.c
--rw-rw-r--   0 root         (0) root         (0)       86 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/stats_pusher_statsd/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/symcall/
--rw-rw-r--   0 root         (0) root         (0)     6471 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/symcall/symcall_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       81 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/symcall/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/syslog/
--rw-rw-r--   0 root         (0) root         (0)     2685 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/syslog/syslog_plugin.c
--rw-rw-r--   0 root         (0) root         (0)       79 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/syslog/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/systemd_logger/
--rw-rw-r--   0 root         (0) root         (0)      753 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/systemd_logger/systemd_logger.c
--rw-rw-r--   0 root         (0) root         (0)      241 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/systemd_logger/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/tornado/
--rw-rw-r--   0 root         (0) root         (0)    12664 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/tornado/tornado.c
--rw-rw-r--   0 root         (0) root         (0)      193 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/tornado/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_chunked/
--rw-rw-r--   0 root         (0) root         (0)     1475 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_chunked/chunked.c
--rw-rw-r--   0 root         (0) root         (0)       89 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_chunked/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_gzip/
--rw-rw-r--   0 root         (0) root         (0)     2168 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_gzip/gzip.c
--rw-rw-r--   0 root         (0) root         (0)       83 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_gzip/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_offload/
--rw-rw-r--   0 root         (0) root         (0)     3974 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_offload/offload.c
--rw-rw-r--   0 root         (0) root         (0)       89 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_offload/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_template/
--rw-rw-r--   0 root         (0) root         (0)     1393 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_template/tt.c
--rw-rw-r--   0 root         (0) root         (0)       85 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_template/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_tofile/
--rw-rw-r--   0 root         (0) root         (0)     3582 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_tofile/tofile.c
--rw-rw-r--   0 root         (0) root         (0)       87 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_tofile/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_toupper/
--rw-rw-r--   0 root         (0) root         (0)      830 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_toupper/toupper.c
--rw-rw-r--   0 root         (0) root         (0)       89 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/transformation_toupper/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/tuntap/
--rw-rw-r--   0 root         (0) root         (0)    10117 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/tuntap/common.c
--rw-rw-r--   0 root         (0) root         (0)     3593 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/tuntap/common.h
--rw-rw-r--   0 root         (0) root         (0)    11771 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/tuntap/firewall.c
--rw-rw-r--   0 root         (0) root         (0)    18448 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/tuntap/tuntap.c
--rw-rw-r--   0 root         (0) root         (0)       83 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/tuntap/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ugreen/
--rw-rw-r--   0 root         (0) root         (0)     3213 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ugreen/ugreen.c
--rw-rw-r--   0 root         (0) root         (0)       73 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/ugreen/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/v8/
--rw-rw-r--   0 root         (0) root         (0)     1049 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/v8/plugin.c
--rw-rw-r--   0 root         (0) root         (0)      326 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/v8/uwsgiplugin.py
--rw-rw-r--   0 root         (0) root         (0)     4621 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/v8/v8_commonjs.cc
--rw-rw-r--   0 root         (0) root         (0)     7053 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/v8/v8_jsgi.cc
--rw-rw-r--   0 root         (0) root         (0)    10737 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/v8/v8_uwsgi.cc
--rw-rw-r--   0 root         (0) root         (0)      937 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/v8/v8_uwsgi.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/webdav/
--rw-rw-r--   0 root         (0) root         (0)      189 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/webdav/uwsgiplugin.py
--rw-rw-r--   0 root         (0) root         (0)    51108 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/webdav/webdav.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/xattr/
--rw-rw-r--   0 root         (0) root         (0)       63 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/xattr/uwsgiplugin.py
--rw-rw-r--   0 root         (0) root         (0)     2531 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/xattr/xattr.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/xslt/
--rw-rw-r--   0 root         (0) root         (0)      185 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/xslt/uwsgiplugin.py
--rw-rw-r--   0 root         (0) root         (0)    15063 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/xslt/xslt.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/zabbix/
--rw-rw-r--   0 root         (0) root         (0)     6255 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/zabbix/plugin.c
--rw-rw-r--   0 root         (0) root         (0)       73 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/zabbix/uwsgiplugin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/zergpool/
--rw-rw-r--   0 root         (0) root         (0)       77 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/zergpool/uwsgiplugin.py
--rw-rw-r--   0 root         (0) root         (0)     3736 2014-10-26 04:30:44.000000 uwsgi-2.0.8/plugins/zergpool/zergpool.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/proto/
--rw-rw-r--   0 root         (0) root         (0)    12475 2014-10-26 04:30:44.000000 uwsgi-2.0.8/proto/base.c
--rw-rw-r--   0 root         (0) root         (0)    11986 2014-10-26 04:30:44.000000 uwsgi-2.0.8/proto/fastcgi.c
--rw-rw-r--   0 root         (0) root         (0)    22670 2014-10-26 04:30:44.000000 uwsgi-2.0.8/proto/http.c
--rw-rw-r--   0 root         (0) root         (0)     4090 2014-10-26 04:30:44.000000 uwsgi-2.0.8/proto/puwsgi.c
--rw-rw-r--   0 root         (0) root         (0)     4423 2014-10-26 04:30:44.000000 uwsgi-2.0.8/proto/scgi.c
--rw-rw-r--   0 root         (0) root         (0)     7943 2014-10-26 04:30:44.000000 uwsgi-2.0.8/proto/uwsgi.c
--rw-rw-r--   0 root         (0) root         (0)     2824 2014-10-26 04:30:44.000000 uwsgi-2.0.8/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/
--rw-rw-r--   0 root         (0) root         (0)      600 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/cachebitmap.ini
--rw-rw-r--   0 root         (0) root         (0)     5698 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/cachebitmap.py
--rw-rw-r--   0 root         (0) root         (0)      716 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/cachetest.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/clojure/
--rw-rw-r--   0 root         (0) root         (0)      292 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/clojure/myapp.clj
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/core/
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/core/apps/
--rw-rw-r--   0 root         (0) root         (0)      168 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/core/apps/read_body_and_send.pl
--rw-rw-r--   0 root         (0) root         (0)      789 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/core/read_body_and_send.pl
--rw-rw-r--   0 root         (0) root         (0)     1583 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/core/url_sanitize.pl
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/go/
--rw-rw-r--   0 root         (0) root         (0)     1554 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/go/cachetest.go
--rw-rw-r--   0 root         (0) root         (0)     1097 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/go/complextest.go
--rw-rw-r--   0 root         (0) root         (0)     1003 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/go/uploadtest.go
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/java/
--rw-rw-r--   0 root         (0) root         (0)      396 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/java/rpc.java
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/lua/
--rw-rw-r--   0 root         (0) root         (0)      565 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/lua/basic.lua
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/mono/
--rw-rw-r--   0 root         (0) root         (0)      130 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/mono/cache.aspx
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/apps/
--rw-rw-r--   0 root         (0) root         (0)      309 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/apps/input_with_offset.pl
--rw-rw-r--   0 root         (0) root         (0)     1720 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/test.psgi
--rw-rw-r--   0 root         (0) root         (0)     1894 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/test_benchmark.pl
--rw-rw-r--   0 root         (0) root         (0)      100 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/test_hello.psgi
--rw-rw-r--   0 root         (0) root         (0)     1828 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/test_input_with_offset.pl
--rw-rw-r--   0 root         (0) root         (0)     1303 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/test_post.psgi
--rw-rw-r--   0 root         (0) root         (0)      535 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/test_sleepy.psgi
--rw-rw-r--   0 root         (0) root         (0)     1370 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/perl/test_streaming.psgi
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/pypy/
--rw-rw-r--   0 root         (0) root         (0)     1191 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/pypy/t_continulet1.py
--rw-rw-r--   0 root         (0) root         (0)     1403 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/pypy/t_continulet2.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/python/
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/python/manage_script_name/
--rw-rw-r--   0 root         (0) root         (0)      232 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/python/manage_script_name/manage_script_name_test.ini
--rw-rw-r--   0 root         (0) root         (0)     1392 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/python/manage_script_name/test_manage_script_name.py
--rw-rw-r--   0 root         (0) root         (0)      130 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/python/manage_script_name/useless_app.py
--rw-rw-r--   0 root         (0) root         (0)      186 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/python/testba.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/
--rw-rw-r--   0 root         (0) root         (0)      310 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/README.md
--rw-rw-r--   0 root         (0) root         (0)      258 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/config.ini
--rw-rw-r--   0 root         (0) root         (0)      291 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/project.clj
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/src/
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/src/uwsgi/
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/src/uwsgi/ring/
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/
--rw-rw-r--   0 root         (0) root         (0)      857 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/app.clj
--rw-rw-r--   0 root         (0) root         (0)     1122 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/basic.clj
--rw-rw-r--   0 root         (0) root         (0)      595 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/body.clj
--rw-rw-r--   0 root         (0) root         (0)      301 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/simple.clj
--rw-rw-r--   0 root         (0) root         (0)      560 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/upload.clj
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/routing/
--rw-rw-r--   0 root         (0) root         (0)     1811 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/routing/auth.ini
--rw-rw-r--   0 root         (0) root         (0)     1018 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/routing/errorlimiter.ini
--rw-rw-r--   0 root         (0) root         (0)      674 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/routing/limiter.ini
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/webdav/
--rw-rw-r--   0 root         (0) root         (0)      459 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/webdav/carddav.ini
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/xslt/
--rw-rw-r--   0 root         (0) root         (0)      436 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/xslt/cd.xml
--rw-rw-r--   0 root         (0) root         (0)      675 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/xslt/cd.xml.xslt
--rw-rw-r--   0 root         (0) root         (0)      214 2014-10-26 04:30:44.000000 uwsgi-2.0.8/t/xslt/routex.ini
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/
--rw-rw-r--   0 root         (0) root         (0)     1013 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/Responder.pm
--rw-rw-r--   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       55 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/badthread.py
--rw-rw-r--   0 root         (0) root         (0)      584 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/badwrites.py
--rw-rw-r--   0 root         (0) root         (0)      189 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/cpubound_async.py
--rw-rw-r--   0 root         (0) root         (0)      379 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/cpubound_green.py
--rw-rw-r--   0 root         (0) root         (0)      319 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/cpubound_stackless.py
--rw-rw-r--   0 root         (0) root         (0)     3604 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/decoratortest.py
--rw-rw-r--   0 root         (0) root         (0)      403 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/fileserve_async.py
--rw-rw-r--   0 root         (0) root         (0)      407 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/gevent_spool.py
--rw-rw-r--   0 root         (0) root         (0)      525 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/grunter.py
--rw-rw-r--   0 root         (0) root         (0)      818 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/iobound_async.py
--rw-rw-r--   0 root         (0) root         (0)     1085 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/iobound_async_unix.py
--rw-rw-r--   0 root         (0) root         (0)      862 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/iobound_green.py
--rw-rw-r--   0 root         (0) root         (0)      259 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/logger.py
--rw-rw-r--   0 root         (0) root         (0)      473 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/mako_ugreen.py
--rw-rw-r--   0 root         (0) root         (0)      684 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/mulefunc.py
--rw-rw-r--   0 root         (0) root         (0)      223 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/multiapp.txt
--rw-rw-r--   0 root         (0) root         (0)      382 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/myadmin.py
--rw-rw-r--   0 root         (0) root         (0)     1230 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/pgbound_async.py
--rw-rw-r--   0 root         (0) root         (0)      528 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/picazzo.py
--rw-rw-r--   0 root         (0) root         (0)      981 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/psycogreen_green.py
--rw-rw-r--   0 root         (0) root         (0)     1108 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/psycopg2_green.py
--rw-rw-r--   0 root         (0) root         (0)      196 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/pump.py
--rw-rw-r--   0 root         (0) root         (0)     1342 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/queue.py
--rw-rw-r--   0 root         (0) root         (0)      158 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/refcount.py
--rw-rw-r--   0 root         (0) root         (0)      425 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/rpc.lua
--rw-rw-r--   0 root         (0) root         (0)      128 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/rpc.py
--rw-rw-r--   0 root         (0) root         (0)      304 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/runningthread.py
--rw-rw-r--   0 root         (0) root         (0)      317 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/sendchunked.py
--rw-rw-r--   0 root         (0) root         (0)      372 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/sharedarea.py
--rw-rw-r--   0 root         (0) root         (0)      278 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/sig.lua
--rw-rw-r--   0 root         (0) root         (0)      997 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/signals.py
--rw-rw-r--   0 root         (0) root         (0)      646 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/sigwait.py
--rw-rw-r--   0 root         (0) root         (0)      290 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/sleeping_async.py
--rw-rw-r--   0 root         (0) root         (0)      472 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/sleeping_green.py
--rw-rw-r--   0 root         (0) root         (0)      353 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/sleepthreadasync.py
--rw-rw-r--   0 root         (0) root         (0)      229 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/slow.py
--rw-rw-r--   0 root         (0) root         (0)      385 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/spoolme.py
--rw-rw-r--   0 root         (0) root         (0)      370 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/staticfile.py
--rw-rw-r--   0 root         (0) root         (0)      378 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/streamer.psgi
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/t/
--rw-rw-r--   0 root         (0) root         (0)     1857 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/t/static.pl
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/templates/
--rw-rw-r--   0 root         (0) root         (0)     1273 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/templates/queue.html
--rw-rw-r--   0 root         (0) root         (0)     4874 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/testapp.py
--rw-rw-r--   0 root         (0) root         (0)      887 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/testgevent.py
--rw-rw-r--   0 root         (0) root         (0)      322 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/testpy3.py
--rw-rw-r--   0 root         (0) root         (0)      397 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/testsignals.py
--rw-rw-r--   0 root         (0) root         (0)      679 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/threads.py
--rwxrwxr-x   0 root         (0) root         (0)     3076 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/travis.sh
--rw-rw-r--   0 root         (0) root         (0)     1631 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/ugevent.py
--rw-rw-r--   0 root         (0) root         (0)      236 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/web3.py
--rw-rw-r--   0 root         (0) root         (0)     2119 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/websockets.py
--rw-rw-r--   0 root         (0) root         (0)     3764 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/websockets_chat.pl
--rw-rw-r--   0 root         (0) root         (0)     2622 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/websockets_chat.py
--rw-rw-r--   0 root         (0) root         (0)     3165 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/websockets_chat_async.py
--rw-rw-r--   0 root         (0) root         (0)     4294 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/websockets_chat_asyncio.py
--rw-rw-r--   0 root         (0) root         (0)     1867 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/websockets_echo.lua
--rw-rw-r--   0 root         (0) root         (0)     1824 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/websockets_echo.pl
--rw-rw-r--   0 root         (0) root         (0)     1787 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/websockets_echo.py
--rw-rw-r--   0 root         (0) root         (0)     1856 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/websockets_echo.ru
--rw-rw-r--   0 root         (0) root         (0)      109 2014-10-26 04:30:44.000000 uwsgi-2.0.8/tests/werkzeug.py
--rw-rw-r--   0 root         (0) root         (0)      557 2014-10-26 04:30:44.000000 uwsgi-2.0.8/uwsgi.gemspec
--rw-rw-r--   0 root         (0) root         (0)   124329 2014-10-26 04:30:44.000000 uwsgi-2.0.8/uwsgi.h
--rw-rw-r--   0 root         (0) root         (0)      134 2014-10-26 04:30:44.000000 uwsgi-2.0.8/uwsgi_main.c
--rw-rw-r--   0 root         (0) root         (0)    60000 2014-10-26 04:30:44.000000 uwsgi-2.0.8/uwsgiconfig.py
--rw-rw-r--   0 root         (0) root         (0)    10206 2014-10-26 04:30:44.000000 uwsgi-2.0.8/uwsgidecorators.py
--rw-rw-r--   0 root         (0) root         (0)     2839 2014-10-26 04:30:44.000000 uwsgi-2.0.8/uwsgidsl.rb
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/valgrind/
--rw-rw-r--   0 root         (0) root         (0)      316 2014-10-26 04:30:44.000000 uwsgi-2.0.8/valgrind/README
--rwxrwxr-x   0 root         (0) root         (0)      430 2014-10-26 04:30:44.000000 uwsgi-2.0.8/valgrind/valgrind-generate-sups.sh
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vassals/
--rw-rw-r--   0 root         (0) root         (0)      319 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vassals/broodlord.ini
--rw-rw-r--   0 root         (0) root         (0)      175 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vassals/cc.ini
--rw-rw-r--   0 root         (0) root         (0)      490 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vassals/multi.xml
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask001/
--rw-rw-r--   0 root         (0) root         (0)      102 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask001/app1.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask002/
--rw-rw-r--   0 root         (0) root         (0)      111 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask002/app2.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask003/
--rw-rw-r--   0 root         (0) root         (0)      107 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask003/app3.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask004/
--rw-rw-r--   0 root         (0) root         (0)      107 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask004/app4.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask005/
--rw-rw-r--   0 root         (0) root         (0)      107 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/flask005/app5.py
--rw-rw-r--   0 root         (0) root         (0)      742 2014-10-26 04:30:44.000000 uwsgi-2.0.8/vhosttest/nginx.conf
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/
+-rw-rw-r--   0 root         (0) root         (0)      178 2014-12-29 09:07:07.000000 uwsgi-2.0.9/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)     1881 2014-12-29 09:07:07.000000 uwsgi-2.0.9/.travis.yml
+-rw-rw-r--   0 root         (0) root         (0)      717 2014-12-29 09:07:07.000000 uwsgi-2.0.9/CONTRIBUTORS
+-rw-rw-r--   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/INSTALL
+-rw-rw-r--   0 root         (0) root         (0)    18628 2014-12-29 09:07:07.000000 uwsgi-2.0.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      261 2014-12-29 09:07:07.000000 uwsgi-2.0.9/Makefile
+-rw-rw-r--   0 root         (0) root         (0)      148 2014-12-29 09:07:07.000000 uwsgi-2.0.9/README
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/apache2/
+-rw-rw-r--   0 root         (0) root         (0)    24733 2014-12-29 09:07:07.000000 uwsgi-2.0.9/apache2/mod_Ruwsgi.c
+-rw-rw-r--   0 root         (0) root         (0)    15632 2014-12-29 09:07:07.000000 uwsgi-2.0.9/apache2/mod_proxy_uwsgi.c
+-rw-rw-r--   0 root         (0) root         (0)    22714 2014-12-29 09:07:07.000000 uwsgi-2.0.9/apache2/mod_uwsgi.c
+-rw-rw-r--   0 root         (0) root         (0)      190 2014-12-29 09:07:07.000000 uwsgi-2.0.9/attach.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/bin/
+-rw-rw-r--   0 root         (0) root         (0)      113 2014-12-29 09:07:07.000000 uwsgi-2.0.9/bin/uwsgi
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/
+-rw-rw-r--   0 root         (0) root         (0)      243 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/all.ini
+-rw-rw-r--   0 root         (0) root         (0)       61 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/asyncio.ini
+-rw-rw-r--   0 root         (0) root         (0)      922 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/base.ini
+-rw-rw-r--   0 root         (0) root         (0)       41 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/cgi.ini
+-rw-rw-r--   0 root         (0) root         (0)       61 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/core.ini
+-rw-rw-r--   0 root         (0) root         (0)       49 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/coroae.ini
+-rw-rw-r--   0 root         (0) root         (0)      170 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/coverity.ini
+-rw-rw-r--   0 root         (0) root         (0)       51 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/default.ini
+-rw-rw-r--   0 root         (0) root         (0)       93 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/django.ini
+-rw-rw-r--   0 root         (0) root         (0)       89 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/embedded.ini
+-rw-rw-r--   0 root         (0) root         (0)       44 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/erlang.ini
+-rw-rw-r--   0 root         (0) root         (0)       43 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/gccgo.ini
+-rw-rw-r--   0 root         (0) root         (0)       51 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/gevent.ini
+-rw-rw-r--   0 root         (0) root         (0)       47 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/glusterfs.ini
+-rw-rw-r--   0 root         (0) root         (0)       44 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/gridfs.ini
+-rw-rw-r--   0 root         (0) root         (0)       47 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/jwsgi.ini
+-rw-rw-r--   0 root         (0) root         (0)       95 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/lib.ini
+-rw-rw-r--   0 root         (0) root         (0)       41 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/lua.ini
+-rw-rw-r--   0 root         (0) root         (0)       52 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/luap.ini
+-rw-rw-r--   0 root         (0) root         (0)      390 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/minimal.ini
+-rw-rw-r--   0 root         (0) root         (0)      128 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/modular.ini
+-rw-rw-r--   0 root         (0) root         (0)       42 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/mono.ini
+-rw-rw-r--   0 root         (0) root         (0)       37 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/nolang.ini
+-rw-rw-r--   0 root         (0) root         (0)       70 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/package.ini
+-rw-rw-r--   0 root         (0) root         (0)       41 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/php.ini
+-rw-rw-r--   0 root         (0) root         (0)       45 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/plonly.ini
+-rw-rw-r--   0 root         (0) root         (0)      408 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/ppa.ini
+-rw-rw-r--   0 root         (0) root         (0)       42 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/psgi.ini
+-rw-rw-r--   0 root         (0) root         (0)       58 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/pyerl.ini
+-rw-rw-r--   0 root         (0) root         (0)       48 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/pylua.ini
+-rw-rw-r--   0 root         (0) root         (0)       47 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/pyonly.ini
+-rw-rw-r--   0 root         (0) root         (0)       42 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/pypy.ini
+-rw-rw-r--   0 root         (0) root         (0)       45 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/pypyonly.ini
+-rw-rw-r--   0 root         (0) root         (0)       86 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/pyring.ini
+-rw-rw-r--   0 root         (0) root         (0)       92 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/pyuwsgi.ini
+-rw-rw-r--   0 root         (0) root         (0)       42 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/rack.ini
+-rw-rw-r--   0 root         (0) root         (0)       43 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/rados.ini
+-rw-rw-r--   0 root         (0) root         (0)       45 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/rbonly.ini
+-rw-rw-r--   0 root         (0) root         (0)       46 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/ring.ini
+-rw-rw-r--   0 root         (0) root         (0)       58 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/ruby2.ini
+-rw-rw-r--   0 root         (0) root         (0)       49 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/servlet.ini
+-rw-rw-r--   0 root         (0) root         (0)       37 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/travis.ini
+-rw-rw-r--   0 root         (0) root         (0)      432 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/unbit.ini
+-rw-rw-r--   0 root         (0) root         (0)      108 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/unbitstaff.ini
+-rw-rw-r--   0 root         (0) root         (0)      396 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/uwsgi.it.ini
+-rw-rw-r--   0 root         (0) root         (0)       40 2014-12-29 09:07:07.000000 uwsgi-2.0.9/buildconf/v8.ini
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/
+-rw-rw-r--   0 root         (0) root         (0)     3490 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/Uwsgi.pm
+-rw-rw-r--   0 root         (0) root         (0)      657 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/binder.pl
+-rw-rw-r--   0 root         (0) root         (0)     1629 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/centos_init_script
+-rw-rw-r--   0 root         (0) root         (0)     1586 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/cgi_python.c
+-rw-rw-r--   0 root         (0) root         (0)      450 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/cryptologger.rb
+-rw-rw-r--   0 root         (0) root         (0)     3311 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/emperormon.ru
+-rw-rw-r--   0 root         (0) root         (0)      101 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/fdconf.pl
+-rw-rw-r--   0 root         (0) root         (0)     1003 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/graphite_uwsgi.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/launchd/
+-rw-rw-r--   0 root         (0) root         (0)      478 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/launchd/it.unbit.uwsgi.emperor.plist
+-rw-rw-r--   0 root         (0) root         (0)      544 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/launchd/it.unbit.uwsgi.plist
+-rw-rw-r--   0 root         (0) root         (0)      513 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/loadapp.pl
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/pypy/
+-rw-rw-r--   0 root         (0) root         (0)     1768 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/pypy/uwsgi_pypy_greenlets.py
+-rw-rw-r--   0 root         (0) root         (0)      331 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/pyuwsgi.py
+-rw-rw-r--   0 root         (0) root         (0)     2560 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/runuwsgi.py
+-rw-rw-r--   0 root         (0) root         (0)      814 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/securesubscribe.pl
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/spoolqueue/
+-rw-rw-r--   0 root         (0) root         (0)      183 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/spoolqueue/producer.py
+-rw-rw-r--   0 root         (0) root         (0)      191 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/spoolqueue/tasks.py
+-rw-rw-r--   0 root         (0) root         (0)      958 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/spoolqueue/tasksconsumer.py
+-rw-rw-r--   0 root         (0) root         (0)      445 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/subscribe.pl
+-rw-rw-r--   0 root         (0) root         (0)     4043 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/twuwsgi.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/upstart/
+-rw-rw-r--   0 root         (0) root         (0)      245 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/upstart/emperor.conf
+-rw-rw-r--   0 root         (0) root         (0)      344 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/upstart/uwsgi.conf
+-rw-rw-r--   0 root         (0) root         (0)      245 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/upython
+-rw-rw-r--   0 root         (0) root         (0)    10028 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/urack.rb
+-rw-rw-r--   0 root         (0) root         (0)     4587 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/uwsgi-cache-monitor.py
+-rw-rw-r--   0 root         (0) root         (0)      693 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/uwsgi.erl
+-rw-rw-r--   0 root         (0) root         (0)     6765 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/uwsgi.java
+-rw-rw-r--   0 root         (0) root         (0)     3563 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/uwsgi.rb
+-rw-rw-r--   0 root         (0) root         (0)     1780 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/uwsgi_client.c
+-rw-rw-r--   0 root         (0) root         (0)     1779 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/uwsgi_dynamic_client.c
+-rw-rw-r--   0 root         (0) root         (0)     2783 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/uwsgisubscribers.ru
+-rw-rw-r--   0 root         (0) root         (0)      411 2014-12-29 09:07:07.000000 uwsgi-2.0.9/contrib/xinetd_uwsgi
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/
+-rw-rw-r--   0 root         (0) root         (0)    11552 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/alarm.c
+-rw-rw-r--   0 root         (0) root         (0)    15214 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/async.c
+-rw-rw-r--   0 root         (0) root         (0)    12177 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/buffer.c
+-rw-rw-r--   0 root         (0) root         (0)    64704 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/cache.c
+-rw-rw-r--   0 root         (0) root         (0)     5462 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/chunked.c
+-rw-rw-r--   0 root         (0) root         (0)       14 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/clang_fake.c
+-rw-rw-r--   0 root         (0) root         (0)      907 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/clock.c
+-rw-rw-r--   0 root         (0) root         (0)    21879 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/config.c
+-rw-rw-r--   0 root         (0) root         (0)     1601 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/cookie.c
+-rw-rw-r--   0 root         (0) root         (0)     8454 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/cron.c
+-rw-rw-r--   0 root         (0) root         (0)    14989 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/daemons.c
+-rw-rw-r--   0 root         (0) root         (0)    63020 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/emperor.c
+-rw-rw-r--   0 root         (0) root         (0)     3055 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/errors.c
+-rw-rw-r--   0 root         (0) root         (0)    28826 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/event.c
+-rw-rw-r--   0 root         (0) root         (0)    16778 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/exceptions.c
+-rw-rw-r--   0 root         (0) root         (0)     4358 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/fifo.c
+-rw-rw-r--   0 root         (0) root         (0)     4427 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/fsmon.c
+-rw-rw-r--   0 root         (0) root         (0)     4713 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/gateway.c
+-rw-rw-r--   0 root         (0) root         (0)     2365 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/hash.c
+-rw-rw-r--   0 root         (0) root         (0)    16123 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/hooks.c
+-rw-rw-r--   0 root         (0) root         (0)     2820 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/ini.c
+-rw-rw-r--   0 root         (0) root         (0)    14071 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/init.c
+-rw-rw-r--   0 root         (0) root         (0)    34521 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/io.c
+-rw-rw-r--   0 root         (0) root         (0)     8700 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/json.c
+-rw-rw-r--   0 root         (0) root         (0)    35763 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/legion.c
+-rw-rw-r--   0 root         (0) root         (0)    20134 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/lock.c
+-rw-rw-r--   0 root         (0) root         (0)    55355 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/logging.c
+-rw-rw-r--   0 root         (0) root         (0)     3469 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/loop.c
+-rw-rw-r--   0 root         (0) root         (0)    31292 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/master.c
+-rw-rw-r--   0 root         (0) root         (0)    11233 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/master_checks.c
+-rw-rw-r--   0 root         (0) root         (0)     7616 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/master_events.c
+-rw-rw-r--   0 root         (0) root         (0)    49038 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/master_utils.c
+-rw-rw-r--   0 root         (0) root         (0)    31489 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/metrics.c
+-rw-rw-r--   0 root         (0) root         (0)     6147 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/mount.c
+-rw-rw-r--   0 root         (0) root         (0)    11749 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/mule.c
+-rw-rw-r--   0 root         (0) root         (0)     2803 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/notify.c
+-rw-rw-r--   0 root         (0) root         (0)    17328 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/offload.c
+-rw-rw-r--   0 root         (0) root         (0)     7702 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/plugins.c
+-rw-rw-r--   0 root         (0) root         (0)     2662 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/plugins_builder.c
+-rw-rw-r--   0 root         (0) root         (0)     2813 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/progress.c
+-rw-rw-r--   0 root         (0) root         (0)    30720 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/protocol.c
+-rw-rw-r--   0 root         (0) root         (0)     1128 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/querystring.c
+-rw-rw-r--   0 root         (0) root         (0)     4452 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/queue.c
+-rw-rw-r--   0 root         (0) root         (0)     7567 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/rb_timers.c
+-rw-rw-r--   0 root         (0) root         (0)    20712 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/reader.c
+-rw-rw-r--   0 root         (0) root         (0)     2491 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/regexp.c
+-rw-rw-r--   0 root         (0) root         (0)    69503 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/routing.c
+-rw-rw-r--   0 root         (0) root         (0)     5052 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/rpc.c
+-rw-rw-r--   0 root         (0) root         (0)     2555 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/sendfile.c
+-rw-rw-r--   0 root         (0) root         (0)     4108 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/setup_utils.c
+-rw-rw-r--   0 root         (0) root         (0)    12712 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/sharedarea.c
+-rw-rw-r--   0 root         (0) root         (0)    13541 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/signal.c
+-rw-rw-r--   0 root         (0) root         (0)      214 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/skel.c
+-rw-rw-r--   0 root         (0) root         (0)     9561 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/snmp.c
+-rw-rw-r--   0 root         (0) root         (0)    50465 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/socket.c
+-rw-rw-r--   0 root         (0) root         (0)    16524 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/spooler.c
+-rw-rw-r--   0 root         (0) root         (0)    21462 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/ssl.c
+-rw-rw-r--   0 root         (0) root         (0)    18218 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/static.c
+-rw-rw-r--   0 root         (0) root         (0)    14340 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/stats.c
+-rw-rw-r--   0 root         (0) root         (0)     1191 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/storage.c
+-rw-rw-r--   0 root         (0) root         (0)     9867 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/strings.c
+-rw-rw-r--   0 root         (0) root         (0)    30989 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/subscription.c
+-rw-rw-r--   0 root         (0) root         (0)     1187 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/timebomb.c
+-rw-rw-r--   0 root         (0) root         (0)     3839 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/transformations.c
+-rw-rw-r--   0 root         (0) root         (0)   100692 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/utils.c
+-rw-rw-r--   0 root         (0) root         (0)   210952 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/uwsgi.c
+-rw-rw-r--   0 root         (0) root         (0)    13930 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/websockets.c
+-rw-rw-r--   0 root         (0) root         (0)    23183 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/writer.c
+-rw-rw-r--   0 root         (0) root         (0)     6491 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/xmlconf.c
+-rw-rw-r--   0 root         (0) root         (0)     5035 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/yaml.c
+-rw-rw-r--   0 root         (0) root         (0)     2043 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/zeus.c
+-rw-rw-r--   0 root         (0) root         (0)     4420 2014-12-29 09:07:07.000000 uwsgi-2.0.9/core/zlib.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/
+-rw-rw-r--   0 root         (0) root         (0)      128 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/bootstrap.py
+-rw-rw-r--   0 root         (0) root         (0)       91 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/bootstrap2.py
+-rw-rw-r--   0 root         (0) root         (0)      186 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/bootstrap3.py
+-rw-rw-r--   0 root         (0) root         (0)       80 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/bootstrap4.py
+-rw-rw-r--   0 root         (0) root         (0)       46 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/bootstrap5.py
+-rw-rw-r--   0 root         (0) root         (0)      227 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/config.lua
+-rw-rw-r--   0 root         (0) root         (0)      195 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/config.ru
+-rw-rw-r--   0 root         (0) root         (0)      530 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/config17.ru
+-rw-rw-r--   0 root         (0) root         (0)      198 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/config2.lua
+-rw-rw-r--   0 root         (0) root         (0)       77 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/config2.ru
+-rw-rw-r--   0 root         (0) root         (0)     1120 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/config30.ru
+-rw-rw-r--   0 root         (0) root         (0)     1803 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/corostream.pl
+-rw-rw-r--   0 root         (0) root         (0)       27 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/debug.ini
+-rw-rw-r--   0 root         (0) root         (0)      739 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/fibers.ru
+-rw-rw-r--   0 root         (0) root         (0)      125 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/fibers.yml
+-rw-rw-r--   0 root         (0) root         (0)      497 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/flaskpost.py
+-rw-rw-r--   0 root         (0) root         (0)      418 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/heavytest.ini
+-rw-rw-r--   0 root         (0) root         (0)      530 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/heavytest.py
+-rw-rw-r--   0 root         (0) root         (0)      755 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/info_uwsgi.php
+-rw-rw-r--   0 root         (0) root         (0)      678 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/logic.ini
+-rw-rw-r--   0 root         (0) root         (0)      389 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/mega.xml
+-rw-rw-r--   0 root         (0) root         (0)      629 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/mjpeg_stream.py
+-rw-rw-r--   0 root         (0) root         (0)      373 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/mojoapp.pl
+-rw-rw-r--   0 root         (0) root         (0)      461 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/multi.ini
+-rw-rw-r--   0 root         (0) root         (0)     1075 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/multi.xml
+-rw-rw-r--   0 root         (0) root         (0)      573 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/multiapp.py
+-rw-rw-r--   0 root         (0) root         (0)      424 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/protected.ini
+-rw-rw-r--   0 root         (0) root         (0)      582 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/router.lua
+-rw-rw-r--   0 root         (0) root         (0)      831 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/simple_app.py
+-rw-rw-r--   0 root         (0) root         (0)      319 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/simple_app_wsgi2.py
+-rw-rw-r--   0 root         (0) root         (0)      108 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/simple_logger.py
+-rw-rw-r--   0 root         (0) root         (0)      451 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/sites.xml
+-rw-rw-r--   0 root         (0) root         (0)      217 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/sputnik.ws
+-rw-rw-r--   0 root         (0) root         (0)      474 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/staticfilesnmp.py
+-rw-rw-r--   0 root         (0) root         (0)      757 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/taskqueue.py
+-rw-rw-r--   0 root         (0) root         (0)      592 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/uwsgi.xml
+-rw-rw-r--   0 root         (0) root         (0)     1882 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/uwsgirouter.py
+-rw-rw-r--   0 root         (0) root         (0)      160 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/uwsgirouter2.py
+-rw-rw-r--   0 root         (0) root         (0)      405 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/uwsgirouter3.py
+-rw-rw-r--   0 root         (0) root         (0)      258 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/uwsgirouter4.py
+-rw-rw-r--   0 root         (0) root         (0)      178 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/uwsgirouter5.py
+-rw-rw-r--   0 root         (0) root         (0)     1793 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/uwsgistatus.py
+-rw-rw-r--   0 root         (0) root         (0)      229 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/welcome.ini
+-rw-rw-r--   0 root         (0) root         (0)     3232 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/welcome.py
+-rw-rw-r--   0 root         (0) root         (0)     1074 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/welcome3.py
+-rw-rw-r--   0 root         (0) root         (0)      235 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/werkzeug.js
+-rw-rw-r--   0 root         (0) root         (0)      533 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/werkzeug.yml
+-rw-rw-r--   0 root         (0) root         (0)      193 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/werkzeug_strict.yml
+-rw-rw-r--   0 root         (0) root         (0)     3600 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/xmlindex-html.xsl
+-rw-rw-r--   0 root         (0) root         (0)      530 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/xmlindex.ini
+-rw-rw-r--   0 root         (0) root         (0)      212 2014-12-29 09:07:07.000000 uwsgi-2.0.9/examples/zmqgevent.ini
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/ext/
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/ext/uwsgi/
+-rw-rw-r--   0 root         (0) root         (0)      641 2014-12-29 09:07:07.000000 uwsgi-2.0.9/ext/uwsgi/extconf.rb
+-rw-rw-r--   0 root         (0) root         (0)      551 2014-12-29 09:07:07.000000 uwsgi-2.0.9/install.sh
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/lib/
+-rw-rw-r--   0 root         (0) root         (0)     6341 2014-12-29 09:07:07.000000 uwsgi-2.0.9/lib/linux_ns.c
+-rw-rw-r--   0 root         (0) root         (0)    10633 2014-12-29 09:07:07.000000 uwsgi-2.0.9/lib/netlink.c
+-rw-rw-r--   0 root         (0) root         (0)      644 2014-12-29 09:07:07.000000 uwsgi-2.0.9/lib/sun_fixes.c
+-rw-rw-r--   0 root         (0) root         (0)     5971 2014-12-29 09:07:07.000000 uwsgi-2.0.9/logo_uWSGI.png
+-rw-rw-r--   0 root         (0) root         (0)     4142 2014-12-29 09:07:07.000000 uwsgi-2.0.9/logo_uWSGI.svg
+-rw-rw-r--   0 root         (0) root         (0)      665 2014-12-29 09:07:07.000000 uwsgi-2.0.9/mongrel2-uwsgi.conf
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/airbrake/
+-rw-rw-r--   0 root         (0) root         (0)     8660 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/airbrake/airbrake_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      184 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/airbrake/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_curl/
+-rw-rw-r--   0 root         (0) root         (0)     7686 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_curl/alarm_curl_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       95 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_curl/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_speech/
+-rw-rw-r--   0 root         (0) root         (0)     1313 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_speech/alarm_speech.m
+-rw-rw-r--   0 root         (0) root         (0)      237 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_speech/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_xmpp/
+-rw-rw-r--   0 root         (0) root         (0)      745 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_xmpp/alarm_xmpp_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)     4504 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_xmpp/gloox.cc
+-rw-rw-r--   0 root         (0) root         (0)      108 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/alarm_xmpp/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/asyncio/
+-rw-rw-r--   0 root         (0) root         (0)    11941 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/asyncio/asyncio.c
+-rw-rw-r--   0 root         (0) root         (0)      193 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/asyncio/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cache/
+-rw-rw-r--   0 root         (0) root         (0)    11738 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cache/cache.c
+-rw-rw-r--   0 root         (0) root         (0)       71 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cache/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/carbon/
+-rw-rw-r--   0 root         (0) root         (0)    15323 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/carbon/carbon.c
+-rw-rw-r--   0 root         (0) root         (0)       73 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/carbon/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cgi/
+-rw-rw-r--   0 root         (0) root         (0)    27579 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cgi/cgi_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       72 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cgi/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cheaper_backlog2/
+-rw-rw-r--   0 root         (0) root         (0)     2192 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cheaper_backlog2/cheaper_backlog2.c
+-rw-rw-r--   0 root         (0) root         (0)       92 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cheaper_backlog2/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cheaper_busyness/
+-rw-rw-r--   0 root         (0) root         (0)    18536 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cheaper_busyness/cheaper_busyness.c
+-rw-rw-r--   0 root         (0) root         (0)       92 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cheaper_busyness/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/clock_monotonic/
+-rw-rw-r--   0 root         (0) root         (0)      730 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/clock_monotonic/clock_monotonic.c
+-rw-rw-r--   0 root         (0) root         (0)       96 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/clock_monotonic/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/clock_realtime/
+-rw-rw-r--   0 root         (0) root         (0)      718 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/clock_realtime/clock_realtime.c
+-rw-rw-r--   0 root         (0) root         (0)       94 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/clock_realtime/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/corerouter/
+-rw-rw-r--   0 root         (0) root         (0)    33868 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/corerouter/corerouter.c
+-rw-rw-r--   0 root         (0) root         (0)    12686 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/corerouter/cr.h
+-rw-rw-r--   0 root         (0) root         (0)     8368 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/corerouter/cr_common.c
+-rw-rw-r--   0 root         (0) root         (0)     6140 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/corerouter/cr_map.c
+-rw-rw-r--   0 root         (0) root         (0)      104 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/corerouter/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/coroae/
+-rw-rw-r--   0 root         (0) root         (0)    10245 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/coroae/coroae.c
+-rw-rw-r--   0 root         (0) root         (0)      588 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/coroae/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cplusplus/
+-rw-rw-r--   0 root         (0) root         (0)     1365 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cplusplus/base.cc
+-rw-rw-r--   0 root         (0) root         (0)      405 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cplusplus/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       96 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/cplusplus/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/curl_cron/
+-rw-rw-r--   0 root         (0) root         (0)     2862 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/curl_cron/curl_cron.c
+-rw-rw-r--   0 root         (0) root         (0)       86 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/curl_cron/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/dumbloop/
+-rw-rw-r--   0 root         (0) root         (0)     2274 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/dumbloop/dumb.c
+-rw-rw-r--   0 root         (0) root         (0)       72 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/dumbloop/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/dummy/
+-rw-rw-r--   0 root         (0) root         (0)      254 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/dummy/dummy.c
+-rw-rw-r--   0 root         (0) root         (0)       71 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/dummy/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/echo/
+-rw-rw-r--   0 root         (0) root         (0)      321 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/echo/echo_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       75 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/echo/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_amqp/
+-rw-rw-r--   0 root         (0) root         (0)    17144 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_amqp/amqp.c
+-rw-rw-r--   0 root         (0) root         (0)     3239 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_amqp/emperor_amqp.c
+-rw-rw-r--   0 root         (0) root         (0)       92 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_amqp/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_mongodb/
+-rw-rw-r--   0 root         (0) root         (0)     5411 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_mongodb/emperor_mongodb.cc
+-rw-rw-r--   0 root         (0) root         (0)      619 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_mongodb/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      316 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_mongodb/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_pg/
+-rw-rw-r--   0 root         (0) root         (0)     2896 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_pg/emperor_pg.c
+-rw-rw-r--   0 root         (0) root         (0)      330 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_pg/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_zeromq/
+-rw-rw-r--   0 root         (0) root         (0)     5962 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_zeromq/emperor_zeromq.c
+-rw-rw-r--   0 root         (0) root         (0)       96 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/emperor_zeromq/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/example/
+-rw-rw-r--   0 root         (0) root         (0)      827 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/example/example_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       81 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/example/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/exception_log/
+-rw-rw-r--   0 root         (0) root         (0)     3483 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/exception_log/exception_log.c
+-rw-rw-r--   0 root         (0) root         (0)       86 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/exception_log/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/fastrouter/
+-rw-rw-r--   0 root         (0) root         (0)    14874 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/fastrouter/fastrouter.c
+-rw-rw-r--   0 root         (0) root         (0)      108 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/fastrouter/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/fiber/
+-rw-rw-r--   0 root         (0) root         (0)     2516 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/fiber/fiber.c
+-rw-rw-r--   0 root         (0) root         (0)     1255 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/fiber/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/forkptyrouter/
+-rw-rw-r--   0 root         (0) root         (0)     9753 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/forkptyrouter/forkptyrouter.c
+-rw-rw-r--   0 root         (0) root         (0)      113 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/forkptyrouter/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gccgo/
+-rw-rw-r--   0 root         (0) root         (0)    13843 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gccgo/gccgo_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)     4336 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gccgo/uwsgi.go
+-rw-rw-r--   0 root         (0) root         (0)      389 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gccgo/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/geoip/
+-rw-rw-r--   0 root         (0) root         (0)     4141 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/geoip/geoip.c
+-rw-rw-r--   0 root         (0) root         (0)       81 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/geoip/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gevent/
+-rw-rw-r--   0 root         (0) root         (0)    19078 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gevent/gevent.c
+-rw-rw-r--   0 root         (0) root         (0)     2404 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gevent/gevent.h
+-rw-rw-r--   0 root         (0) root         (0)     3879 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gevent/hooks.c
+-rw-rw-r--   0 root         (0) root         (0)      200 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gevent/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/glusterfs/
+-rw-rw-r--   0 root         (0) root         (0)     9098 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/glusterfs/glusterfs.c
+-rw-rw-r--   0 root         (0) root         (0)      221 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/glusterfs/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/graylog2/
+-rw-rw-r--   0 root         (0) root         (0)     2438 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/graylog2/graylog2_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       88 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/graylog2/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/greenlet/
+-rw-rw-r--   0 root         (0) root         (0)     4384 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/greenlet/greenlet.c
+-rw-rw-r--   0 root         (0) root         (0)      195 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/greenlet/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gridfs/
+-rw-rw-r--   0 root         (0) root         (0)     9353 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gridfs/gridfs.cc
+-rw-rw-r--   0 root         (0) root         (0)      719 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gridfs/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      360 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/gridfs/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/http/
+-rw-rw-r--   0 root         (0) root         (0)     4230 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/http/common.h
+-rw-rw-r--   0 root         (0) root         (0)    35712 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/http/http.c
+-rw-rw-r--   0 root         (0) root         (0)    14537 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/http/https.c
+-rw-rw-r--   0 root         (0) root         (0)     5676 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/http/keepalive.c
+-rw-rw-r--   0 root         (0) root         (0)    22903 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/http/spdy3.c
+-rw-rw-r--   0 root         (0) root         (0)    12685 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/http/spdy3.h
+-rw-rw-r--   0 root         (0) root         (0)      127 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/http/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/jvm/
+-rw-rw-r--   0 root         (0) root         (0)     3420 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/jvm/jvm.h
+-rw-rw-r--   0 root         (0) root         (0)    42889 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/jvm/jvm_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)     1543 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/jvm/uwsgi.java
+-rw-rw-r--   0 root         (0) root         (0)     3069 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/jvm/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/jwsgi/
+-rw-rw-r--   0 root         (0) root         (0)     5364 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/jwsgi/jwsgi_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      298 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/jwsgi/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ldap/
+-rw-rw-r--   0 root         (0) root         (0)    15137 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ldap/ldap.c
+-rw-rw-r--   0 root         (0) root         (0)       77 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ldap/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/legion_cache_fetch/
+-rw-rw-r--   0 root         (0) root         (0)     1938 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/legion_cache_fetch/legion_cache_fetch.c
+-rw-rw-r--   0 root         (0) root         (0)      100 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/legion_cache_fetch/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/libffi/
+-rw-rw-r--   0 root         (0) root         (0)     1830 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/libffi/libffi.c
+-rw-rw-r--   0 root         (0) root         (0)       70 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/libffi/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/libtcc/
+-rw-rw-r--   0 root         (0) root         (0)     1315 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/libtcc/libtcc.c
+-rw-rw-r--   0 root         (0) root         (0)       70 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/libtcc/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logcrypto/
+-rw-rw-r--   0 root         (0) root         (0)     5282 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logcrypto/logcrypto.c
+-rw-rw-r--   0 root         (0) root         (0)       78 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logcrypto/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logfile/
+-rw-rw-r--   0 root         (0) root         (0)     2169 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logfile/logfile.c
+-rw-rw-r--   0 root         (0) root         (0)       74 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logfile/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logpipe/
+-rw-rw-r--   0 root         (0) root         (0)     1186 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logpipe/logpipe.c
+-rw-rw-r--   0 root         (0) root         (0)       74 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logpipe/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logsocket/
+-rw-rw-r--   0 root         (0) root         (0)     1590 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logsocket/logsocket_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       85 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logsocket/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logzmq/
+-rw-rw-r--   0 root         (0) root         (0)     1743 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logzmq/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       80 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/logzmq/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/lua/
+-rw-rw-r--   0 root         (0) root         (0)    27053 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/lua/lua_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      726 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/lua/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/matheval/
+-rw-rw-r--   0 root         (0) root         (0)     1860 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/matheval/math.c
+-rw-rw-r--   0 root         (0) root         (0)       84 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/matheval/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mongodb/
+-rw-rw-r--   0 root         (0) root         (0)      172 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mongodb/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      195 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mongodb/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mongodblog/
+-rw-rw-r--   0 root         (0) root         (0)     4063 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mongodblog/mongodblog_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       87 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mongodblog/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mongrel2/
+-rw-rw-r--   0 root         (0) root         (0)    22912 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mongrel2/mongrel2.c
+-rw-rw-r--   0 root         (0) root         (0)       84 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mongrel2/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mono/
+-rw-rw-r--   0 root         (0) root         (0)    22929 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mono/mono_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)     5011 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mono/uwsgi.cs
+-rw-rw-r--   0 root         (0) root         (0)      595 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/mono/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/msgpack/
+-rw-rw-r--   0 root         (0) root         (0)    12175 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/msgpack/msgpack.c
+-rw-rw-r--   0 root         (0) root         (0)       67 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/msgpack/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/nagios/
+-rw-rw-r--   0 root         (0) root         (0)     1622 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/nagios/nagios.c
+-rw-rw-r--   0 root         (0) root         (0)       73 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/nagios/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/notfound/
+-rw-rw-r--   0 root         (0) root         (0)      740 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/notfound/notfound.c
+-rw-rw-r--   0 root         (0) root         (0)       76 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/notfound/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/objc_gc/
+-rw-rw-r--   0 root         (0) root         (0)       82 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/objc_gc/objc_gc.m
+-rw-rw-r--   0 root         (0) root         (0)       78 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/objc_gc/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pam/
+-rw-rw-r--   0 root         (0) root         (0)     1604 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pam/pam.c
+-rw-rw-r--   0 root         (0) root         (0)       73 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pam/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/php/
+-rw-rw-r--   0 root         (0) root         (0)      215 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/php/common.h
+-rw-rw-r--   0 root         (0) root         (0)    27433 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/php/php_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      983 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/php/session.c
+-rw-rw-r--   0 root         (0) root         (0)      728 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/php/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ping/
+-rw-rw-r--   0 root         (0) root         (0)     1972 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ping/ping_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       74 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ping/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/psgi/
+-rw-rw-r--   0 root         (0) root         (0)     2152 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/psgi/psgi.h
+-rw-rw-r--   0 root         (0) root         (0)    16762 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/psgi/psgi_loader.c
+-rw-rw-r--   0 root         (0) root         (0)    25764 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/psgi/psgi_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)     5493 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/psgi/psgi_response.c
+-rw-rw-r--   0 root         (0) root         (0)    19869 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/psgi/uwsgi_plmodule.c
+-rw-rw-r--   0 root         (0) root         (0)      436 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/psgi/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pty/
+-rw-rw-r--   0 root         (0) root         (0)     9807 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pty/pty.c
+-rw-rw-r--   0 root         (0) root         (0)      171 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pty/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pypy/
+-rw-rw-r--   0 root         (0) root         (0)     1469 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pypy/README
+-rw-rw-r--   0 root         (0) root         (0)    11588 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pypy/pypy_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)    28863 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pypy/pypy_setup.py
+-rw-rw-r--   0 root         (0) root         (0)      249 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pypy/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/
+-rw-rw-r--   0 root         (0) root         (0)      761 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/gil.c
+-rw-rw-r--   0 root         (0) root         (0)     2185 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/profiler.c
+-rw-rw-r--   0 root         (0) root         (0)     9413 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/pump_subhandler.c
+-rw-rw-r--   0 root         (0) root         (0)    21847 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/pyloader.c
+-rw-rw-r--   0 root         (0) root         (0)    54714 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/python_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)     9897 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/pyutils.c
+-rw-rw-r--   0 root         (0) root         (0)     2440 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/raw.c
+-rw-rw-r--   0 root         (0) root         (0)    22860 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/symimporter.c
+-rw-rw-r--   0 root         (0) root         (0)     8155 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/tracebacker.c
+-rw-rw-r--   0 root         (0) root         (0)    94381 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/uwsgi_pymodule.c
+-rw-rw-r--   0 root         (0) root         (0)     8913 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/uwsgi_python.h
+-rw-rw-r--   0 root         (0) root         (0)     2657 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/uwsgiplugin.py
+-rw-rw-r--   0 root         (0) root         (0)     6789 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/web3_subhandler.c
+-rw-rw-r--   0 root         (0) root         (0)    14122 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/wsgi_handlers.c
+-rw-rw-r--   0 root         (0) root         (0)     4976 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/wsgi_headers.c
+-rw-rw-r--   0 root         (0) root         (0)    11275 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/python/wsgi_subhandler.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pyuwsgi/
+-rw-rw-r--   0 root         (0) root         (0)     1660 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pyuwsgi/pyuwsgi.c
+-rw-rw-r--   0 root         (0) root         (0)      243 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/pyuwsgi/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rack/
+-rw-rw-r--   0 root         (0) root         (0)    34133 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rack/rack_api.c
+-rw-rw-r--   0 root         (0) root         (0)    37245 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rack/rack_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      963 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rack/uwsgi_rack.h
+-rw-rw-r--   0 root         (0) root         (0)     3183 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rack/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rados/
+-rw-rw-r--   0 root         (0) root         (0)    18779 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rados/rados.c
+-rw-rw-r--   0 root         (0) root         (0)       89 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rados/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rawrouter/
+-rw-rw-r--   0 root         (0) root         (0)    10024 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rawrouter/rawrouter.c
+-rw-rw-r--   0 root         (0) root         (0)      106 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rawrouter/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rbthreads/
+-rw-rw-r--   0 root         (0) root         (0)     6321 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rbthreads/rbthreads.c
+-rw-rw-r--   0 root         (0) root         (0)     1263 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rbthreads/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/redislog/
+-rw-rw-r--   0 root         (0) root         (0)     3839 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/redislog/redislog_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       83 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/redislog/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ring/
+-rw-rw-r--   0 root         (0) root         (0)    14609 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ring/ring_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      642 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ring/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_access/
+-rw-rw-r--   0 root         (0) root         (0)     2109 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_access/router_access.c
+-rw-rw-r--   0 root         (0) root         (0)      111 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_access/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_basicauth/
+-rw-rw-r--   0 root         (0) root         (0)     5126 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_basicauth/router_basicauth.c
+-rw-rw-r--   0 root         (0) root         (0)      217 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_basicauth/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_cache/
+-rw-rw-r--   0 root         (0) root         (0)    20078 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_cache/router_cache.c
+-rw-rw-r--   0 root         (0) root         (0)       84 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_cache/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_expires/
+-rw-rw-r--   0 root         (0) root         (0)     3266 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_expires/expires.c
+-rw-rw-r--   0 root         (0) root         (0)       81 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_expires/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_hash/
+-rw-rw-r--   0 root         (0) root         (0)     3759 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_hash/router_hash.c
+-rw-rw-r--   0 root         (0) root         (0)       82 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_hash/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_http/
+-rw-rw-r--   0 root         (0) root         (0)     4950 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_http/router_http.c
+-rw-rw-r--   0 root         (0) root         (0)       82 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_http/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_memcached/
+-rw-rw-r--   0 root         (0) root         (0)    11224 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_memcached/router_memcached.c
+-rw-rw-r--   0 root         (0) root         (0)       92 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_memcached/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_metrics/
+-rw-rw-r--   0 root         (0) root         (0)     4102 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_metrics/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       80 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_metrics/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_radius/
+-rw-rw-r--   0 root         (0) root         (0)     8199 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_radius/radius.c
+-rw-rw-r--   0 root         (0) root         (0)       79 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_radius/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_redirect/
+-rw-rw-r--   0 root         (0) root         (0)     2580 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_redirect/router_redirect.c
+-rw-rw-r--   0 root         (0) root         (0)       90 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_redirect/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_redis/
+-rw-rw-r--   0 root         (0) root         (0)    11248 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_redis/router_redis.c
+-rw-rw-r--   0 root         (0) root         (0)       84 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_redis/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_rewrite/
+-rw-rw-r--   0 root         (0) root         (0)     2684 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_rewrite/router_rewrite.c
+-rw-rw-r--   0 root         (0) root         (0)       88 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_rewrite/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_spnego/
+-rw-rw-r--   0 root         (0) root         (0)     7877 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_spnego/router_spnego.c
+-rw-rw-r--   0 root         (0) root         (0)      217 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_spnego/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_static/
+-rw-rw-r--   0 root         (0) root         (0)    11016 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_static/router_static.c
+-rw-rw-r--   0 root         (0) root         (0)       86 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_static/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_uwsgi/
+-rw-rw-r--   0 root         (0) root         (0)     5147 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_uwsgi/router_uwsgi.c
+-rw-rw-r--   0 root         (0) root         (0)       84 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_uwsgi/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_xmldir/
+-rw-rw-r--   0 root         (0) root         (0)     6212 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_xmldir/router_xmldir.c
+-rw-rw-r--   0 root         (0) root         (0)       85 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/router_xmldir/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rpc/
+-rw-rw-r--   0 root         (0) root         (0)    21047 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rpc/rpc_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       73 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rpc/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rrdtool/
+-rw-rw-r--   0 root         (0) root         (0)     4827 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rrdtool/rrdtool.c
+-rw-rw-r--   0 root         (0) root         (0)       75 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rrdtool/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rsyslog/
+-rw-rw-r--   0 root         (0) root         (0)     2941 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rsyslog/rsyslog_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       81 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/rsyslog/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ruby19/
+-rw-rw-r--   0 root         (0) root         (0)     1868 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ruby19/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/servlet/
+-rw-rw-r--   0 root         (0) root         (0)     2577 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/servlet/servlet_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)    12278 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/servlet/uwsgi_servlet.java
+-rw-rw-r--   0 root         (0) root         (0)      327 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/servlet/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/signal/
+-rw-rw-r--   0 root         (0) root         (0)      639 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/signal/signal_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       80 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/signal/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/spooler/
+-rw-rw-r--   0 root         (0) root         (0)     1622 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/spooler/spooler_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       81 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/spooler/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/sqlite3/
+-rw-rw-r--   0 root         (0) root         (0)     2221 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/sqlite3/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       85 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/sqlite3/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ssi/
+-rw-rw-r--   0 root         (0) root         (0)    12876 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ssi/ssi.c
+-rw-rw-r--   0 root         (0) root         (0)       66 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ssi/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/sslrouter/
+-rw-rw-r--   0 root         (0) root         (0)    14372 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/sslrouter/sslrouter.c
+-rw-rw-r--   0 root         (0) root         (0)      106 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/sslrouter/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stackless/
+-rw-rw-r--   0 root         (0) root         (0)     2917 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stackless/stackless.c
+-rw-rw-r--   0 root         (0) root         (0)      197 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stackless/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_file/
+-rw-rw-r--   0 root         (0) root         (0)     1988 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_file/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       84 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_file/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_mongodb/
+-rw-rw-r--   0 root         (0) root         (0)      372 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_mongodb/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)     1713 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_mongodb/stats_pusher_mongodb.cc
+-rw-rw-r--   0 root         (0) root         (0)      326 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_mongodb/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_socket/
+-rw-rw-r--   0 root         (0) root         (0)     3092 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_socket/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       86 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_socket/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_statsd/
+-rw-rw-r--   0 root         (0) root         (0)     3199 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_statsd/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       86 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/stats_pusher_statsd/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/symcall/
+-rw-rw-r--   0 root         (0) root         (0)     6471 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/symcall/symcall_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       81 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/symcall/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/syslog/
+-rw-rw-r--   0 root         (0) root         (0)     2685 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/syslog/syslog_plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       79 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/syslog/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/systemd_logger/
+-rw-rw-r--   0 root         (0) root         (0)      759 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/systemd_logger/systemd_logger.c
+-rw-rw-r--   0 root         (0) root         (0)      241 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/systemd_logger/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/tornado/
+-rw-rw-r--   0 root         (0) root         (0)    12664 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/tornado/tornado.c
+-rw-rw-r--   0 root         (0) root         (0)      193 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/tornado/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_chunked/
+-rw-rw-r--   0 root         (0) root         (0)     1475 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_chunked/chunked.c
+-rw-rw-r--   0 root         (0) root         (0)       89 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_chunked/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_gzip/
+-rw-rw-r--   0 root         (0) root         (0)     2168 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_gzip/gzip.c
+-rw-rw-r--   0 root         (0) root         (0)       83 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_gzip/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_offload/
+-rw-rw-r--   0 root         (0) root         (0)     3974 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_offload/offload.c
+-rw-rw-r--   0 root         (0) root         (0)       89 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_offload/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_template/
+-rw-rw-r--   0 root         (0) root         (0)     1393 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_template/tt.c
+-rw-rw-r--   0 root         (0) root         (0)       85 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_template/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_tofile/
+-rw-rw-r--   0 root         (0) root         (0)     3582 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_tofile/tofile.c
+-rw-rw-r--   0 root         (0) root         (0)       87 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_tofile/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_toupper/
+-rw-rw-r--   0 root         (0) root         (0)      830 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_toupper/toupper.c
+-rw-rw-r--   0 root         (0) root         (0)       89 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/transformation_toupper/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/tuntap/
+-rw-rw-r--   0 root         (0) root         (0)    10117 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/tuntap/common.c
+-rw-rw-r--   0 root         (0) root         (0)     3593 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/tuntap/common.h
+-rw-rw-r--   0 root         (0) root         (0)    11771 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/tuntap/firewall.c
+-rw-rw-r--   0 root         (0) root         (0)    18448 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/tuntap/tuntap.c
+-rw-rw-r--   0 root         (0) root         (0)       83 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/tuntap/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ugreen/
+-rw-rw-r--   0 root         (0) root         (0)     3213 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ugreen/ugreen.c
+-rw-rw-r--   0 root         (0) root         (0)       73 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/ugreen/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/v8/
+-rw-rw-r--   0 root         (0) root         (0)     1049 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/v8/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)      326 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/v8/uwsgiplugin.py
+-rw-rw-r--   0 root         (0) root         (0)     4621 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/v8/v8_commonjs.cc
+-rw-rw-r--   0 root         (0) root         (0)     7053 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/v8/v8_jsgi.cc
+-rw-rw-r--   0 root         (0) root         (0)    10737 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/v8/v8_uwsgi.cc
+-rw-rw-r--   0 root         (0) root         (0)      937 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/v8/v8_uwsgi.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/webdav/
+-rw-rw-r--   0 root         (0) root         (0)      189 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/webdav/uwsgiplugin.py
+-rw-rw-r--   0 root         (0) root         (0)    51108 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/webdav/webdav.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/xattr/
+-rw-rw-r--   0 root         (0) root         (0)       63 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/xattr/uwsgiplugin.py
+-rw-rw-r--   0 root         (0) root         (0)     2531 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/xattr/xattr.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/xslt/
+-rw-rw-r--   0 root         (0) root         (0)      185 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/xslt/uwsgiplugin.py
+-rw-rw-r--   0 root         (0) root         (0)    15063 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/xslt/xslt.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/zabbix/
+-rw-rw-r--   0 root         (0) root         (0)     6255 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/zabbix/plugin.c
+-rw-rw-r--   0 root         (0) root         (0)       73 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/zabbix/uwsgiplugin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/zergpool/
+-rw-rw-r--   0 root         (0) root         (0)       77 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/zergpool/uwsgiplugin.py
+-rw-rw-r--   0 root         (0) root         (0)     3736 2014-12-29 09:07:07.000000 uwsgi-2.0.9/plugins/zergpool/zergpool.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/proto/
+-rw-rw-r--   0 root         (0) root         (0)    12475 2014-12-29 09:07:07.000000 uwsgi-2.0.9/proto/base.c
+-rw-rw-r--   0 root         (0) root         (0)    11986 2014-12-29 09:07:07.000000 uwsgi-2.0.9/proto/fastcgi.c
+-rw-rw-r--   0 root         (0) root         (0)    25856 2014-12-29 09:07:07.000000 uwsgi-2.0.9/proto/http.c
+-rw-rw-r--   0 root         (0) root         (0)     4090 2014-12-29 09:07:07.000000 uwsgi-2.0.9/proto/puwsgi.c
+-rw-rw-r--   0 root         (0) root         (0)     4423 2014-12-29 09:07:07.000000 uwsgi-2.0.9/proto/scgi.c
+-rw-rw-r--   0 root         (0) root         (0)     7943 2014-12-29 09:07:07.000000 uwsgi-2.0.9/proto/uwsgi.c
+-rw-rw-r--   0 root         (0) root         (0)     2824 2014-12-29 09:07:07.000000 uwsgi-2.0.9/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/
+-rw-rw-r--   0 root         (0) root         (0)      600 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/cachebitmap.ini
+-rw-rw-r--   0 root         (0) root         (0)     5698 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/cachebitmap.py
+-rw-rw-r--   0 root         (0) root         (0)      716 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/cachetest.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/clojure/
+-rw-rw-r--   0 root         (0) root         (0)      292 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/clojure/myapp.clj
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/core/
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/core/apps/
+-rw-rw-r--   0 root         (0) root         (0)      168 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/core/apps/read_body_and_send.pl
+-rw-rw-r--   0 root         (0) root         (0)      789 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/core/read_body_and_send.pl
+-rw-rw-r--   0 root         (0) root         (0)     1583 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/core/url_sanitize.pl
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/go/
+-rw-rw-r--   0 root         (0) root         (0)     1554 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/go/cachetest.go
+-rw-rw-r--   0 root         (0) root         (0)     1097 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/go/complextest.go
+-rw-rw-r--   0 root         (0) root         (0)     1003 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/go/uploadtest.go
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/java/
+-rw-rw-r--   0 root         (0) root         (0)      396 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/java/rpc.java
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/lua/
+-rw-rw-r--   0 root         (0) root         (0)      565 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/lua/basic.lua
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/mono/
+-rw-rw-r--   0 root         (0) root         (0)      130 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/mono/cache.aspx
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/
+-rw-rw-r--   0 root         (0) root         (0)      285 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/active_workers_signal.pl
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/apps/
+-rw-rw-r--   0 root         (0) root         (0)      309 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/apps/input_with_offset.pl
+-rw-rw-r--   0 root         (0) root         (0)     1720 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/test.psgi
+-rw-rw-r--   0 root         (0) root         (0)     1894 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/test_benchmark.pl
+-rw-rw-r--   0 root         (0) root         (0)      537 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/test_harakiri.psgi
+-rw-rw-r--   0 root         (0) root         (0)      100 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/test_hello.psgi
+-rw-rw-r--   0 root         (0) root         (0)     1828 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/test_input_with_offset.pl
+-rw-rw-r--   0 root         (0) root         (0)     1303 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/test_post.psgi
+-rw-rw-r--   0 root         (0) root         (0)      535 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/test_sleepy.psgi
+-rw-rw-r--   0 root         (0) root         (0)     1370 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/perl/test_streaming.psgi
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/pypy/
+-rw-rw-r--   0 root         (0) root         (0)     1191 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/pypy/t_continulet1.py
+-rw-rw-r--   0 root         (0) root         (0)     1403 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/pypy/t_continulet2.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/python/
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/python/manage_script_name/
+-rw-rw-r--   0 root         (0) root         (0)      232 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/python/manage_script_name/manage_script_name_test.ini
+-rw-rw-r--   0 root         (0) root         (0)     1392 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/python/manage_script_name/test_manage_script_name.py
+-rw-rw-r--   0 root         (0) root         (0)      130 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/python/manage_script_name/useless_app.py
+-rw-rw-r--   0 root         (0) root         (0)      186 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/python/testba.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/
+-rw-rw-r--   0 root         (0) root         (0)      310 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/README.md
+-rw-rw-r--   0 root         (0) root         (0)      258 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/config.ini
+-rw-rw-r--   0 root         (0) root         (0)      291 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/project.clj
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/src/
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/src/uwsgi/
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/src/uwsgi/ring/
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/
+-rw-rw-r--   0 root         (0) root         (0)      857 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/app.clj
+-rw-rw-r--   0 root         (0) root         (0)     1122 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/basic.clj
+-rw-rw-r--   0 root         (0) root         (0)      595 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/body.clj
+-rw-rw-r--   0 root         (0) root         (0)      301 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/simple.clj
+-rw-rw-r--   0 root         (0) root         (0)      560 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/upload.clj
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/routing/
+-rw-rw-r--   0 root         (0) root         (0)     1811 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/routing/auth.ini
+-rw-rw-r--   0 root         (0) root         (0)     1018 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/routing/errorlimiter.ini
+-rw-rw-r--   0 root         (0) root         (0)      674 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/routing/limiter.ini
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/webdav/
+-rw-rw-r--   0 root         (0) root         (0)      459 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/webdav/carddav.ini
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/xslt/
+-rw-rw-r--   0 root         (0) root         (0)      436 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/xslt/cd.xml
+-rw-rw-r--   0 root         (0) root         (0)      675 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/xslt/cd.xml.xslt
+-rw-rw-r--   0 root         (0) root         (0)      214 2014-12-29 09:07:07.000000 uwsgi-2.0.9/t/xslt/routex.ini
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/
+-rw-rw-r--   0 root         (0) root         (0)     1013 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/Responder.pm
+-rw-rw-r--   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       55 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/badthread.py
+-rw-rw-r--   0 root         (0) root         (0)      584 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/badwrites.py
+-rw-rw-r--   0 root         (0) root         (0)      189 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/cpubound_async.py
+-rw-rw-r--   0 root         (0) root         (0)      379 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/cpubound_green.py
+-rw-rw-r--   0 root         (0) root         (0)      319 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/cpubound_stackless.py
+-rw-rw-r--   0 root         (0) root         (0)     3604 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/decoratortest.py
+-rw-rw-r--   0 root         (0) root         (0)      403 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/fileserve_async.py
+-rw-rw-r--   0 root         (0) root         (0)      407 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/gevent_spool.py
+-rw-rw-r--   0 root         (0) root         (0)      525 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/grunter.py
+-rw-rw-r--   0 root         (0) root         (0)      818 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/iobound_async.py
+-rw-rw-r--   0 root         (0) root         (0)     1085 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/iobound_async_unix.py
+-rw-rw-r--   0 root         (0) root         (0)      862 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/iobound_green.py
+-rw-rw-r--   0 root         (0) root         (0)      259 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/logger.py
+-rw-rw-r--   0 root         (0) root         (0)      473 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/mako_ugreen.py
+-rw-rw-r--   0 root         (0) root         (0)      684 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/mulefunc.py
+-rw-rw-r--   0 root         (0) root         (0)      223 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/multiapp.txt
+-rw-rw-r--   0 root         (0) root         (0)      382 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/myadmin.py
+-rw-rw-r--   0 root         (0) root         (0)     1230 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/pgbound_async.py
+-rw-rw-r--   0 root         (0) root         (0)      528 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/picazzo.py
+-rw-rw-r--   0 root         (0) root         (0)      981 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/psycogreen_green.py
+-rw-rw-r--   0 root         (0) root         (0)     1108 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/psycopg2_green.py
+-rw-rw-r--   0 root         (0) root         (0)      196 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/pump.py
+-rw-rw-r--   0 root         (0) root         (0)     1342 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/queue.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/refcount.py
+-rw-rw-r--   0 root         (0) root         (0)      425 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/rpc.lua
+-rw-rw-r--   0 root         (0) root         (0)      128 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/rpc.py
+-rw-rw-r--   0 root         (0) root         (0)      304 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/runningthread.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/sendchunked.py
+-rw-rw-r--   0 root         (0) root         (0)      372 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/sharedarea.py
+-rw-rw-r--   0 root         (0) root         (0)      278 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/sig.lua
+-rw-rw-r--   0 root         (0) root         (0)      997 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/signals.py
+-rw-rw-r--   0 root         (0) root         (0)      646 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/sigwait.py
+-rw-rw-r--   0 root         (0) root         (0)      290 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/sleeping_async.py
+-rw-rw-r--   0 root         (0) root         (0)      472 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/sleeping_green.py
+-rw-rw-r--   0 root         (0) root         (0)      353 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/sleepthreadasync.py
+-rw-rw-r--   0 root         (0) root         (0)      229 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/slow.py
+-rw-rw-r--   0 root         (0) root         (0)      385 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/spoolme.py
+-rw-rw-r--   0 root         (0) root         (0)      370 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/staticfile.py
+-rw-rw-r--   0 root         (0) root         (0)      378 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/streamer.psgi
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/t/
+-rw-rw-r--   0 root         (0) root         (0)     1857 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/t/static.pl
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/templates/
+-rw-rw-r--   0 root         (0) root         (0)     1273 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/templates/queue.html
+-rw-rw-r--   0 root         (0) root         (0)     4874 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/testapp.py
+-rw-rw-r--   0 root         (0) root         (0)      887 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/testgevent.py
+-rw-rw-r--   0 root         (0) root         (0)      322 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/testpy3.py
+-rw-rw-r--   0 root         (0) root         (0)      397 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/testsignals.py
+-rw-rw-r--   0 root         (0) root         (0)      679 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/threads.py
+-rwxrwxr-x   0 root         (0) root         (0)     3076 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/travis.sh
+-rw-rw-r--   0 root         (0) root         (0)     1631 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/ugevent.py
+-rw-rw-r--   0 root         (0) root         (0)      236 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/web3.py
+-rw-rw-r--   0 root         (0) root         (0)     2119 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/websockets.py
+-rw-rw-r--   0 root         (0) root         (0)     3764 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/websockets_chat.pl
+-rw-rw-r--   0 root         (0) root         (0)     2622 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/websockets_chat.py
+-rw-rw-r--   0 root         (0) root         (0)     3165 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/websockets_chat_async.py
+-rw-rw-r--   0 root         (0) root         (0)     4294 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/websockets_chat_asyncio.py
+-rw-rw-r--   0 root         (0) root         (0)     1867 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/websockets_echo.lua
+-rw-rw-r--   0 root         (0) root         (0)     1824 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/websockets_echo.pl
+-rw-rw-r--   0 root         (0) root         (0)     1787 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/websockets_echo.py
+-rw-rw-r--   0 root         (0) root         (0)     1856 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/websockets_echo.ru
+-rw-rw-r--   0 root         (0) root         (0)      109 2014-12-29 09:07:07.000000 uwsgi-2.0.9/tests/werkzeug.py
+-rw-rw-r--   0 root         (0) root         (0)      557 2014-12-29 09:07:07.000000 uwsgi-2.0.9/uwsgi.gemspec
+-rw-rw-r--   0 root         (0) root         (0)   124520 2014-12-29 09:07:07.000000 uwsgi-2.0.9/uwsgi.h
+-rw-rw-r--   0 root         (0) root         (0)      134 2014-12-29 09:07:07.000000 uwsgi-2.0.9/uwsgi_main.c
+-rw-rw-r--   0 root         (0) root         (0)    60125 2014-12-29 09:07:07.000000 uwsgi-2.0.9/uwsgiconfig.py
+-rw-rw-r--   0 root         (0) root         (0)    10206 2014-12-29 09:07:07.000000 uwsgi-2.0.9/uwsgidecorators.py
+-rw-rw-r--   0 root         (0) root         (0)     2839 2014-12-29 09:07:07.000000 uwsgi-2.0.9/uwsgidsl.rb
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/valgrind/
+-rw-rw-r--   0 root         (0) root         (0)      316 2014-12-29 09:07:07.000000 uwsgi-2.0.9/valgrind/README
+-rwxrwxr-x   0 root         (0) root         (0)      430 2014-12-29 09:07:07.000000 uwsgi-2.0.9/valgrind/valgrind-generate-sups.sh
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vassals/
+-rw-rw-r--   0 root         (0) root         (0)      319 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vassals/broodlord.ini
+-rw-rw-r--   0 root         (0) root         (0)      175 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vassals/cc.ini
+-rw-rw-r--   0 root         (0) root         (0)      490 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vassals/multi.xml
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask001/
+-rw-rw-r--   0 root         (0) root         (0)      102 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask001/app1.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask002/
+-rw-rw-r--   0 root         (0) root         (0)      111 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask002/app2.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask003/
+-rw-rw-r--   0 root         (0) root         (0)      107 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask003/app3.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask004/
+-rw-rw-r--   0 root         (0) root         (0)      107 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask004/app4.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask005/
+-rw-rw-r--   0 root         (0) root         (0)      107 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/flask005/app5.py
+-rw-rw-r--   0 root         (0) root         (0)      742 2014-12-29 09:07:07.000000 uwsgi-2.0.9/vhosttest/nginx.conf
```

### Comparing `uwsgi-2.0.8/.travis.yml` & `uwsgi-2.0.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/CONTRIBUTORS` & `uwsgi-2.0.9/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/LICENSE` & `uwsgi-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/apache2/mod_Ruwsgi.c` & `uwsgi-2.0.9/apache2/mod_Ruwsgi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/apache2/mod_proxy_uwsgi.c` & `uwsgi-2.0.9/apache2/mod_proxy_uwsgi.c`

 * *Files 4% similar despite different names*

```diff
@@ -361,20 +361,21 @@
 		}
 
 
 	if ((buf = apr_table_get(r->headers_out, "Content-Type"))) {
                 ap_set_content_type(r, apr_pstrdup(r->pool, buf));
             }
 	
-	for(;;) {
+	int finish = 0;
+	while(!finish) {
 		rv = ap_get_brigade(rp->input_filters, bb,
                                         AP_MODE_READBYTES, mode,
                                         conf->io_buffer_size);
-		if (mode == APR_NONBLOCK_READ && (APR_STATUS_IS_EAGAIN(rv)
-                        || (rv == APR_SUCCESS && APR_BRIGADE_EMPTY(bb)))) {
+		if (APR_STATUS_IS_EAGAIN(rv)
+                        || (rv == APR_SUCCESS && APR_BRIGADE_EMPTY(bb)) ) {
 			e = apr_bucket_flush_create(c->bucket_alloc);
 			APR_BRIGADE_INSERT_TAIL(bb, e);
 			if (ap_pass_brigade(r->output_filters, bb) || c->aborted) {
 				break;
 			}
 			apr_brigade_cleanup(bb);
 			mode = APR_BLOCK_READ;
@@ -397,15 +398,24 @@
 		if (APR_BRIGADE_EMPTY(bb)) {
                         apr_brigade_cleanup(bb);
                         break;
                 }
 
 		ap_proxy_buckets_lifetime_transform(r, bb, pass_bb);
 
-		ap_pass_brigade(r->output_filters, pass_bb);
+		// found the last brigade?
+		if (APR_BUCKET_IS_EOS(APR_BRIGADE_LAST(bb))) finish = 1;
+
+		// do not pass chunk if it is zero_sized
+		apr_brigade_length(pass_bb, 0, &readbytes);
+
+		if ((readbytes > 0 && ap_pass_brigade(r->output_filters, pass_bb) != APR_SUCCESS) || c->aborted) {
+			finish = 1;
+		}
+
 		apr_brigade_cleanup(bb);
 		apr_brigade_cleanup(pass_bb);
 	}
 
 	e = apr_bucket_eos_create(c->bucket_alloc);
 	APR_BRIGADE_INSERT_TAIL(bb, e);
         ap_pass_brigade(r->output_filters, bb);
```

### Comparing `uwsgi-2.0.8/apache2/mod_uwsgi.c` & `uwsgi-2.0.9/apache2/mod_uwsgi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/buildconf/base.ini` & `uwsgi-2.0.9/buildconf/base.ini`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/Uwsgi.pm` & `uwsgi-2.0.9/contrib/Uwsgi.pm`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/binder.pl` & `uwsgi-2.0.9/contrib/binder.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/centos_init_script` & `uwsgi-2.0.9/contrib/centos_init_script`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/cgi_python.c` & `uwsgi-2.0.9/contrib/cgi_python.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/emperormon.ru` & `uwsgi-2.0.9/contrib/emperormon.ru`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/graphite_uwsgi.py` & `uwsgi-2.0.9/contrib/graphite_uwsgi.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/launchd/it.unbit.uwsgi.plist` & `uwsgi-2.0.9/contrib/launchd/it.unbit.uwsgi.plist`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/loadapp.pl` & `uwsgi-2.0.9/contrib/loadapp.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/pypy/uwsgi_pypy_greenlets.py` & `uwsgi-2.0.9/contrib/pypy/uwsgi_pypy_greenlets.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/runuwsgi.py` & `uwsgi-2.0.9/contrib/runuwsgi.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/securesubscribe.pl` & `uwsgi-2.0.9/contrib/securesubscribe.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/spoolqueue/tasksconsumer.py` & `uwsgi-2.0.9/contrib/spoolqueue/tasksconsumer.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/twuwsgi.py` & `uwsgi-2.0.9/contrib/twuwsgi.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/urack.rb` & `uwsgi-2.0.9/contrib/urack.rb`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/uwsgi-cache-monitor.py` & `uwsgi-2.0.9/contrib/uwsgi-cache-monitor.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/uwsgi.erl` & `uwsgi-2.0.9/contrib/uwsgi.erl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/uwsgi.java` & `uwsgi-2.0.9/contrib/uwsgi.java`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/uwsgi.rb` & `uwsgi-2.0.9/contrib/uwsgi.rb`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/uwsgi_client.c` & `uwsgi-2.0.9/contrib/uwsgi_client.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/uwsgi_dynamic_client.c` & `uwsgi-2.0.9/contrib/uwsgi_dynamic_client.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/contrib/uwsgisubscribers.ru` & `uwsgi-2.0.9/contrib/uwsgisubscribers.ru`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/alarm.c` & `uwsgi-2.0.9/core/alarm.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/async.c` & `uwsgi-2.0.9/core/async.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/buffer.c` & `uwsgi-2.0.9/core/buffer.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/cache.c` & `uwsgi-2.0.9/core/cache.c`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 	where need is the size of the object
 
 */
 
 static void cache_full(struct uwsgi_cache *uc) {
 	uint64_t i;
+	int force_clear = 0;
 
 	if (!uc->ignore_full) {
         	if (uc->purge_lru)
                 	uwsgi_log("LRU item will be purged from cache \"%s\"\n", uc->name);
                 else
                 	uwsgi_log("*** DANGER cache \"%s\" is FULL !!! ***\n", uc->name);
 	}
@@ -37,27 +38,33 @@
         uc->full++;
 
         if (uc->purge_lru && uc->lru_head)
         	uwsgi_cache_del2(uc, NULL, 0, uc->lru_head, UWSGI_CACHE_FLAG_LOCAL);
 
 	// we do not need locking here !
 	if (uc->sweep_on_full) {
+		uint64_t removed = 0;
 		uint64_t now = (uint64_t) uwsgi_now();
 		if (uc->next_scan <= now) {
 			uc->next_scan = now + uc->sweep_on_full;
                 	for (i = 1; i < uc->max_items; i++) {
 				struct uwsgi_cache_item *uci = cache_item(i);
 				if (uci->expires > 0 && uci->expires <= now) {
-                			uwsgi_cache_del2(uc, NULL, 0, i, 0);
+                			if (!uwsgi_cache_del2(uc, NULL, 0, i, 0)) {
+						removed++;
+					}
 				}
 			}
+			if (removed == 0) {
+				force_clear = 1;
+			}
                 }
 	}
 
-	if (uc->clear_on_full) {
+	if (uc->clear_on_full || force_clear) {
                 for (i = 1; i < uc->max_items; i++) {
                 	uwsgi_cache_del2(uc, NULL, 0, i, 0);
                 }
 	}
 }
 
 static uint64_t uwsgi_cache_find_free_blocks(struct uwsgi_cache *uc, uint64_t need) {
```

### Comparing `uwsgi-2.0.8/core/chunked.c` & `uwsgi-2.0.9/core/chunked.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/clock.c` & `uwsgi-2.0.9/core/clock.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/config.c` & `uwsgi-2.0.9/core/config.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/cookie.c` & `uwsgi-2.0.9/core/cookie.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/cron.c` & `uwsgi-2.0.9/core/cron.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/daemons.c` & `uwsgi-2.0.9/core/daemons.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/emperor.c` & `uwsgi-2.0.9/core/emperor.c`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 extern struct uwsgi_server uwsgi;
 extern char **environ;
 
 void emperor_send_stats(int);
 
 time_t emperor_throttle;
 int emperor_throttle_level;
+int emperor_warming_up = 1;
 
 struct uwsgi_instance *ui;
 
 time_t on_royal_death = 0;
 
 /*
 
@@ -863,15 +864,24 @@
 		}
 	}
 
 	emperor_throttle = now;
 #ifdef UWSGI_DEBUG
 	uwsgi_log("emperor throttle = %d\n", emperor_throttle_level);
 #endif
-	usleep(emperor_throttle_level);
+	if (emperor_warming_up) {
+		if (emperor_throttle_level > 0) {
+			// wait 10 milliseconds in case of fork-bombing
+			// pretty random value, but should avoid the load average to increase
+			usleep(10);
+		}
+	}
+	else {
+		usleep(emperor_throttle_level);
+	}
 
 	if (uwsgi.emperor_tyrant) {
 		if (uid == 0 || gid == 0) {
 			uwsgi_log("[emperor-tyrant] invalid permissions for vassal %s\n", name);
 			return;
 		}
 	}
@@ -1550,14 +1560,15 @@
 
 void uwsgi_emperor_run_scanners(void) {
 	struct uwsgi_emperor_scanner *ues = emperor_scanners;
 	while (ues) {
 		ues->monitor->func(ues);
 		ues = ues->next;
 	}
+	emperor_warming_up = 0;
 }
 
 void emperor_build_scanners() {
 	struct uwsgi_string_list *usl = uwsgi.emperor;
 	glob_t g;
 	while (usl) {
 		struct uwsgi_imperial_monitor *uim = imperial_monitor_get_by_scheme(usl->value);
```

### Comparing `uwsgi-2.0.8/core/errors.c` & `uwsgi-2.0.9/core/errors.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/event.c` & `uwsgi-2.0.9/core/event.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/exceptions.c` & `uwsgi-2.0.9/core/exceptions.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/fifo.c` & `uwsgi-2.0.9/core/fifo.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/fsmon.c` & `uwsgi-2.0.9/core/fsmon.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/gateway.c` & `uwsgi-2.0.9/core/gateway.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/hash.c` & `uwsgi-2.0.9/core/hash.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/hooks.c` & `uwsgi-2.0.9/core/hooks.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/ini.c` & `uwsgi-2.0.9/core/ini.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/init.c` & `uwsgi-2.0.9/core/init.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/io.c` & `uwsgi-2.0.9/core/io.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/json.c` & `uwsgi-2.0.9/core/json.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/legion.c` & `uwsgi-2.0.9/core/legion.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/lock.c` & `uwsgi-2.0.9/core/lock.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/logging.c` & `uwsgi-2.0.9/core/logging.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/loop.c` & `uwsgi-2.0.9/core/loop.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/master.c` & `uwsgi-2.0.9/core/master.c`

 * *Files 0% similar despite different names*

```diff
@@ -857,15 +857,18 @@
         			struct uwsgi_daemon *ud = uwsgi.daemons;
         			while (ud) {
                 			if (ud->pid > 0 && ud->touch) {
                         			touched = uwsgi_check_touches(ud->touch);
 						if (touched) {
 							uwsgi_log_verbose("*** %s has been touched... reloading daemon \"%s\" (pid: %d) !!! ***\n", touched, ud->command, (int) ud->pid);
 							if (kill(-ud->pid, ud->stop_signal)) {
-								uwsgi_error("[uwsgi-daemon/touch] kill()");
+								// killing process group failed, try to kill by process id
+								if (kill(ud->pid, ud->stop_signal)) {
+									uwsgi_error("[uwsgi-daemon/touch] kill()");
+								}
 							}
 						}
                 			}
 					ud = ud->next;
                 		}
 
 				// hook touches
```

### Comparing `uwsgi-2.0.8/core/master_checks.c` & `uwsgi-2.0.9/core/master_checks.c`

 * *Files 5% similar despite different names*

```diff
@@ -134,20 +134,33 @@
 			}
 			return;
 		}
 		for (i = 1; i <= uwsgi.numproc; i++) {
 			uwsgi.workers[i].cheaped = 1;
 			if (uwsgi.workers[i].pid == 0)
 				continue;
+			// first send SIGINT
+			kill(uwsgi.workers[i].pid, SIGINT);
+			// and start waiting upto 3 seconds
+			int j;
+			for(j=0;j<3;j++) {
+				sleep(1);
+				int ret = waitpid(uwsgi.workers[i].pid, &waitpid_status, WNOHANG);
+				if (ret == 0) continue;
+				if (ret == (int) uwsgi.workers[i].pid) goto done;
+				// on error, directly send SIGKILL
+				break;
+			}
 			kill(uwsgi.workers[i].pid, SIGKILL);
 			if (waitpid(uwsgi.workers[i].pid, &waitpid_status, 0) < 0) {
 				if (errno != ECHILD)
 					uwsgi_error("uwsgi_master_check_idle()/waitpid()");
 			}
 			else {
+done:
 				uwsgi.workers[i].pid = 0;
 				uwsgi.workers[i].rss_size = 0;
 				uwsgi.workers[i].vsz_size = 0;
 			}
 		}
 		uwsgi_add_sockets_to_queue(uwsgi.master_queue, -1);
 		uwsgi_log("cheap mode enabled: waiting for socket connection...\n");
@@ -331,14 +344,15 @@
 		return -1;
 	}
 	return 0;
 }
 
 int uwsgi_worker_is_busy(int wid) {
 	int i;
+	if (uwsgi.workers[uwsgi.mywid].sig) return 1;
 	for(i=0;i<uwsgi.cores;i++) {
 		if (uwsgi.workers[wid].cores[i].in_request) {
 			return 1;
 		}
 	}
 	return 0;
 }
```

### Comparing `uwsgi-2.0.8/core/master_events.c` & `uwsgi-2.0.9/core/master_events.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/master_utils.c` & `uwsgi-2.0.9/core/master_utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -158,24 +158,26 @@
 	// then check for fifo
 	if (uwsgi.cheaper_fifo_delta != 0) {
 		if (!ignore_algo) {
 			needed_workers = uwsgi.cheaper_fifo_delta;
 			ignore_algo = 1;
 		}
 		uwsgi.cheaper_fifo_delta = 0;
+		goto safe;
 	}
 
 	// if cheaper limits wants to change worker count, then skip cheaper algo
 	if (!needed_workers) needed_workers = uwsgi.cheaper_algo(!ignore_algo);
 	// safe check to verify if cheaper algo obeyed ignore_algo value
 	if (ignore_algo && needed_workers > 0) {
 		uwsgi_log("BUG! cheaper algo returned %d but it cannot spawn any worker at this time!\n", needed_workers);
 		needed_workers = 0;
 	}
 
+safe:
 	if (needed_workers > 0) {
 		for (i = 1; i <= uwsgi.numproc; i++) {
 			if (uwsgi.workers[i].cheaped == 1 && uwsgi.workers[i].pid == 0) {
 				if (uwsgi_respawn_worker(i))
 					return 0;
 				needed_workers--;
 			}
```

### Comparing `uwsgi-2.0.8/core/metrics.c` & `uwsgi-2.0.9/core/metrics.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/mount.c` & `uwsgi-2.0.9/core/mount.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/mule.c` & `uwsgi-2.0.9/core/mule.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/notify.c` & `uwsgi-2.0.9/core/notify.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/offload.c` & `uwsgi-2.0.9/core/offload.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/plugins.c` & `uwsgi-2.0.9/core/plugins.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/plugins_builder.c` & `uwsgi-2.0.9/core/plugins_builder.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/progress.c` & `uwsgi-2.0.9/core/progress.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/protocol.c` & `uwsgi-2.0.9/core/protocol.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/querystring.c` & `uwsgi-2.0.9/core/querystring.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/queue.c` & `uwsgi-2.0.9/core/queue.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/rb_timers.c` & `uwsgi-2.0.9/core/rb_timers.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/reader.c` & `uwsgi-2.0.9/core/reader.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/regexp.c` & `uwsgi-2.0.9/core/regexp.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/routing.c` & `uwsgi-2.0.9/core/routing.c`

 * *Files 1% similar despite different names*

```diff
@@ -2041,9 +2041,23 @@
 		*space = 0;
 		usl->custom = strlen(usl->value);
 		*space = ' ';
 		usl->custom_ptr = space+1;
 		usl->custom2 = strlen(space+1);
 		uwsgi_log("collecting header %.*s to var %s\n", usl->custom, usl->value, usl->custom_ptr);
 	}
+
+	uwsgi_foreach(usl, uwsgi.pull_headers) {
+                char *space = strchr(usl->value, ' ');
+                if (!space) {
+                        uwsgi_log("invalid pull header syntax, must be <header> <var>\n");
+                        exit(1);
+                }
+                *space = 0;
+                usl->custom = strlen(usl->value);
+                *space = ' ';
+                usl->custom_ptr = space+1;
+                usl->custom2 = strlen(space+1);
+                uwsgi_log("pulling header %.*s to var %s\n", usl->custom, usl->value, usl->custom_ptr);
+        }
 }
 #endif
```

### Comparing `uwsgi-2.0.8/core/rpc.c` & `uwsgi-2.0.9/core/rpc.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/sendfile.c` & `uwsgi-2.0.9/core/sendfile.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/setup_utils.c` & `uwsgi-2.0.9/core/setup_utils.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/sharedarea.c` & `uwsgi-2.0.9/core/sharedarea.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/signal.c` & `uwsgi-2.0.9/core/signal.c`

 * *Files 2% similar despite different names*

```diff
@@ -327,14 +327,24 @@
 	else if (!strcmp(use->receiver, "workers")) {
 		for (i = 1; i <= uwsgi.numproc; i++) {
 			if (uwsgi_signal_send(uwsgi.workers[i].signal_pipe[0], sig)) {
 				uwsgi_log("could not deliver signal %d to worker %d\n", sig, i);
 			}
 		}
 	}
+	// send to al lactive workers
+	else if (!strcmp(use->receiver, "active-workers")) {
+                for (i = 1; i <= uwsgi.numproc; i++) {
+			if (uwsgi.workers[i].pid > 0 && !uwsgi.workers[i].cheaped && !uwsgi.workers[i].suspended) {
+                        	if (uwsgi_signal_send(uwsgi.workers[i].signal_pipe[0], sig)) {
+                                	uwsgi_log("could not deliver signal %d to worker %d\n", sig, i);
+                        	}
+			}
+                }
+        }
 	// route to specific worker
 	else if (!strncmp(use->receiver, "worker", 6)) {
 		i = atoi(use->receiver + 6);
 		if (i > uwsgi.numproc) {
 			uwsgi_log("invalid signal target: %s\n", use->receiver);
 		}
 		if (uwsgi_signal_send(uwsgi.workers[i].signal_pipe[0], sig)) {
```

### Comparing `uwsgi-2.0.8/core/snmp.c` & `uwsgi-2.0.9/core/snmp.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/socket.c` & `uwsgi-2.0.9/core/socket.c`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,18 @@
 		uwsgi_error("malloc()");
 		uwsgi_nuclear_blast();
 		return -1;
 	}
 
 	memset(uws_addr, 0, sizeof(struct sockaddr_un));
 	serverfd = create_server_socket(AF_UNIX, SOCK_STREAM);
-	if (serverfd < 0) return -1;
+	if (serverfd < 0) {
+		free(uws_addr);
+		return -1;
+	}
 	if (abstract_socket == 0) {
 		if (unlink(socket_name) != 0 && errno != ENOENT) {
 			uwsgi_error("error removing unix socket, unlink()");
 		}
 	}
 
 	if (abstract_socket == 1) {
```

### Comparing `uwsgi-2.0.8/core/spooler.c` & `uwsgi-2.0.9/core/spooler.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/ssl.c` & `uwsgi-2.0.9/core/ssl.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/static.c` & `uwsgi-2.0.9/core/static.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/stats.c` & `uwsgi-2.0.9/core/stats.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/storage.c` & `uwsgi-2.0.9/core/storage.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/strings.c` & `uwsgi-2.0.9/core/strings.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/subscription.c` & `uwsgi-2.0.9/core/subscription.c`

 * *Files 1% similar despite different names*

```diff
@@ -675,14 +675,18 @@
 	// make space for uwsgi header
 	ub->pos = 4;
 
 	if (uwsgi_buffer_append_keyval(ub, "key", 3, key, keysize))
 		goto end;
 	if (uwsgi_buffer_append_keyval(ub, "address", 7, socket_name, strlen(socket_name)))
 		goto end;
+
+	if (uwsgi.subscribe_with_modifier1) {
+		modifier1 = atoi(uwsgi.subscribe_with_modifier1);
+	}
 	if (uwsgi_buffer_append_keynum(ub, "modifier1", 9, modifier1))
 		goto end;
 	if (uwsgi_buffer_append_keynum(ub, "modifier2", 9, modifier2))
 		goto end;
 	if (uwsgi_buffer_append_keynum(ub, "cores", 5, uwsgi.numproc * uwsgi.cores))
 		goto end;
 	if (uwsgi_buffer_append_keynum(ub, "load", 4, uwsgi.shared->load))
```

### Comparing `uwsgi-2.0.8/core/timebomb.c` & `uwsgi-2.0.9/core/timebomb.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/transformations.c` & `uwsgi-2.0.9/core/transformations.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/utils.c` & `uwsgi-2.0.9/core/utils.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/uwsgi.c` & `uwsgi-2.0.9/core/uwsgi.c`

 * *Files 0% similar despite different names*

```diff
@@ -628,14 +628,17 @@
 	{"st", required_argument, 0, "subscribe to the specified subscription server", uwsgi_opt_add_string_list, &uwsgi.subscriptions, UWSGI_OPT_MASTER},
 	{"subscribe", required_argument, 0, "subscribe to the specified subscription server", uwsgi_opt_add_string_list, &uwsgi.subscriptions, UWSGI_OPT_MASTER},
 	{"subscribe2", required_argument, 0, "subscribe to the specified subscription server using advanced keyval syntax", uwsgi_opt_add_string_list, &uwsgi.subscriptions2, UWSGI_OPT_MASTER},
 	{"subscribe-freq", required_argument, 0, "send subscription announce at the specified interval", uwsgi_opt_set_int, &uwsgi.subscribe_freq, 0},
 	{"subscription-tolerance", required_argument, 0, "set tolerance for subscription servers", uwsgi_opt_set_int, &uwsgi.subscription_tolerance, 0},
 	{"unsubscribe-on-graceful-reload", no_argument, 0, "force unsubscribe request even during graceful reload", uwsgi_opt_true, &uwsgi.unsubscribe_on_graceful_reload, 0},
 	{"start-unsubscribed", no_argument, 0, "configure subscriptions but do not send them (useful with master fifo)", uwsgi_opt_true, &uwsgi.subscriptions_blocked, 0},
+
+	{"subscribe-with-modifier1", required_argument, 0, "force the specififed modifier1 when subscribing", uwsgi_opt_set_str, &uwsgi.subscribe_with_modifier1, UWSGI_OPT_MASTER},
+
 	{"snmp", optional_argument, 0, "enable the embedded snmp server", uwsgi_opt_snmp, NULL, 0},
 	{"snmp-community", required_argument, 0, "set the snmp community string", uwsgi_opt_snmp_community, NULL, 0},
 #ifdef UWSGI_SSL
 	{"ssl-verbose", no_argument, 0, "be verbose about SSL errors", uwsgi_opt_true, &uwsgi.ssl_verbose, 0},
 	// force master, as ssl sessions caching initialize locking early
 	{"ssl-sessions-use-cache", optional_argument, 0, "use uWSGI cache for ssl sessions storage", uwsgi_opt_set_str, &uwsgi.ssl_sessions_use_cache, UWSGI_OPT_MASTER},
 	{"ssl-session-use-cache", optional_argument, 0, "use uWSGI cache for ssl sessions storage", uwsgi_opt_set_str, &uwsgi.ssl_sessions_use_cache, UWSGI_OPT_MASTER},
@@ -855,14 +858,16 @@
 
 	{"add-header", required_argument, 0, "automatically add HTTP headers to response", uwsgi_opt_add_string_list, &uwsgi.additional_headers, 0},
 	{"rem-header", required_argument, 0, "automatically remove specified HTTP header from the response", uwsgi_opt_add_string_list, &uwsgi.remove_headers, 0},
 	{"del-header", required_argument, 0, "automatically remove specified HTTP header from the response", uwsgi_opt_add_string_list, &uwsgi.remove_headers, 0},
 	{"collect-header", required_argument, 0, "store the specified response header in a request var (syntax: header var)", uwsgi_opt_add_string_list, &uwsgi.collect_headers, 0},
 	{"response-header-collect", required_argument, 0, "store the specified response header in a request var (syntax: header var)", uwsgi_opt_add_string_list, &uwsgi.collect_headers, 0},
 
+	{"pull-header", required_argument, 0, "store the specified response header in a request var and remove it from the response (syntax: header var)", uwsgi_opt_add_string_list, &uwsgi.pull_headers, 0},
+
 	{"check-static", required_argument, 0, "check for static files in the specified directory", uwsgi_opt_check_static, NULL, UWSGI_OPT_MIME},
 	{"check-static-docroot", no_argument, 0, "check for static files in the requested DOCUMENT_ROOT", uwsgi_opt_true, &uwsgi.check_static_docroot, UWSGI_OPT_MIME},
 	{"static-check", required_argument, 0, "check for static files in the specified directory", uwsgi_opt_check_static, NULL, UWSGI_OPT_MIME},
 	{"static-map", required_argument, 0, "map mountpoint to static directory (or file)", uwsgi_opt_static_map, &uwsgi.static_maps, UWSGI_OPT_MIME},
 	{"static-map2", required_argument, 0, "like static-map but completely appending the requested resource to the docroot", uwsgi_opt_static_map, &uwsgi.static_maps2, UWSGI_OPT_MIME},
 	{"static-skip-ext", required_argument, 0, "skip specified extension from staticfile checks", uwsgi_opt_add_string_list, &uwsgi.static_skip_ext, UWSGI_OPT_MIME},
 	{"static-index", required_argument, 0, "search for specified file if a directory is requested", uwsgi_opt_add_string_list, &uwsgi.static_index, UWSGI_OPT_MIME},
```

### Comparing `uwsgi-2.0.8/core/websockets.c` & `uwsgi-2.0.9/core/websockets.c`

 * *Files identical despite different names*

```diff
@@ -269,14 +269,15 @@
 				case 2:
 					if (wsgi_req->websocket_has_mask) {
 						wsgi_req->websocket_need += 4;
 						wsgi_req->websocket_phase = 3;
 					}
 					else {
 						wsgi_req->websocket_need += wsgi_req->websocket_size;
+						wsgi_req->websocket_pktsize += wsgi_req->websocket_size;
 						wsgi_req->websocket_phase = 4;
 					}
 					break;
 				// mask
 				case 3:
 					wsgi_req->websocket_pktsize += wsgi_req->websocket_size;
 					wsgi_req->websocket_need += wsgi_req->websocket_size;
```

### Comparing `uwsgi-2.0.8/core/writer.c` & `uwsgi-2.0.9/core/writer.c`

 * *Files 0% similar despite different names*

```diff
@@ -120,17 +120,26 @@
 	return -1;
 }
 
 //each protocol has its header generator
 static int uwsgi_response_add_header_do(struct wsgi_request *wsgi_req, char *key, uint16_t key_len, char *value, uint16_t value_len) {
 
 
-	// collect the header ?
+	// pull/collect the header ?
 	struct uwsgi_string_list *usl = NULL;
 
+	uwsgi_foreach(usl, uwsgi.pull_headers) {
+                if (!uwsgi_strnicmp(key, key_len, usl->value, usl->custom)) {
+                        if (!uwsgi_req_append(wsgi_req, usl->custom_ptr, usl->custom2, value, value_len)) {
+                                wsgi_req->write_errors++ ; return -1;
+                        }
+			return 0;
+                }
+        }
+
 	uwsgi_foreach(usl, uwsgi.collect_headers) {
 		if (!uwsgi_strnicmp(key, key_len, usl->value, usl->custom)) {
 			if (!uwsgi_req_append(wsgi_req, usl->custom_ptr, usl->custom2, value, value_len)) {
 				wsgi_req->write_errors++ ; return -1;
 			}
 		}
 	}
```

### Comparing `uwsgi-2.0.8/core/xmlconf.c` & `uwsgi-2.0.9/core/xmlconf.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/yaml.c` & `uwsgi-2.0.9/core/yaml.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/zeus.c` & `uwsgi-2.0.9/core/zeus.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/core/zlib.c` & `uwsgi-2.0.9/core/zlib.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/config17.ru` & `uwsgi-2.0.9/examples/config17.ru`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/config30.ru` & `uwsgi-2.0.9/examples/config30.ru`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/corostream.pl` & `uwsgi-2.0.9/examples/corostream.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/fibers.ru` & `uwsgi-2.0.9/examples/fibers.ru`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/heavytest.py` & `uwsgi-2.0.9/examples/heavytest.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/info_uwsgi.php` & `uwsgi-2.0.9/examples/info_uwsgi.php`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/logic.ini` & `uwsgi-2.0.9/examples/logic.ini`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/mjpeg_stream.py` & `uwsgi-2.0.9/examples/mjpeg_stream.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/multi.xml` & `uwsgi-2.0.9/examples/multi.xml`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/multiapp.py` & `uwsgi-2.0.9/examples/multiapp.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/router.lua` & `uwsgi-2.0.9/examples/router.lua`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/simple_app.py` & `uwsgi-2.0.9/examples/simple_app.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/taskqueue.py` & `uwsgi-2.0.9/examples/taskqueue.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/uwsgi.xml` & `uwsgi-2.0.9/examples/uwsgi.xml`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/uwsgirouter.py` & `uwsgi-2.0.9/examples/uwsgirouter.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/uwsgistatus.py` & `uwsgi-2.0.9/examples/uwsgistatus.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/welcome.py` & `uwsgi-2.0.9/examples/welcome.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/welcome3.py` & `uwsgi-2.0.9/examples/welcome3.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/werkzeug.yml` & `uwsgi-2.0.9/examples/werkzeug.yml`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/xmlindex-html.xsl` & `uwsgi-2.0.9/examples/xmlindex-html.xsl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/examples/xmlindex.ini` & `uwsgi-2.0.9/examples/xmlindex.ini`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/ext/uwsgi/extconf.rb` & `uwsgi-2.0.9/ext/uwsgi/extconf.rb`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/install.sh` & `uwsgi-2.0.9/install.sh`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/lib/linux_ns.c` & `uwsgi-2.0.9/lib/linux_ns.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/lib/netlink.c` & `uwsgi-2.0.9/lib/netlink.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/lib/sun_fixes.c` & `uwsgi-2.0.9/lib/sun_fixes.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/logo_uWSGI.png` & `uwsgi-2.0.9/logo_uWSGI.png`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/logo_uWSGI.svg` & `uwsgi-2.0.9/logo_uWSGI.svg`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/mongrel2-uwsgi.conf` & `uwsgi-2.0.9/mongrel2-uwsgi.conf`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/airbrake/airbrake_plugin.c` & `uwsgi-2.0.9/plugins/airbrake/airbrake_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/alarm_curl/alarm_curl_plugin.c` & `uwsgi-2.0.9/plugins/alarm_curl/alarm_curl_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/alarm_speech/alarm_speech.m` & `uwsgi-2.0.9/plugins/alarm_speech/alarm_speech.m`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/alarm_xmpp/alarm_xmpp_plugin.c` & `uwsgi-2.0.9/plugins/alarm_xmpp/alarm_xmpp_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/alarm_xmpp/gloox.cc` & `uwsgi-2.0.9/plugins/alarm_xmpp/gloox.cc`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/asyncio/asyncio.c` & `uwsgi-2.0.9/plugins/asyncio/asyncio.c`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 	if (!uwsgi.schedule_to_req) {
 		uwsgi.schedule_to_req = async_schedule_to_req_green;
 	}
 	else {
 		uwsgi.schedule_fix = uwsgi_asyncio_schedule_fix;
 	}
 
-#ifndef UWSGI_PYTHREE
+#ifndef PYTHREE
 	PyObject *asyncio = PyImport_ImportModule("trollius");
 #else
 	PyObject *asyncio = PyImport_ImportModule("asyncio");
 #endif
 	if (!asyncio) uwsgi_pyexit;
 
 	uasyncio.mod = asyncio;
```

### Comparing `uwsgi-2.0.8/plugins/cache/cache.c` & `uwsgi-2.0.9/plugins/cache/cache.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/carbon/carbon.c` & `uwsgi-2.0.9/plugins/carbon/carbon.c`

 * *Files 1% similar despite different names*

```diff
@@ -67,24 +67,27 @@
 
 	while(usl) {
 		struct carbon_server_list *u_server = uwsgi_calloc(sizeof(struct carbon_server_list));
 		u_server->healthy = 1;
 		u_server->errors = 0;
 
 		char *p, *ctx = NULL;
-		uwsgi_foreach_token(usl->value, ":", p, ctx) {
+		// make a copy to not clobber argv
+		char *tmp = uwsgi_str(usl->value);
+		uwsgi_foreach_token(tmp, ":", p, ctx) {
 			if (!u_server->hostname) {
 				u_server->hostname = uwsgi_str(p);
 			}
 			else if (!u_server->port) {
 				u_server->port = uwsgi_str(p);
 			}
 			else
 				break;
 		}
+		free(tmp);
 		if (!u_server->hostname || !u_server->port) {
 			uwsgi_log("[carbon] invalid carbon server address (%s)\n", usl->value);
 			usl = usl->next;
 
 			if (u_server->hostname) free(u_server->hostname);
 			if (u_server->port) free(u_server->port);
 			free(u_server);
```

### Comparing `uwsgi-2.0.8/plugins/cgi/cgi_plugin.c` & `uwsgi-2.0.9/plugins/cgi/cgi_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/cheaper_backlog2/cheaper_backlog2.c` & `uwsgi-2.0.9/plugins/cheaper_backlog2/cheaper_backlog2.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/cheaper_busyness/cheaper_busyness.c` & `uwsgi-2.0.9/plugins/cheaper_busyness/cheaper_busyness.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/clock_monotonic/clock_monotonic.c` & `uwsgi-2.0.9/plugins/clock_monotonic/clock_monotonic.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/clock_realtime/clock_realtime.c` & `uwsgi-2.0.9/plugins/clock_realtime/clock_realtime.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/corerouter/corerouter.c` & `uwsgi-2.0.9/plugins/corerouter/corerouter.c`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,20 @@
 		close(peer->fd);
 		peer->session->corerouter->cr_table[peer->fd] = NULL;
 		peer->fd = -1;
 		peer->hook_read = NULL;
 		peer->hook_write = NULL;
 	}
 
+	if (peer->is_buffering) {
+		if (peer->buffering_fd != -1) {
+			close(peer->buffering_fd);
+		}
+	}
+
 	peer->failed = 0;
 	peer->soopt = 0;
 	peer->timed_out = 0;
 
 	peer->un = NULL;
 	peer->static_node = NULL;
 }
```

### Comparing `uwsgi-2.0.8/plugins/corerouter/cr.h` & `uwsgi-2.0.9/plugins/corerouter/cr.h`

 * *Files 0% similar despite different names*

```diff
@@ -176,27 +176,30 @@
 
 	// can retry ?
 	int can_retry;
 	// how many retries ?
 	uint16_t retries;
 
 	// parsed key
-        char *key;
-        uint16_t key_len;
+        char key[0xff];
+        uint8_t key_len;
 
 	uint8_t modifier1;
 	uint8_t modifier2;
 
 	struct corerouter_peer *prev;
 	struct corerouter_peer *next;
 
 	int current_timeout;
 
 	ssize_t (*flush)(struct corerouter_peer *);
+
 	int is_flushing;
+	int is_buffering;
+        int buffering_fd;
 };
 
 struct uwsgi_corerouter {
 
 	char *name;
 	char *short_name;
 	size_t session_size;
```

### Comparing `uwsgi-2.0.8/plugins/corerouter/cr_common.c` & `uwsgi-2.0.9/plugins/corerouter/cr_common.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/corerouter/cr_map.c` & `uwsgi-2.0.9/plugins/corerouter/cr_map.c`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 int uwsgi_cr_map_use_subscription(struct uwsgi_corerouter *ucr, struct corerouter_peer *peer) {
 
 	peer->un = uwsgi_get_subscribe_node(ucr->subscriptions, peer->key, peer->key_len);
 	if (peer->un && peer->un->len) {
 		peer->instance_address = peer->un->name;
 		peer->instance_address_len = peer->un->len;
 		peer->modifier1 = peer->un->modifier1;
+		peer->modifier2 = peer->un->modifier2;
 	}
 	else if (ucr->cheap && !ucr->i_am_cheap && uwsgi_no_subscriptions(ucr->subscriptions)) {
 		uwsgi_gateway_go_cheap(ucr->name, ucr->queue, &ucr->i_am_cheap);
 	}
 
 	return 0;
 }
@@ -84,14 +85,15 @@
 		}
 	}
 
         if (peer->un && peer->un->len) {
                 peer->instance_address = peer->un->name;
                 peer->instance_address_len = peer->un->len;
                 peer->modifier1 = peer->un->modifier1;
+                peer->modifier2 = peer->un->modifier2;
         }
         else if (ucr->cheap && !ucr->i_am_cheap && uwsgi_no_subscriptions(ucr->subscriptions)) {
                 uwsgi_gateway_go_cheap(ucr->name, ucr->queue, &ucr->i_am_cheap);
         }
 
         return 0;
 }
```

### Comparing `uwsgi-2.0.8/plugins/coroae/coroae.c` & `uwsgi-2.0.9/plugins/coroae/coroae.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/coroae/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/coroae/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/cplusplus/base.cc` & `uwsgi-2.0.9/plugins/cplusplus/base.cc`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/curl_cron/curl_cron.c` & `uwsgi-2.0.9/plugins/curl_cron/curl_cron.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/dumbloop/dumb.c` & `uwsgi-2.0.9/plugins/dumbloop/dumb.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/emperor_amqp/amqp.c` & `uwsgi-2.0.9/plugins/emperor_amqp/amqp.c`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 #include "../../uwsgi.h"
 
 #define AMQP_CONNECTION_HEADER "AMQP\0\0\x09\x01"
 
-#ifdef __BIG_ENDIAN__
-#define ntohll(x) x
-#else
-#define ntohll(x) ( ( (uint64_t)(ntohl( (uint32_t)((x << 32) >> 32) )) << 32) | ntohl( ((uint32_t)(x >> 32)) ) )     
-#endif
-#define htonll(x) ntohll(x)
-
 #define amqp_send(a, b, c) if (send(a, b, c, 0) < 0) { uwsgi_error("send()"); return -1; }
 
 struct amqp_frame_header {
 
 	char type;
 	uint16_t channel;
 	uint32_t size;
@@ -65,50 +58,48 @@
 
 	*lv = ntohl(tmp_long);
 	return ptr+4;
 }
 
 static char *amqp_get_longlong(char *ptr, char *watermark, uint64_t *llv) {
 
-        uint64_t tmp_longlong;
-
 	if (ptr+8 > watermark) return NULL;
-
-        memcpy(&tmp_longlong, ptr, 8);
-
-        *llv = ntohll(tmp_longlong);
+        *llv = uwsgi_be64(ptr);
         return ptr+8;
 }
 
 
 
 static int amqp_send_ack(int fd, uint64_t delivery_tag) {
 
 	uint32_t size = 4 + 8 + 1;
 
-        size = htonl(size);
+	struct uwsgi_buffer *ub = uwsgi_buffer_new(64);
         // send type and channel
-        amqp_send(fd, "\1\0\1", 3);
+	if (uwsgi_buffer_append(ub, "\1\0\1", 3)) goto end;
         // send size
-        amqp_send(fd, &size, 4);
-
-        // send class 60 method 80
-        amqp_send(fd, "\x00\x3C\x00\x50", 4);
-
+	if (uwsgi_buffer_u32be(ub, size)) goto end;
+	// send class 60 method 80
+	if (uwsgi_buffer_append(ub, "\x00\x3C\x00\x50", 4)) goto end;
 	// set delivery_tag
-	delivery_tag = htonll(delivery_tag);
-	amqp_send(fd, &delivery_tag, 8);
+	if (uwsgi_buffer_u64be(ub, delivery_tag)) goto end;
+	if (uwsgi_buffer_append(ub, "\0\xCE", 2)) goto end;
 
-        // empty bits
-        amqp_send(fd, "\0", 1);
+        // send buffer to socket
+        if (write(fd, ub->buf, ub->pos) < 0) {
+		uwsgi_error("amqp_send_ack()/write()");
+		goto end;
+	}
 
-        // send frame-end
-        amqp_send(fd, "\xCE", 1);
 
+	uwsgi_buffer_destroy(ub);	
 	return 0;
+end:
+	uwsgi_buffer_destroy(ub);
+	return -1;
 }
 
 char *uwsgi_amqp_consume(int fd, uint64_t *msgsize, char **routing_key) {
 
 	uint32_t size;
 	struct amqp_frame_header fh;
 	uint64_t delivery_tag;
```

### Comparing `uwsgi-2.0.8/plugins/emperor_amqp/emperor_amqp.c` & `uwsgi-2.0.9/plugins/emperor_amqp/emperor_amqp.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/emperor_mongodb/emperor_mongodb.cc` & `uwsgi-2.0.9/plugins/emperor_mongodb/emperor_mongodb.cc`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/emperor_mongodb/plugin.c` & `uwsgi-2.0.9/plugins/emperor_mongodb/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/emperor_pg/emperor_pg.c` & `uwsgi-2.0.9/plugins/emperor_pg/emperor_pg.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/emperor_zeromq/emperor_zeromq.c` & `uwsgi-2.0.9/plugins/emperor_zeromq/emperor_zeromq.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/example/example_plugin.c` & `uwsgi-2.0.9/plugins/example/example_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/exception_log/exception_log.c` & `uwsgi-2.0.9/plugins/exception_log/exception_log.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/fastrouter/fastrouter.c` & `uwsgi-2.0.9/plugins/fastrouter/fastrouter.c`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 } ufr;
 
 extern struct uwsgi_server uwsgi;
 
 struct fastrouter_session {
 	struct corerouter_session session;
 	int has_key;
+	uint64_t content_length;
+	uint64_t buffered;
 };
 
 static struct uwsgi_option fastrouter_options[] = {
 	{"fastrouter", required_argument, 0, "run the fastrouter on the specified port", uwsgi_opt_corerouter, &ufr, 0},
 	{"fastrouter-processes", required_argument, 0, "prefork the specified number of fastrouter processes", uwsgi_opt_set_int, &ufr.cr.processes, 0},
 	{"fastrouter-workers", required_argument, 0, "prefork the specified number of fastrouter processes", uwsgi_opt_set_int, &ufr.cr.processes, 0},
 	{"fastrouter-zerg", required_argument, 0, "attach the fastrouter to a zerg server", uwsgi_opt_corerouter_zerg, &ufr, 0},
@@ -38,15 +40,15 @@
 	{"fastrouter-quiet", required_argument, 0, "do not report failed connections to instances", uwsgi_opt_true, &ufr.cr.quiet, 0},
 	{"fastrouter-cheap", no_argument, 0, "run the fastrouter in cheap mode", uwsgi_opt_true, &ufr.cr.cheap, 0},
 	{"fastrouter-subscription-server", required_argument, 0, "run the fastrouter subscription server on the specified address", uwsgi_opt_corerouter_ss, &ufr, 0},
 	{"fastrouter-subscription-slot", required_argument, 0, "*** deprecated ***", uwsgi_opt_deprecated, (void *) "useless thanks to the new implementation", 0},
 
 	{"fastrouter-timeout", required_argument, 0, "set fastrouter timeout", uwsgi_opt_set_int, &ufr.cr.socket_timeout, 0},
 	{"fastrouter-post-buffering", required_argument, 0, "enable fastrouter post buffering", uwsgi_opt_set_64bit, &ufr.cr.post_buffering, 0},
-	{"fastrouter-post-buffering-dir", required_argument, 0, "put fastrouter buffered files to the specified directory", uwsgi_opt_set_str, &ufr.cr.pb_base_dir, 0},
+	{"fastrouter-post-buffering-dir", required_argument, 0, "put fastrouter buffered files to the specified directory (noop, use TMPDIR env)", uwsgi_opt_set_str, &ufr.cr.pb_base_dir, 0},
 
 	{"fastrouter-stats", required_argument, 0, "run the fastrouter stats server", uwsgi_opt_set_str, &ufr.cr.stats_server, 0},
 	{"fastrouter-stats-server", required_argument, 0, "run the fastrouter stats server", uwsgi_opt_set_str, &ufr.cr.stats_server, 0},
 	{"fastrouter-ss", required_argument, 0, "run the fastrouter stats server", uwsgi_opt_set_str, &ufr.cr.stats_server, 0},
 	{"fastrouter-harakiri", required_argument, 0, "enable fastrouter harakiri", uwsgi_opt_set_int, &ufr.cr.harakiri, 0},
 
 	{"fastrouter-uid", required_argument, 0, "drop fastrouter privileges to the specified uid", uwsgi_opt_uid, &ufr.cr.uid, 0 },
@@ -62,29 +64,35 @@
 static void fr_get_hostname(char *key, uint16_t keylen, char *val, uint16_t vallen, void *data) {
 
 	struct corerouter_peer *peer = (struct corerouter_peer *) data;
 	struct fastrouter_session *fr = (struct fastrouter_session *) peer->session;
 
 	//uwsgi_log("%.*s = %.*s\n", keylen, key, vallen, val);
 	if (!uwsgi_strncmp("SERVER_NAME", 11, key, keylen) && !peer->key_len) {
-		peer->key = val;
-		peer->key_len = vallen;
+		if (vallen <= 0xff) {
+			memcpy(peer->key, val, vallen);
+			peer->key_len = vallen;
+		}
 		return;
 	}
 
 	if (!uwsgi_strncmp("HTTP_HOST", 9, key, keylen) && !fr->has_key) {
-		peer->key = val;
-		peer->key_len = vallen;
+		if (vallen <= 0xff) {
+                        memcpy(peer->key, val, vallen);
+                        peer->key_len = vallen;
+                }
 		return;
 	}
 
 	if (!uwsgi_strncmp("UWSGI_FASTROUTER_KEY", 20, key, keylen)) {
-		fr->has_key = 1;
-		peer->key = val;
-		peer->key_len = vallen;
+		if (vallen <= 0xff) {
+			fr->has_key = 1;
+                        memcpy(peer->key, val, vallen);
+                        peer->key_len = vallen;
+		}
 		return;
 	}
 
 	if (!uwsgi_strncmp("REMOTE_ADDR", 11, key, keylen)) {
 		if (vallen < sizeof(peer->session->client_address)) {
 			strncpy(peer->session->client_address, val, vallen);
 		}
@@ -93,14 +101,20 @@
 
 	if (!uwsgi_strncmp("REMOTE_PORT", 11, key, keylen)) {
 		if (vallen < sizeof(peer->session->client_port)) {
 			strncpy(peer->session->client_port, val, vallen);
 		}
                 return;
         }
+
+	if (ufr.cr.post_buffering > 0) {
+		if (!uwsgi_strncmp("CONTENT_LENGTH", 14, key, keylen)) {
+			fr->content_length = uwsgi_str_num(val, vallen);
+		}
+	}
 }
 
 // writing client body to the instance
 static ssize_t fr_instance_write_body(struct corerouter_peer *peer) {
 	ssize_t len = cr_write(peer, "fr_instance_write_body()");
         // end on empty write
         if (!len) return 0;
@@ -153,68 +167,145 @@
         peer->session->main_peer->out = peer->in;
         peer->session->main_peer->out_pos = 0;
 
         cr_write_to_main(peer, fr_write);
         return len;
 }
 
+static ssize_t fr_instance_sendfile(struct corerouter_peer *peer) {
+	struct fastrouter_session *fr = (struct fastrouter_session *) peer->session;
+	ssize_t len = uwsgi_sendfile_do(peer->fd, peer->session->main_peer->buffering_fd, fr->buffered, fr->content_length - fr->buffered);
+	if (len < 0) {
+		cr_try_again;
+		uwsgi_cr_error(peer, "fr_instance_sendfile()/sendfile()");
+		return -1;
+	}
+	if (len == 0) return 0;
+	fr->buffered += len;
+	if (peer != peer->session->main_peer && peer->un) peer->un->rx+=len;
+	if (fr->buffered >= fr->content_length) {
+		cr_reset_hooks(peer);	
+	}
+	return len;
+}
+
 // send the uwsgi request header and vars
 static ssize_t fr_instance_send_request(struct corerouter_peer *peer) {
 	ssize_t len = cr_write(peer, "fr_instance_send_request()");
         // end on empty write
         if (!len) return 0;
 
         // the chunk has been sent, start (again) reading from client and instances
         if (cr_write_complete(peer)) {
                 // reset the original read buffer
                 peer->out->pos = 0;
-		// start waiting for body
-		peer->session->main_peer->last_hook_read = fr_read_body;
-                cr_reset_hooks(peer);
+		if (!peer->session->main_peer->is_buffering) {
+			// start waiting for body
+			peer->session->main_peer->last_hook_read = fr_read_body;
+                	cr_reset_hooks(peer);
+		}
+		else {
+			peer->hook_write = fr_instance_sendfile;
+			// stop reading from the client
+			peer->session->main_peer->last_hook_read = NULL;
+		}
         }
 
 	return len;
 }
 
 // instance is connected
 static ssize_t fr_instance_connected(struct corerouter_peer *peer) {
 
 	cr_peer_connected(peer, "fr_instance_connected()");
 
 	// we are connected, we cannot retry anymore
 	peer->can_retry = 0;
 
 	// fix modifiers
-	peer->in->buf[0] = peer->session->main_peer->modifier1;
-	peer->in->buf[3] = peer->session->main_peer->modifier2;
+	peer->in->buf[0] = peer->modifier1;
+	peer->in->buf[3] = peer->modifier2;
 
 	// prepare to write the uwsgi packet
 	peer->out = peer->session->main_peer->in;
 	peer->out_pos = 0;	
 
 	peer->last_hook_write = fr_instance_send_request;
 	return fr_instance_send_request(peer);
 }
 
 // called after receaving the uwsgi header (read vars)
 static ssize_t fr_recv_uwsgi_vars(struct corerouter_peer *main_peer) {
+	struct fastrouter_session *fr = (struct fastrouter_session *) main_peer->session;
+
+	struct corerouter_peer *new_peer = NULL;
+	ssize_t len = 0;
+
 	struct uwsgi_header *uh = (struct uwsgi_header *) main_peer->in->buf;
 	// better to store it as the original buf address could change
 	uint16_t pktsize = uh->pktsize;
+
+	// are we buffering ?
+	if (main_peer->is_buffering) {
+		// memory or disk ?
+		if (fr->content_length <= ufr.cr.post_buffering) {
+			// increase buffer if needed
+        		if (uwsgi_buffer_fix(main_peer->in, pktsize+4+fr->content_length))
+                		return -1;
+        		len = cr_read_exact(main_peer, pktsize+4+fr->content_length, "fr_recv_uwsgi_vars()");
+        		if (!len) return 0;
+			// whole body read ?
+			if (main_peer->in->pos == (size_t)(pktsize+4+fr->content_length)) {
+				main_peer->is_buffering = 0;
+				goto done;
+			}
+			return len;
+		}
+		// first round ?
+		if (main_peer->buffering_fd == -1) {
+			main_peer->buffering_fd = uwsgi_tmpfd();
+			if (main_peer->buffering_fd < 0) return -1;
+		}
+		char buf[32768];
+		size_t remains = fr->content_length - fr->buffered;
+		ssize_t rlen = read(main_peer->fd, buf, UMIN(32768, remains));
+		if (rlen < 0) {
+			cr_try_again;
+			uwsgi_cr_error(main_peer, "fr_recv_uwsgi_vars()/read()");
+			return -1;
+		}
+		if (rlen == 0) return 0;
+		fr->buffered += rlen;
+		if (write(main_peer->buffering_fd, buf, rlen) != rlen) {
+			uwsgi_cr_error(main_peer, "fr_recv_uwsgi_vars()/write()");
+                        return -1;
+		}
+
+		// have we done ?
+		if (fr->buffered >= fr->content_length) {
+			fr->buffered = 0;
+			len = rlen;
+			goto done;
+		}
+
+		return rlen;
+	}
+
 	// increase buffer if needed
 	if (uwsgi_buffer_fix(main_peer->in, pktsize+4))
 		return -1;
-	ssize_t len = cr_read_exact(main_peer, pktsize+4, "fr_recv_uwsgi_vars()");
+	len = cr_read_exact(main_peer, pktsize+4, "fr_recv_uwsgi_vars()");
 	if (!len) return 0;
 
 	// headers received, ready to choose the instance
 	if (main_peer->in->pos == (size_t)(pktsize+4)) {
+
 		struct uwsgi_corerouter *ucr = main_peer->session->corerouter;
 
-		struct corerouter_peer *new_peer = uwsgi_cr_peer_add(main_peer->session);
+		new_peer = uwsgi_cr_peer_add(main_peer->session);
 		new_peer->last_hook_read = fr_instance_read;
 
 		// find the hostname
 		if (uwsgi_hooked_parse(main_peer->in->buf+4, pktsize, fr_get_hostname, (void *) new_peer)) {
 			return -1;
 		}
 
@@ -233,14 +324,26 @@
 				new_peer->can_retry = 1;
 				corerouter_close_peer(&ufr.cr, new_peer);
 				return len;
 			}
 			return -1;
 		}
 
+		// buffering ?
+		if (ufr.cr.post_buffering > 0 && fr->content_length > 0) {
+			main_peer->is_buffering = 1;
+			main_peer->buffering_fd = -1;
+			return len;
+		}
+
+done:
+		if (!new_peer) {
+			new_peer = main_peer->session->peers;
+		}
+
 		new_peer->can_retry = 1;
 
 		cr_connect(new_peer, fr_instance_connected);
 	}
 
 	return len;
 }
```

### Comparing `uwsgi-2.0.8/plugins/fiber/fiber.c` & `uwsgi-2.0.9/plugins/fiber/fiber.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/fiber/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/fiber/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/forkptyrouter/forkptyrouter.c` & `uwsgi-2.0.9/plugins/forkptyrouter/forkptyrouter.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/gccgo/gccgo_plugin.c` & `uwsgi-2.0.9/plugins/gccgo/gccgo_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/gccgo/uwsgi.go` & `uwsgi-2.0.9/plugins/gccgo/uwsgi.go`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/geoip/geoip.c` & `uwsgi-2.0.9/plugins/geoip/geoip.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/gevent/gevent.c` & `uwsgi-2.0.9/plugins/gevent/gevent.c`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,39 @@
 		PyObject_CallMethod(ugevent.ctrl_gl, "kill", NULL);
 	}
 
 	Py_INCREF(Py_None);
 	return Py_None;
 }
 
+PyObject *py_uwsgi_gevent_int(PyObject *self, PyObject *args) {
+
+        uwsgi_log("Brutally killing worker %d (pid: %d)...\n", uwsgi.mywid, uwsgi.mypid);
+        uwsgi.workers[uwsgi.mywid].manage_next_request = 0;
+
+        uwsgi_log_verbose("stopping gevent signals watchers for worker %d (pid: %d)...\n", uwsgi.mywid, uwsgi.mypid);
+        PyObject_CallMethod(ugevent.my_signal_watcher, "stop", NULL);
+        PyObject_CallMethod(ugevent.signal_watcher, "stop", NULL);
+
+        uwsgi_log_verbose("stopping gevent sockets watchers for worker %d (pid: %d)...\n", uwsgi.mywid, uwsgi.mypid);
+        int i,count = uwsgi_count_sockets(uwsgi.sockets);
+        for(i=0;i<count;i++) {
+                PyObject_CallMethod(ugevent.watchers[i], "stop", NULL);
+        }
+        uwsgi_log_verbose("main gevent watchers stopped for worker %d (pid: %d)...\n", uwsgi.mywid, uwsgi.mypid);
+
+        if (!ugevent.wait_for_hub) {
+                PyObject_CallMethod(ugevent.ctrl_gl, "kill", NULL);
+        }
+
+        Py_INCREF(Py_None);
+        return Py_None;
+}
+
+
 static void uwsgi_gevent_gbcw() {
 
 	// already running
 	if (ugevent.destroy) return;
 
 	uwsgi_log("...The work of process %d is done. Seeya!\n", getpid());
 
@@ -329,14 +354,15 @@
 
 PyMethodDef uwsgi_gevent_main_def[] = { {"uwsgi_gevent_main", py_uwsgi_gevent_main, METH_VARARGS, ""} };
 PyMethodDef uwsgi_gevent_request_def[] = { {"uwsgi_gevent_request", py_uwsgi_gevent_request, METH_VARARGS, ""} };
 PyMethodDef uwsgi_gevent_signal_def[] = { {"uwsgi_gevent_signal", py_uwsgi_gevent_signal, METH_VARARGS, ""} };
 PyMethodDef uwsgi_gevent_my_signal_def[] = { {"uwsgi_gevent_my_signal", py_uwsgi_gevent_my_signal, METH_VARARGS, ""} };
 PyMethodDef uwsgi_gevent_signal_handler_def[] = { {"uwsgi_gevent_signal_handler", py_uwsgi_gevent_signal_handler, METH_VARARGS, ""} };
 PyMethodDef uwsgi_gevent_unix_signal_handler_def[] = { {"uwsgi_gevent_unix_signal_handler", py_uwsgi_gevent_graceful, METH_VARARGS, ""} };
+PyMethodDef uwsgi_gevent_unix_signal_int_handler_def[] = { {"uwsgi_gevent_unix_signal_int_handler", py_uwsgi_gevent_int, METH_VARARGS, ""} };
 PyMethodDef uwsgi_gevent_ctrl_gl_def[] = { {"uwsgi_gevent_ctrl_gl_handler", py_uwsgi_gevent_ctrl_gl, METH_VARARGS, ""} };
 
 static void gil_gevent_get() {
 	pthread_setspecific(up.upt_gil_key, (void *) PyGILState_Ensure());
 }
 
 static void gil_gevent_release() {
@@ -484,14 +510,30 @@
 	PyTuple_SetItem(ge_signal_tuple, 0, PyInt_FromLong(SIGHUP));
 	PyObject *uwsgi_gevent_unix_signal_handler = PyCFunction_New(uwsgi_gevent_unix_signal_handler_def, NULL);
         Py_INCREF(uwsgi_gevent_unix_signal_handler);
 	PyTuple_SetItem(ge_signal_tuple, 1, uwsgi_gevent_unix_signal_handler);
 
 	python_call(ugevent.signal, ge_signal_tuple, 0, NULL);
 
+	// map SIGINT/SIGTERM with gevent.signal
+	ge_signal_tuple = PyTuple_New(2);
+	PyTuple_SetItem(ge_signal_tuple, 0, PyInt_FromLong(SIGINT));
+	PyObject *uwsgi_gevent_unix_signal_int_handler = PyCFunction_New(uwsgi_gevent_unix_signal_int_handler_def, NULL);
+        Py_INCREF(uwsgi_gevent_unix_signal_int_handler);
+	PyTuple_SetItem(ge_signal_tuple, 1, uwsgi_gevent_unix_signal_int_handler);
+	python_call(ugevent.signal, ge_signal_tuple, 0, NULL);
+
+	ge_signal_tuple = PyTuple_New(2);
+	PyTuple_SetItem(ge_signal_tuple, 0, PyInt_FromLong(SIGTERM));
+	PyTuple_SetItem(ge_signal_tuple, 1, uwsgi_gevent_unix_signal_int_handler);
+	python_call(ugevent.signal, ge_signal_tuple, 0, NULL);
+
+
+
+
 	PyObject *wait_for_me = ugevent.hub;
 
 	if (!ugevent.wait_for_hub) {
 		// spawn the control greenlet
 		PyObject *uwsgi_greenlet_ctrl_gl_handler = PyCFunction_New(uwsgi_gevent_ctrl_gl_def, NULL);
                 Py_INCREF(uwsgi_greenlet_ctrl_gl_handler);
 		PyObject *ctrl_gl_args = PyTuple_New(1);
```

### Comparing `uwsgi-2.0.8/plugins/gevent/gevent.h` & `uwsgi-2.0.9/plugins/gevent/gevent.h`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/gevent/hooks.c` & `uwsgi-2.0.9/plugins/gevent/hooks.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/glusterfs/glusterfs.c` & `uwsgi-2.0.9/plugins/glusterfs/glusterfs.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/graylog2/graylog2_plugin.c` & `uwsgi-2.0.9/plugins/graylog2/graylog2_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/greenlet/greenlet.c` & `uwsgi-2.0.9/plugins/greenlet/greenlet.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/gridfs/gridfs.cc` & `uwsgi-2.0.9/plugins/gridfs/gridfs.cc`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/gridfs/plugin.c` & `uwsgi-2.0.9/plugins/gridfs/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/http/common.h` & `uwsgi-2.0.9/plugins/http/common.h`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/http/http.c` & `uwsgi-2.0.9/plugins/http/http.c`

 * *Files 2% similar despite different names*

```diff
@@ -137,17 +137,22 @@
 			hr->websocket_key = val;
 			hr->websocket_key_len = vallen;
 			goto done;
 		}
 	}	
 
 	if (!uwsgi_strncmp("HOST", 4, hh, keylen)) {
-		peer->key = val;
-		peer->key_len = vallen;
-		if (uhttp.server_name_as_http_host && uwsgi_buffer_append_keyval(out, "SERVER_NAME", 11, peer->key, peer->key_len)) return -1;
+		if (vallen <= 0xff) {
+			memcpy(peer->key, val, vallen);
+			peer->key_len = vallen;
+			if (uhttp.server_name_as_http_host && uwsgi_buffer_append_keyval(out, "SERVER_NAME", 11, peer->key, peer->key_len)) return -1;
+		}
+		else {
+			return -1;
+		}
 	}
 
 	else if (!uwsgi_strncmp("CONTENT_LENGTH", 14, hh, keylen)) {
 		hr->content_length = uwsgi_str_num(val, vallen);
 	}
 
 	// in the future we could support chunked requests...
@@ -162,16 +167,18 @@
 
 	else if (!uwsgi_strncmp("CONNECTION", 10, hh, keylen)) {
 		if (!uwsgi_strnicmp(val, vallen, "close", 5) || !uwsgi_strnicmp(val, vallen, "upgrade", 7)) {
 			hr->session.can_keepalive = 0;
 		}
 	}
 	else if (peer->key == uwsgi.hostname && hr->raw_body && !uwsgi_strncmp("ICE_URL", 7, hh, keylen)) {
-		peer->key = val;
-		peer->key_len = vallen;
+		if (vallen <= 0xff) {
+                        memcpy(peer->key, val, vallen);
+                        peer->key_len = vallen;
+		}
 	}
 
 #ifdef UWSGI_ZLIB
 	else if (uhttp.auto_gzip && !uwsgi_strncmp("ACCEPT_ENCODING", 15, hh, keylen)) {
 		if ( uwsgi_contains_n(val, vallen, "gzip", 4) ) {
 			hr->can_gzip = 1;
 		}
@@ -341,15 +348,15 @@
         }
 
 	// SCRIPT_NAME
 	if (uwsgi_buffer_append_keyval(out, "SCRIPT_NAME", 11, "", 0)) return -1;
 
 	// SERVER_NAME
 	if (!uhttp.server_name_as_http_host && uwsgi_buffer_append_keyval(out, "SERVER_NAME", 11, uwsgi.hostname, uwsgi.hostname_len)) return -1;
-	peer->key = uwsgi.hostname;
+	memcpy(peer->key, uwsgi.hostname, uwsgi.hostname_len);
 	peer->key_len = uwsgi.hostname_len;
 
 	// SERVER_PORT
 	if (uwsgi_buffer_append_keyval(out, "SERVER_PORT", 11, hr->port, hr->port_len)) return -1;
 
 	// UWSGI_ROUTER
 	if (uwsgi_buffer_append_keyval(out, "UWSGI_ROUTER", 12, "http", 4)) return -1;
@@ -457,18 +464,20 @@
 		hv = hv->next;
 	}
 
 	if (hr->is_rtsp) {
 		if (uwsgi_starts_with("rtsp://", 7, hr->path_info, hr->path_info_len)) {
 			char *slash = memchr(hr->path_info + 7, '/', hr->path_info_len - 7);
 			if (!slash) return -1;
-			peer->key = hr->path_info + 7;
-			peer->key_len = slash - (hr->path_info + 7);
-			// override PATH_INFO
-			if (uwsgi_buffer_append_keyval(out, "PATH_INFO", 9, slash, hr->path_info_len - (7 + peer->key_len))) return -1;
+			if (slash - (hr->path_info + 7) <= 0xff) {
+				peer->key_len = slash - (hr->path_info + 7);
+				memcpy(peer->key, hr->path_info + 7, peer->key_len);
+				// override PATH_INFO
+				if (uwsgi_buffer_append_keyval(out, "PATH_INFO", 9, slash, hr->path_info_len - (7 + peer->key_len))) return -1;
+			}
 		}
 	}
 
 	return 0;
 
 clear:
 	usl = headers;
@@ -827,18 +836,24 @@
                 	if (ucr->mapper(ucr, new_peer))
                         	return -1;
 
                 	// check instance
                 	if (new_peer->instance_address_len == 0)
                         	return -1;
 
+			// fix modifiers
+			if (uhttp.modifier1)
+				new_peer->modifier1 = uhttp.modifier1;
+			if (uhttp.modifier2)
+				new_peer->modifier2 = uhttp.modifier2;
+
 			uint16_t pktsize = new_peer->out->pos-4;
         		// fix modifiers
-        		new_peer->out->buf[0] = new_peer->session->main_peer->modifier1;
-        		new_peer->out->buf[3] = new_peer->session->main_peer->modifier2;
+        		new_peer->out->buf[0] = new_peer->modifier1;
+        		new_peer->out->buf[3] = new_peer->modifier2;
         		// fix pktsize
         		new_peer->out->buf[1] = (uint8_t) (pktsize & 0xff);
         		new_peer->out->buf[2] = (uint8_t) ((pktsize >> 8) & 0xff);
 
 			if (hr->remains > 0) {
 				if (hr->content_length < hr->remains) { 
 					hr->remains = hr->content_length;
@@ -848,14 +863,20 @@
 				}
 				else {
 					hr->content_length -= hr->remains;
 				}
 				if (uwsgi_buffer_append(new_peer->out, main_peer->in->buf + hr->headers_size + 1, hr->remains)) return -1;
 			}
 
+			if (new_peer->modifier1 == 123) {
+				// reset modifier1 to 0
+				new_peer->out->buf[0] = 0;
+				hr->raw_body = 1;
+			}
+
 			if (hr->websockets > 2 && hr->websocket_key_len > 0) {
 				hr->raw_body = 1;
 			}
 
 			// on raw body, ensure keepalive is disabled
 			if (hr->raw_body) hr->session.can_keepalive = 0;
 
@@ -972,17 +993,14 @@
 
 	if (!uhttp.headers_timeout) uhttp.headers_timeout = uhttp.cr.socket_timeout;
 	if (!uhttp.connect_timeout) uhttp.connect_timeout = uhttp.cr.socket_timeout;
 
 	// set the retry hook
         cs->retry = hr_retry;
 	struct http_session *hr = (struct http_session *) cs;
-	// set the modifier1
-	cs->main_peer->modifier1 = uhttp.modifier1;
-	cs->main_peer->modifier2 = uhttp.modifier2;
 	// default hook
 	cs->main_peer->last_hook_read = hr_read;
 
 	// headers timeout
 	cs->main_peer->current_timeout = uhttp.headers_timeout;
 
 	if (uhttp.raw_body) {
```

### Comparing `uwsgi-2.0.8/plugins/http/https.c` & `uwsgi-2.0.9/plugins/http/https.c`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 
 #include "common.h"
 
 #ifdef UWSGI_SSL
 
 extern struct uwsgi_http uhttp;
 
+// taken from nginx
+static void hr_ssl_clear_errors() {
+	while (ERR_peek_error()) {
+		(void) ERR_get_error();
+	}
+	ERR_clear_error();
+}
+
 void uwsgi_opt_https(char *opt, char *value, void *cr) {
         struct uwsgi_corerouter *ucr = (struct uwsgi_corerouter *) cr;
         char *client_ca = NULL;
 
         // build socket, certificate and key file
         char *sock = uwsgi_str(value);
         char *crt = strchr(sock, ',');
@@ -168,17 +176,17 @@
 
 int hr_https_add_vars(struct http_session *hr, struct corerouter_peer *peer, struct uwsgi_buffer *out) {
 // HTTPS (adapted from nginx)
         if (hr->session.ugs->mode == UWSGI_HTTP_SSL) {
                 if (uwsgi_buffer_append_keyval(out, "HTTPS", 5, "on", 2)) return -1;
 #ifdef SSL_CTRL_SET_TLSEXT_HOSTNAME
 			const char *servername = SSL_get_servername(hr->ssl, TLSEXT_NAMETYPE_host_name);
-                        if (servername) {
-                        	peer->key = (char *) servername;
-                                peer->key_len = strlen(servername);
+                        if (servername && strlen(servername) <= 0xff) {
+				peer->key_len = strlen(servername);
+                        	memcpy(peer->key, servername, peer->key_len) ;
                         }
 #endif
                 hr->ssl_client_cert = SSL_get_peer_certificate(hr->ssl);
                 if (hr->ssl_client_cert) {
                         X509_NAME *name = X509_get_subject_name(hr->ssl_client_cert);
                         if (name) {
                                 hr->ssl_client_dn = X509_NAME_oneline(name, NULL, 0);
@@ -230,15 +238,15 @@
 	if (hr->spdy) {
 		deflateEnd(&hr->spdy_z_in);
 		deflateEnd(&hr->spdy_z_out);
 	}
 #endif
 
 	// clear the errors (otherwise they could be propagated)
-	ERR_clear_error();
+	hr_ssl_clear_errors();
         SSL_free(hr->ssl);
 }
 
 int hr_force_https(struct corerouter_peer *peer) {
 	struct corerouter_session *cs = peer->session;
         struct http_session *hr = (struct http_session *) cs;
 
@@ -266,14 +274,16 @@
         return 0;
 }
 
 ssize_t hr_ssl_write(struct corerouter_peer *main_peer) {
         struct corerouter_session *cs = main_peer->session;
         struct http_session *hr = (struct http_session *) cs;
 
+	hr_ssl_clear_errors();
+
         int ret = SSL_write(hr->ssl, main_peer->out->buf + main_peer->out_pos, main_peer->out->pos - main_peer->out_pos);
         if (ret > 0) {
                 main_peer->out_pos += ret;
                 if (main_peer->out->pos == main_peer->out_pos) {
 			// reset the buffer (if needed)
 			main_peer->out->pos = 0;
 			if (main_peer->session->wait_full_write) {
@@ -290,17 +300,19 @@
 			if (hr->spdy) {
 				return spdy_parse(main_peer);
 			}
 #endif
                 }
                 return ret;
         }
-        if (ret == 0) return 0;
+
         int err = SSL_get_error(hr->ssl, ret);
 
+	if (err == SSL_ERROR_ZERO_RETURN || err == 0) return 0;
+
         if (err == SSL_ERROR_WANT_READ) {
                 cr_reset_hooks_and_read(main_peer, hr_ssl_write);
                 return 1;
         }
 
         else if (err == SSL_ERROR_WANT_WRITE) {
                 cr_write_to_main(main_peer, hr_ssl_write);
@@ -318,14 +330,16 @@
         return -1;
 }
 
 ssize_t hr_ssl_read(struct corerouter_peer *main_peer) {
         struct corerouter_session *cs = main_peer->session;
         struct http_session *hr = (struct http_session *) cs;
 
+	hr_ssl_clear_errors();
+
         // try to always leave 4k available
         if (uwsgi_buffer_ensure(main_peer->in, uwsgi.page_size)) return -1;
         int ret = SSL_read(hr->ssl, main_peer->in->buf + main_peer->in->pos, main_peer->in->len - main_peer->in->pos);
         if (ret > 0) {
                 // fix the buffer
                 main_peer->in->pos += ret;
                 // check for pending data
@@ -346,17 +360,19 @@
                 if (hr->spdy) {
                         //uwsgi_log("RUNNING THE SPDY PARSER FOR %d bytes\n", main_peer->in->pos);
                         return spdy_parse(main_peer);
                 }
 #endif
                 return http_parse(main_peer);
         }
-        if (ret == 0) return 0;
+
         int err = SSL_get_error(hr->ssl, ret);
 
+	if (err == SSL_ERROR_ZERO_RETURN || err == 0) return 0;
+
         if (err == SSL_ERROR_WANT_READ) {
                 cr_reset_hooks_and_read(main_peer, hr_ssl_read);
                 return 1;
         }
 
         else if (err == SSL_ERROR_WANT_WRITE) {
                 cr_write_to_main(main_peer, hr_ssl_read);
@@ -377,26 +393,25 @@
 ssize_t hr_ssl_shutdown(struct corerouter_peer *peer) {
 	// ensure no hooks are set
 	if (uwsgi_cr_set_hooks(peer, NULL, NULL)) return -1;
 
 	struct corerouter_session *cs = peer->session;
         struct http_session *hr = (struct http_session *) cs;	
 
-	int ret = SSL_shutdown(hr->ssl);
-	if (ret < 0) return -1;
-	if (ret == 1) return 0;
+	hr_ssl_clear_errors();
 
+	int ret = SSL_shutdown(hr->ssl);
 	int err = 0;
 
-	if (ERR_peek_error()) {
+	if (ret != 1 && ERR_peek_error()) {
 		err = SSL_get_error(hr->ssl, ret);
 	}
 
 	// no error, close the connection
-	if (err == 0 || err == SSL_ERROR_ZERO_RETURN) return -1;
+	if (ret == 1 || err == 0 || err == SSL_ERROR_ZERO_RETURN) return 0;
 
 	if (err == SSL_ERROR_WANT_READ) {
 		if (uwsgi_cr_set_hooks(peer, hr_ssl_shutdown, NULL)) return -1;
                 return 1;
         }
 
         else if (err == SSL_ERROR_WANT_WRITE) {
```

### Comparing `uwsgi-2.0.8/plugins/http/keepalive.c` & `uwsgi-2.0.9/plugins/http/keepalive.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/http/spdy3.c` & `uwsgi-2.0.9/plugins/http/spdy3.c`

 * *Files 1% similar despite different names*

```diff
@@ -552,16 +552,18 @@
 
 		if (uwsgi_buffer_append_keyval(new_peer->out, cgi_name, nk_len, v, v_len)) {
 			uwsgi_buffer_destroy(ub);
 			return -1;
 		}
 
 		if (!uwsgi_strncmp(cgi_name, nk_len, "HTTP_HOST", 9)) {
-			new_peer->key = new_peer->out->buf + (new_peer->out->pos - v_len);
-			new_peer->key_len = v_len;
+			if (v_len <= 0xff) {
+				memcpy(new_peer->key, new_peer->out->buf + (new_peer->out->pos - v_len), v_len);
+				new_peer->key_len = v_len;
+			}
 		}
 		else if (!uwsgi_strncmp(cgi_name, nk_len, "REQUEST_URI", 11)) {
 			char *path_info = new_peer->out->buf + (new_peer->out->pos - v_len);
 			uint16_t path_info_len = v_len;
 			char *query_string = memchr(path_info, '?', v_len);
 			if (query_string) {
 				query_string++;
```

### Comparing `uwsgi-2.0.8/plugins/http/spdy3.h` & `uwsgi-2.0.9/plugins/http/spdy3.h`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/jvm/jvm.h` & `uwsgi-2.0.9/plugins/jvm/jvm.h`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/jvm/jvm_plugin.c` & `uwsgi-2.0.9/plugins/jvm/jvm_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/jvm/uwsgi.java` & `uwsgi-2.0.9/plugins/jvm/uwsgi.java`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/jvm/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/jvm/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/jwsgi/jwsgi_plugin.c` & `uwsgi-2.0.9/plugins/jwsgi/jwsgi_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/ldap/ldap.c` & `uwsgi-2.0.9/plugins/ldap/ldap.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/legion_cache_fetch/legion_cache_fetch.c` & `uwsgi-2.0.9/plugins/legion_cache_fetch/legion_cache_fetch.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/libffi/libffi.c` & `uwsgi-2.0.9/plugins/libffi/libffi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/libtcc/libtcc.c` & `uwsgi-2.0.9/plugins/libtcc/libtcc.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/logcrypto/logcrypto.c` & `uwsgi-2.0.9/plugins/logcrypto/logcrypto.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/logfile/logfile.c` & `uwsgi-2.0.9/plugins/logfile/logfile.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/logpipe/logpipe.c` & `uwsgi-2.0.9/plugins/logpipe/logpipe.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/logsocket/logsocket_plugin.c` & `uwsgi-2.0.9/plugins/logsocket/logsocket_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/logzmq/plugin.c` & `uwsgi-2.0.9/plugins/logzmq/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/lua/lua_plugin.c` & `uwsgi-2.0.9/plugins/lua/lua_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/lua/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/lua/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/matheval/math.c` & `uwsgi-2.0.9/plugins/matheval/math.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/mongodblog/mongodblog_plugin.c` & `uwsgi-2.0.9/plugins/mongodblog/mongodblog_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/mongrel2/mongrel2.c` & `uwsgi-2.0.9/plugins/mongrel2/mongrel2.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/mono/mono_plugin.c` & `uwsgi-2.0.9/plugins/mono/mono_plugin.c`

 * *Files 1% similar despite different names*

```diff
@@ -539,15 +539,15 @@
 	if (key == NULL) {
 		key = "";
 		key_len = 0;
 	}
 
         wsgi_req->app_id = uwsgi_get_app_id(NULL, key, key_len, mono_plugin.modifier1);
         // if it is -1, try to load a dynamic app
-        if (wsgi_req->app_id == -1) {
+        if (wsgi_req->app_id == -1 && key_len > 0) {
         	if (uwsgi.threads > 1) {
                 	pthread_mutex_lock(&umono.lock_loader);
                 }
 
 		// check if in the mean time, something changed		
 		wsgi_req->app_id = uwsgi_get_app_id(NULL, key, key_len, mono_plugin.modifier1);
 
@@ -558,18 +558,23 @@
                 if (uwsgi.threads > 1) {
                 	pthread_mutex_unlock(&umono.lock_loader);
                 }
         }
 
 
         if (wsgi_req->app_id == -1) {
-        	uwsgi_500(wsgi_req);
-                uwsgi_log("--- unable to find Mono/ASP.NET application ---\n");
-                // nothing to clear/free
-                return UWSGI_OK;
+		if (!uwsgi.no_default_app && uwsgi.default_app > -1 && uwsgi_apps[uwsgi.default_app].modifier1 == mono_plugin.modifier1) {
+               		wsgi_req->app_id = uwsgi.default_app;
+                }
+		else {
+        		uwsgi_500(wsgi_req);
+                	uwsgi_log("--- unable to find Mono/ASP.NET application ---\n");
+                	// nothing to clear/free
+                	return UWSGI_OK;
+		}
         }
 
         struct uwsgi_app *app = &uwsgi_apps[wsgi_req->app_id];
         app->requests++;
 
 	// check for directory without slash
 	char *path = uwsgi_concat3n(app->interpreter, strlen(app->interpreter), "/", 1, wsgi_req->path_info, wsgi_req->path_info_len);
```

### Comparing `uwsgi-2.0.8/plugins/mono/uwsgi.cs` & `uwsgi-2.0.9/plugins/mono/uwsgi.cs`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/mono/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/mono/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/msgpack/msgpack.c` & `uwsgi-2.0.9/plugins/msgpack/msgpack.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/nagios/nagios.c` & `uwsgi-2.0.9/plugins/nagios/nagios.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/notfound/notfound.c` & `uwsgi-2.0.9/plugins/notfound/notfound.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/pam/pam.c` & `uwsgi-2.0.9/plugins/pam/pam.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/php/php_plugin.c` & `uwsgi-2.0.9/plugins/php/php_plugin.c`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 	if (wsgi_req->write_errors > uwsgi.write_errors_tolerance) {
 		php_handle_aborted_connection();
 		return -1;
 	}
 	return str_length;
 }
 
-static int sapi_uwsgi_send_headers(sapi_headers_struct *sapi_headers)
+static int sapi_uwsgi_send_headers(sapi_headers_struct *sapi_headers TSRMLS_DC)
 {
 	sapi_header_struct *h;
 	zend_llist_position pos;
 
 	if (SG(request_info).no_headers == 1) {
                 return SAPI_HEADER_SENT_SUCCESSFULLY;
         }
@@ -131,15 +131,15 @@
 		break;
         }
 
         return read_bytes;
 }
 
 
-static char *sapi_uwsgi_read_cookies(void)
+static char *sapi_uwsgi_read_cookies(TSRMLS_D)
 {
 	uint16_t len = 0;
 	struct wsgi_request *wsgi_req = (struct wsgi_request *) SG(server_context);
 
 	char *cookie = uwsgi_get_var(wsgi_req, (char *)"HTTP_COOKIE", 11, &len);
 	if (cookie) {
 		return estrndup(cookie, len);
@@ -514,15 +514,15 @@
 	if (php_module_startup(&uwsgi_sapi_module, &uwsgi_module_entry, 1)==FAILURE) {
 		return FAILURE;
 	} else {
 		return SUCCESS;
 	}
 }
 
-static void sapi_uwsgi_log_message(char *message) {
+static void sapi_uwsgi_log_message(char *message TSRMLS_DC) {
 
 	uwsgi_log("%s\n", message);
 }
 
 static sapi_module_struct uwsgi_sapi_module = {
 	"uwsgi",
 	"uWSGI/php",
@@ -555,14 +555,18 @@
 };
 
 int uwsgi_php_init(void) {
 
 	struct uwsgi_string_list *pset = uphp.set;
 	struct uwsgi_string_list *append_config = uphp.append_config;
 
+#ifdef ZTS
+        tsrm_startup(1, 1, 0, NULL);
+#endif
+
 	sapi_startup(&uwsgi_sapi_module);
 
 	// applying custom options
 	while(append_config) {
 		uwsgi_php_append_config(append_config->value);
 		append_config = append_config->next;
 	}
@@ -659,14 +663,18 @@
 	size_t real_filename_len = 0;
 	struct stat php_stat;
 	char *filename = NULL;
 	int force_empty_script_name = 0;
 
 	zend_file_handle file_handle;
 
+#ifdef ZTS
+	TSRMLS_FETCH();
+#endif
+
 	SG(server_context) = (void *) wsgi_req;
 
 	if (uwsgi_parse_vars(wsgi_req)) {
 		return -1;
 	}
 
 	char *orig_path_info = wsgi_req->path_info;
```

### Comparing `uwsgi-2.0.8/plugins/php/session.c` & `uwsgi-2.0.9/plugins/php/session.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/php/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/php/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/ping/ping_plugin.c` & `uwsgi-2.0.9/plugins/ping/ping_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/psgi/psgi.h` & `uwsgi-2.0.9/plugins/psgi/psgi.h`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/psgi/psgi_loader.c` & `uwsgi-2.0.9/plugins/psgi/psgi_loader.c`

 * *Files 13% similar despite different names*

```diff
@@ -21,35 +21,37 @@
 	dXSARGS;
 	struct wsgi_request *wsgi_req = current_wsgi_req();
 	struct uwsgi_app *wi = &uwsgi_apps[wsgi_req->app_id];
 
         psgi_check_args(0);
 
 	if (uwsgi.threads > 1) {
-        	ST(0) = sv_bless(newRV(sv_newmortal()), ((HV **)wi->error)[wsgi_req->async_id]);
+        	ST(0) = sv_bless(newRV_noinc(newSV(0)), ((HV **)wi->error)[wsgi_req->async_id]);
 	}
 	else {
-        	ST(0) = sv_bless(newRV(sv_newmortal()), ((HV **)wi->error)[0]);
+        	ST(0) = sv_bless(newRV_noinc(newSV(0)), ((HV **)wi->error)[0]);
 	}
+        sv_2mortal(ST(0));
         XSRETURN(1);
 }
 
 XS(XS_input) {
 
         dXSARGS;
 	struct wsgi_request *wsgi_req = current_wsgi_req();
 	struct uwsgi_app *wi = &uwsgi_apps[wsgi_req->app_id];
         psgi_check_args(0);
 
 	if (uwsgi.threads > 1) {
-        	ST(0) = sv_bless(newRV(sv_newmortal()), ((HV **)wi->input)[wsgi_req->async_id]);
+        	ST(0) = sv_bless(newRV_noinc(newSV(0)), ((HV **)wi->input)[wsgi_req->async_id]);
 	}
 	else {
-        	ST(0) = sv_bless(newRV(sv_newmortal()), ((HV **)wi->input)[0]);
+        	ST(0) = sv_bless(newRV_noinc(newSV(0)), ((HV **)wi->input)[0]);
 	}
+        sv_2mortal(ST(0));
         XSRETURN(1);
 }
 
 XS(XS_psgix_logger) {
 	dXSARGS;
 	psgi_check_args(1);
 	HV *hv_args = (HV *) (SvRV(ST(0)));
@@ -76,19 +78,20 @@
 		while (psgi_response(wsgi_req, response) != UWSGI_OK);
 	}
 	else if (av_len(response) == 1) {
 		while (psgi_response(wsgi_req, response) != UWSGI_OK);
 
 		SvREFCNT_dec(response);
 		if (uwsgi.threads > 1) {
-                	ST(0) = sv_bless(newRV(sv_newmortal()), ((HV **)wi->stream)[wsgi_req->async_id]);
+                	ST(0) = sv_bless(newRV_noinc(newSV(0)), ((HV **)wi->stream)[wsgi_req->async_id]);
 		}
 		else {
-                	ST(0) = sv_bless(newRV(sv_newmortal()), ((HV **)wi->stream)[0]);
+                	ST(0) = sv_bless(newRV_noinc(newSV(0)), ((HV **)wi->stream)[0]);
 		}
+                sv_2mortal(ST(0));
                 XSRETURN(1);
 	}
 	else {
 		uwsgi_log("invalid PSGI response: array size %d\n", av_len(response));
 	}
 
 	SvREFCNT_dec(response);
@@ -267,14 +270,59 @@
 
 	stash = gv_stashpv("uwsgi", 1);
 	newCONSTSUB(stash, "VERSION", newSVpv(UWSGI_VERSION, 0));
 	newCONSTSUB(stash, "SPOOL_OK", newSViv(-2));
 	newCONSTSUB(stash, "SPOOL_RETRY", newSViv(-1));
 	newCONSTSUB(stash, "SPOOL_IGNORE", newSViv(0));
 
+	HV *_opts = newHV();
+
+	int i;
+	for (i = 0; i < uwsgi.exported_opts_cnt; i++) {
+		if (hv_exists(_opts, uwsgi.exported_opts[i]->key, strlen(uwsgi.exported_opts[i]->key))) {
+			SV **value = hv_fetch(_opts, uwsgi.exported_opts[i]->key, strlen(uwsgi.exported_opts[i]->key), 0);
+			// last resort !!!
+			if (!value) {
+				uwsgi_log("[perl] WARNING !!! unable to build uwsgi::opt hash !!!\n");
+				goto end;
+			}
+			if (SvTYPE(SvRV(*value)) == SVt_PVAV) {
+				if (uwsgi.exported_opts[i]->value == NULL) {
+                                        av_push((AV *)SvRV(*value), newSViv(1));
+                                }
+                                else {
+                                        av_push((AV *)SvRV(*value), newSVpv(uwsgi.exported_opts[i]->value, 0));
+                                }
+			}
+			else {
+				AV *_opt_a = newAV();
+				av_push(_opt_a, SvREFCNT_inc(*value));
+				if (uwsgi.exported_opts[i]->value == NULL) {
+					av_push(_opt_a, newSViv(1));
+				}
+				else {
+					av_push(_opt_a, newSVpv(uwsgi.exported_opts[i]->value, 0));
+				}
+				hv_store(_opts, uwsgi.exported_opts[i]->key, strlen(uwsgi.exported_opts[i]->key), newRV_inc((SV *) _opt_a), 0);
+			}
+		}
+		else {
+			if (uwsgi.exported_opts[i]->value == NULL) {
+				hv_store(_opts, uwsgi.exported_opts[i]->key, strlen(uwsgi.exported_opts[i]->key), newSViv(1), 0);
+			}
+			else {
+				hv_store(_opts, uwsgi.exported_opts[i]->key, strlen(uwsgi.exported_opts[i]->key), newSVpv(uwsgi.exported_opts[i]->value, 0), 0);
+			}
+		}
+	}
+
+	newCONSTSUB(stash, "opt", newRV_inc((SV *) _opts));
+
+end:
+
         init_perl_embedded_module();
 
 }
 
 /* end of automagically generated part */
 
 PerlInterpreter *uwsgi_perl_new_interpreter(void) {
```

### Comparing `uwsgi-2.0.8/plugins/psgi/psgi_plugin.c` & `uwsgi-2.0.9/plugins/psgi/psgi_plugin.c`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 	XPUSHs(sv_2mortal(newSVpv( class, class_len)));
 	PUTBACK;
 
 	call_method( "new", G_SCALAR);
 
 	SPAGAIN;
 
-	newobj = POPs;	
+	newobj = SvREFCNT_inc(POPs);
 	PUTBACK;
 	FREETMPS;
 	LEAVE;
 
 	return newobj;
 	
 }
@@ -657,23 +657,29 @@
 
 	// check for psgix.harakiri
 	if (hv_exists((HV *)env, "psgix.harakiri.commit", 21)) {
 		SV **harakiri = hv_fetch((HV *)env, "psgix.harakiri.commit", 21, 0);
 		if (SvTRUE(*harakiri)) wsgi_req->async_plagued = 1;
 	}
 
+	// Free the $env hash
+	SvREFCNT_dec(wsgi_req->async_environ);
+
 	// async plagued could be defined in other areas...
 	if (wsgi_req->async_plagued) {
 		uwsgi_log("*** psgix.harakiri.commit requested ***\n");
+		// Before we call exit(0) we'll run the
+		// uwsgi_perl_atexit() hook which'll properly tear
+		// down the interpreter.
+
+		// mark the request as ended (otherwise the atexit hook will be skipped)
+		uwsgi.workers[uwsgi.mywid].cores[wsgi_req->async_id].in_request = 0;
 		goodbye_cruel_world();
 	}
 
-	// clear the env
-	SvREFCNT_dec(wsgi_req->async_environ);
-
 	// now we can check for changed files
         if (uperl.auto_reload) {
                 time_t now = uwsgi_now();
                 if (now - uperl.last_auto_reload > uperl.auto_reload) {
                         uwsgi_perl_check_auto_reload();
                 }
         }
@@ -799,32 +805,47 @@
 
         PUTBACK;
         FREETMPS;
         LEAVE;
 }
 
 static void uwsgi_perl_atexit() {
+	int i;
+
 	if (uwsgi.mywid == 0) goto realstuff;
 
-        // if hijacked do not run atexit hooks
+        // if hijacked do not run atexit hooks -- TODO: explain why
+        // not.
         if (uwsgi.workers[uwsgi.mywid].hijacked)
-                return;
+                goto destroyperl;
 
-        // if busy do not run atexit hooks
+	// if busy do not run atexit hooks (as this part could be called in a signal handler
+	// while a subroutine is running)
         if (uwsgi_worker_is_busy(uwsgi.mywid))
                 return;
 
-        // managing atexit in async mode is a real pain...skip it for now
-        if (uwsgi.async > 1)
-                return;
 realstuff:
 
 	if (uperl.atexit) {
 		uwsgi_perl_run_hook(uperl.atexit);
 	}
+
+destroyperl:
+
+        // We must free our perl context(s) so any DESTROY hooks
+        // etc. will run.
+        for(i=0;i<uwsgi.threads;i++) {
+            PERL_SET_CONTEXT(uperl.main[i]);
+
+            // Destroy the PerlInterpreter, see "perldoc perlembed"
+            perl_destruct(uperl.main[i]);
+            perl_free(uperl.main[i]);
+        }
+        PERL_SYS_TERM();
+        free(uperl.main);
 }
 
 static uint64_t uwsgi_perl_rpc(void *func, uint8_t argc, char **argv, uint16_t argvs[], char **buffer) {
 
 	int i;
 	uint64_t ret = 0;
```

### Comparing `uwsgi-2.0.8/plugins/psgi/psgi_response.c` & `uwsgi-2.0.9/plugins/psgi/psgi_response.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/psgi/uwsgi_plmodule.c` & `uwsgi-2.0.9/plugins/psgi/uwsgi_plmodule.c`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,21 @@
 	msg = SvPV(ST(1), msg_len);
 
 	uwsgi_alarm_trigger(alarm, msg, msg_len);
 
         XSRETURN_UNDEF;
 }
 
+XS(XS_worker_id) {
+	dXSARGS;
+        psgi_check_args(0);
+	ST(0) = newSViv(uwsgi.mywid);	
+	XSRETURN(1);
+}
+
 XS(XS_async_connect) {
 
 	dXSARGS;
 	psgi_check_args(1);
 
 	ST(0) = newSViv(uwsgi_connect(SvPV_nolen(ST(0)), 0, 1));
 
@@ -1038,9 +1045,10 @@
 	psgi_xs(sharedarea_write);
 	psgi_xs(sharedarea_wait);
 
 	psgi_xs(spooler);
 	psgi_xs(spool);
 
 	psgi_xs(add_var);
+	psgi_xs(worker_id);
 	
 }
```

### Comparing `uwsgi-2.0.8/plugins/pty/pty.c` & `uwsgi-2.0.9/plugins/pty/pty.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/pypy/README` & `uwsgi-2.0.9/plugins/pypy/README`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/pypy/pypy_plugin.c` & `uwsgi-2.0.9/plugins/pypy/pypy_plugin.c`

 * *Files 4% similar despite different names*

```diff
@@ -62,25 +62,42 @@
 		goto ready;
 	}
 	else if (upypy.lib) {
 		upypy.handler = dlopen(upypy.lib, RTLD_NOW | RTLD_GLOBAL);
 	}
 	else {
 		if (upypy.home) {
+			// first try with /bin way:
 #ifdef __CYGWIN__
-                        char *libpath = uwsgi_concat2(upypy.home, "/libpypy-c.dll");
+                        char *libpath = uwsgi_concat2(upypy.home, "/bin/libpypy-c.dll");
 #elif defined(__APPLE__)
-                        char *libpath = uwsgi_concat2(upypy.home, "/libpypy-c.dylib");
+                        char *libpath = uwsgi_concat2(upypy.home, "/bin/libpypy-c.dylib");
 #else
-                        char *libpath = uwsgi_concat2(upypy.home, "/libpypy-c.so");
+                        char *libpath = uwsgi_concat2(upypy.home, "/bin/libpypy-c.so");
 #endif
 			if (uwsgi_file_exists(libpath)) {
-				upypy.handler = dlopen(libpath, RTLD_NOW | RTLD_GLOBAL);
+                                upypy.handler = dlopen(libpath, RTLD_NOW | RTLD_GLOBAL);
+                        }
+                        free(libpath);
+
+			// fallback to old-style way
+			if (!upypy.handler) {
+			
+#ifdef __CYGWIN__
+                        	char *libpath = uwsgi_concat2(upypy.home, "/libpypy-c.dll");
+#elif defined(__APPLE__)
+                        	char *libpath = uwsgi_concat2(upypy.home, "/libpypy-c.dylib");
+#else
+                        	char *libpath = uwsgi_concat2(upypy.home, "/libpypy-c.so");
+#endif
+				if (uwsgi_file_exists(libpath)) {
+					upypy.handler = dlopen(libpath, RTLD_NOW | RTLD_GLOBAL);
+				}
+				free(libpath);
 			}
-			free(libpath);
 		}
 		// fallback to standard library search path
 		if (!upypy.handler) {
 #ifdef __CYGWIN__
 			upypy.handler = dlopen("libpypy-c.dll", RTLD_NOW | RTLD_GLOBAL);
 #elif defined(__APPLE__)
 			upypy.handler = dlopen("libpypy-c.dylib", RTLD_NOW | RTLD_GLOBAL);
```

### Comparing `uwsgi-2.0.8/plugins/pypy/pypy_setup.py` & `uwsgi-2.0.9/plugins/pypy/pypy_setup.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/gil.c` & `uwsgi-2.0.9/plugins/python/gil.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/profiler.c` & `uwsgi-2.0.9/plugins/python/profiler.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/pump_subhandler.c` & `uwsgi-2.0.9/plugins/python/pump_subhandler.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/pyloader.c` & `uwsgi-2.0.9/plugins/python/pyloader.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/python_plugin.c` & `uwsgi-2.0.9/plugins/python/python_plugin.c`

 * *Files 1% similar despite different names*

```diff
@@ -1421,15 +1421,23 @@
 #endif
 		PyObject *mod_name, *mod;
                 while (PyDict_Next(modules, &pos, &mod_name, &mod)) {
 			if (mod == NULL) continue;
 			int found = 0;
 			struct uwsgi_string_list *usl = up.auto_reload_ignore;
 			while(usl) {
+#ifdef PYTHREE
+				PyObject *zero = PyUnicode_AsUTF8String(mod_name);
+				char *str_mod_name = PyString_AsString(zero);
+				int ret_cmp = strcmp(usl->value, str_mod_name);
+				Py_DECREF(zero);
+				if (!ret_cmp) {
+#else
 				if (!strcmp(usl->value, PyString_AsString(mod_name))) {
+#endif
 					found = 1;
 					break;
 				}
 				usl = usl->next;
 			}
 			if (found) continue;
 			if (!PyObject_HasAttrString(mod, "__file__")) continue;
```

### Comparing `uwsgi-2.0.8/plugins/python/pyutils.c` & `uwsgi-2.0.9/plugins/python/pyutils.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/raw.c` & `uwsgi-2.0.9/plugins/python/raw.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/symimporter.c` & `uwsgi-2.0.9/plugins/python/symimporter.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/tracebacker.c` & `uwsgi-2.0.9/plugins/python/tracebacker.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/uwsgi_pymodule.c` & `uwsgi-2.0.9/plugins/python/uwsgi_pymodule.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/uwsgi_python.h` & `uwsgi-2.0.9/plugins/python/uwsgi_python.h`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/python/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/web3_subhandler.c` & `uwsgi-2.0.9/plugins/python/web3_subhandler.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/wsgi_handlers.c` & `uwsgi-2.0.9/plugins/python/wsgi_handlers.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/wsgi_headers.c` & `uwsgi-2.0.9/plugins/python/wsgi_headers.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/python/wsgi_subhandler.c` & `uwsgi-2.0.9/plugins/python/wsgi_subhandler.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/pyuwsgi/pyuwsgi.c` & `uwsgi-2.0.9/plugins/pyuwsgi/pyuwsgi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rack/rack_api.c` & `uwsgi-2.0.9/plugins/rack/rack_api.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rack/rack_plugin.c` & `uwsgi-2.0.9/plugins/rack/rack_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rack/uwsgi_rack.h` & `uwsgi-2.0.9/plugins/rack/uwsgi_rack.h`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rack/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/rack/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rados/rados.c` & `uwsgi-2.0.9/plugins/rados/rados.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rawrouter/rawrouter.c` & `uwsgi-2.0.9/plugins/rawrouter/rawrouter.c`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 	// add a new peer
 	struct corerouter_peer *peer = uwsgi_cr_peer_add(cs);
 
 	// set default peer hook
 	peer->last_hook_read = rr_instance_read;
 
 	// use the address as hostname
-        peer->key = cs->ugs->name;
+        memcpy(peer->key, cs->ugs->name, cs->ugs->name_len);
         peer->key_len = cs->ugs->name_len;
 
         // the mapper hook
         if (ucr->mapper(ucr, peer)) {
 		return -1;
 	}
```

### Comparing `uwsgi-2.0.8/plugins/rbthreads/rbthreads.c` & `uwsgi-2.0.9/plugins/rbthreads/rbthreads.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rbthreads/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/rbthreads/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/redislog/redislog_plugin.c` & `uwsgi-2.0.9/plugins/redislog/redislog_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/ring/ring_plugin.c` & `uwsgi-2.0.9/plugins/ring/ring_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/ring/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/ring/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_access/router_access.c` & `uwsgi-2.0.9/plugins/router_access/router_access.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_basicauth/router_basicauth.c` & `uwsgi-2.0.9/plugins/router_basicauth/router_basicauth.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_cache/router_cache.c` & `uwsgi-2.0.9/plugins/router_cache/router_cache.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_expires/expires.c` & `uwsgi-2.0.9/plugins/router_expires/expires.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_hash/router_hash.c` & `uwsgi-2.0.9/plugins/router_hash/router_hash.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_http/router_http.c` & `uwsgi-2.0.9/plugins/router_http/router_http.c`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 		}
 	}
 
 	// convert the wsgi_request to an http proxy request
 	if (ur->custom & 0x02) {
 		ub = uwsgi_buffer_new(uwsgi.page_size);
 	}
+	else if (ur->custom & 0x04) {
+		ub = uwsgi_to_http_dumb(wsgi_req, ur->data2, ur->data2_len, ub_url ? ub_url->buf : NULL, ub_url ? ub_url->pos : 0);
+	}
 	else {
 		ub = uwsgi_to_http(wsgi_req, ur->data2, ur->data2_len, ub_url ? ub_url->buf : NULL, ub_url ? ub_url->pos : 0);	
 	}
 
 	if (!ub) {
 		if (ub_url) uwsgi_buffer_destroy(ub_url);
 		uwsgi_log("unable to generate http request for %s\n", ub_addr->buf);
@@ -129,18 +132,24 @@
 }
 
 static int uwsgi_router_http_connect(struct uwsgi_route *ur, char *args) {
         ur->custom = 0x02;
         return uwsgi_router_http(ur, args);
 }
 
+static int uwsgi_router_httpdumb(struct uwsgi_route *ur, char *args) {
+        ur->custom = 0x04;
+        return uwsgi_router_http(ur, args);
+}
+
 
 static void router_http_register(void) {
 
 	uwsgi_register_router("http", uwsgi_router_http);
+	uwsgi_register_router("httpdumb", uwsgi_router_httpdumb);
 	uwsgi_register_router("proxyhttp", uwsgi_router_proxyhttp);
 	uwsgi_register_router("httpconnect", uwsgi_router_http_connect);
 	uwsgi_register_router("proxyhttpconnect", uwsgi_router_proxyhttp_connect);
 }
 
 struct uwsgi_plugin router_http_plugin = {
 	.name = "router_http",
```

### Comparing `uwsgi-2.0.8/plugins/router_memcached/router_memcached.c` & `uwsgi-2.0.9/plugins/router_memcached/router_memcached.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_metrics/plugin.c` & `uwsgi-2.0.9/plugins/router_metrics/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_radius/radius.c` & `uwsgi-2.0.9/plugins/router_radius/radius.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_redirect/router_redirect.c` & `uwsgi-2.0.9/plugins/router_redirect/router_redirect.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_redis/router_redis.c` & `uwsgi-2.0.9/plugins/router_redis/router_redis.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_rewrite/router_rewrite.c` & `uwsgi-2.0.9/plugins/router_rewrite/router_rewrite.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_spnego/router_spnego.c` & `uwsgi-2.0.9/plugins/router_spnego/router_spnego.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_static/router_static.c` & `uwsgi-2.0.9/plugins/router_static/router_static.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_uwsgi/router_uwsgi.c` & `uwsgi-2.0.9/plugins/router_uwsgi/router_uwsgi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/router_xmldir/router_xmldir.c` & `uwsgi-2.0.9/plugins/router_xmldir/router_xmldir.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rpc/rpc_plugin.c` & `uwsgi-2.0.9/plugins/rpc/rpc_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rrdtool/rrdtool.c` & `uwsgi-2.0.9/plugins/rrdtool/rrdtool.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/rsyslog/rsyslog_plugin.c` & `uwsgi-2.0.9/plugins/rsyslog/rsyslog_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/ruby19/uwsgiplugin.py` & `uwsgi-2.0.9/plugins/ruby19/uwsgiplugin.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/servlet/servlet_plugin.c` & `uwsgi-2.0.9/plugins/servlet/servlet_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/servlet/uwsgi_servlet.java` & `uwsgi-2.0.9/plugins/servlet/uwsgi_servlet.java`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/signal/signal_plugin.c` & `uwsgi-2.0.9/plugins/signal/signal_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/spooler/spooler_plugin.c` & `uwsgi-2.0.9/plugins/spooler/spooler_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/sqlite3/plugin.c` & `uwsgi-2.0.9/plugins/sqlite3/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/ssi/ssi.c` & `uwsgi-2.0.9/plugins/ssi/ssi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/sslrouter/sslrouter.c` & `uwsgi-2.0.9/plugins/sslrouter/sslrouter.c`

 * *Files 0% similar despite different names*

```diff
@@ -284,23 +284,23 @@
                 }
 		if (!main_peer->session->peers) {
 			// add a new peer
         		struct corerouter_peer *peer = uwsgi_cr_peer_add(cs);
         		// set default peer hook
         		peer->last_hook_read = sr_instance_read;
         		// use the address as hostname
-        		peer->key = cs->ugs->name;
+        		memcpy(peer->key, cs->ugs->name, cs->ugs->name_len);
         		peer->key_len = cs->ugs->name_len;
 
 #ifdef SSL_CTRL_SET_TLSEXT_HOSTNAME
 			if (usr.sni) {
 				const char *servername = SSL_get_servername(sr->ssl, TLSEXT_NAMETYPE_host_name);
-				if (servername) {
-        				peer->key = (char *) servername;
+				if (servername && strlen(servername) <= 0xff) {
         				peer->key_len = strlen(servername);
+        				memcpy(peer->key, servername, peer->key_len);
 				}
 			}
 #endif
         		// the mapper hook
         		if (cs->corerouter->mapper(cs->corerouter, peer)) {
                 		return -1;
         		}
```

### Comparing `uwsgi-2.0.8/plugins/stackless/stackless.c` & `uwsgi-2.0.9/plugins/stackless/stackless.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/stats_pusher_file/plugin.c` & `uwsgi-2.0.9/plugins/stats_pusher_file/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/stats_pusher_mongodb/stats_pusher_mongodb.cc` & `uwsgi-2.0.9/plugins/stats_pusher_mongodb/stats_pusher_mongodb.cc`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/stats_pusher_socket/plugin.c` & `uwsgi-2.0.9/plugins/stats_pusher_socket/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/stats_pusher_statsd/plugin.c` & `uwsgi-2.0.9/plugins/stats_pusher_statsd/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/symcall/symcall_plugin.c` & `uwsgi-2.0.9/plugins/symcall/symcall_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/syslog/syslog_plugin.c` & `uwsgi-2.0.9/plugins/syslog/syslog_plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/systemd_logger/systemd_logger.c` & `uwsgi-2.0.9/plugins/systemd_logger/systemd_logger.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 	// split multiline log messages to multiple journal lines
 	size_t i;
 	char *base = message;
 	for(i=0;i<len;i++) {
 		if (message[i] == '\n') {
 			message[i] = 0;
-			sd_journal_print(LOG_INFO, base);
+			sd_journal_print(LOG_INFO, "%s", base);
 			base = message+i+1;
 		}
 	}
 
 	// last \n is missing...
 	if (base < message+len) {
 		sd_journal_print(LOG_INFO, "%.*s", (int) ((message+len) - base), base);
```

### Comparing `uwsgi-2.0.8/plugins/tornado/tornado.c` & `uwsgi-2.0.9/plugins/tornado/tornado.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/transformation_chunked/chunked.c` & `uwsgi-2.0.9/plugins/transformation_chunked/chunked.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/transformation_gzip/gzip.c` & `uwsgi-2.0.9/plugins/transformation_gzip/gzip.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/transformation_offload/offload.c` & `uwsgi-2.0.9/plugins/transformation_offload/offload.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/transformation_template/tt.c` & `uwsgi-2.0.9/plugins/transformation_template/tt.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/transformation_tofile/tofile.c` & `uwsgi-2.0.9/plugins/transformation_tofile/tofile.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/transformation_toupper/toupper.c` & `uwsgi-2.0.9/plugins/transformation_toupper/toupper.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/tuntap/common.c` & `uwsgi-2.0.9/plugins/tuntap/common.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/tuntap/common.h` & `uwsgi-2.0.9/plugins/tuntap/common.h`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/tuntap/firewall.c` & `uwsgi-2.0.9/plugins/tuntap/firewall.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/tuntap/tuntap.c` & `uwsgi-2.0.9/plugins/tuntap/tuntap.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/ugreen/ugreen.c` & `uwsgi-2.0.9/plugins/ugreen/ugreen.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/v8/plugin.c` & `uwsgi-2.0.9/plugins/v8/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/v8/v8_commonjs.cc` & `uwsgi-2.0.9/plugins/v8/v8_commonjs.cc`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/v8/v8_jsgi.cc` & `uwsgi-2.0.9/plugins/v8/v8_jsgi.cc`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/v8/v8_uwsgi.cc` & `uwsgi-2.0.9/plugins/v8/v8_uwsgi.cc`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/v8/v8_uwsgi.h` & `uwsgi-2.0.9/plugins/v8/v8_uwsgi.h`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/webdav/webdav.c` & `uwsgi-2.0.9/plugins/webdav/webdav.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/xattr/xattr.c` & `uwsgi-2.0.9/plugins/xattr/xattr.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/xslt/xslt.c` & `uwsgi-2.0.9/plugins/xslt/xslt.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/zabbix/plugin.c` & `uwsgi-2.0.9/plugins/zabbix/plugin.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/plugins/zergpool/zergpool.c` & `uwsgi-2.0.9/plugins/zergpool/zergpool.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/proto/base.c` & `uwsgi-2.0.9/proto/base.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/proto/fastcgi.c` & `uwsgi-2.0.9/proto/fastcgi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/proto/http.c` & `uwsgi-2.0.9/proto/http.c`

 * *Files 18% similar despite different names*

```diff
@@ -476,14 +476,104 @@
 			continue;
 		}
 
 		buf[i] = tolower( (int) buf[i]);
 	}
 }
 
+struct uwsgi_buffer *uwsgi_to_http_dumb(struct wsgi_request *wsgi_req, char *host, uint16_t host_len, char *uri, uint16_t uri_len) {
+
+        struct uwsgi_buffer *ub = uwsgi_buffer_new(4096);
+
+        if (uwsgi_buffer_append(ub, wsgi_req->method, wsgi_req->method_len)) goto clear;
+        if (uwsgi_buffer_append(ub, " ", 1)) goto clear;
+
+        if (uri_len && uri) {
+                if (uwsgi_buffer_append(ub, uri, uri_len)) goto clear;
+        }
+        else {
+                if (uwsgi_buffer_append(ub, wsgi_req->uri, wsgi_req->uri_len)) goto clear;
+        }
+
+        if (uwsgi_buffer_append(ub, " ", 1)) goto clear;
+        if (uwsgi_buffer_append(ub, wsgi_req->protocol, wsgi_req->protocol_len)) goto clear;
+        if (uwsgi_buffer_append(ub, "\r\n", 2)) goto clear;
+
+        int i;
+        char *x_forwarded_for = NULL;
+        size_t x_forwarded_for_len = 0;
+
+        // start adding headers
+        for(i=0;i<wsgi_req->var_cnt;i++) {
+                if (!uwsgi_starts_with(wsgi_req->hvec[i].iov_base, wsgi_req->hvec[i].iov_len, "HTTP_", 5)) {
+
+                        char *header = wsgi_req->hvec[i].iov_base+5;
+                        size_t header_len = wsgi_req->hvec[i].iov_len-5;
+
+                        if (host && !uwsgi_strncmp(header, header_len, "HOST", 4)) goto next;
+
+                        if (!uwsgi_strncmp(header, header_len, "X_FORWARDED_FOR", 15)) {
+                                x_forwarded_for = wsgi_req->hvec[i+1].iov_base;
+                                x_forwarded_for_len = wsgi_req->hvec[i+1].iov_len;
+                                goto next;
+                        }
+
+                        if (uwsgi_buffer_append(ub, header, header_len)) goto clear;
+
+                        // transofmr uwsgi var to http header
+                        uwsgi_httpize_var((ub->buf+ub->pos) - header_len, header_len);
+
+                        if (uwsgi_buffer_append(ub, ": ", 2)) goto clear;
+                        if (uwsgi_buffer_append(ub, wsgi_req->hvec[i+1].iov_base, wsgi_req->hvec[i+1].iov_len)) goto clear;
+                        if (uwsgi_buffer_append(ub, "\r\n", 2)) goto clear;
+
+                }
+next:
+                i++;
+        }
+
+
+        // append custom Host (if needed)
+        if (host) {
+                if (uwsgi_buffer_append(ub, "Host: ", 6)) goto clear;
+                if (uwsgi_buffer_append(ub, host, host_len)) goto clear;
+                if (uwsgi_buffer_append(ub, "\r\n", 2)) goto clear;
+        }
+
+        if (wsgi_req->content_type_len > 0) {
+                if (uwsgi_buffer_append(ub, "Content-Type: ", 14)) goto clear;
+                if (uwsgi_buffer_append(ub, wsgi_req->content_type, wsgi_req->content_type_len)) goto clear;
+                if (uwsgi_buffer_append(ub, "\r\n", 2)) goto clear;
+        }
+
+        if (wsgi_req->post_cl > 0) {
+                if (uwsgi_buffer_append(ub, "Content-Length: ", 16)) goto clear;
+                if (uwsgi_buffer_num64(ub, (int64_t) wsgi_req->post_cl)) goto clear;
+                if (uwsgi_buffer_append(ub, "\r\n", 2)) goto clear;
+        }
+
+        // append required headers
+        if (uwsgi_buffer_append(ub, "X-Forwarded-For: ", 17)) goto clear;
+
+        if (x_forwarded_for_len > 0) {
+                if (uwsgi_buffer_append(ub, x_forwarded_for, x_forwarded_for_len)) goto clear;
+                if (uwsgi_buffer_append(ub, ", ", 2)) goto clear;
+        }
+
+        if (uwsgi_buffer_append(ub, wsgi_req->remote_addr, wsgi_req->remote_addr_len)) goto clear;
+
+        if (uwsgi_buffer_append(ub, "\r\n\r\n", 4)) goto clear;
+
+        return ub;
+clear:
+        uwsgi_buffer_destroy(ub);
+        return NULL;
+}
+
+
 struct uwsgi_buffer *uwsgi_to_http(struct wsgi_request *wsgi_req, char *host, uint16_t host_len, char *uri, uint16_t uri_len) {
 
         struct uwsgi_buffer *ub = uwsgi_buffer_new(4096);
 
         if (uwsgi_buffer_append(ub, wsgi_req->method, wsgi_req->method_len)) goto clear;
         if (uwsgi_buffer_append(ub, " ", 1)) goto clear;
 
@@ -509,22 +599,16 @@
 			size_t header_len = wsgi_req->hvec[i].iov_len-5;
 
 			if (host && !uwsgi_strncmp(header, header_len, "HOST", 4)) goto next;
 
 			// remove dangerous headers
 			if (!uwsgi_strncmp(header, header_len, "CONNECTION", 10)) goto next;
 			if (!uwsgi_strncmp(header, header_len, "KEEP_ALIVE", 10)) goto next;
-			if (!uwsgi_strncmp(header, header_len, "ACCEPT_ENCODING", 15)) goto next;
 			if (!uwsgi_strncmp(header, header_len, "TE", 2)) goto next;
 			if (!uwsgi_strncmp(header, header_len, "TRAILER", 7)) goto next;
-			if (!uwsgi_strncmp(header, header_len, "IF_MATCH", 8)) goto next;
-			if (!uwsgi_strncmp(header, header_len, "IF_MODIFIED_SINCE", 17)) goto next;
-			if (!uwsgi_strncmp(header, header_len, "IF_RANGE", 8)) goto next;
-			if (!uwsgi_strncmp(header, header_len, "IF_UNMODIFIED_SINCE", 19)) goto next;
-			if (!uwsgi_strncmp(header, header_len, "IF_NONE_MATCH", 13)) goto next;
 			if (!uwsgi_strncmp(header, header_len, "X_FORWARDED_FOR", 15)) {
 				x_forwarded_for = wsgi_req->hvec[i+1].iov_base;
 				x_forwarded_for_len = wsgi_req->hvec[i+1].iov_len;
 				goto next;
 			}
 
 			if (uwsgi_buffer_append(ub, header, header_len)) goto clear;
```

### Comparing `uwsgi-2.0.8/proto/puwsgi.c` & `uwsgi-2.0.9/proto/puwsgi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/proto/scgi.c` & `uwsgi-2.0.9/proto/scgi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/proto/uwsgi.c` & `uwsgi-2.0.9/proto/uwsgi.c`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/setup.py` & `uwsgi-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/cachebitmap.ini` & `uwsgi-2.0.9/t/cachebitmap.ini`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/cachebitmap.py` & `uwsgi-2.0.9/t/cachebitmap.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/cachetest.py` & `uwsgi-2.0.9/t/cachetest.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/core/read_body_and_send.pl` & `uwsgi-2.0.9/t/core/read_body_and_send.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/core/url_sanitize.pl` & `uwsgi-2.0.9/t/core/url_sanitize.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/go/cachetest.go` & `uwsgi-2.0.9/t/go/cachetest.go`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/go/complextest.go` & `uwsgi-2.0.9/t/go/complextest.go`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/go/uploadtest.go` & `uwsgi-2.0.9/t/go/uploadtest.go`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/lua/basic.lua` & `uwsgi-2.0.9/t/lua/basic.lua`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/perl/test.psgi` & `uwsgi-2.0.9/t/perl/test.psgi`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/perl/test_benchmark.pl` & `uwsgi-2.0.9/t/perl/test_benchmark.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/perl/test_input_with_offset.pl` & `uwsgi-2.0.9/t/perl/test_input_with_offset.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/perl/test_post.psgi` & `uwsgi-2.0.9/t/perl/test_post.psgi`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/perl/test_sleepy.psgi` & `uwsgi-2.0.9/t/perl/test_sleepy.psgi`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/perl/test_streaming.psgi` & `uwsgi-2.0.9/t/perl/test_streaming.psgi`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/pypy/t_continulet1.py` & `uwsgi-2.0.9/t/pypy/t_continulet1.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/pypy/t_continulet2.py` & `uwsgi-2.0.9/t/pypy/t_continulet2.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/python/manage_script_name/test_manage_script_name.py` & `uwsgi-2.0.9/t/python/manage_script_name/test_manage_script_name.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/app.clj` & `uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/app.clj`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/basic.clj` & `uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/basic.clj`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/body.clj` & `uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/body.clj`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/ring/src/uwsgi/ring/tests/upload.clj` & `uwsgi-2.0.9/t/ring/src/uwsgi/ring/tests/upload.clj`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/routing/auth.ini` & `uwsgi-2.0.9/t/routing/auth.ini`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/routing/errorlimiter.ini` & `uwsgi-2.0.9/t/routing/errorlimiter.ini`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/routing/limiter.ini` & `uwsgi-2.0.9/t/routing/limiter.ini`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/t/xslt/cd.xml.xslt` & `uwsgi-2.0.9/t/xslt/cd.xml.xslt`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/Responder.pm` & `uwsgi-2.0.9/tests/Responder.pm`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/badwrites.py` & `uwsgi-2.0.9/tests/badwrites.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/decoratortest.py` & `uwsgi-2.0.9/tests/decoratortest.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/grunter.py` & `uwsgi-2.0.9/tests/grunter.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/iobound_async.py` & `uwsgi-2.0.9/tests/iobound_async.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/iobound_async_unix.py` & `uwsgi-2.0.9/tests/iobound_async_unix.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/iobound_green.py` & `uwsgi-2.0.9/tests/iobound_green.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/mulefunc.py` & `uwsgi-2.0.9/tests/mulefunc.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/pgbound_async.py` & `uwsgi-2.0.9/tests/pgbound_async.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/picazzo.py` & `uwsgi-2.0.9/tests/picazzo.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/psycogreen_green.py` & `uwsgi-2.0.9/tests/psycogreen_green.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/psycopg2_green.py` & `uwsgi-2.0.9/tests/psycopg2_green.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/queue.py` & `uwsgi-2.0.9/tests/queue.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/signals.py` & `uwsgi-2.0.9/tests/signals.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/sigwait.py` & `uwsgi-2.0.9/tests/sigwait.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/t/static.pl` & `uwsgi-2.0.9/tests/t/static.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/templates/queue.html` & `uwsgi-2.0.9/tests/templates/queue.html`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/testapp.py` & `uwsgi-2.0.9/tests/testapp.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/testgevent.py` & `uwsgi-2.0.9/tests/testgevent.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/threads.py` & `uwsgi-2.0.9/tests/threads.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/travis.sh` & `uwsgi-2.0.9/tests/travis.sh`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/ugevent.py` & `uwsgi-2.0.9/tests/ugevent.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/websockets.py` & `uwsgi-2.0.9/tests/websockets.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/websockets_chat.pl` & `uwsgi-2.0.9/tests/websockets_chat.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/websockets_chat.py` & `uwsgi-2.0.9/tests/websockets_chat.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/websockets_chat_async.py` & `uwsgi-2.0.9/tests/websockets_chat_async.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/websockets_chat_asyncio.py` & `uwsgi-2.0.9/tests/websockets_chat_asyncio.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/websockets_echo.lua` & `uwsgi-2.0.9/tests/websockets_echo.lua`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/websockets_echo.pl` & `uwsgi-2.0.9/tests/websockets_echo.pl`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/websockets_echo.py` & `uwsgi-2.0.9/tests/websockets_echo.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/tests/websockets_echo.ru` & `uwsgi-2.0.9/tests/websockets_echo.ru`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/uwsgi.gemspec` & `uwsgi-2.0.9/uwsgi.gemspec`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Gem::Specification.new do |s|
   s.name        = 'uwsgi'
   s.license     = 'GPL-2'
   s.version     = `python -c "import uwsgiconfig as uc; print uc.uwsgi_version"`.sub(/-dev-.*/,'')
-  s.date        = '2014-10-26'
+  s.date        = '2014-12-30'
   s.summary     = "uWSGI"
   s.description = "The uWSGI server for Ruby/Rack"
   s.authors     = ["Unbit"]
   s.email       = 'info@unbit.it'
   s.extensions  = ['ext/uwsgi/extconf.rb']
   s.files       = []
   s.require_paths = ['.']
```

### Comparing `uwsgi-2.0.8/uwsgi.h` & `uwsgi-2.0.9/uwsgi.h`

 * *Files 0% similar despite different names*

```diff
@@ -2749,14 +2749,18 @@
 	struct uwsgi_string_list *wait_for_mountpoint;
 #ifdef UWSGI_SSL
 	int sslv3;
 	struct uwsgi_string_list *ssl_options;
 #endif
 	struct uwsgi_string_list *hook_post_fork;
 
+	// uWSGI 2.0.9
+	char *subscribe_with_modifier1;
+	struct uwsgi_string_list *pull_headers;
+
 };
 
 struct uwsgi_rpc {
 	char name[UMAX8];
 	void *func;
 	uint8_t args;
 	uint8_t shared;
@@ -4178,14 +4182,15 @@
 int uwsgi_buffer_set_uh(struct uwsgi_buffer *, uint8_t, uint8_t);
 void uwsgi_buffer_map(struct uwsgi_buffer *, char *, size_t);
 struct uwsgi_buffer *uwsgi_buffer_from_file(char *);
 
 ssize_t uwsgi_buffer_write_simple(struct wsgi_request *, struct uwsgi_buffer *);
 
 struct uwsgi_buffer *uwsgi_to_http(struct wsgi_request *, char *, uint16_t, char *, uint16_t);
+struct uwsgi_buffer *uwsgi_to_http_dumb(struct wsgi_request *, char *, uint16_t, char *, uint16_t);
 
 ssize_t uwsgi_pipe(int, int, int);
 ssize_t uwsgi_pipe_sized(int, int, size_t, int);
 
 int uwsgi_buffer_send(struct uwsgi_buffer *, int);
 void uwsgi_master_cleanup_hooks(void);
```

### Comparing `uwsgi-2.0.8/uwsgiconfig.py` & `uwsgi-2.0.9/uwsgiconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # uWSGI build system
 
-uwsgi_version = '2.0.8'
+uwsgi_version = '2.0.9'
 
 import os
 import re
 import time
 uwsgi_os = os.uname()[0]
 uwsgi_os_k = re.split('[-+]', os.uname()[2])[0]
 uwsgi_os_v = os.uname()[3]
@@ -1167,14 +1167,16 @@
                     self.cflags.append("-DUWSGI_JSON")
                     self.gcc_list.append('core/json')
                     self.libs.append('-ljansson')
                     report['json'] = 'jansson'
                 else:
                     jsonconf = spcall("pkg-config --cflags yajl")
                     if jsonconf:
+                        if jsonconf.endswith('include/yajl'):
+                            jsonconf = jsonconf.rstrip('yajl')
                         self.cflags.append(jsonconf)
                         self.cflags.append("-DUWSGI_JSON")
                         self.gcc_list.append('core/json')
                         self.libs.append(spcall("pkg-config --libs yajl"))
                         self.cflags.append("-DUWSGI_JSON_YAJL")
                         report['json'] = 'yajl'
                     elif self.get('json') == 'true':
```

### Comparing `uwsgi-2.0.8/uwsgidecorators.py` & `uwsgi-2.0.9/uwsgidecorators.py`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/uwsgidsl.rb` & `uwsgi-2.0.9/uwsgidsl.rb`

 * *Files identical despite different names*

### Comparing `uwsgi-2.0.8/vhosttest/nginx.conf` & `uwsgi-2.0.9/vhosttest/nginx.conf`

 * *Files identical despite different names*

