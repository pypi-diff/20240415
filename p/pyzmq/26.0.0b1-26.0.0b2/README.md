# Comparing `tmp/pyzmq-26.0.0b1.tar.gz` & `tmp/pyzmq-26.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzmq-26.0.0b1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyzmq-26.0.0b2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyzmq-26.0.0b1.tar` & `pyzmq-26.0.0b2.tar`

### file list

```diff
@@ -1,287 +1,284 @@
--rw-r--r--   0        0        0     1853 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.circleci/config.yml
--rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.coveragerc
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.flake8
--rw-r--r--   0        0        0     2697 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.github/dependabot.yml
--rw-r--r--   0        0        0     5033 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.github/workflows/test.yml
--rw-r--r--   0        0        0     6029 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.gitignore
--rw-r--r--   0        0        0      733 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.mailmap
--rw-r--r--   0        0        0      128 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.obs/workflows.yml
--rw-r--r--   0        0        0     2067 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.prettierignore
--rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/.readthedocs.yml
--rw-r--r--   0        0        0     4810 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/AUTHORS.md
--rw-r--r--   0        0        0    12777 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/CMakeLists.txt
--rw-r--r--   0        0        0     2251 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/LICENSE.md
--rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/MANIFEST.in
--rw-r--r--   0        0        0     2964 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/README.md
--rw-r--r--   0        0        0     2116 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/README.md
--rw-r--r--   0        0        0     2751 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/authors.py
--rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/chrislaws.md
--rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/ellisonbg.md
--rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/frankwiles.md
--rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/juliantaylor.md
--rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/ledgerx.md
--rw-r--r--   0        0        0      731 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/lothiraldan.md
--rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/minrk.md
--rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/takluyver.md
--rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/templates/relicense-template-bsd.txt
--rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/templates/relicense-template-mplv2-any-osi.txt
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/RELICENSE/templates/relicense-template-mplv2.txt
--rw-r--r--   0        0        0     1541 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/SECURITY.md
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/Vagrantfile
--rw-r--r--   0        0        0      692 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/buildutils/build_cffi.py
--rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/buildutils/bundle.py
--rw-r--r--   0        0        0     3634 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/buildutils/constants.py
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/buildutils/templates/constant_enums.pxi
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/buildutils/templates/constants.py
--rw-r--r--   0        0        0    11525 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/cmake/FindVcvars.cmake
--rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/cmake/Findsodium.cmake
--rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/codecov.yml
--rw-r--r--   0        0        0     3631 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/Makefile
--rwxr-xr-x   0        0        0     1456 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/autogen_api.py
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/requirements.txt
--rw-r--r--   0        0        0     8686 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/_static/logo.png
--rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/_static/zeromq.ico
--rw-r--r--   0        0        0      470 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/index.rst
--rw-r--r--   0        0        0     1872 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.asyncio.rst
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.auth.asyncio.rst
--rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.auth.ioloop.rst
--rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.auth.rst
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.auth.thread.rst
--rw-r--r--   0        0        0      258 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.decorators.rst
--rw-r--r--   0        0        0     1683 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.devices.rst
--rw-r--r--   0        0        0     1951 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.eventloop.future.rst
--rw-r--r--   0        0        0      170 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.eventloop.ioloop.rst
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.eventloop.zmqstream.rst
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.green.rst
--rw-r--r--   0        0        0      456 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.log.handlers.rst
--rw-r--r--   0        0        0     3610 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.rst
--rw-r--r--   0        0        0      514 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.ssh.tunnel.rst
--rw-r--r--   0        0        0      308 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.utils.jsonapi.rst
--rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.utils.monitor.rst
--rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.utils.win32.rst
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/api/zmq.utils.z85.rst
--rw-r--r--   0        0        0    41585 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/changelog.md
--rw-r--r--   0        0        0     7408 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/conf.py
--rw-r--r--   0        0        0    10786 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/howto/build.md
--rw-r--r--   0        0        0     3982 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/howto/devices.md
--rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/howto/draft.md
--rw-r--r--   0        0        0     8531 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/howto/eventloop.md
--rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/howto/index.md
--rw-r--r--   0        0        0     9610 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/howto/logging.md
--rw-r--r--   0        0        0     7619 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/howto/morethanbindings.md
--rw-r--r--   0        0        0     3569 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/howto/serialization.md
--rw-r--r--   0        0        0     2868 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/howto/ssh.md
--rw-r--r--   0        0        0     2053 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/index.md
--rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/notes/index.md
--rw-r--r--   0        0        0     7076 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/notes/pyversions.md
--rw-r--r--   0        0        0     8843 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/docs/source/notes/unicode.md
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/LICENSE
--rw-r--r--   0        0        0      326 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/README.md
--rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/asyncio/coroutines.py
--rw-r--r--   0        0        0     7089 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/asyncio/helloworld_pubsub_dealerrouter.py
--rw-r--r--   0        0        0     2290 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/asyncio/router_router.py
--rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/asyncio/tornado_asyncio.py
--rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/cython/.gitignore
--rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/cython/README.md
--rw-r--r--   0        0        0     1680 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/cython/cyzmq.pyx
--rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/cython/example.py
--rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/cython/setup.py
--rw-r--r--   0        0        0     1598 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/device/device.py
--rw-r--r--   0        0        0      550 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/draft/client-server.py
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/draft/install.sh
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/draft/radio-dish.py
--rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/eventloop/asyncweb.py
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/eventloop/coroutines.py
--rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/eventloop/echo.py
--rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/eventloop/echofuture.py
--rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/eventloop/echostream.py
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/gevent/poll.py
--rw-r--r--   0        0        0     1109 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/gevent/reqrep.py
--rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/gevent/simple.py
--rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/heartbeat/heart.py
--rw-r--r--   0        0        0     2775 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/heartbeat/heartbeater.py
--rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/heartbeat/ping.py
--rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/heartbeat/pong.py
--rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/logger/zmqlogger.py
--rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/mongodb/client.py
--rw-r--r--   0        0        0     3256 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/mongodb/controller.py
--rw-r--r--   0        0        0     2341 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/monitoring/simple_monitor.py
--rw-r--r--   0        0        0     5001 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/monitoring/zmq_monitor_class.py
--rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/poll/pair.py
--rw-r--r--   0        0        0     1401 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/poll/pubsub.py
--rw-r--r--   0        0        0     1767 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/poll/reqrep.py
--rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/pubsub/publisher.py
--rw-r--r--   0        0        0     1849 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/pubsub/subscriber.py
--rwxr-xr-x   0        0        0     2033 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/pubsub/topics_pub.py
--rwxr-xr-x   0        0        0     1773 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/pubsub/topics_sub.py
--rw-r--r--   0        0        0     3746 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/security/asyncio-ironhouse.py
--rw-r--r--   0        0        0     2007 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/security/generate_certificates.py
--rw-r--r--   0        0        0      569 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/security/grasslands.py
--rw-r--r--   0        0        0     4265 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/security/ioloop-ironhouse.py
--rw-r--r--   0        0        0     3172 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/security/ironhouse.py
--rw-r--r--   0        0        0     3181 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/security/stonehouse.py
--rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/security/strawhouse.py
--rw-r--r--   0        0        0     2353 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/security/woodhouse.py
--rw-r--r--   0        0        0     2575 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/serialization/serialsocket.py
--rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/examples/win32-interrupt/display.py
--rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/mypy.ini
--rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/mypy_tests/test_context.py
--rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/mypy_tests/test_socket.py
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/mypy_tests/test_toplevel.py
--rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/README.md
--rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/debian/changelog
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/debian/compat
--rw-r--r--   0        0        0     2298 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/debian/control
--rw-r--r--   0        0        0     6045 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/debian/copyright
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/debian/pyzmq.dsc.obs
--rwxr-xr-x   0        0        0     1708 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/debian/rules
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/debian/source/format
--rw-r--r--   0        0        0     2338 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/obs/_service
--rw-r--r--   0        0        0     7812 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/packaging/redhat/python-pyzmq.spec
--rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/perf/Dockerfile
--rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/perf/Makefile
--rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/perf/collect.py
--rw-r--r--   0        0        0   167790 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/perf/perf.ipynb
--rw-r--r--   0        0        0     6333 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/perf/perf.py
--rw-r--r--   0        0        0     4665 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/pytest.ini
--rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/test-requirements.txt
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/tools/backend_imports.py
--rw-r--r--   0        0        0     1668 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/tools/collect_cmake.py
--rw-r--r--   0        0        0     1655 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/tools/find_vcredist.py
--rw-r--r--   0        0        0     1959 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/tools/install_libzmq.sh
--rw-r--r--   0        0        0     3786 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/tools/run_with_env.cmd
--rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/tools/showvcvars.py
--rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/tools/test_sdist.py
--rw-r--r--   0        0        0     1340 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/tools/test_wheel.py
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/tools/wheel-requirements.txt
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/__init__.pxd
--rw-r--r--   0        0        0     2196 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/__init__.py
--rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/__init__.pyi
--rw-r--r--   0        0        0    24618 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/_future.py
--rw-r--r--   0        0        0      489 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/_typing.py
--rw-r--r--   0        0        0     6271 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/asyncio.py
--rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/auth/__init__.py
--rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/auth/asyncio.py
--rw-r--r--   0        0        0    16337 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/auth/base.py
--rw-r--r--   0        0        0     4331 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/auth/certs.py
--rw-r--r--   0        0        0     1298 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/auth/ioloop.py
--rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/auth/thread.py
--rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/__init__.py
--rw-r--r--   0        0        0     3483 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/__init__.pyi
--rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/README.md
--rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/__init__.py
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/_cdefs.h
--rw-r--r--   0        0        0     1314 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/_cffi_src.c
--rw-r--r--   0        0        0     2886 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/_poll.py
--rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/context.py
--rw-r--r--   0        0        0     1572 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/devices.py
--rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/error.py
--rw-r--r--   0        0        0     6488 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/message.py
--rw-r--r--   0        0        0    11450 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/socket.py
--rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cffi/utils.py
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cython/__init__.pxd
--rw-r--r--   0        0        0      322 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cython/__init__.py
--rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cython/_externs.pxd
--rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cython/_zmq.pxd
--rw-r--r--   0        0        0    57680 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cython/_zmq.py
--rw-r--r--   0        0        0     7562 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cython/constant_enums.pxi
--rw-r--r--   0        0        0     4564 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/cython/libzmq.pxd
--rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/backend/select.py
--rw-r--r--   0        0        0    28329 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/constants.py
--rw-r--r--   0        0        0     5076 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/decorators.py
--rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/devices/__init__.py
--rw-r--r--   0        0        0     9564 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/devices/basedevice.py
--rw-r--r--   0        0        0     1294 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/devices/monitoredqueue.py
--rw-r--r--   0        0        0     1930 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/devices/monitoredqueuedevice.py
--rw-r--r--   0        0        0     2849 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/devices/proxydevice.py
--rw-r--r--   0        0        0     3212 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/devices/proxysteerabledevice.py
--rw-r--r--   0        0        0     5392 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/error.py
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/eventloop/__init__.py
--rw-r--r--   0        0        0     6444 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/eventloop/_deprecated.py
--rw-r--r--   0        0        0     2569 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/eventloop/future.py
--rw-r--r--   0        0        0      767 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/eventloop/ioloop.py
--rw-r--r--   0        0        0    23640 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/eventloop/zmqstream.py
--rw-r--r--   0        0        0     1331 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/green/__init__.py
--rw-r--r--   0        0        0    10827 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/green/core.py
--rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/green/device.py
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/green/eventloop/__init__.py
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/green/eventloop/ioloop.py
--rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/green/eventloop/zmqstream.py
--rw-r--r--   0        0        0     2950 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/green/poll.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/log/__init__.py
--rw-r--r--   0        0        0     4008 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/log/__main__.py
--rw-r--r--   0        0        0     7108 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/log/handlers.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/py.typed
--rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/ssh/__init__.py
--rw-r--r--   0        0        0     3358 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/ssh/forward.py
--rw-r--r--   0        0        0    13532 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/ssh/tunnel.py
--rw-r--r--   0        0        0      722 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/__init__.py
--rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/__init__.pyi
--rw-r--r--   0        0        0     2603 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/attrsettr.py
--rw-r--r--   0        0        0    14384 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/context.py
--rw-r--r--   0        0        0     4331 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/frame.py
--rw-r--r--   0        0        0     5725 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/poll.py
--rw-r--r--   0        0        0    34005 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/socket.py
--rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/stopwatch.py
--rw-r--r--   0        0        0     3700 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/tracker.py
--rw-r--r--   0        0        0     1606 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/sugar/version.py
--rw-r--r--   0        0        0     8169 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/__init__.py
--rw-r--r--   0        0        0     5564 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/conftest.py
--rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/cython_ext.pyx
--rw-r--r--   0        0        0     9993 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_asyncio.py
--rw-r--r--   0        0        0    14750 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_auth.py
--rw-r--r--   0        0        0     8945 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_cffi_backend.py
--rw-r--r--   0        0        0      962 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_constants.py
--rw-r--r--   0        0        0    12600 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_context.py
--rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_cython.py
--rw-r--r--   0        0        0     9623 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_decorators.py
--rw-r--r--   0        0        0     6004 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_device.py
--rw-r--r--   0        0        0     1371 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_draft.py
--rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_error.py
--rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_etc.py
--rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_ext.py
--rw-r--r--   0        0        0    10608 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_future.py
--rw-r--r--   0        0        0     1973 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_imports.py
--rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_includes.py
--rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_ioloop.py
--rw-r--r--   0        0        0     6948 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_log.py
--rw-r--r--   0        0        0    11320 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_message.py
--rw-r--r--   0        0        0     3059 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_monitor.py
--rw-r--r--   0        0        0     8285 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_monqueue.py
--rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_multipart.py
--rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_mypy.py
--rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_pair.py
--rw-r--r--   0        0        0     7106 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_poll.py
--rw-r--r--   0        0        0     4004 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_proxy_steerable.py
--rw-r--r--   0        0        0     1015 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_pubsub.py
--rw-r--r--   0        0        0     1764 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_reqrep.py
--rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_retry_eintr.py
--rw-r--r--   0        0        0     7805 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_security.py
--rw-r--r--   0        0        0    23771 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_socket.py
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_ssh.py
--rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_version.py
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_win32_shim.py
--rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_z85.py
--rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/tests/test_zmqstream.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/__init__.py
--rw-r--r--   0        0        0     7031 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/buffers.pxd
--rw-r--r--   0        0        0     6125 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/garbage.py
--rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/getpid_compat.h
--rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/interop.py
--rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/ipcmaxlen.h
--rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/jsonapi.py
--rw-r--r--   0        0        0     3300 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/monitor.py
--rw-r--r--   0        0        0     1625 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/mutex.h
--rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/pyversion_compat.h
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/strtypes.py
--rw-r--r--   0        0        0     4896 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/win32.py
--rw-r--r--   0        0        0     1806 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/z85.py
--rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmq/utils/zmq_compat.h
--rw-r--r--   0        0        0     4103 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/zmqversion.py
--rw-r--r--   0        0        0     6126 2022-11-09 12:37:21.000000 pyzmq-26.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1853 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.circleci/config.yml
+-rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.coveragerc
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.flake8
+-rw-r--r--   0        0        0     2697 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/workflows/test-docs.yml
+-rw-r--r--   0        0        0     5095 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     6029 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.gitignore
+-rw-r--r--   0        0        0      733 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.mailmap
+-rw-r--r--   0        0        0      128 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.obs/workflows.yml
+-rw-r--r--   0        0        0     2067 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.prettierignore
+-rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.readthedocs.yml
+-rw-r--r--   0        0        0     4810 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/AUTHORS.md
+-rw-r--r--   0        0        0    13427 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/CMakeLists.txt
+-rw-r--r--   0        0        0     2251 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/LICENSE.md
+-rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/MANIFEST.in
+-rw-r--r--   0        0        0     2964 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/README.md
+-rw-r--r--   0        0        0     2116 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/README.md
+-rw-r--r--   0        0        0     2751 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/authors.py
+-rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/chrislaws.md
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/ellisonbg.md
+-rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/frankwiles.md
+-rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/juliantaylor.md
+-rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/ledgerx.md
+-rw-r--r--   0        0        0      731 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/lothiraldan.md
+-rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/minrk.md
+-rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/takluyver.md
+-rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-bsd.txt
+-rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-mplv2-any-osi.txt
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-mplv2.txt
+-rw-r--r--   0        0        0     1541 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/SECURITY.md
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/Vagrantfile
+-rw-r--r--   0        0        0      692 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/build_cffi.py
+-rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/bundle.py
+-rw-r--r--   0        0        0     3634 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/constants.py
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/templates/constant_enums.pxi
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/templates/constants.py
+-rw-r--r--   0        0        0    11525 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/cmake/FindVcvars.cmake
+-rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/cmake/Findsodium.cmake
+-rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/codecov.yml
+-rw-r--r--   0        0        0     3639 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/Makefile
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/requirements.txt
+-rw-r--r--   0        0        0     8686 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/_static/logo.png
+-rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/_static/zeromq.ico
+-rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/index.md
+-rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.asyncio.md
+-rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.auth.asyncio.md
+-rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.auth.ioloop.md
+-rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.auth.md
+-rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.auth.thread.md
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.decorators.md
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.devices.md
+-rw-r--r--   0        0        0     1807 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.eventloop.future.md
+-rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.eventloop.ioloop.md
+-rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.eventloop.zmqstream.md
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.green.md
+-rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.log.handlers.md
+-rw-r--r--   0        0        0     4381 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.md
+-rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.ssh.tunnel.md
+-rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.utils.jsonapi.md
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.utils.monitor.md
+-rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.utils.win32.md
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.utils.z85.md
+-rw-r--r--   0        0        0    41718 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/changelog.md
+-rw-r--r--   0        0        0     8271 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/conf.py
+-rw-r--r--   0        0        0    10786 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/build.md
+-rw-r--r--   0        0        0     3980 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/devices.md
+-rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/draft.md
+-rw-r--r--   0        0        0     5732 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/eventloop.md
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/index.md
+-rw-r--r--   0        0        0     9610 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/logging.md
+-rw-r--r--   0        0        0     6548 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/morethanbindings.md
+-rw-r--r--   0        0        0     3569 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/serialization.md
+-rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/ssh.md
+-rw-r--r--   0        0        0     2025 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/index.md
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/LICENSE
+-rw-r--r--   0        0        0      326 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/README.md
+-rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/asyncio/coroutines.py
+-rw-r--r--   0        0        0     7089 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/asyncio/helloworld_pubsub_dealerrouter.py
+-rw-r--r--   0        0        0     2290 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/asyncio/router_router.py
+-rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/asyncio/tornado_asyncio.py
+-rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/.gitignore
+-rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/README.md
+-rw-r--r--   0        0        0     1680 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/cyzmq.pyx
+-rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/example.py
+-rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/setup.py
+-rw-r--r--   0        0        0     1598 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/device/device.py
+-rw-r--r--   0        0        0      550 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/draft/client-server.py
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/draft/install.sh
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/draft/radio-dish.py
+-rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/asyncweb.py
+-rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/coroutines.py
+-rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/echo.py
+-rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/echofuture.py
+-rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/echostream.py
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/gevent/poll.py
+-rw-r--r--   0        0        0     1109 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/gevent/reqrep.py
+-rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/gevent/simple.py
+-rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/heartbeat/heart.py
+-rw-r--r--   0        0        0     2775 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/heartbeat/heartbeater.py
+-rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/heartbeat/ping.py
+-rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/heartbeat/pong.py
+-rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/logger/zmqlogger.py
+-rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/mongodb/client.py
+-rw-r--r--   0        0        0     3256 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/mongodb/controller.py
+-rw-r--r--   0        0        0     2341 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/monitoring/simple_monitor.py
+-rw-r--r--   0        0        0     5001 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/monitoring/zmq_monitor_class.py
+-rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/poll/pair.py
+-rw-r--r--   0        0        0     1401 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/poll/pubsub.py
+-rw-r--r--   0        0        0     1767 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/poll/reqrep.py
+-rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/pubsub/publisher.py
+-rw-r--r--   0        0        0     1849 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/pubsub/subscriber.py
+-rwxr-xr-x   0        0        0     2033 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/pubsub/topics_pub.py
+-rwxr-xr-x   0        0        0     1773 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/pubsub/topics_sub.py
+-rw-r--r--   0        0        0     3746 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/asyncio-ironhouse.py
+-rw-r--r--   0        0        0     2007 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/generate_certificates.py
+-rw-r--r--   0        0        0      569 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/grasslands.py
+-rw-r--r--   0        0        0     4265 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/ioloop-ironhouse.py
+-rw-r--r--   0        0        0     3172 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/ironhouse.py
+-rw-r--r--   0        0        0     3181 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/stonehouse.py
+-rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/strawhouse.py
+-rw-r--r--   0        0        0     2353 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/woodhouse.py
+-rw-r--r--   0        0        0     2575 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/serialization/serialsocket.py
+-rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/win32-interrupt/display.py
+-rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/mypy.ini
+-rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/mypy_tests/test_context.py
+-rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/mypy_tests/test_socket.py
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/mypy_tests/test_toplevel.py
+-rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/README.md
+-rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/changelog
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/compat
+-rw-r--r--   0        0        0     2298 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/control
+-rw-r--r--   0        0        0     6045 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/copyright
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/pyzmq.dsc.obs
+-rwxr-xr-x   0        0        0     1708 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/rules
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/source/format
+-rw-r--r--   0        0        0     2338 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/obs/_service
+-rw-r--r--   0        0        0     7812 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/redhat/python-pyzmq.spec
+-rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/Dockerfile
+-rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/Makefile
+-rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/collect.py
+-rw-r--r--   0        0        0   167790 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/perf.ipynb
+-rw-r--r--   0        0        0     6333 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/perf.py
+-rw-r--r--   0        0        0     4665 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/pytest.ini
+-rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/test-requirements.txt
+-rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/backend_imports.py
+-rw-r--r--   0        0        0     1668 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/collect_cmake.py
+-rw-r--r--   0        0        0     1655 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/find_vcredist.py
+-rw-r--r--   0        0        0     1959 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/install_libzmq.sh
+-rw-r--r--   0        0        0     3786 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/run_with_env.cmd
+-rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/showvcvars.py
+-rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/test_sdist.py
+-rw-r--r--   0        0        0     1340 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/test_wheel.py
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/wheel-requirements.txt
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/__init__.pxd
+-rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/__init__.py
+-rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/__init__.pyi
+-rw-r--r--   0        0        0    24516 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/_future.py
+-rw-r--r--   0        0        0      525 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/_typing.py
+-rw-r--r--   0        0        0     6306 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/asyncio.py
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/__init__.py
+-rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/asyncio.py
+-rw-r--r--   0        0        0    16337 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/base.py
+-rw-r--r--   0        0        0     4331 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/certs.py
+-rw-r--r--   0        0        0     1298 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/ioloop.py
+-rw-r--r--   0        0        0     4103 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/thread.py
+-rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/__init__.py
+-rw-r--r--   0        0        0     3483 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/__init__.pyi
+-rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/README.md
+-rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/__init__.py
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/_cdefs.h
+-rw-r--r--   0        0        0     1314 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/_cffi_src.c
+-rw-r--r--   0        0        0     2886 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/_poll.py
+-rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/context.py
+-rw-r--r--   0        0        0     1572 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/devices.py
+-rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/error.py
+-rw-r--r--   0        0        0     6488 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/message.py
+-rw-r--r--   0        0        0    11450 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/socket.py
+-rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/utils.py
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/__init__.pxd
+-rw-r--r--   0        0        0      322 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/__init__.py
+-rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/_externs.pxd
+-rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/_zmq.pxd
+-rw-r--r--   0        0        0    57809 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/_zmq.py
+-rw-r--r--   0        0        0     7562 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/constant_enums.pxi
+-rw-r--r--   0        0        0     4564 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/libzmq.pxd
+-rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/select.py
+-rw-r--r--   0        0        0    28341 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/constants.py
+-rw-r--r--   0        0        0     5112 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/decorators.py
+-rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/__init__.py
+-rw-r--r--   0        0        0     9581 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/basedevice.py
+-rw-r--r--   0        0        0     1294 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/monitoredqueue.py
+-rw-r--r--   0        0        0     1930 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/monitoredqueuedevice.py
+-rw-r--r--   0        0        0     2849 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/proxydevice.py
+-rw-r--r--   0        0        0     3212 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/proxysteerabledevice.py
+-rw-r--r--   0        0        0     5368 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/error.py
+-rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/__init__.py
+-rw-r--r--   0        0        0     6444 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/_deprecated.py
+-rw-r--r--   0        0        0     2596 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/future.py
+-rw-r--r--   0        0        0      767 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/ioloop.py
+-rw-r--r--   0        0        0    23439 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/zmqstream.py
+-rw-r--r--   0        0        0     1366 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/__init__.py
+-rw-r--r--   0        0        0    10836 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/core.py
+-rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/device.py
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/eventloop/__init__.py
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/eventloop/ioloop.py
+-rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/eventloop/zmqstream.py
+-rw-r--r--   0        0        0     2986 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/poll.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/log/__init__.py
+-rw-r--r--   0        0        0     4008 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/log/__main__.py
+-rw-r--r--   0        0        0     7101 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/log/handlers.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/py.typed
+-rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/ssh/__init__.py
+-rw-r--r--   0        0        0     3358 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/ssh/forward.py
+-rw-r--r--   0        0        0    13534 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/ssh/tunnel.py
+-rw-r--r--   0        0        0      722 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/__init__.py
+-rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/__init__.pyi
+-rw-r--r--   0        0        0     2638 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/attrsettr.py
+-rw-r--r--   0        0        0    14552 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/context.py
+-rw-r--r--   0        0        0     4259 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/frame.py
+-rw-r--r--   0        0        0     5752 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/poll.py
+-rw-r--r--   0        0        0    34639 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/socket.py
+-rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/stopwatch.py
+-rw-r--r--   0        0        0     3605 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/tracker.py
+-rw-r--r--   0        0        0     1615 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/version.py
+-rw-r--r--   0        0        0     8169 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/__init__.py
+-rw-r--r--   0        0        0     5564 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/conftest.py
+-rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/cython_ext.pyx
+-rw-r--r--   0        0        0     9993 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_asyncio.py
+-rw-r--r--   0        0        0    14750 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_auth.py
+-rw-r--r--   0        0        0     8945 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_cffi_backend.py
+-rw-r--r--   0        0        0      962 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_constants.py
+-rw-r--r--   0        0        0    12600 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_context.py
+-rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_cython.py
+-rw-r--r--   0        0        0     9623 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_decorators.py
+-rw-r--r--   0        0        0     6004 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_device.py
+-rw-r--r--   0        0        0     1371 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_draft.py
+-rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_error.py
+-rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_etc.py
+-rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_ext.py
+-rw-r--r--   0        0        0    10608 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_future.py
+-rw-r--r--   0        0        0     1973 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_imports.py
+-rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_includes.py
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_ioloop.py
+-rw-r--r--   0        0        0     6948 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_log.py
+-rw-r--r--   0        0        0    11320 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_message.py
+-rw-r--r--   0        0        0     3059 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_monitor.py
+-rw-r--r--   0        0        0     8285 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_monqueue.py
+-rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_multipart.py
+-rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_mypy.py
+-rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_pair.py
+-rw-r--r--   0        0        0     7106 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_poll.py
+-rw-r--r--   0        0        0     4004 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_proxy_steerable.py
+-rw-r--r--   0        0        0     1015 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_pubsub.py
+-rw-r--r--   0        0        0     1764 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_reqrep.py
+-rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_retry_eintr.py
+-rw-r--r--   0        0        0     7805 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_security.py
+-rw-r--r--   0        0        0    24126 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_socket.py
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_ssh.py
+-rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_version.py
+-rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_win32_shim.py
+-rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_z85.py
+-rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_zmqstream.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/__init__.py
+-rw-r--r--   0        0        0     7031 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/buffers.pxd
+-rw-r--r--   0        0        0     6125 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/garbage.py
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/getpid_compat.h
+-rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/interop.py
+-rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/ipcmaxlen.h
+-rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/jsonapi.py
+-rw-r--r--   0        0        0     3312 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/monitor.py
+-rw-r--r--   0        0        0     1625 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/mutex.h
+-rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/pyversion_compat.h
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/strtypes.py
+-rw-r--r--   0        0        0     4918 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/win32.py
+-rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/z85.py
+-rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/zmq_compat.h
+-rw-r--r--   0        0        0     4103 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmqversion.py
+-rw-r--r--   0        0        0     6126 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/PKG-INFO
```

### Comparing `pyzmq-26.0.0b1/.circleci/config.yml` & `pyzmq-26.0.0b2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/.github/ISSUE_TEMPLATE/bug.yml` & `pyzmq-26.0.0b2/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/.github/ISSUE_TEMPLATE/config.yml` & `pyzmq-26.0.0b2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/.github/workflows/test.yml` & `pyzmq-26.0.0b2/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,22 @@
   push:
     branches-ignore:
       - "dependabot/**"
       - "pre-commit-ci-update-config"
     paths-ignore:
       - "docs/**"
       - "tools/**"
-      - .github/workflows/wheels.yml
+      - ".github/workflows/*"
+      - "!.github/workflows/test.yml"
   pull_request:
     paths-ignore:
       - "docs/**"
       - "tools/**"
-      - .github/workflows/wheels.yml
+      - ".github/workflows/*"
+      - "!.github/workflows/test.yml"
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 env:
   FORCE_COLOR: "1"
```

### Comparing `pyzmq-26.0.0b1/.github/workflows/wheels.yml` & `pyzmq-26.0.0b2/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/.gitignore` & `pyzmq-26.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/.mailmap` & `pyzmq-26.0.0b2/.mailmap`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/.pre-commit-config.yaml` & `pyzmq-26.0.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/AUTHORS.md` & `pyzmq-26.0.0b2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/CMakeLists.txt` & `pyzmq-26.0.0b2/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -221,46 +221,64 @@
         "builds/msvc/vs${PYZMQ_LIBSODIUM_VS_VERSION}/libsodium.sln"
       )
       list(APPEND libsodium_build ${PYZMQ_LIBSODIUM_MSBUILD_ARGS})
       execute_process(
         COMMAND ${libsodium_build}
         WORKING_DIRECTORY ${bundled_libsodium_SOURCE_DIR}
         COMMAND_ECHO STDOUT
-        COMMAND_ERROR_IS_FATAL ANY
+        # COMMAND_ERROR_IS_FATAL ANY
+        RESULT_VARIABLE _status
       )
+      if (_status) 
+        message(FATAL_ERROR "failed to build libsodium")
+      endif()
       file(GLOB_RECURSE BUILT_LIB "${bundled_libsodium_SOURCE_DIR}/**/libsodium.lib")
       message(STATUS "copy ${BUILT_LIB} ${libsodium_lib}")
       file(COPY_FILE ${BUILT_LIB} ${libsodium_lib})
     else()
       list(APPEND libsodium_configure
         ./configure
         --prefix=${BUNDLE_DIR}
         --with-pic
+        --disable-dependency-tracking
         --disable-shared
         --enable-static
       )
       list(APPEND libsodium_configure ${PYZMQ_LIBSODIUM_CONFIGURE_ARGS})
       execute_process(
         COMMAND ${libsodium_configure}
         WORKING_DIRECTORY ${bundled_libsodium_SOURCE_DIR}
         COMMAND_ECHO      STDOUT
-        COMMAND_ERROR_IS_FATAL ANY
+        # COMMAND_ERROR_IS_FATAL ANY
+        RESULT_VARIABLE _status
       )
+      # COMMAND_ERROR_IS_FATAL requires cmake 3.19, ubuntu 20.04 has 3.16
+      if (_status) 
+        message(FATAL_ERROR "failed to configure libsodium")
+      endif()
       execute_process(
         COMMAND make
         WORKING_DIRECTORY ${bundled_libsodium_SOURCE_DIR}
         COMMAND_ECHO STDOUT
-        COMMAND_ERROR_IS_FATAL ANY
+        # COMMAND_ERROR_IS_FATAL ANY
+        RESULT_VARIABLE _status
       )
+      if (_status) 
+        message(FATAL_ERROR "failed to build libsodium")
+      endif()
       execute_process(
         COMMAND make install
         WORKING_DIRECTORY ${bundled_libsodium_SOURCE_DIR}
         COMMAND_ECHO STDOUT
-        COMMAND_ERROR_IS_FATAL ANY
+        # COMMAND_ERROR_IS_FATAL ANY
+        RESULT_VARIABLE _status
       )
+      if (_status) 
+        message(FATAL_ERROR "failed to install libsodium")
+      endif()
     endif()
   endif()
 
   # use libzmq's own cmake, so we can import the libzmq-static target
   set(ENABLE_CURVE ON)
   set(ENABLE_DRAFTS ${ZMQ_DRAFT_API})
   set(WITH_LIBSODIUM ON)
@@ -347,15 +365,16 @@
   set(ZMQ_EXT_NAME "_zmq")
   set(ZMQ_C "${EXT_SRC_DIR}/${ZMQ_EXT_NAME}.c")
   set(ZMQ_PYX "${CMAKE_CURRENT_SOURCE_DIR}/zmq/backend/cython/${ZMQ_EXT_NAME}.py")
   add_custom_command(
     OUTPUT ${ZMQ_C}
     DEPENDS ${ZMQ_PYX}
     VERBATIM
-    COMMAND "${CYTHON}"
+    COMMAND "${Python_EXECUTABLE}"
+            -mcython
             --3str
             --output-file ${ZMQ_C}
             --module-name "zmq.backend.cython._zmq"
             ${ZMQ_PYX}
   )
 endif()
```

### Comparing `pyzmq-26.0.0b1/CONTRIBUTING.md` & `pyzmq-26.0.0b2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/LICENSE.md` & `pyzmq-26.0.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/README.md` & `pyzmq-26.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/README.md` & `pyzmq-26.0.0b2/RELICENSE/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/authors.py` & `pyzmq-26.0.0b2/RELICENSE/authors.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/chrislaws.md` & `pyzmq-26.0.0b2/RELICENSE/chrislaws.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/ellisonbg.md` & `pyzmq-26.0.0b2/RELICENSE/ellisonbg.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/frankwiles.md` & `pyzmq-26.0.0b2/RELICENSE/frankwiles.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/juliantaylor.md` & `pyzmq-26.0.0b2/RELICENSE/juliantaylor.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/ledgerx.md` & `pyzmq-26.0.0b2/RELICENSE/ledgerx.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/lothiraldan.md` & `pyzmq-26.0.0b2/RELICENSE/lothiraldan.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/minrk.md` & `pyzmq-26.0.0b2/RELICENSE/minrk.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/takluyver.md` & `pyzmq-26.0.0b2/RELICENSE/takluyver.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/templates/relicense-template-bsd.txt` & `pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-bsd.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/templates/relicense-template-mplv2-any-osi.txt` & `pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-mplv2-any-osi.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/RELICENSE/templates/relicense-template-mplv2.txt` & `pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-mplv2.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/SECURITY.md` & `pyzmq-26.0.0b2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/Vagrantfile` & `pyzmq-26.0.0b2/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/buildutils/build_cffi.py` & `pyzmq-26.0.0b2/buildutils/build_cffi.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/buildutils/constants.py` & `pyzmq-26.0.0b2/buildutils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             if "AUTOGENERATED_BELOW_HERE" in line:
                 original_file = "".join(original_lines)
                 break
         else:
             raise ValueError("Never encountered AUTOGENERATED_BELOW_HERE")
 
     global_assignments = []
-    all_lines = ["__all__: List[str] = ["]
+    all_lines = ["__all__: list[str] = ["]
     for cls_name in sorted(dir(constants)):
         if cls_name.startswith("_"):
             continue
         cls = getattr(constants, cls_name)
         if not isinstance(cls, type) or not issubclass(cls, enum.Enum):
             continue
```

### Comparing `pyzmq-26.0.0b1/cmake/FindVcvars.cmake` & `pyzmq-26.0.0b2/cmake/FindVcvars.cmake`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/cmake/Findsodium.cmake` & `pyzmq-26.0.0b2/cmake/Findsodium.cmake`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/docs/Makefile` & `pyzmq-26.0.0b2/docs/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
-SPHINXOPTS    =
-SPHINXBUILD   = sphinx-build
-PAPER         =
-BUILDDIR      = build
-SRCDIR        = source
+SPHINXOPTS    ?= -n
+SPHINXBUILD   ?= sphinx-build
+PAPER         ?=
+BUILDDIR      ?= build
+SRCDIR        ?= source
 
 # Internal variables.
 PAPEROPT_a4     = -D latex_paper_size=a4
 PAPEROPT_letter = -D latex_paper_size=letter
 ALLSPHINXOPTS   = -d $(BUILDDIR)/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) $(SRCDIR)
 
 .PHONY: help clean html dirhtml pickle json htmlhelp qthelp latex changes linkcheck doctest
```

### Comparing `pyzmq-26.0.0b1/docs/source/_static/logo.png` & `pyzmq-26.0.0b2/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/docs/source/_static/zeromq.ico` & `pyzmq-26.0.0b2/docs/source/_static/zeromq.ico`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/docs/source/changelog.md` & `pyzmq-26.0.0b2/docs/source/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 Please [report](https://github.com/zeromq/pyzmq/issues/new) any issues you encounter building pyzmq.
 
 See [build docs](building-pyzmq) for more info.
 
 __New__:
 
 - Experimental support for wheels on windows-arm64
+- `Socket.bind('tcp://ip:0')` can be used as a context manager to bind to a random port.
+  The resulting URL can be retrieved as `socket.last_endpoint`.
 
 __Enhancements__:
 
 - `repr(Frame)` now produces a nice repr, summarizing Frame contents (without getting too large),
   e.g. `<zmq.Frame(b'abcdefghijkl'...52B)>`
 
 __Breaking changes__:
@@ -116,16 +118,16 @@
 - Fixed toml parse error in `pyproject.toml`,
   when installing from source with very old pip.
 - Removed expressed dependency on `py` when running with pypy,
   which hasn't been used in some time.
 
 Deprecated:
 
-- {class}`zmq.auth.ioloop.IOLoopAuthenticator` is deprecated in favor of {class}`zmq.auth.asyncio.AsyncioAuthenticator`
-- As part of migrating toward modern pytest, {class}`zmq.tests.BaseZMQTestCase` is deprecated and should not be used outside pyzmq.
+- `zmq.auth.ioloop.IOLoopAuthenticator` is deprecated in favor of {class}`zmq.auth.asyncio.AsyncioAuthenticator`
+- As part of migrating toward modern pytest, `zmq.tests.BaseZMQTestCase` is deprecated and should not be used outside pyzmq.
 - `python setup.py test` is deprecated as a way to launch the tests.
   Just use `pytest`.
 
 Removed:
 
 - Bundled subset of tornado's IOLoop (deprecated since pyzmq 17) is removed,
   so ZMQStream cannot be used without an actual install of tornado.
@@ -193,15 +195,15 @@
 Fixing some regressions in 23.0:
 
 - Fix global name of `zmq.EVENT_HANDSHAKE_*` constants
 - Fix constants missing when using `import zmq.green as zmq`
 
 Compatibility fixes:
 
-- {func}`zmq.utils.monitor.recv_monitor_msg` now supports async Sockets.
+- {func}`zmq.utils.monitor.recv_monitor_message` now supports async Sockets.
 - Fix build with mingw
 
 ## 23.0.0
 
 Changes:
 
 - all zmq constants are now available as Python enums
@@ -427,15 +429,15 @@
 - Fixes in tests and examples
 
 ## 19.0
 
 - Cython backend: Build Cython extensions with language level "3str" (requires Cython 0.29)
 - Cython backend: You can now `cimport zmq`
 - Asyncio: Fix memory leak in Poller
-- Log: Much improved logging in {mod}`zmq.log` (see {doc}`howto/logging`)
+- Log: Much improved logging in {mod}`zmq.log.handlers` (see {doc}`howto/logging`)
 - Log: add `python -m zmq.log` entrypoint
 - Sources generated with Cython 0.29.15
 
 ## 18.1.1
 
 - Fix race condition when shutting down ZAP thread while events are still processing (only affects tests)
 - Publish wheels for Python 3.8 on all platforms
@@ -482,15 +484,15 @@
 - Remove unneeded link of libstdc++ on PyPy
 
 ## 17.1.0
 
 - Bump bundled libzmq to 4.2.5
 - Improve tornado 5.0 compatibility
   (use {meth}`~tornado.ioloop.IOLoop.current` instead of {meth}`~tornado.ioloop.IOLoop.instance`
-  to get default loops in {class}`.ZMQStream` and {class}`.IOLoopAuthenticator`)
+  to get default loops in {class}`.ZMQStream` and `.IOLoopAuthenticator`)
 - Add support for {func}`.curve_public`
 - Remove delayed import of json in `send/recv_json`
 - Add {meth}`.Authenticator.configure_curve_callback`
 - Various build fixes
 - sdist sources generated with Cython 0.28.3
 - Stop building wheels for Python 3.4, start building wheels for Python 3.7
 
@@ -503,21 +505,21 @@
   Messages smaller than this are always copied, regardless of `copy=False`,
   to avoid overhead of zero-copy bookkeeping on small messages.
 
 - Added visible deprecation warnings to bundled tornado IOLoop.
   Tornado eventloop integration shouldn't be used without a proper tornado install
   since pyzmq 14.
 
-- Allow pyzmq asyncio/tornado integration to run without installing {func}`zmq_poll`
+- Allow pyzmq asyncio/tornado integration to run without installing `zmq_poll`
   implementation. The following methods and classes are deprecated and no longer required:
 
-  - {func}`zmq.eventloop.ioloop.install`
-  - {class}`zmq.eventloop.ioloop.IOLoop`
-  - {func}`zmq.asyncio.install`
-  - {class}`zmq.asyncio.ZMQEventLoop`
+  - `zmq.eventloop.ioloop.install`
+  - `zmq.eventloop.ioloop.IOLoop`
+  - `zmq.asyncio.install`
+  - `zmq.asyncio.ZMQEventLoop`
 
 - Set RPATH correctly when building on macOS.
 
 - Compatibility fixes with tornado 5.0.dev (may not be quite enough for 5.0 final,
   which is not yet released as of pyzmq 17).
 
 - Draft support for CLIENT-SERVER `routing_id` and `group`.
@@ -548,21 +550,21 @@
 
 ## 16.0
 
 - Support for Python 2.6 and Python 3.2 is dropped. For old Pythons, use {command}`pip install "pyzmq<16"` to get the last version of pyzmq that supports these versions.
 - Include zmq.h
 - Deprecate `zmq.Stopwatch`. Native Python timing tools can be used instead.
 - Better support for using pyzmq as a Cython library
-  \- bundle zmq.h when pyzmq bundles libzmq as an extension
-  \- add {func}`zmq.get_library_dirs` to find bundled libzmq
+  - bundle zmq.h when pyzmq bundles libzmq as an extension
+  - add {func}`zmq.get_library_dirs` to find bundled libzmq
 - Updates to setup.py for Cython 0.25 compatibility
 - Various asyncio/future fixes:
-  \- support raw sockets in pollers
-  \- allow cancelling async sends
-- Fix {meth}`IOLoop.current` in {mod}`zmq.green`
+  - support raw sockets in pollers
+  - allow cancelling async sends
+- Fix `IOLoop.current()` in {mod}`zmq.green`
 
 ## 15.4
 
 - Load bundled libzmq extension with import rather than CDLL,
   which should fix some manifest issues in certain cases on Windows.
 - Avoid installing asyncio sources on Python 2, which confuses some tools that run `python -m compileall`, which reports errors on the Python 3-only files.
 - Bundle msvcp.dll in Windows wheels on CPython 3.5,
@@ -579,20 +581,20 @@
 - Bump bundled libzmq to 4.1.5, using tweetnacl for bundled curve support instead of libsodium
 - FIX: include .pxi includes in installation for consumers of Cython API
 - FIX: various fixes in new async sockets
 - Introduce {mod}`zmq.decorators` API for decorating functions to create sockets or contexts
 - Add {meth}`zmq.Socket.subscribe` and {meth}`zmq.Socket.unsubscribe` methods to sockets, so that assignment is no longer needed for subscribing. Verbs should be methods!
   Assignment is still supported for backward-compatibility.
 - Accept text (unicode) input to z85 encoding, not just bytes
-- {meth}`zmq.Context.socket` forwards keyword arguments to the {class}`Socket` constructor
+- {meth}`zmq.Context.socket` forwards keyword arguments to the {class}`~.zmq.Socket` constructor
 
 ## 15.2
 
 - FIX: handle multiple events in a single register call in {mod}`zmq.asyncio`
-- FIX: unicode/bytes bug in password prompt in {mod}`zmq.ssh` on Python 3
+- FIX: unicode/bytes bug in password prompt in `zmq.ssh` on Python 3
 - FIX: workaround gevent monkeypatches in garbage collection thread
 - update bundled minitornado from tornado-4.3.
 - improved inspection by setting `binding=True` in cython compile options
 - add asyncio Authenticator implementation in {mod}`zmq.auth.asyncio`
 - workaround overflow bug in libzmq preventing receiving messages larger than `MAX_INT`
 
 ## 15.1
@@ -600,18 +602,18 @@
 - FIX: Remove inadvertent tornado dependency when using {mod}`zmq.asyncio`
 - FIX: 15.0 Python 3.5 wheels didn't work on Windows
 - Add GSSAPI support to Authenticators
 - Support new constants defined in upcoming libzmq-4.2.dev
 
 ## 15.0
 
-PyZMQ 15 adds Future-returning sockets and pollers for both {mod}`asyncio` and {mod}`tornado`.
+PyZMQ 15 adds Future-returning sockets and pollers for both {mod}`asyncio` and {mod}`tornado.concurrent`.
 
 - add {mod}`asyncio` support via {mod}`zmq.asyncio`
-- add {mod}`tornado` future support via {mod}`zmq.eventloop.future`
+- add {mod}`tornado.concurrent` future support via {mod}`zmq.eventloop.future`
 - trigger bundled libzmq if system libzmq is found to be \< 3.
   System libzmq 2 can be forced by explicitly requesting `--zmq=/prefix/`.
 
 ## 14.7.0
 
 Changes:
 
@@ -636,15 +638,15 @@
   - catch EACCES on Windows
 - include libsodium when building bundled libzmq on Windows (includes wheels on PyPI)
 - pyzmq no longer bundles external libzmq when making a bdist.
   You can use [delocate](https://pypi.org/project/delocate/) to do this.
 
 Bugfixes:
 
-- add missing {attr}`ndim` on memoryviews of Frames
+- add missing `ndim` on memoryviews of Frames
 - allow {func}`copy.copy` and {func}`copy.deepcopy` on Sockets, Contexts
 
 ## 14.5.0
 
 Changes:
 
 - use pickle.DEFAULT_PROTOCOL by default in send_pickle
@@ -668,15 +670,15 @@
 ## 14.4.0
 
 New features:
 
 - Experimental support for libzmq-4.1.0 rc (new constants, plus {func}`zmq.has`).
 - Update bundled libzmq to 4.0.5
 - Update bundled libsodium to 1.0.0
-- Fixes for SSH dialogs when using {mod}`zmq.ssh` to create tunnels
+- Fixes for SSH dialogs when using {mod}`zmq.ssh.tunnel` to create tunnels
 - More build/link/load fixes on OS X and Solaris
 - Get Frame metadata via dict access (libzmq 4)
 - Contexts and Sockets are context managers (term/close on `__exit__`)
 - Add {class}`zmq.utils.win32.allow_interrupt` context manager for catching SIGINT on Windows
 
 Bugs fixed:
 
@@ -695,15 +697,15 @@
 - Fixes to tests
 - Pull upstream fixes to zmq.ssh for ssh multiplexing
 
 ## 14.3.0
 
 - PyZMQ no longer calls {meth}`.Socket.close` or {meth}`.Context.term` during process cleanup.
   Changes to garbage collection in Python 3.4 make this impossible to do sensibly.
-- {meth}`ZMQStream.close` closes its socket immediately, rather than scheduling a timeout.
+- {meth}`.ZMQStream.close` closes its socket immediately, rather than scheduling a timeout.
 - Raise the original ImportError when importing zmq fails.
   Should be more informative than `no module cffi...`.
 
 ```{warning}
 Users of Python 3.4 should not use pyzmq \< 14.3, due to changes in garbage collection.
 ```
 
@@ -752,15 +754,15 @@
 ## 14.0.1
 
 Bugfix release
 
 - Update bundled libzmq to current (4.0.3).
 - Fix bug in {meth}`.Context.destroy` with no open sockets.
 - Threadsafety fixes in the garbage collector.
-- Python 3 fixes in {mod}`zmq.ssh`.
+- Python 3 fixes in {mod}`zmq.ssh.tunnel`.
 
 ## 14.0.0
 
 - Update bundled libzmq to current (4.0.1).
 - Backends are now implemented in `zmq.backend` instead of `zmq.core`.
   This has no effect on public APIs.
 - Various build improvements for Cython and CFFI backends (PyPy compiles at build time).
@@ -816,15 +818,15 @@
 **must declare these attributes at the class level**.
 ```
 
 ### Experiments Removed
 
 - The Threadsafe ZMQStream experiment in 2.2.0.1 was deemed inappropriate and not useful,
   and has been removed.
-- The {mod}`zmq.web` experiment has been removed,
+- The `zmq.web` experiment has been removed,
   to be developed as a [standalone project](https://github.com/ellisonbg/zmqweb).
 
 ### New Stuff
 
 - Support for PyPy via CFFI backend (requires py, ctypes-configure, and cffi).
 
 - Add support for new APIs in libzmq-3
@@ -834,15 +836,15 @@
   - {meth}`.Context.set`
   - {meth}`.Context.get`
   - {meth}`.Frame.set`
   - {meth}`.Frame.get`
   - {func}`zmq.proxy`
   - {class}`zmq.devices.Proxy`
   - Exceptions for common zmq errnos: {class}`zmq.Again`, {class}`zmq.ContextTerminated`
-    (subclass {class}`ZMQError`, so fully backward-compatible).
+    (subclass {class}`~.ZMQError`, so fully backward-compatible).
 
 - Setting and getting {attr}`.Socket.hwm` sets or gets *both* SNDHWM/RCVHWM for libzmq-3.
 
 - Implementation splits core Cython bindings from pure-Python subclasses
   with sugar methods (send/recv_multipart). This should facilitate
   non-Cython backends and PyPy support \[spoiler: it did!\].
 
@@ -863,15 +865,15 @@
 
 These features are marked 'experimental', which means that their APIs are not set in stone,
 and may be removed or changed in incompatible ways in later releases.
 
 #### Threadsafe ZMQStream
 
 With the IOLoop inherited from tornado, there is exactly one method that is threadsafe:
-{meth}`.IOLoop.add_callback`.  With this release, we are trying an experimental option
+{meth}`~.tornado.ioloop.IOLoop.add_callback`.  With this release, we are trying an experimental option
 to pass all IOLoop calls via this method, so that ZMQStreams can be used from one thread
 while the IOLoop runs in another.  To try out a threadsafe stream:
 
 ```python
 stream = ZMQStream(socket, threadsafe=True)
 ```
 
@@ -909,81 +911,81 @@
 ```{note}
 As of this release, all code outside `zmq.core` is BSD licensed (where
 possible), to allow more permissive use of less-critical code and utilities.
 ```
 
 ### Name Changes
 
-- The {class}`~.Message` class has been renamed to {class}`~.Frame`, to better match other
+- The `Message` class has been renamed to {class}`~.Frame`, to better match other
   zmq bindings. The old Message name remains for backwards-compatibility.  Wherever pyzmq
   docs say "Message", they should refer to a complete zmq atom of communication (one or
   more Frames, connected by ZMQ_SNDMORE). Please report any remaining instances of
   Message==MessagePart with an Issue (or better yet a Pull Request).
 - All `foo_unicode` methods are now called `foo_string` (`_unicode` remains for
   backwards compatibility).  This is not only for cross-language consistency, but it makes
   more sense in Python 3, where native strings are unicode, and the `_unicode` suffix
   was wedded too much to Python 2.
 
 ### Other Changes and Removals
 
-- `prefix` removed as an unused keyword argument from {meth}`~.Socket.send_multipart`.
+- `prefix` removed as an unused keyword argument from {meth}`~.zmq.Socket.send_multipart`.
 - ZMQStream {meth}`~.ZMQStream.send` default has been changed to `copy=True`, so it matches
-  Socket {meth}`~.Socket.send`.
+  Socket {meth}`~.zmq.Socket.send`.
 - ZMQStream {meth}`~.ZMQStream.on_err` is deprecated, because it never did anything.
 - Python 2.5 compatibility has been dropped, and some code has been cleaned up to reflect
   no-longer-needed hacks.
-- Some Cython files in {mod}`zmq.core` have been split, to reduce the amount of
+- Some Cython files in `zmq.core` have been split, to reduce the amount of
   Cython-compiled code.  Much of the body of these files were pure Python, and thus did
   not benefit from the increased compile time.  This change also aims to ease maintaining
   feature parity in other projects, such as
   [pyzmq-ctypes](https://github.com/svpcom/pyzmq-ctypes).
 
 ### New Stuff
 
-- {class}`~.Context` objects can now set default options when they create a socket. These
+- {class}`~.zmq.Context` objects can now set default options when they create a socket. These
   are set and accessed as attributes to the context.  Socket options that do not apply to a
   socket (e.g. SUBSCRIBE on non-SUB sockets) will simply be ignored.
 - {meth}`~.ZMQStream.on_recv_stream` has been added, which adds the stream itself as a
   second argument to the callback, making it easier to use a single callback on multiple
   streams.
-- A {attr}`~Frame.more` boolean attribute has been added to the {class}`~.Frame` (née
+- A `Frame.more` boolean attribute has been added to the {class}`~.Frame` (née
   Message) class, so that frames can be identified as terminal without extra queries of
-  {attr}`~.Socket.rcvmore`.
+  `Socket.rcvmore`.
 
 ### Experimental New Stuff
 
 These features are marked 'experimental', which means that their APIs are not
 set in stone, and may be removed or changed in incompatible ways in later releases.
 
-- {mod}`zmq.web` added for load-balancing requests in a tornado webapp with zeromq.
+- `zmq.web` added for load-balancing requests in a tornado webapp with zeromq.
 
 ## 2.1.11
 
 - remove support for LABEL prefixes.  A major feature of libzmq-3.0, the LABEL
   prefix, has been removed from libzmq, prior to the first stable libzmq 3.x release.
 
-  - The prefix argument to {meth}`~.Socket.send_multipart` remains, but it continue to behave in
+  - The prefix argument to {meth}`~.zmq.Socket.send_multipart` remains, but it continue to behave in
     exactly the same way as it always has on 2.1.x, simply prepending message parts.
-  - {meth}`~.Socket.recv_multipart` will always return a list, because prefixes are once
+  - {meth}`~.zmq.Socket.recv_multipart` will always return a list, because prefixes are once
     again indistinguishable from regular message parts.
 
-- add {meth}`.Socket.poll` method, for simple polling of events on a single socket.
+- add {meth}`.zmq.Socket.poll` method, for simple polling of events on a single socket.
 
-- no longer require monkeypatching tornado IOLoop.  The {class}`.ioloop.ZMQPoller` class
+- no longer require monkeypatching tornado IOLoop.  The `ioloop.ZMQPoller` class
   is a poller implementation that matches tornado's expectations, and pyzmq sockets can
   be used with any tornado application just by specifying the use of this poller.  The
   pyzmq IOLoop implementation now only trivially differs from tornado's.
 
-  It is still recommended to use {func}`.ioloop.install`, which sets *both* the zmq and
+  It is still recommended to use `ioloop.install()`, which sets *both* the zmq and
   tornado global IOLoop instances to the same object, but it is no longer necessary.
 
   ```{warning}
   The most important part of this change is that the `IOLoop.READ/WRITE/ERROR`
   constants now match tornado's, rather than being mapped directly to the zmq
-  `POLLIN/OUT/ERR`. So applications that used the low-level {meth}`IOLoop.add_handler`
+  `POLLIN/OUT/ERR`. So applications that used the low-level `IOLoop.add_handler`
   code with `POLLIN/OUT/ERR` directly (used to work, but was incorrect), rather than
   using the IOLoop class constants will no longer work. Fixing these to use the IOLoop
   constants should be insensitive to the actual value of the constants.
   ```
 
 ## 2.1.10
 
@@ -996,68 +998,68 @@
 
   - send a message with label-prefix with:
 
     ```python
     send_multipart([b"msg", b"parts"], prefix=[b"label", b"prefix"])
     ```
 
-  - {meth}`recv_multipart` returns a tuple of `(prefix,msg)` if a label prefix is detected
+  - {meth}`zmq.Socket.recv_multipart` returns a tuple of `(prefix,msg)` if a label prefix is detected
 
   - ZMQStreams and devices also respect the LABEL prefix
 
-- add czmq-style close&term as {meth}`ctx.destroy`, so that {meth}`ctx.term`
+- add czmq-style close&term as {meth}`zmq.Context.destroy`, so that {meth}`zmq.Context.term`
   remains threadsafe and 1:1 with libzmq.
 
-- {meth}`Socket.close` takes optional linger option, for setting linger prior
+- {meth}`zmq.Socket.close` takes optional linger option, for setting linger prior
   to closing.
 
-- add {func}`~zmq.core.version.zmq_version_info` and
-  {func}`~zmq.core.version.pyzmq_version_info` for getting libzmq and pyzmq versions as
+- add {func}`~.zmq_version_info` and
+  {func}`~.pyzmq_version_info` for getting libzmq and pyzmq versions as
   tuples of numbers. This helps with the fact that version string comparison breaks down
   once versions get into double-digits.
 
 - ioloop changes merged from upstream [Tornado](https://www.tornadoweb.org) 2.1
 
 ## 2.1.9
 
 - added zmq.ssh tools for tunneling socket connections, copied from IPython
 - Expanded sockopt support to cover changes in libzmq-4.0 dev.
-- Fixed an issue that prevented {exc}`KeyboardInterrupts` from being catchable.
-- Added attribute-access for set/getsockopt.  Setting/Getting attributes of {class}`Sockets`
+- Fixed an issue that prevented {exc}`KeyboardInterrupt` from being catchable.
+- Added attribute-access for set/getsockopt.  Setting/Getting attributes of {class}`~.zmq.Socket`s
   with the names of socket options is mapped to calls of set/getsockopt.
 
 ```python
 s.hwm = 10
 s.identity = b"whoda"
 s.linger
 # -1
 ```
 
-- Terminating a {class}`~Context` closes the sockets it created, matching the behavior in
+- Terminating a {class}`~.zmq.Context` closes the sockets it created, matching the behavior in
   [czmq](http://czmq.zeromq.org/).
-- {class}`ThreadDevices` use {meth}`Context.instance` to create sockets, so they can use
+- {class}`.ThreadDevice`s use {meth}`.zmq.Context.instance` to create sockets, so they can use
   inproc connections to sockets in other threads.
 - fixed units error on {func}`zmq.select`, where the poll timeout was 1000 times longer
   than expected.
 - Add missing `DEALER/ROUTER` socket type names (currently aliases, to be replacements for `XREP/XREQ`).
 - base libzmq dependency raised to 2.1.4 (first stable release) from 2.1.0.
 
 ## 2.1.7.1
 
 - bdist for 64b Windows only.  This fixed a type mismatch on the `ZMQ_FD` sockopt
   that only affected that platform.
 
 ## 2.1.7
 
 - Added experimental support for libzmq-3.0 API
-- Add {func}`zmq.eventloop.ioloop.install` for using pyzmq's IOLoop in a tornado
+- Add `zmq.eventloop.ioloop.install` for using pyzmq's IOLoop in a tornado
   application.
 
 ## 2.1.4
 
 - First version with binary distribution support
-- Added {meth}`~Context.instance()` method for using a single Context throughout an application
+- Added {meth}`zmq.Context.instance()` method for using a single Context throughout an application
   without passing references around.
 
 [cython-build-requires]: https://groups.google.com/g/cython-users/c/ZqKFQmS0JdA/m/1FrK1ApYBAAJ
 [pyczmq]: https://github.com/zeromq/pyczmq
 [scikit-build-core]: https://scikit-build-core.readthedocs.io
```

### Comparing `pyzmq-26.0.0b1/docs/source/conf.py` & `pyzmq-26.0.0b2/docs/source/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
 import sys
+from pathlib import Path
 
-# add repo root to sys.path
-here = os.path.dirname(__file__)
-sys.path.append(os.path.abspath(os.path.join(here, os.pardir, os.pardir)))
+# add repo root to sys.path for buildutils import
+here = Path(__file__).parent.absolute()
+repo_root = here.parents[1]
+sys.path.append(str(repo_root))
 
 # set target libzmq version
 from buildutils.bundle import bundled_version
 
+# remove repo root from sys.path
+sys.path = sys.path[:-1]
+
 target_libzmq = bundled_version
 
 # -- General configuration -----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
@@ -37,16 +41,18 @@
 myst_enable_extensions = [
     "colon_fence",
     "linkify",
     "smartquotes",
     "substitution",
 ]
 
+myst_linkify_fuzzy_links = False
+
 # The suffix of source filenames.
-source_suffix = ['.md', '.rst']
+source_suffix = ['.md']
 
 # The encoding of source files.
 source_encoding = 'utf-8'
 
 # The master toctree document.
 master_doc = 'index'
 
@@ -113,15 +119,41 @@
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 # List of Sphinx warnings that will not be raised
 suppress_warnings = ['epub.unknown_project_files']
 
+nitpick_ignore = [
+    # napoleon seems to try to resolve everything
+    # in type descriptions, leave some prose keywords alone
+    ('py:class', 'optional'),
+    ('py:class', 'Python object'),
+    ('py:class', 'native socket'),
+    ('py:class', 'iterable'),
+    ('py:class', 'callable'),
+    # suppress warnings on some old outdated symbols
+    ('py:class', 'basestring'),
+    ('py:class', 'unicode'),
+]
 
+autodoc_type_aliases = {
+    # 'Socket': 'zmq.Socket',
+    # 'Context': 'zmq.Context',
+    # Cython
+    'C.int': 'int',
+    'bint': 'bool',
+    # type aliases
+    '_MonitorMessage': 'dict',
+    'Frame': 'zmq.Frame',
+    'Socket': 'zmq.Socket',
+    'Context': 'zmq.Context',
+    '_SocketType': 'zmq.Socket',
+    '_ContextType': 'zmq.Context',
+}
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  Major themes that come with
 # Sphinx are currently 'default' and 'sphinxdoc'.
 html_theme = "pydata_sphinx_theme"
 
 html_logo = "_static/logo.png"
```

### Comparing `pyzmq-26.0.0b1/docs/source/howto/build.md` & `pyzmq-26.0.0b2/docs/source/howto/build.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/docs/source/howto/devices.md` & `pyzmq-26.0.0b2/docs/source/howto/devices.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 ```{seealso}
 ØMQ Guide [Device coverage](https://zguide.zeromq.org/docs/chapter2/#ZeroMQ-s-Built-In-Proxy-Function).
 ```
 
 ØMQ has a notion of Devices - simple programs that manage a send-recv pattern for
 connecting two or more sockets. Being full programs, devices include a `while(True)`
 loop and thus block execution permanently once invoked. We have provided in the
-{mod}`devices` subpackage some facilities for running these devices in the background, as
+{mod}`~.zmq.devices` subpackage some facilities for running these devices in the background, as
 well as a custom three-socket [MonitoredQueue](monitored-queue) device.
 
 ## BackgroundDevices
 
 It seems fairly rare that in a Python program one would actually want to create a zmq
 device via {func}`.device` in the main thread, since such a call would block execution
 forever. The most likely model for launching devices is in background threads or
 processes. We have provided classes for launching devices in a background thread with
 {class}`.ThreadDevice` and via multiprocessing with {class}`.ProcessDevice`. For
 threadsafety and running across processes, these methods do not take Socket objects as
 arguments, but rather socket types, and then the socket creation and configuration happens
-via the BackgroundDevice's {meth}`foo_in` proxy methods. For each configuration method
+via the BackgroundDevice's `foo_in()` proxy methods. For each configuration method
 (bind/connect/setsockopt), there are proxy methods for calling those methods on the Socket
 objects created in the background thread or process, prefixed with 'in\_' or 'out\_',
 corresponding to the `in_socket` and `out_socket`:
 
 ```
 from zmq.devices import ProcessDevice
 
@@ -75,8 +75,8 @@
 is most logical for the monitor socket, since it will never receive messages, and the
 in/out prefix is well suited to the PUB/SUB topic subscription model. All messages sent on
 `mons` will be multipart, the first part being the prefix corresponding to the socket that
 received the message.
 
 Or for launching an MQ in the background, there are {class}`.ThreadMonitoredQueue` and
 {class}`.ProcessMonitoredQueue`, which function just like the base
-BackgroundDevice objects, but add {meth}`foo_mon` methods for configuring the monitor socket.
+BackgroundDevice objects, but add `foo_mon()` methods for configuring the monitor socket.
```

### Comparing `pyzmq-26.0.0b1/docs/source/howto/draft.md` & `pyzmq-26.0.0b2/docs/source/howto/draft.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/docs/source/howto/eventloop.md` & `pyzmq-26.0.0b2/docs/source/howto/eventloop.md`

 * *Files 25% similar despite different names*

```diff
@@ -29,87 +29,40 @@
     s.subscribe(b"")
     while True:
         msg = await s.recv_multipart()
         print("received", msg)
     s.close()
 ```
 
-````{note}
-In PyZMQ \< 17, an additional step is needed to register the zmq poller prior to starting any async code:
-
-```python
-import zmq.asyncio
-zmq.asyncio.install()
-
-ctx = zmq.asyncio.Context()
-```
-
-This step is no longer needed in pyzmq 17.
-
-````
-
 ## Tornado IOLoop
 
-[Tornado] includes an eventloop for handing poll events on filedescriptors and
-native sockets. We have included a small part of Tornado (specifically its
-{mod}`.ioloop`), and adapted its {class}`IOStream` class into {class}`.ZMQStream` for
-handling poll events on ØMQ sockets. A ZMQStream object works much like a Socket object,
-but instead of calling {meth}`~.Socket.recv` directly, you register a callback with
-{meth}`~.ZMQStream.on_recv`. Callbacks can also be registered for send events
-with {meth}`~.ZMQStream.on_send`.
-
-(futures)=
-
-### Futures and coroutines
-
-```{note}
-With recent Python (3.6) and tornado (5),
-there's no reason to use {mod}`zmq.eventloop.future`
-instead of the strictly-more-compatible {mod}`zmq.asyncio`.
-```
-
-PyZMQ 15 adds {mod}`zmq.eventloop.future`, containing a Socket subclass
-that returns {class}`~.tornado.concurrent.Future` objects for use in {mod}`tornado` coroutines.
-To use this API, import {class}`zmq.eventloop.future.Context`.
-Sockets created by this Context will return Futures from any would-be blocking method.
-
-```python
-from tornado import gen, ioloop
-import zmq
-from zmq.eventloop.future import Context
-
-ctx = Context.instance()
+[Tornado] adds some utility on top of asyncio.
+You can use {mod}`zmq.asyncio` socket in a tornado application without any special handling.
 
+We have adapted tornado's {class}`~.tornado.iostream.IOStream` class into {class}`~.ZMQStream` for
+handling message events on ØMQ sockets. A ZMQStream object works much like a Socket object,
+but instead of calling {meth}`~.zmq.Socket.recv` directly, you register a callback with
+{meth}`~.ZMQStream.on_recv_stream`, which will be called with the result of `~.zmq.Socket.recv_multipart`.
+Callbacks can also be registered for send events with {meth}`~.ZMQStream.on_send`.
 
-@gen.coroutine
-def recv():
-    s = ctx.socket(zmq.SUB)
-    s.connect("tcp://127.0.0.1:5555")
-    s.subscribe(b"")
-    while True:
-        msg = yield s.recv_multipart()
-        print("received", msg)
-    s.close()
-```
-
-### {class}`ZMQStream`
+### {class}`.ZMQStream`
 
-{class}`ZMQStream` objects let you register callbacks to handle messages as they arrive,
+{class}`.ZMQStream` objects let you register callbacks to handle messages as they arrive,
 for use with the tornado eventloop.
 
-#### {meth}`send`
+#### {meth}`.ZMQStream.send`
 
 ZMQStream objects do have {meth}`~.ZMQStream.send` and {meth}`~.ZMQStream.send_multipart`
-methods, which behaves the same way as {meth}`.Socket.send`, but instead of sending right
-away, the {class}`.IOLoop` will wait until socket is able to send (for instance if `HWM`
+methods, which behaves the same way as {meth}`.zmq.Socket.send`, but instead of sending right
+away, the {class}`~.tornado.ioloop.IOLoop` will wait until socket is able to send (for instance if `HWM`
 is met, or a `REQ/REP` pattern prohibits sending at a certain point). Messages sent via
 send will also be passed to the callback registered with {meth}`~.ZMQStream.on_send` after
 sending.
 
-#### {meth}`on_recv`
+#### {meth}`~.ZMQStream.on_recv`
 
 {meth}`.ZMQStream.on_recv` is the primary method for using a ZMQStream. It registers a
 callback to fire with messages as they are received, which will *always* be multipart,
 even if its length is 1. You can easily use this to build things like an echo socket:
 
 ```python
 s = ctx.socket(zmq.REP)
@@ -121,27 +74,27 @@
     stream.send_multipart(msg)
 
 
 stream.on_recv(echo)
 ioloop.IOLoop.instance().start()
 ```
 
-on_recv can also take a `copy` flag, just like {meth}`.Socket.recv`. If `copy=False`, then
+on_recv can also take a `copy` flag, just like {meth}`.zmq.Socket.recv`. If `copy=False`, then
 callbacks registered with on_recv will receive tracked {class}`.Frame` objects instead of
 bytes.
 
 ```{note}
 A callback must be registered using either {meth}`.ZMQStream.on_recv` or
 {meth}`.ZMQStream.on_recv_stream` before any data will be received on the
 underlying socket.  This allows you to temporarily pause processing on a
 socket by setting both callbacks to None.  Processing can later be resumed
 by restoring either callback.
 ```
 
-#### {meth}`on_recv_stream`
+#### {meth}`~.ZMQStream.on_recv_stream`
 
 {meth}`.ZMQStream.on_recv_stream` is just like on_recv above, but the callback will be
 passed both the message and the stream, rather than just the message.  This is meant to make
 it easier to use a single callback with multiple streams.
 
 ```python
 s1 = ctx.socket(zmq.REP)
@@ -159,87 +112,23 @@
 
 stream1.on_recv_stream(echo)
 stream2.on_recv_stream(echo)
 
 ioloop.IOLoop.instance().start()
 ```
 
-#### {meth}`flush`
+#### {meth}`~.ZMQStream.flush`
 
 Sometimes with an eventloop, there can be multiple events ready on a single iteration of
-the loop. The {meth}`~.ZMQStream.flush` method allows developers to pull messages off of
+the loop. The {meth}`.ZMQStream.flush` method allows developers to pull messages off of
 the queue to enforce some priority over the event loop ordering. flush pulls any pending
 events off of the queue. You can specify to flush only recv events, only send events, or
 any events, and you can specify a limit for how many events to flush in order to prevent
 starvation.
 
-### {func}`install()`
-
-```{note}
-If you are using pyzmq \< 17, there is an additional step
-to tell tornado to use the zmq poller instead of its default.
-{func}`.ioloop.install` is no longer needed for pyzmq ≥ 17.
-```
-
-With PyZMQ's ioloop, you can use zmq sockets in any tornado application.  You can tell tornado to use zmq's poller by calling the {func}`.ioloop.install` function:
-
-```python
-from zmq.eventloop import ioloop
-
-ioloop.install()
-```
-
-You can also do the same thing by requesting the global instance from pyzmq:
-
-```python
-from zmq.eventloop.ioloop import IOLoop
-
-loop = IOLoop.current()
-```
-
-This configures tornado's {class}`tornado.ioloop.IOLoop` to use zmq's poller,
-and registers the current instance.
-
-Either `install()` or retrieving the zmq instance must be done before the global * instance is registered, else there will be a conflict.
-
-It is possible to use PyZMQ sockets with tornado *without* registering as the global instance,
-but it is less convenient. First, you must instruct the tornado IOLoop to use the zmq poller:
-
-```python
-from zmq.eventloop.ioloop import ZMQIOLoop
-
-loop = ZMQIOLoop()
-```
-
-Then, when you instantiate tornado and ZMQStream objects, you must pass the `io_loop`
-argument to ensure that they use this loop, instead of the global instance.
-
-This is especially useful for writing tests, such as this:
-
-```python
-from tornado.testing import AsyncTestCase
-from zmq.eventloop.ioloop import ZMQIOLoop
-from zmq.eventloop.zmqstream import ZMQStream
-
-
-class TestZMQBridge(AsyncTestCase):
-    # Use a ZMQ-compatible I/O loop so that we can use `ZMQStream`.
-    def get_new_ioloop(self):
-        return ZMQIOLoop()
-```
-
-You can also manually install this IOLoop as the global tornado instance, with:
-
-```python
-from zmq.eventloop.ioloop import ZMQIOLoop
-
-loop = ZMQIOLoop()
-loop.install()
-```
-
 (zmq-green)=
 
 ## PyZMQ and gevent
 
 PyZMQ ≥ 2.2.0.1 ships with a [gevent](https://www.gevent.org/) compatible API as {mod}`zmq.green`.
 To use it, simply:
 
@@ -272,8 +161,8 @@
 ```{seealso}
 zmq.green examples [on GitHub](https://github.com/zeromq/pyzmq/tree/HEAD/examples/gevent).
 ```
 
 {mod}`zmq.green` began as [gevent_zeromq](https://github.com/tmc/gevent-zeromq),
 merged into the pyzmq project.
 
-[tornado]: https://tornadoweb.org
+[tornado]: https://www.tornadoweb.org
```

### Comparing `pyzmq-26.0.0b1/docs/source/howto/logging.md` & `pyzmq-26.0.0b2/docs/source/howto/logging.md`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 the PUBHandler does work with topics, and the handler has an attribute `root_topic`:
 
 ```python
 handler.root_topic = "myprogram"
 ```
 
 Python loggers also have loglevels. The base topic of messages emitted by the PUBHandler
-will be of the form: `<handler.root_topic>.<loglevel>`, e.g. 'myprogram.INFO' or
+will be of the form: `<handler.root_topic>.<loglevel>`, e.g. `myprogram.INFO` or
 'whatever.ERROR'. This way, subscribers can easily subscribe to subsets of the logging
 messages. Log messages are always two-part, where the first part is the topic tree, and
 the second part is the actual log message.
 
 ```python
 logger.info("hello there")
 print(sub.recv_multipart())
```

### Comparing `pyzmq-26.0.0b1/docs/source/howto/morethanbindings.md` & `pyzmq-26.0.0b2/docs/source/howto/morethanbindings.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,30 +6,19 @@
 
 PyZMQ is ostensibly the Python bindings for [ØMQ], but the project, following
 Python's 'batteries included' philosophy, provides more than just Python methods and
 objects for calling into the ØMQ C++ library.
 
 ## The Core as Bindings
 
-PyZMQ is currently broken up into four subpackages. First, is the Core. {mod}`zmq.core`
+PyZMQ is currently broken up into subpackages. First, is the Backend. `zmq.backend`
 contains the actual bindings for ZeroMQ, and no extended functionality beyond the very
-basic. The core modules are split, such that each basic ZeroMQ object (or function, if no
-object is associated) is a separate module, e.g. {mod}`zmq.core.context` contains the
-{class}`.Context` object, {mod}`zmq.core.poll` contains a {class}`.Poller` object, as well
-as the {func}`.select` function, etc. ZMQ constants are, for convenience, all kept
-together in {mod}`zmq.core.constants`.
-
-There are two reasons for breaking the core into submodules: *recompilation* and
-*derivative projects*. The monolithic PyZMQ became quite tedious to have to recompile
-everything for a small change to a single object. With separate files, that's no longer
-necessary. The second reason has to do with Cython. PyZMQ is written in Cython, a tool for
-efficiently writing C-extensions for Python. By separating out our objects into individual
-`pyx` files, each with their declarations in a `pxd` header, other projects can write
-extensions in Cython and call directly to ZeroMQ at the C-level without the penalty of
-going through our Python objects.
+basics required.
+This is the _compiled_ portion of pyzmq,
+either with Cython (for CPython) or CFFI (for PyPy).
 
 ## Thread Safety
 
 In ØMQ, Contexts are threadsafe objects, but Sockets are **not**. It is safe to use a
 single Context (e.g. via {meth}`zmq.Context.instance`) in your entire multithreaded
 application, but you should create sockets on a per-thread basis. If you share sockets
 across threads, you are likely to encounter uncatchable c-level crashes of your
@@ -42,15 +31,15 @@
 ```
 
 ## Socket Options as Attributes
 
 ```{versionadded} 2.1.9
 ```
 
-In 0MQ, socket options are set/retrieved with the {meth}`set/getsockopt` methods. With the
+In 0MQ, socket options are set/retrieved with the `set/getsockopt()` methods. With the
 class-based approach in pyzmq, it would be logical to perform these operations with
 simple attribute access, and this has been added in pyzmq 2.1.9. Simply assign to or
 request a Socket attribute with the (case-insensitive) name of a sockopt, and it should
 behave just as you would expect:
 
 ```python
 s = ctx.socket(zmq.DEALER)
@@ -120,57 +109,54 @@
 with socket.connect(url):
     s.send_multipart([b"message"])
 # exiting connect context calls socket.disconnect(url)
 ```
 
 ## Core Extensions
 
-We have extended the core functionality in two ways that appear inside the {mod}`core`
-bindings, and are not general ØMQ features.
+We have extended the core functionality in some ways that appear inside the `zmq.sugar` layer, and are not general ØMQ features.
 
 ### Builtin Serialization
 
 First, we added common serialization with the builtin {py:mod}`json` and {py:mod}`pickle`
-as first-class methods to the {class}`Socket` class. A socket has the methods
-{meth}`~.Socket.send_json` and {meth}`~.Socket.send_pyobj`, which correspond to sending an
+as first-class methods to the {class}`~.zmq.Socket` class. A socket has the methods
+{meth}`~.zmq.Socket.send_json` and {meth}`~.zmq.Socket.send_pyobj`, which correspond to sending an
 object over the wire after serializing with {mod}`json` and {mod}`pickle` respectively,
 and any object sent via those methods can be reconstructed with the
-{meth}`~.Socket.recv_json` and {meth}`~.Socket.recv_pyobj` methods. Unicode strings are
+{meth}`~.zmq.Socket.recv_json` and {meth}`~.zmq.Socket.recv_pyobj` methods. Unicode strings are
 other objects that are not unambiguously sendable over the wire, so we include
-{meth}`~.Socket.send_string` and {meth}`~.Socket.recv_string` that simply send bytes
+{meth}`~.zmq.Socket.send_string` and {meth}`~.zmq.Socket.recv_string` that simply send bytes
 after encoding the message ('utf-8' is the default).
 
 ```{seealso}
 - {ref}`Further information <serialization>` on serialization in pyzmq.
-- {ref}`Our Unicode discussion <unicode>` for more information on the trials and
-  tribulations of working with Unicode in a C extension while supporting Python 2 and 3.
 ```
 
 ### MessageTracker
 
-The second extension of basic ØMQ functionality is the {class}`MessageTracker`. The
+The second extension of basic ØMQ functionality is the {class}`.MessageTracker`. The
 MessageTracker is an object used to track when the underlying ZeroMQ is done with a
 message buffer. One of the main use cases for ØMQ in Python is the ability to perform
 non-copying sends. Thanks to Python's buffer interface, many objects (including NumPy
 arrays) provide the buffer interface, and are thus directly sendable. However, as with any
 asynchronous non-copying messaging system like ØMQ or MPI, it can be important to know
 when the message has actually been sent, so it is safe again to edit the buffer without
 worry of corrupting the message. This is what the MessageTracker is for.
 
 The MessageTracker is a simple object, but there is a penalty to its use. Since by its
 very nature, the MessageTracker must involve threadsafe communication (specifically a
-builtin {py:class}`~Queue.Queue` object), instantiating a MessageTracker takes a modest
+builtin {py:class}`~queue.Queue` object), instantiating a MessageTracker takes a modest
 amount of time (10s of µs), so in situations instantiating many small messages, this can
 actually dominate performance. As a result, tracking is optional, via the `track` flag,
 which is optionally passed, always defaulting to `False`, in each of the three places
 where a Frame object (the pyzmq object for wrapping a segment of a message) is
 instantiated: The {class}`.Frame` constructor, and non-copying sends and receives.
 
 A MessageTracker is very simple, and has just one method and one attribute. The property
-{attr}`MessageTracker.done` will be `True` when the Frame(s) being tracked are no
+{attr}`.MessageTracker.done` will be `True` when the Frame(s) being tracked are no
 longer in use by ØMQ, and {meth}`.MessageTracker.wait` will block, waiting for the
 Frame(s) to be released.
 
 ```{Note}
 A Frame cannot be tracked after it has been instantiated without tracking. If a
 Frame is to even have the *option* of tracking, it must be constructed with
 `track=True`.
```

### Comparing `pyzmq-26.0.0b1/docs/source/howto/serialization.md` & `pyzmq-26.0.0b2/docs/source/howto/serialization.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/docs/source/howto/ssh.md` & `pyzmq-26.0.0b2/docs/source/howto/ssh.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ```{versionadded} 2.1.9
 ```
 
 You may want to connect ØMQ sockets across machines, or untrusted networks. One common way
 to do this is to tunnel the connection via SSH. [IPython] introduced some tools for
 tunneling ØMQ connections over ssh in simple cases. These functions have been brought into
-pyzmq as {mod}`zmq.ssh` under IPython's BSD license.
+pyzmq as {mod}`zmq.ssh.tunnel` under IPython's BSD license.
 
 PyZMQ will use the shell ssh command via [pexpect] by default, but it also supports
 using [paramiko] for tunnels, so it should work on Windows.
 
 An SSH tunnel has five basic components:
 
 - server : the SSH server through which the tunnel will be created
@@ -43,29 +43,29 @@
 from zmq import ssh
 
 ssh.tunnel_connection(sock, "tcp://10.0.1.2:5555", "server")
 ```
 
 Note that `"server"` can actually be a fully specified `"user@server:port"` ssh url.
 Since this really just launches a shell command, all your ssh configuration of usernames,
-aliases, keys, etc. will be respected. If necessary, {func}`tunnel_connection` does take
+aliases, keys, etc. will be respected. If necessary, {func}`.tunnel_connection` does take
 arguments for specific passwords, private keys (the ssh `-i` option), and non-default
 choice of whether to use paramiko.
 
 If you are on the same network as the machine, but it is only listening on localhost, you
 can still connect by making the machine itself the server, and using loopback as the
 remote ip:
 
 ```python
 from zmq import ssh
 
 ssh.tunnel_connection(sock, "tcp://127.0.0.1:5555", "10.0.1.2")
 ```
 
-The {func}`tunnel_connection` function is a simple utility that forwards a random
+The {func}`.tunnel_connection` function is a simple utility that forwards a random
 localhost port to the real destination, and connects a socket to the new local url,
 rather than the remote one that wouldn't actually work.
 
 ```{seealso}
 A short discussion of ssh tunnels: <https://www.revsys.com/writings/quicktips/ssh-tunnel.html>
 ```
```

### Comparing `pyzmq-26.0.0b1/docs/source/index.md` & `pyzmq-26.0.0b2/docs/source/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -41,18 +41,17 @@
 
 You can also check out the [examples in the pyzmq repo](https://github.com/zeromq/pyzmq/tree/HEAD/examples).
 
 ```{toctree}
 ---
 maxdepth: 2
 ---
-api/index.rst
-changelog.rst
-howto/index.rst
-notes/index.rst
+api/index
+changelog
+howto/index
 ```
 
 # Indices and tables
 
 - {ref}`genindex`
 - {ref}`modindex`
 - {ref}`search`
```

### Comparing `pyzmq-26.0.0b1/examples/asyncio/coroutines.py` & `pyzmq-26.0.0b2/examples/asyncio/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/asyncio/helloworld_pubsub_dealerrouter.py` & `pyzmq-26.0.0b2/examples/asyncio/helloworld_pubsub_dealerrouter.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/asyncio/router_router.py` & `pyzmq-26.0.0b2/examples/asyncio/router_router.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/asyncio/tornado_asyncio.py` & `pyzmq-26.0.0b2/examples/asyncio/tornado_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/cython/README.md` & `pyzmq-26.0.0b2/examples/cython/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/cython/cyzmq.pyx` & `pyzmq-26.0.0b2/examples/cython/cyzmq.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/cython/example.py` & `pyzmq-26.0.0b2/examples/cython/example.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/device/device.py` & `pyzmq-26.0.0b2/examples/device/device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/draft/client-server.py` & `pyzmq-26.0.0b2/examples/draft/client-server.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/draft/install.sh` & `pyzmq-26.0.0b2/examples/draft/install.sh`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/draft/radio-dish.py` & `pyzmq-26.0.0b2/examples/draft/radio-dish.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/eventloop/asyncweb.py` & `pyzmq-26.0.0b2/examples/eventloop/asyncweb.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/eventloop/coroutines.py` & `pyzmq-26.0.0b2/examples/eventloop/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/eventloop/echo.py` & `pyzmq-26.0.0b2/examples/eventloop/echo.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/gevent/poll.py` & `pyzmq-26.0.0b2/examples/gevent/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/gevent/reqrep.py` & `pyzmq-26.0.0b2/examples/gevent/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/gevent/simple.py` & `pyzmq-26.0.0b2/examples/gevent/simple.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/heartbeat/heart.py` & `pyzmq-26.0.0b2/examples/heartbeat/heart.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/heartbeat/heartbeater.py` & `pyzmq-26.0.0b2/examples/heartbeat/heartbeater.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/heartbeat/ping.py` & `pyzmq-26.0.0b2/examples/heartbeat/ping.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/heartbeat/pong.py` & `pyzmq-26.0.0b2/examples/heartbeat/pong.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/logger/zmqlogger.py` & `pyzmq-26.0.0b2/examples/logger/zmqlogger.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/mongodb/client.py` & `pyzmq-26.0.0b2/examples/mongodb/client.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/mongodb/controller.py` & `pyzmq-26.0.0b2/examples/mongodb/controller.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/monitoring/simple_monitor.py` & `pyzmq-26.0.0b2/examples/monitoring/simple_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/monitoring/zmq_monitor_class.py` & `pyzmq-26.0.0b2/examples/monitoring/zmq_monitor_class.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/poll/pair.py` & `pyzmq-26.0.0b2/examples/poll/pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/poll/pubsub.py` & `pyzmq-26.0.0b2/examples/poll/pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/poll/reqrep.py` & `pyzmq-26.0.0b2/examples/poll/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/pubsub/publisher.py` & `pyzmq-26.0.0b2/examples/pubsub/publisher.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/pubsub/subscriber.py` & `pyzmq-26.0.0b2/examples/pubsub/subscriber.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/pubsub/topics_pub.py` & `pyzmq-26.0.0b2/examples/pubsub/topics_pub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/pubsub/topics_sub.py` & `pyzmq-26.0.0b2/examples/pubsub/topics_sub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/security/asyncio-ironhouse.py` & `pyzmq-26.0.0b2/examples/security/asyncio-ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/security/generate_certificates.py` & `pyzmq-26.0.0b2/examples/security/generate_certificates.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/security/grasslands.py` & `pyzmq-26.0.0b2/examples/security/grasslands.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/security/ioloop-ironhouse.py` & `pyzmq-26.0.0b2/examples/security/ioloop-ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/security/ironhouse.py` & `pyzmq-26.0.0b2/examples/security/ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/security/stonehouse.py` & `pyzmq-26.0.0b2/examples/security/stonehouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/security/strawhouse.py` & `pyzmq-26.0.0b2/examples/security/strawhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/security/woodhouse.py` & `pyzmq-26.0.0b2/examples/security/woodhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/serialization/serialsocket.py` & `pyzmq-26.0.0b2/examples/serialization/serialsocket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/examples/win32-interrupt/display.py` & `pyzmq-26.0.0b2/examples/win32-interrupt/display.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/packaging/debian/control` & `pyzmq-26.0.0b2/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/packaging/debian/copyright` & `pyzmq-26.0.0b2/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/packaging/debian/pyzmq.dsc.obs` & `pyzmq-26.0.0b2/packaging/debian/pyzmq.dsc.obs`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/packaging/debian/rules` & `pyzmq-26.0.0b2/packaging/debian/rules`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/packaging/obs/_service` & `pyzmq-26.0.0b2/packaging/obs/_service`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/packaging/redhat/python-pyzmq.spec` & `pyzmq-26.0.0b2/packaging/redhat/python-pyzmq.spec`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/perf/Makefile` & `pyzmq-26.0.0b2/perf/Makefile`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/perf/collect.py` & `pyzmq-26.0.0b2/perf/collect.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/perf/perf.ipynb` & `pyzmq-26.0.0b2/perf/perf.ipynb`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/perf/perf.py` & `pyzmq-26.0.0b2/perf/perf.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/pyproject.toml` & `pyzmq-26.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # build-backend = "setuptools.build_meta"
 
 # Project metadata
 # ref: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "pyzmq"
-version = "26.0.0b1"
+version = "26.0.0b2"
 authors = [
   { name = "PyZMQ Contributors", email = "zeromq-dev@lists.zeromq.org" },
   { name = "Brian E. Granger" },
   { name = "Min Ragan-Kelley" },
 ]
 license = { file = "LICENSE.md" }
 requires-python = ">=3.7"
@@ -89,15 +89,15 @@
 skip = ["zmq/__init__.py"]
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/zeromq/pyzmq"
 
 [tool.tbump.version]
-current = "26.0.0b1"
+current = "26.0.0b2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc|)\d+)|.dev\d*|)
```

### Comparing `pyzmq-26.0.0b1/test-requirements.txt` & `pyzmq-26.0.0b2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/tools/collect_cmake.py` & `pyzmq-26.0.0b2/tools/collect_cmake.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/tools/find_vcredist.py` & `pyzmq-26.0.0b2/tools/find_vcredist.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/tools/install_libzmq.sh` & `pyzmq-26.0.0b2/tools/install_libzmq.sh`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/tools/run_with_env.cmd` & `pyzmq-26.0.0b2/tools/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/tools/test_sdist.py` & `pyzmq-26.0.0b2/tools/test_sdist.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/tools/test_wheel.py` & `pyzmq-26.0.0b2/tools/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/__init__.py` & `pyzmq-26.0.0b2/zmq/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Python bindings for 0MQ"""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
+from __future__ import annotations
+
 import os
 import sys
 from contextlib import contextmanager
 
 
 @contextmanager
 def _libs_on_path():
```

### Comparing `pyzmq-26.0.0b1/zmq/__init__.pyi` & `pyzmq-26.0.0b2/zmq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/_future.py` & `pyzmq-26.0.0b2/zmq/_future.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,29 @@
 """Future-returning APIs for coroutines."""
 
 # Copyright (c) PyZMQ Developers.
 # Distributed under the terms of the Modified BSD License.
+from __future__ import annotations
 
 import warnings
 from asyncio import Future
 from collections import deque
 from functools import partial
 from itertools import chain
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    Dict,
-    List,
-    NamedTuple,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    cast,
-    overload,
-)
+from typing import Any, Awaitable, Callable, NamedTuple, TypeVar, cast, overload
 
 import zmq as _zmq
 from zmq import EVENTS, POLLIN, POLLOUT
 from zmq._typing import Literal
 
 
 class _FutureEvent(NamedTuple):
     future: Future
     kind: str
-    kwargs: Dict
+    kwargs: dict
     msg: Any
     timer: Any
 
 
 # These are incomplete classes and need a Mixin for compatibility with an eventloop
 # defining the following attributes:
 #
@@ -46,15 +33,15 @@
 # _default_loop()
 
 
 class _Async:
     """Mixin for common async logic"""
 
     _current_loop: Any = None
-    _Future: Type[Future]
+    _Future: type[Future]
 
     def _get_loop(self) -> Any:
         """Get event loop
 
         Notice if event loop has changed,
         and register init_io_state on activation of a new event loop
         """
@@ -75,28 +62,28 @@
     def _init_io_state(self, loop=None) -> None:
         pass
 
 
 class _AsyncPoller(_Async, _zmq.Poller):
     """Poller that returns a Future on poll, instead of blocking."""
 
-    _socket_class: Type["_AsyncSocket"]
+    _socket_class: type[_AsyncSocket]
     _READ: int
     _WRITE: int
-    raw_sockets: List[Any]
+    raw_sockets: list[Any]
 
     def _watch_raw_socket(self, loop: Any, socket: Any, evt: int, f: Callable) -> None:
         """Schedule callback for a raw socket"""
         raise NotImplementedError()
 
     def _unwatch_raw_sockets(self, loop: Any, *sockets: Any) -> None:
         """Unschedule callback for a raw socket"""
         raise NotImplementedError()
 
-    def poll(self, timeout=-1) -> Awaitable[List[Tuple[Any, int]]]:  # type: ignore
+    def poll(self, timeout=-1) -> Awaitable[list[tuple[Any, int]]]:  # type: ignore
         """Return a Future for a poll event"""
         future = self._Future()
         if timeout == 0:
             try:
                 result = super().poll(0)
             except Exception as e:
                 future.set_exception(e)
@@ -106,25 +93,25 @@
 
         loop = self._get_loop()
 
         # register Future to be called as soon as any event is available on any socket
         watcher = self._Future()
 
         # watch raw sockets:
-        raw_sockets: List[Any] = []
+        raw_sockets: list[Any] = []
 
         def wake_raw(*args):
             if not watcher.done():
                 watcher.set_result(None)
 
         watcher.add_done_callback(
             lambda f: self._unwatch_raw_sockets(loop, *raw_sockets)
         )
 
-        wrapped_sockets: List[_AsyncSocket] = []
+        wrapped_sockets: list[_AsyncSocket] = []
 
         def _clear_wrapper_io(f):
             for s in wrapped_sockets:
                 s._clear_io_state()
 
         for socket, mask in self.sockets:
             if isinstance(socket, _zmq.Socket):
@@ -206,24 +193,24 @@
 
 class _AsyncSocket(_Async, _zmq.Socket[Future]):
     # Warning : these class variables are only here to allow to call super().__setattr__.
     # They be overridden at instance initialization and not shared in the whole class
     _recv_futures = None
     _send_futures = None
     _state = 0
-    _shadow_sock: "_zmq.Socket"
+    _shadow_sock: _zmq.Socket
     _poller_class = _AsyncPoller
     _fd = None
 
     def __init__(
         self,
         context=None,
         socket_type=-1,
         io_loop=None,
-        _from_socket: Optional["_zmq.Socket"] = None,
+        _from_socket: _zmq.Socket | None = None,
         **kwargs,
     ) -> None:
         if isinstance(context, _zmq.Socket):
             context, _from_socket = (None, context)
         if _from_socket is not None:
             super().__init__(shadow=_from_socket.underlying)  # type: ignore
             self._shadow_sock = _from_socket
@@ -240,21 +227,21 @@
             )
         self._recv_futures = deque()
         self._send_futures = deque()
         self._state = 0
         self._fd = self._shadow_sock.FD
 
     @classmethod
-    def from_socket(cls: Type[T], socket: "_zmq.Socket", io_loop: Any = None) -> T:
+    def from_socket(cls: type[T], socket: _zmq.Socket, io_loop: Any = None) -> T:
         """Create an async socket from an existing Socket"""
         return cls(_from_socket=socket, io_loop=io_loop)
 
-    def close(self, linger: Optional[int] = None) -> None:
+    def close(self, linger: int | None = None) -> None:
         if not self.closed and self._fd is not None:
-            event_list: List[_FutureEvent] = list(
+            event_list: list[_FutureEvent] = list(
                 chain(self._recv_futures or [], self._send_futures or [])
             )
             for event in event_list:
                 if not event.future.done():
                     try:
                         event.future.cancel()
                     except RuntimeError:
@@ -272,57 +259,57 @@
         return result
 
     get.__doc__ = _zmq.Socket.get.__doc__
 
     @overload  # type: ignore
     def recv_multipart(
         self, flags: int = 0, *, track: bool = False
-    ) -> Awaitable[List[bytes]]: ...
+    ) -> Awaitable[list[bytes]]: ...
 
     @overload
     def recv_multipart(
         self, flags: int = 0, *, copy: Literal[True], track: bool = False
-    ) -> Awaitable[List[bytes]]: ...
+    ) -> Awaitable[list[bytes]]: ...
 
     @overload
     def recv_multipart(
         self, flags: int = 0, *, copy: Literal[False], track: bool = False
-    ) -> Awaitable[List[_zmq.Frame]]:  # type: ignore
+    ) -> Awaitable[list[_zmq.Frame]]:  # type: ignore
         ...
 
     @overload
     def recv_multipart(
         self, flags: int = 0, copy: bool = True, track: bool = False
-    ) -> Awaitable[Union[List[bytes], List[_zmq.Frame]]]: ...
+    ) -> Awaitable[list[bytes] | list[_zmq.Frame]]: ...
 
     def recv_multipart(
         self, flags: int = 0, copy: bool = True, track: bool = False
-    ) -> Awaitable[Union[List[bytes], List[_zmq.Frame]]]:
+    ) -> Awaitable[list[bytes] | list[_zmq.Frame]]:
         """Receive a complete multipart zmq message.
 
         Returns a Future whose result will be a multipart message.
         """
         return self._add_recv_event(
             'recv_multipart', dict(flags=flags, copy=copy, track=track)
         )
 
     def recv(  # type: ignore
         self, flags: int = 0, copy: bool = True, track: bool = False
-    ) -> Awaitable[Union[bytes, _zmq.Frame]]:
+    ) -> Awaitable[bytes | _zmq.Frame]:
         """Receive a single zmq frame.
 
         Returns a Future, whose result will be the received frame.
 
         Recommend using recv_multipart instead.
         """
         return self._add_recv_event('recv', dict(flags=flags, copy=copy, track=track))
 
     def send_multipart(  # type: ignore
         self, msg_parts: Any, flags: int = 0, copy: bool = True, track=False, **kwargs
-    ) -> Awaitable[Optional[_zmq.MessageTracker]]:
+    ) -> Awaitable[_zmq.MessageTracker | None]:
         """Send a complete multipart zmq message.
 
         Returns a Future that resolves when sending is complete.
         """
         kwargs['flags'] = flags
         kwargs['copy'] = copy
         kwargs['track'] = track
@@ -331,15 +318,15 @@
     def send(  # type: ignore
         self,
         data: Any,
         flags: int = 0,
         copy: bool = True,
         track: bool = False,
         **kwargs: Any,
-    ) -> Awaitable[Optional[_zmq.MessageTracker]]:
+    ) -> Awaitable[_zmq.MessageTracker | None]:
         """Send a single zmq frame.
 
         Returns a Future that resolves when sending is complete.
 
         Recommend using send_multipart instead.
         """
         kwargs['flags'] = flags
```

### Comparing `pyzmq-26.0.0b1/zmq/asyncio.py` & `pyzmq-26.0.0b2/zmq/asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """AsyncIO support for zmq
 
 Requires asyncio and Python 3.
 """
 
 # Copyright (c) PyZMQ Developers.
 # Distributed under the terms of the Modified BSD License.
+from __future__ import annotations
 
 import asyncio
 import selectors
 import sys
 import warnings
 from asyncio import Future, SelectorEventLoop
 from weakref import WeakKeyDictionary
```

### Comparing `pyzmq-26.0.0b1/zmq/auth/asyncio.py` & `pyzmq-26.0.0b2/zmq/auth/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/auth/base.py` & `pyzmq-26.0.0b2/zmq/auth/base.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/auth/certs.py` & `pyzmq-26.0.0b2/zmq/auth/certs.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/auth/ioloop.py` & `pyzmq-26.0.0b2/zmq/auth/ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/auth/thread.py` & `pyzmq-26.0.0b2/zmq/auth/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     poller: Optional[zmq.asyncio.Poller] = None
 
     def __init__(
         self,
         authenticator: Authenticator,
         pipe: zmq.Socket,
     ) -> None:
-        super().__init__()
+        super().__init__(daemon=True)
         self.authenticator = authenticator
         self.log = authenticator.log
         self.pipe = pipe
 
         self.started = Event()
 
     def run(self) -> None:
```

### Comparing `pyzmq-26.0.0b1/zmq/backend/__init__.py` & `pyzmq-26.0.0b2/zmq/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/__init__.pyi` & `pyzmq-26.0.0b2/zmq/backend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cffi/__init__.py` & `pyzmq-26.0.0b2/zmq/backend/cffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cffi/_cdefs.h` & `pyzmq-26.0.0b2/zmq/backend/cffi/_cdefs.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cffi/_cffi_src.c` & `pyzmq-26.0.0b2/zmq/backend/cffi/_cffi_src.c`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cffi/_poll.py` & `pyzmq-26.0.0b2/zmq/backend/cffi/_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cffi/context.py` & `pyzmq-26.0.0b2/zmq/backend/cffi/context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cffi/devices.py` & `pyzmq-26.0.0b2/zmq/backend/cffi/devices.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cffi/message.py` & `pyzmq-26.0.0b2/zmq/backend/cffi/message.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cffi/socket.py` & `pyzmq-26.0.0b2/zmq/backend/cffi/socket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cffi/utils.py` & `pyzmq-26.0.0b2/zmq/backend/cffi/utils.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cython/_zmq.pxd` & `pyzmq-26.0.0b2/zmq/backend/cython/_zmq.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cython/_zmq.py` & `pyzmq-26.0.0b2/zmq/backend/cython/_zmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Cython backend for pyzmq"""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
+from __future__ import annotations
+
 try:
     import cython
 
     if not cython.compiled:
         raise ImportError()
 except ImportError:
     raise ImportError("zmq Cython backend has not been compiled") from None
@@ -330,15 +332,15 @@
         with nogil:
             rc: C.int = zmq_msg_close(address(self.zmq_msg))
         _check_rc(rc)
 
     def __copy__(self):
         return self.fast_copy()
 
-    def fast_copy(self) -> "Frame":
+    def fast_copy(self) -> Frame:
         new_msg: Frame = Frame()
         # This does not copy the contents, but just increases the ref-count
         # of the zmq_msg by one.
         zmq_msg_copy(address(new_msg.zmq_msg), address(self.zmq_msg))
         # Copy the ref to data so the copy won't create a copy when str is
         # called.
         if self._data is not None:
@@ -1011,15 +1013,16 @@
 
         Parameters
         ----------
         addr : str
             The inproc url used for monitoring. Passing None as
             the addr will cause an existing socket monitor to be
             deregistered.
-        events : int [default: zmq.EVENT_ALL]
+        events : int
+            default: zmq.EVENT_ALL
             The zmq event bitmask for which events will be sent to the monitor.
         """
         _check_version((3, 2), "monitor")
 
         if isinstance(addr, str):
             # cast str to utf8 bytes
             addr = addr.encode("utf-8")
@@ -1097,16 +1100,16 @@
             finished with it? (ignored if copy=True)
 
         Returns
         -------
         None : if `copy` or not track
             None if message was sent, raises an exception otherwise.
         MessageTracker : if track and not copy
-            a MessageTracker object, whose `pending` property will
-            be True until the send is completed.
+            a MessageTracker object, whose `done` property will
+            be False until the send is completed.
 
         Raises
         ------
         TypeError
             If a unicode object is passed
         ValueError
             If `track=True`, but an untracked Frame is passed.
@@ -1403,26 +1406,28 @@
     ccap: bytes
     if isinstance(capability, str):
         capability = capability.encode('utf8')
     ccap = capability
     return bool(zmq_has(ccap))
 
 
-def curve_keypair():
+def curve_keypair() -> tuple[bytes, bytes]:
     """generate a Z85 key pair for use with zmq.CURVE security
 
     Requires libzmq (≥ 4.0) to have been built with CURVE support.
 
     .. versionadded:: libzmq-4.0
     .. versionadded:: 14.0
 
     Returns
     -------
-    (public, secret) : two bytestrings
-        The public and private key pair as 40 byte z85-encoded bytestrings.
+    public: bytes
+        The public key as 40 byte z85-encoded bytestring.
+    private: bytes
+        The private key as 40 byte z85-encoded bytestring.
     """
     rc: C.int
     public_key = declare(char[64])
     secret_key = declare(char[64])
     _check_version((4, 0), "curve_keypair")
     # see huge comment in libzmq/src/random.cpp
     # about threadsafety of random initialization
@@ -1440,15 +1445,15 @@
     Parameters
     ----------
     private
         The private key as a 40 byte z85-encoded bytestring
 
     Returns
     -------
-    bytestring
+    bytes
         The public key as a 40 byte z85-encoded bytestring
     """
     if isinstance(secret_key, str):
         secret_key = secret_key.encode('utf8')
     if not len(secret_key) == 40:
         raise ValueError('secret key must be a 40 byte z85 encoded string')
 
@@ -1582,15 +1587,16 @@
     Start a zeromq device.
 
     .. deprecated:: libzmq-3.2
         Use zmq.proxy
 
     Parameters
     ----------
-    device_type : (QUEUE, FORWARDER, STREAMER)
+    device_type : int
+        one of: QUEUE, FORWARDER, STREAMER
         The type of device to start.
     frontend : Socket
         The Socket instance for the incoming traffic.
     backend : Socket
         The Socket instance for the outbound traffic.
     """
     if ZMQ_VERSION_MAJOR >= 3:
@@ -1861,21 +1867,21 @@
 
     - monitored_queue supports both in and out being ROUTER sockets
       (via swapping IDENTITY prefixes).
     - monitor messages are prefixed, making in and out messages distinguishable.
 
     Parameters
     ----------
-    in_socket : Socket
+    in_socket : zmq.Socket
         One of the sockets to the Queue. Its messages will be prefixed with
         'in'.
-    out_socket : Socket
+    out_socket : zmq.Socket
         One of the sockets to the Queue. Its messages will be prefixed with
         'out'. The only difference between in/out socket is this prefix.
-    mon_socket : Socket
+    mon_socket : zmq.Socket
         This socket sends out every message received by each of the others
         with an in/out prefix specifying which one it was.
     in_prefix : str
         Prefix added to broadcast messages from in_socket.
     out_prefix : str
         Prefix added to broadcast messages from out_socket.
     """
```

### Comparing `pyzmq-26.0.0b1/zmq/backend/cython/constant_enums.pxi` & `pyzmq-26.0.0b2/zmq/backend/cython/constant_enums.pxi`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/cython/libzmq.pxd` & `pyzmq-26.0.0b2/zmq/backend/cython/libzmq.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/backend/select.py` & `pyzmq-26.0.0b2/zmq/backend/select.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/constants.py` & `pyzmq-26.0.0b2/zmq/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """zmq constants as enums"""
 
+from __future__ import annotations
+
 import errno
 import sys
 from enum import Enum, IntEnum, IntFlag
-from typing import List
 
 _HAUSNUMERO = 156384712
 
 
 class Errno(IntEnum):
     """libzmq error codes
 
@@ -705,15 +706,15 @@
 DISH: int = SocketType.DISH
 GATHER: int = SocketType.GATHER
 SCATTER: int = SocketType.SCATTER
 DGRAM: int = SocketType.DGRAM
 PEER: int = SocketType.PEER
 CHANNEL: int = SocketType.CHANNEL
 
-__all__: List[str] = [
+__all__: list[str] = [
     "ContextOption",
     "IO_THREADS",
     "MAX_SOCKETS",
     "SOCKET_LIMIT",
     "THREAD_PRIORITY",
     "THREAD_SCHED_POLICY",
     "MAX_MSGSZ",
```

### Comparing `pyzmq-26.0.0b1/zmq/decorators.py` & `pyzmq-26.0.0b2/zmq/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     
     @context()
     @socket(zmq.PUSH)
     def work(ctx, push):
         ...
 """
 
+from __future__ import annotations
+
 # Copyright (c) PyZMQ Developers.
 # Distributed under the terms of the Modified BSD License.
 
 __all__ = (
     'context',
     'socket',
 )
```

### Comparing `pyzmq-26.0.0b1/zmq/devices/__init__.py` & `pyzmq-26.0.0b2/zmq/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/devices/basedevice.py` & `pyzmq-26.0.0b2/zmq/devices/basedevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 
     Attributes
     ----------
     daemon : bool
         sets whether the thread should be run as a daemon
         Default is true, because if it is false, the thread will not
         exit unless it is killed
-    context_factory : callable (class attribute)
+    context_factory : callable
+        This is a class attribute.
         Function for creating the Context. This will be Context.instance
         in ThreadDevices, and Context in ProcessDevices.  The only reason
         it is not instance() in ProcessDevices is that there may be a stale
         Context instance already initialized, and the forked environment
         should *never* try to use it.
     """
```

### Comparing `pyzmq-26.0.0b1/zmq/devices/monitoredqueue.py` & `pyzmq-26.0.0b2/zmq/devices/monitoredqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/devices/monitoredqueuedevice.py` & `pyzmq-26.0.0b2/zmq/devices/monitoredqueuedevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/devices/proxydevice.py` & `pyzmq-26.0.0b2/zmq/devices/proxydevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/devices/proxysteerabledevice.py` & `pyzmq-26.0.0b2/zmq/devices/proxysteerabledevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/error.py` & `pyzmq-26.0.0b2/zmq/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """0MQ Error classes and functions."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
+from __future__ import annotations
 
 from errno import EINTR
-from typing import Optional, Tuple, Union
 
 
 class ZMQBaseError(Exception):
     """Base exception class for 0MQ errors in Python."""
 
 
 class ZMQError(ZMQBaseError):
     """Wrap an errno style error.
 
     Parameters
     ----------
     errno : int
         The ZMQ errno or None.  If None, then ``zmq_errno()`` is called and
         used.
-    msg : string
+    msg : str
         Description of the error or None.
     """
 
-    errno: Optional[int] = None
+    errno: int | None = None
 
-    def __init__(self, errno: Optional[int] = None, msg: Optional[str] = None):
+    def __init__(self, errno: int | None = None, msg: str | None = None):
         """Wrap an errno style error.
 
         Parameters
         ----------
         errno : int
             The ZMQ errno or None.  If None, then ``zmq_errno()`` is called and
             used.
@@ -179,15 +179,15 @@
             self.msg,
             self.min_version,
             self.version,
         )
 
 
 def _check_version(
-    min_version_info: Union[Tuple[int], Tuple[int, int], Tuple[int, int, int]],
+    min_version_info: tuple[int] | tuple[int, int] | tuple[int, int, int],
     msg: str = "Feature",
 ):
     """Check for libzmq
 
     raises ZMQVersionError if current zmq version is not at least min_version
 
     min_version_info is a tuple of integers, and will be compared against zmq.zmq_version_info().
```

### Comparing `pyzmq-26.0.0b1/zmq/eventloop/_deprecated.py` & `pyzmq-26.0.0b2/zmq/eventloop/_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/eventloop/future.py` & `pyzmq-26.0.0b2/zmq/eventloop/future.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
     :mod:`zmq.asyncio`
 
 """
 
 # Copyright (c) PyZMQ Developers.
 # Distributed under the terms of the Modified BSD License.
+from __future__ import annotations
 
 import asyncio
 import warnings
-from typing import Any, Type
+from typing import Any
 
 from tornado.concurrent import Future
 from tornado.ioloop import IOLoop
 
 import zmq as _zmq
 from zmq._future import _AsyncPoller, _AsyncSocket
 
@@ -46,15 +47,15 @@
         self.loop.remove_timeout(self.timeout)
 
 
 # mixin for tornado/asyncio compatibility
 
 
 class _AsyncTornado:
-    _Future: Type[asyncio.Future] = _TornadoFuture
+    _Future: type[asyncio.Future] = _TornadoFuture
     _READ = IOLoop.READ
     _WRITE = IOLoop.WRITE
 
     def _default_loop(self):
         return IOLoop.current()
 
     def _call_later(self, delay, callback):
@@ -87,15 +88,15 @@
 
     io_loop = None
 
     @staticmethod
     def _socket_class(self, socket_type):
         return Socket(self, socket_type)
 
-    def __init__(self: "Context", *args: Any, **kwargs: Any) -> None:
+    def __init__(self: Context, *args: Any, **kwargs: Any) -> None:
         io_loop = kwargs.pop('io_loop', None)
         if io_loop is not None:
             warnings.warn(
                 f"{self.__class__.__name__}(io_loop) argument is deprecated in pyzmq 22.2."
                 " The currently active loop will always be used.",
                 DeprecationWarning,
                 stacklevel=2,
```

### Comparing `pyzmq-26.0.0b1/zmq/eventloop/ioloop.py` & `pyzmq-26.0.0b2/zmq/eventloop/ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/eventloop/zmqstream.py` & `pyzmq-26.0.0b2/zmq/eventloop/zmqstream.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,38 +8,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
+from __future__ import annotations
 
 """A utility class for event-based messaging on a zmq socket using tornado.
 
 .. seealso::
 
     - :mod:`zmq.asyncio`
     - :mod:`zmq.eventloop.future`
 """
 
 import asyncio
 import pickle
 import warnings
 from queue import Queue
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    List,
-    Optional,
-    Sequence,
-    Union,
-    cast,
-    overload,
-)
+from typing import Any, Awaitable, Callable, Sequence, cast, overload
 
 from tornado.ioloop import IOLoop
 from tornado.log import gen_log
 
 import zmq
 import zmq._future
 from zmq import POLLIN, POLLOUT
@@ -101,23 +92,23 @@
         (the list of message frames).
     """
 
     socket: zmq.Socket
     io_loop: IOLoop
     poller: zmq.Poller
     _send_queue: Queue
-    _recv_callback: Optional[Callable]
-    _send_callback: Optional[Callable]
-    _close_callback: Optional[Callable]
+    _recv_callback: Callable | None
+    _send_callback: Callable | None
+    _close_callback: Callable | None
     _state: int = 0
     _flushed: bool = False
     _recv_copy: bool = False
     _fd: int
 
-    def __init__(self, socket: "zmq.Socket", io_loop: Optional[IOLoop] = None):
+    def __init__(self, socket: zmq.Socket, io_loop: IOLoop | None = None):
         if isinstance(socket, zmq._future._AsyncSocket):
             warnings.warn(
                 f"""ZMQStream only supports the base zmq.Socket class.
 
                 Use zmq.Socket(shadow=other_socket)
                 or `ctx.socket(zmq.{socket._type_name}, socket_class=zmq.Socket)`
                 to create a base zmq.Socket object,
@@ -173,47 +164,41 @@
     def on_err(self, callback: Callable):
         """DEPRECATED, does nothing"""
         gen_log.warn("on_err does nothing, and will be removed")
 
     @overload
     def on_recv(
         self,
-        callback: Callable[[List[bytes]], Any],
+        callback: Callable[[list[bytes]], Any],
     ) -> None: ...
 
     @overload
     def on_recv(
         self,
-        callback: Callable[[List[bytes]], Any],
+        callback: Callable[[list[bytes]], Any],
         copy: Literal[True],
     ) -> None: ...
 
     @overload
     def on_recv(
         self,
-        callback: Callable[[List[zmq.Frame]], Any],
+        callback: Callable[[list[zmq.Frame]], Any],
         copy: Literal[False],
     ) -> None: ...
 
     @overload
     def on_recv(
         self,
-        callback: Union[
-            Callable[[List[zmq.Frame]], Any],
-            Callable[[List[bytes]], Any],
-        ],
+        callback: Callable[[list[zmq.Frame]], Any] | Callable[[list[bytes]], Any],
         copy: bool = ...,
     ): ...
 
     def on_recv(
         self,
-        callback: Union[
-            Callable[[List[zmq.Frame]], Any],
-            Callable[[List[bytes]], Any],
-        ],
+        callback: Callable[[list[zmq.Frame]], Any] | Callable[[list[bytes]], Any],
         copy: bool = True,
     ) -> None:
         """Register a callback for when a message is ready to recv.
 
         There can be only one callback registered at a time, so each
         call to `on_recv` replaces previously registered callbacks.
 
@@ -245,47 +230,47 @@
             self._drop_io_state(zmq.POLLIN)
         else:
             self._add_io_state(zmq.POLLIN)
 
     @overload
     def on_recv_stream(
         self,
-        callback: Callable[["ZMQStream", List[bytes]], Any],
+        callback: Callable[[ZMQStream, list[bytes]], Any],
     ) -> None: ...
 
     @overload
     def on_recv_stream(
         self,
-        callback: Callable[["ZMQStream", List[bytes]], Any],
+        callback: Callable[[ZMQStream, list[bytes]], Any],
         copy: Literal[True],
     ) -> None: ...
 
     @overload
     def on_recv_stream(
         self,
-        callback: Callable[["ZMQStream", List[zmq.Frame]], Any],
+        callback: Callable[[ZMQStream, list[zmq.Frame]], Any],
         copy: Literal[False],
     ) -> None: ...
 
     @overload
     def on_recv_stream(
         self,
-        callback: Union[
-            Callable[["ZMQStream", List[zmq.Frame]], Any],
-            Callable[["ZMQStream", List[bytes]], Any],
-        ],
+        callback: (
+            Callable[[ZMQStream, list[zmq.Frame]], Any]
+            | Callable[[ZMQStream, list[bytes]], Any]
+        ),
         copy: bool = ...,
     ): ...
 
     def on_recv_stream(
         self,
-        callback: Union[
-            Callable[["ZMQStream", List[zmq.Frame]], Any],
-            Callable[["ZMQStream", List[bytes]], Any],
-        ],
+        callback: (
+            Callable[[ZMQStream, list[zmq.Frame]], Any]
+            | Callable[[ZMQStream, list[bytes]], Any]
+        ),
         copy: bool = True,
     ):
         """Same as on_recv, but callback will get this stream as first argument
 
         callback must take exactly two arguments, as it will be called as::
 
             callback(stream, msg)
@@ -298,15 +283,15 @@
 
             def stream_callback(msg):
                 return callback(self, msg)
 
             self.on_recv(stream_callback, copy=copy)
 
     def on_send(
-        self, callback: Callable[[Sequence[Any], Optional[zmq.MessageTracker]], Any]
+        self, callback: Callable[[Sequence[Any], zmq.MessageTracker | None], Any]
     ):
         """Register a callback to be called on each send
 
         There will be two arguments::
 
             callback(msg, status)
 
@@ -341,17 +326,15 @@
 
         self._check_closed()
         assert callback is None or callable(callback)
         self._send_callback = callback
 
     def on_send_stream(
         self,
-        callback: Callable[
-            ["ZMQStream", Sequence[Any], Optional[zmq.MessageTracker]], Any
-        ],
+        callback: Callable[[ZMQStream, Sequence[Any], zmq.MessageTracker | None], Any],
     ):
         """Same as on_send, but callback will get this stream as first argument
 
         Callback will be passed three arguments::
 
             callback(stream, msg, status)
 
@@ -372,15 +355,15 @@
 
     def send_multipart(
         self,
         msg: Sequence[Any],
         flags: int = 0,
         copy: bool = True,
         track: bool = False,
-        callback: Optional[Callable] = None,
+        callback: Callable | None = None,
         **kwargs: Any,
     ) -> None:
         """Send a multipart message, optionally also register a new callback for sends.
         See zmq.socket.send_multipart for details.
         """
         kwargs.update(dict(flags=flags, copy=copy, track=track))
         self._send_queue.put((msg, kwargs))
@@ -393,15 +376,15 @@
         self._add_io_state(zmq.POLLOUT)
 
     def send_string(
         self,
         u: str,
         flags: int = 0,
         encoding: str = 'utf-8',
-        callback: Optional[Callable] = None,
+        callback: Callable | None = None,
         **kwargs: Any,
     ):
         """Send a unicode message with an encoding.
         See zmq.socket.send_unicode for details.
         """
         if not isinstance(u, str):
             raise TypeError("unicode/str objects only")
@@ -409,43 +392,43 @@
 
     send_unicode = send_string
 
     def send_json(
         self,
         obj: Any,
         flags: int = 0,
-        callback: Optional[Callable] = None,
+        callback: Callable | None = None,
         **kwargs: Any,
     ):
         """Send json-serialized version of an object.
         See zmq.socket.send_json for details.
         """
         msg = jsonapi.dumps(obj)
         return self.send(msg, flags=flags, callback=callback, **kwargs)
 
     def send_pyobj(
         self,
         obj: Any,
         flags: int = 0,
         protocol: int = -1,
-        callback: Optional[Callable] = None,
+        callback: Callable | None = None,
         **kwargs: Any,
     ):
         """Send a Python object as a message using pickle to serialize.
 
         See zmq.socket.send_json for details.
         """
         msg = pickle.dumps(obj, protocol)
         return self.send(msg, flags, callback=callback, **kwargs)
 
     def _finish_flush(self):
         """callback for unsetting _flushed flag."""
         self._flushed = False
 
-    def flush(self, flag: int = zmq.POLLIN | zmq.POLLOUT, limit: Optional[int] = None):
+    def flush(self, flag: int = zmq.POLLIN | zmq.POLLOUT, limit: int | None = None):
         """Flush pending messages.
 
         This method safely handles all pending incoming and/or outgoing messages,
         bypassing the inner loop, passing them to the registered callbacks.
 
         A limit can be specified, to prevent blocking under high load.
 
@@ -455,26 +438,28 @@
 
         Note that if ``flag|POLLIN != 0``, recv events will be flushed even if no callback
         is registered, unlike normal IOLoop operation. This allows flush to be
         used to remove *and ignore* incoming messages.
 
         Parameters
         ----------
-        flag : int, default=POLLIN|POLLOUT
-                0MQ poll flags.
-                If flag|POLLIN,  recv events will be flushed.
-                If flag|POLLOUT, send events will be flushed.
-                Both flags can be set at once, which is the default.
+        flag : int
+            default=POLLIN|POLLOUT
+            0MQ poll flags.
+            If flag|POLLIN,  recv events will be flushed.
+            If flag|POLLOUT, send events will be flushed.
+            Both flags can be set at once, which is the default.
         limit : None or int, optional
-                The maximum number of messages to send or receive.
-                Both send and recv count against this limit.
+            The maximum number of messages to send or receive.
+            Both send and recv count against this limit.
 
         Returns
         -------
-        int : count of events handled (both send and recv)
+        int :
+            count of events handled (both send and recv)
         """
         self._check_closed()
         # unset self._flushed, so callbacks will execute, in case flush has
         # already been called this iteration
         already_flushed = self._flushed
         self._flushed = False
         # initialize counters
@@ -521,19 +506,19 @@
         elif already_flushed:
             self._flushed = True
 
         # update ioloop poll state, which may have changed
         self._rebuild_io_state()
         return count
 
-    def set_close_callback(self, callback: Optional[Callable]):
+    def set_close_callback(self, callback: Callable | None):
         """Call the given callback when the stream is closed."""
         self._close_callback = callback
 
-    def close(self, linger: Optional[int] = None) -> None:
+    def close(self, linger: int | None = None) -> None:
         """Close this stream."""
         if self.socket is not None:
             if self.socket.closed:
                 # fallback on raw fd for closed sockets
                 # hopefully this happened promptly after close,
                 # otherwise somebody else may have the FD
                 warnings.warn(
```

### Comparing `pyzmq-26.0.0b1/zmq/green/__init__.py` & `pyzmq-26.0.0b2/zmq/green/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,24 +23,25 @@
 Any calls that would have blocked the current thread will now only block the
 current green thread.
 
 This compatibility is accomplished by ensuring the nonblocking flag is set
 before any blocking operation and the ØMQ file descriptor is polled internally
 to trigger needed events.
 """
+from __future__ import annotations
 
 from typing import List
 
 import zmq as _zmq
 from zmq import *
 from zmq.green.core import _Context, _Socket
 from zmq.green.poll import _Poller
 
 Context = _Context  # type: ignore
 Socket = _Socket  # type: ignore
 Poller = _Poller  # type: ignore
 
 from zmq.green.device import device  # type: ignore
 
-__all__: List[str] = []
+__all__: list[str] = []
 # adding `__all__` to __init__.pyi gets mypy all confused
 __all__.extend(_zmq.__all__)  # type: ignore
```

### Comparing `pyzmq-26.0.0b1/zmq/green/core.py` & `pyzmq-26.0.0b2/zmq/green/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,33 +6,32 @@
 #
 #  Distributed under the terms of the New BSD License.  The full license is in
 #  the file LICENSE.BSD, distributed as part of this software.
 # -----------------------------------------------------------------------------
 
 """This module wraps the :class:`Socket` and :class:`Context` found in :mod:`pyzmq <zmq>` to be non blocking
 """
-
+from __future__ import annotations
 
 import sys
 import time
 import warnings
-from typing import Tuple
 
 import gevent
 from gevent.event import AsyncResult
 from gevent.hub import get_hub
 
 import zmq
 from zmq import Context as _original_Context
 from zmq import Socket as _original_Socket
 
 from .poll import _Poller
 
 if hasattr(zmq, 'RCVTIMEO'):
-    TIMEOS: Tuple = (zmq.RCVTIMEO, zmq.SNDTIMEO)
+    TIMEOS: tuple = (zmq.RCVTIMEO, zmq.SNDTIMEO)
 else:
     TIMEOS = ()
 
 
 def _stop(evt):
     """simple wrapper for stopping an Event, allowing for method rename in gevent 1.0"""
     try:
```

### Comparing `pyzmq-26.0.0b1/zmq/green/device.py` & `pyzmq-26.0.0b2/zmq/green/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
+from __future__ import annotations
 
 import zmq
 from zmq.green import Poller
 
 
 def device(device_type, isocket, osocket):
     """Start a zeromq device (gevent-compatible).
```

### Comparing `pyzmq-26.0.0b1/zmq/green/poll.py` & `pyzmq-26.0.0b2/zmq/green/poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import gevent
 from gevent import select
 
 import zmq
 from zmq import Poller as _original_Poller
```

### Comparing `pyzmq-26.0.0b1/zmq/log/__main__.py` & `pyzmq-26.0.0b2/zmq/log/__main__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/log/handlers.py` & `pyzmq-26.0.0b2/zmq/log/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,22 +38,24 @@
 PUB socket.
 
 Code adapted from StarCluster:
 
     https://github.com/jtriley/StarCluster/blob/StarCluster-0.91/starcluster/logger.py
 """
 
+from __future__ import annotations
+
 import logging
 from copy import copy
 
+import zmq
+
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
-from typing import Optional, Union
 
-import zmq
 
 TOPIC_DELIM = "::"  # delimiter for splitting topics on the receiving end.
 
 
 class PUBHandler(logging.Handler):
     """A basic logging handler that emits log messages through a PUB socket.
 
@@ -78,16 +80,16 @@
     """
 
     ctx: zmq.Context
     socket: zmq.Socket
 
     def __init__(
         self,
-        interface_or_socket: Union[str, zmq.Socket],
-        context: Optional[zmq.Context] = None,
+        interface_or_socket: str | zmq.Socket,
+        context: zmq.Context | None = None,
         root_topic: str = '',
     ) -> None:
         logging.Handler.__init__(self)
         self.root_topic = root_topic
         self.formatters = {
             logging.DEBUG: logging.Formatter(
                 "%(levelname)s %(filename)s:%(lineno)d - %(message)s\n"
```

### Comparing `pyzmq-26.0.0b1/zmq/ssh/forward.py` & `pyzmq-26.0.0b2/zmq/ssh/forward.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/ssh/tunnel.py` & `pyzmq-26.0.0b2/zmq/ssh/tunnel.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         The ssh server to connect to. The full ssh server string will be parsed.
         user@server:port
     remoteip : str [Default: 127.0.0.1]
         The remote ip, specifying the destination of the tunnel.
         Default is localhost, which means that the tunnel would redirect
         localhost:lport on this machine to localhost:rport on the *server*.
 
-    keyfile : str; path to public key file
+    keyfile : str; path to private key file
         This specifies a key to be used in ssh login, default None.
         Regular default ssh keys will be used without specifying this argument.
     password : str;
         Your ssh password to the ssh server. Note that if this is left None,
         you will be prompted for it if passwordless key based login is unavailable.
     timeout : int [default: 60]
         The time (in seconds) after which no activity will result in the tunnel
@@ -356,15 +356,15 @@
         The ssh server to connect to. The full ssh server string will be parsed.
         user@server:port
     remoteip : str [Default: 127.0.0.1]
         The remote ip, specifying the destination of the tunnel.
         Default is localhost, which means that the tunnel would redirect
         localhost:lport on this machine to localhost:rport on the *server*.
 
-    keyfile : str; path to public key file
+    keyfile : str; path to private key file
         This specifies a key to be used in ssh login, default None.
         Regular default ssh keys will be used without specifying this argument.
     password : str;
         Your ssh password to the ssh server. Note that if this is left None,
         you will be prompted for it if passwordless key based login is unavailable.
     timeout : int [default: 60]
         The time (in seconds) after which no activity will result in the tunnel
```

### Comparing `pyzmq-26.0.0b1/zmq/sugar/__init__.py` & `pyzmq-26.0.0b2/zmq/sugar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/sugar/attrsettr.py` & `pyzmq-26.0.0b2/zmq/sugar/attrsettr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Mixin for mapping set/getattr to self.set/get"""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
+from __future__ import annotations
 
 import errno
 from typing import TypeVar, Union
 
 from .. import constants
 
 T = TypeVar("T")
```

### Comparing `pyzmq-26.0.0b1/zmq/sugar/context.py` & `pyzmq-26.0.0b2/zmq/sugar/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 """Python bindings for 0MQ."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
+from __future__ import annotations
+
 import atexit
 import os
 from threading import Lock
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Generic,
-    List,
-    Optional,
-    Type,
-    TypeVar,
-    Union,
-    overload,
-)
+from typing import Any, Callable, Generic, TypeVar, overload
 from warnings import warn
 from weakref import WeakSet
 
+import zmq
 from zmq.backend import Context as ContextBase
 from zmq.constants import ContextOption, Errno, SocketOption
 from zmq.error import ZMQError
 from zmq.utils.interop import cast_int_addr
 
 from .attrsettr import AttributeSetter, OptValT
 from .socket import Socket
@@ -36,19 +28,19 @@
 def _notice_atexit() -> None:
     global _exiting
     _exiting = True
 
 
 atexit.register(_notice_atexit)
 
-T = TypeVar('T', bound='Context')
-ST = TypeVar('ST', bound='Socket', covariant=True)
+_ContextType = TypeVar('_ContextType', bound='Context')
+_SocketType = TypeVar('_SocketType', bound='Socket', covariant=True)
 
 
-class Context(ContextBase, AttributeSetter, Generic[ST]):
+class Context(ContextBase, AttributeSetter, Generic[_SocketType]):
     """Create a zmq Context
 
     A zmq Context creates sockets via its ``ctx.socket`` method.
 
     .. versionchanged:: 24
 
         When using a Context as a context manager (``with zmq.Context()``),
@@ -70,40 +62,40 @@
             ctx = zmq.Context(async_ctx)
 
         Which previously had to be::
 
             ctx = zmq.Context.shadow(async_ctx.underlying)
     """
 
-    sockopts: Dict[int, Any]
+    sockopts: dict[int, Any]
     _instance: Any = None
     _instance_lock = Lock()
-    _instance_pid: Optional[int] = None
+    _instance_pid: int | None = None
     _shadow = False
     _shadow_obj = None
     _warn_destroy_close = False
     _sockets: WeakSet
     # mypy doesn't like a default value here
-    _socket_class: Type[ST] = Socket  # type: ignore
+    _socket_class: type[_SocketType] = Socket  # type: ignore
 
     @overload
-    def __init__(self: "Context[Socket]", io_threads: int = 1): ...
+    def __init__(self: Context[Socket], io_threads: int = 1): ...
 
     @overload
-    def __init__(self: "Context[Socket]", io_threads: "Context"):
+    def __init__(self: Context[Socket], io_threads: Context):
         # this should be positional-only, but that requires 3.8
         ...
 
     @overload
-    def __init__(self: "Context[Socket]", *, shadow: Union["Context", int]): ...
+    def __init__(self: Context[Socket], *, shadow: Context | int): ...
 
     def __init__(
-        self: "Context[Socket]",
-        io_threads: Union[int, "Context"] = 1,
-        shadow: Union["Context", int] = 0,
+        self: Context[Socket],
+        io_threads: int | Context = 1,
+        shadow: Context | int = 0,
     ) -> None:
         if isinstance(io_threads, Context):
             # allow positional shadow `zmq.Context(zmq.asyncio.Context())`
             # this s
             shadow = io_threads
             io_threads = 1
 
@@ -162,45 +154,45 @@
             n_sockets = len(self._sockets)
             s = 's' if n_sockets > 1 else ''
             sockets = f"{n_sockets} socket{s}"
         else:
             sockets = ""
         return f"<{_repr_cls}({sockets}) at {hex(id(self))}{closed}>"
 
-    def __enter__(self: T) -> T:
+    def __enter__(self: _ContextType) -> _ContextType:
         return self
 
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
         # warn about any leftover sockets before closing them
         self._warn_destroy_close = True
         self.destroy()
 
-    def __copy__(self: T, memo: Any = None) -> T:
+    def __copy__(self: _ContextType, memo: Any = None) -> _ContextType:
         """Copying a Context creates a shadow copy"""
         return self.__class__.shadow(self.underlying)
 
     __deepcopy__ = __copy__
 
     @classmethod
-    def shadow(cls: Type[T], address: Union[int, "Context"]) -> T:
+    def shadow(cls: type[_ContextType], address: int | zmq.Context) -> _ContextType:
         """Shadow an existing libzmq context
 
         address is a zmq.Context or an integer (or FFI pointer)
         representing the address of the libzmq context.
 
         .. versionadded:: 14.1
 
         .. versionadded:: 25
             Support for shadowing `zmq.Context` objects,
             instead of just integer addresses.
         """
         return cls(shadow=address)
 
     @classmethod
-    def shadow_pyczmq(cls: Type[T], ctx: Any) -> T:
+    def shadow_pyczmq(cls: type[_ContextType], ctx: Any) -> _ContextType:
         """Shadow an existing pyczmq context
 
         ctx is the FFI `zctx_t *` pointer
 
         .. versionadded:: 14.1
         """
         from pyczmq import zctx  # type: ignore
@@ -209,18 +201,18 @@
 
         underlying = zctx.underlying(ctx)
         address = cast_int_addr(underlying)
         return cls(shadow=address)
 
     # static method copied from tornado IOLoop.instance
     @classmethod
-    def instance(cls: Type[T], io_threads: int = 1) -> T:
+    def instance(cls: type[_ContextType], io_threads: int = 1) -> _ContextType:
         """Returns a global Context instance.
 
-        Most single-threaded applications have a single, global Context.
+        Most single-process applications have a single, global Context.
         Use this method instead of passing around Context instances
         throughout your code.
 
         A common pattern for classes that depend on Contexts is to use
         a default argument to enable programs with multiple Contexts
         but not require the argument for simpler applications::
 
@@ -272,15 +264,15 @@
         """
         super().term()
 
     # -------------------------------------------------------------------------
     # Hooks for ctxopt completion
     # -------------------------------------------------------------------------
 
-    def __dir__(self) -> List[str]:
+    def __dir__(self) -> list[str]:
         keys = dir(self.__class__)
         keys.extend(ContextOption.__members__)
         return keys
 
     # -------------------------------------------------------------------------
     # Creating Sockets
     # -------------------------------------------------------------------------
@@ -291,33 +283,33 @@
 
     def _rm_socket(self, socket: Any) -> None:
         """Remove a socket for Context.destroy / reference counting"""
         # allow _sockets to be None in case of process teardown
         if getattr(self, "_sockets", None) is not None:
             self._sockets.discard(socket)
 
-    def destroy(self, linger: Optional[int] = None) -> None:
+    def destroy(self, linger: int | None = None) -> None:
         """Close all sockets associated with this context and then terminate
         the context.
 
         .. warning::
 
-            destroy involves calling ``zmq_close()``, which is **NOT** threadsafe.
+            destroy involves calling :meth:`Socket.close`, which is **NOT** threadsafe.
             If there are active sockets in other threads, this must not be called.
 
         Parameters
         ----------
 
         linger : int, optional
             If specified, set LINGER on sockets prior to closing them.
         """
         if self.closed:
             return
 
-        sockets: List[ST] = list(getattr(self, "_sockets", None) or [])
+        sockets: list[_SocketType] = list(getattr(self, "_sockets", None) or [])
         for s in sockets:
             if s and not s.closed:
                 if self._warn_destroy_close and warn is not None:
                     # warn can be None during process teardown
                     warn(
                         f"Destroying context with unclosed socket {s}",
                         ResourceWarning,
@@ -327,42 +319,44 @@
                 if linger is not None:
                     s.setsockopt(SocketOption.LINGER, linger)
                 s.close()
 
         self.term()
 
     def socket(
-        self: T,
+        self: _ContextType,
         socket_type: int,
-        socket_class: Optional[Callable[[T, int], ST]] = None,
+        socket_class: Callable[[_ContextType, int], _SocketType] | None = None,
         **kwargs: Any,
-    ) -> ST:
+    ) -> _SocketType:
         """Create a Socket associated with this Context.
 
         Parameters
         ----------
         socket_type : int
             The socket type, which can be any of the 0MQ socket types:
             REQ, REP, PUB, SUB, PAIR, DEALER, ROUTER, PULL, PUSH, etc.
 
-        socket_class: zmq.Socket or a subclass
+        socket_class: zmq.Socket
             The socket class to instantiate, if different from the default for this Context.
             e.g. for creating an asyncio socket attached to a default Context or vice versa.
 
             .. versionadded:: 25
 
         kwargs:
             will be passed to the __init__ method of the socket class.
         """
         if self.closed:
             raise ZMQError(Errno.ENOTSUP)
         if socket_class is None:
             socket_class = self._socket_class
-        s: ST = socket_class(  # set PYTHONTRACEMALLOC=2 to get the calling frame
-            self, socket_type, **kwargs
+        s: _SocketType = (
+            socket_class(  # set PYTHONTRACEMALLOC=2 to get the calling frame
+                self, socket_type, **kwargs
+            )
         )
         for opt, value in self.sockopts.items():
             try:
                 s.setsockopt(opt, value)
             except ZMQError:
                 # ignore ZMQErrors, which are likely for socket options
                 # that do not apply to a particular socket type, e.g.
```

### Comparing `pyzmq-26.0.0b1/zmq/sugar/frame.py` & `pyzmq-26.0.0b2/zmq/sugar/frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     if not zmq.DRAFT_API:
         raise RuntimeError(
             "libzmq and pyzmq must be built with draft support for %s" % feature
         )
 
 
 class Frame(FrameBase, AttributeSetter):
-    """Frame(data=None, track=False, copy=None, copy_threshold=zmq.COPY_THRESHOLD)
-
+    """
     A zmq message Frame class for non-copying send/recvs and access to message properties.
 
     A ``zmq.Frame`` wraps an underlying ``zmq_msg_t``.
 
     Message *properties* can be accessed by treating a Frame like a dictionary (``frame["User-Id"]``).
 
     .. versionadded:: 14.4, libzmq 4
@@ -47,23 +46,25 @@
 
     Parameters
     ----------
 
     data : object, optional
         any object that provides the buffer interface will be used to
         construct the 0MQ message data.
-    track : bool [default: False]
+    track : bool
         whether a MessageTracker_ should be created to track this object.
         Tracking a message has a cost at creation, because it creates a threadsafe
         Event object.
-    copy : bool [default: use copy_threshold]
+    copy : bool
+        default: use copy_threshold
         Whether to create a copy of the data to pass to libzmq
         or share the memory with libzmq.
         If unspecified, copy_threshold is used.
-    copy_threshold: int [default: zmq.COPY_THRESHOLD]
+    copy_threshold: int
+        default: :const:`zmq.COPY_THRESHOLD`
         If copy is unspecified, messages smaller than this many bytes
         will be copied and messages larger than this will be shared with libzmq.
     """
 
     def __getitem__(self, key):
         # map Frame['User-Id'] to Frame.get('User-Id')
         return self.get(key)
```

### Comparing `pyzmq-26.0.0b1/zmq/sugar/poll.py` & `pyzmq-26.0.0b2/zmq/sugar/poll.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """0MQ polling related functions and classes."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-from typing import Any, Dict, List, Optional, Tuple
+from __future__ import annotations
+
+from typing import Any
 
 from zmq.backend import zmq_poll
 from zmq.constants import POLLERR, POLLIN, POLLOUT
 
 # -----------------------------------------------------------------------------
 # Polling related methods
 # -----------------------------------------------------------------------------
 
 
 class Poller:
     """A stateful poll interface that mirrors Python's built-in poll."""
 
-    sockets: List[Tuple[Any, int]]
-    _map: Dict
+    sockets: list[tuple[Any, int]]
+    _map: dict
 
     def __init__(self) -> None:
         self.sockets = []
         self._map = {}
 
     def __contains__(self, socket: Any) -> bool:
         return socket in self._map
@@ -71,66 +73,72 @@
         """
         idx = self._map.pop(socket)
         self.sockets.pop(idx)
         # shift indices after deletion
         for socket, flags in self.sockets[idx:]:
             self._map[socket] -= 1
 
-    def poll(self, timeout: Optional[int] = None) -> List[Tuple[Any, int]]:
+    def poll(self, timeout: int | None = None) -> list[tuple[Any, int]]:
         """Poll the registered 0MQ or native fds for I/O.
 
         If there are currently events ready to be processed, this function will return immediately.
         Otherwise, this function will return as soon the first event is available or after timeout
         milliseconds have elapsed.
 
         Parameters
         ----------
         timeout : int
             The timeout in milliseconds. If None, no `timeout` (infinite). This
             is in milliseconds to be compatible with ``select.poll()``.
 
         Returns
         -------
-        events : list of tuples
+        events : list
             The list of events that are ready to be processed.
             This is a list of tuples of the form ``(socket, event_mask)``, where the 0MQ Socket
             or integer fd is the first element, and the poll event mask (POLLIN, POLLOUT) is the second.
             It is common to call ``events = dict(poller.poll())``,
             which turns the list of tuples into a mapping of ``socket : event_mask``.
         """
         if timeout is None or timeout < 0:
             timeout = -1
         elif isinstance(timeout, float):
             timeout = int(timeout)
         return zmq_poll(self.sockets, timeout=timeout)
 
 
-def select(rlist: List, wlist: List, xlist: List, timeout: Optional[float] = None):
+def select(
+    rlist: list, wlist: list, xlist: list, timeout: float | None = None
+) -> tuple[list, list, list]:
     """select(rlist, wlist, xlist, timeout=None) -> (rlist, wlist, xlist)
 
     Return the result of poll as a lists of sockets ready for r/w/exception.
 
     This has the same interface as Python's built-in ``select.select()`` function.
 
     Parameters
     ----------
-    timeout : float, int, optional
+    timeout : float, optional
         The timeout in seconds. If None, no timeout (infinite). This is in seconds to be
         compatible with ``select.select()``.
-    rlist : list of sockets/FDs
+    rlist : list
         sockets/FDs to be polled for read events
-    wlist : list of sockets/FDs
+    wlist : list
         sockets/FDs to be polled for write events
-    xlist : list of sockets/FDs
+    xlist : list
         sockets/FDs to be polled for error events
 
     Returns
     -------
-    (rlist, wlist, xlist) : tuple of lists of sockets (length 3)
-        Lists correspond to sockets available for read/write/error events respectively.
+    rlist: list
+        list of sockets or FDs that are readable
+    wlist: list
+        list of sockets or FDs that are writable
+    xlist: list
+        list of sockets or FDs that had error events (rare)
     """
     if timeout is None:
         timeout = -1
     # Convert from sec -> ms for zmq_poll.
     # zmq_poll accepts 3.x style timeout in ms
     timeout = int(timeout * 1000.0)
     if timeout < 0:
```

### Comparing `pyzmq-26.0.0b1/zmq/sugar/socket.py` & `pyzmq-26.0.0b2/zmq/sugar/socket.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """0MQ Socket pure Python methods."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
+from __future__ import annotations
 
 import errno
 import pickle
 import random
 import sys
 from typing import (
     Any,
     Callable,
-    Dict,
     Generic,
     List,
-    Optional,
     Sequence,
-    Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 from warnings import warn
 
@@ -36,49 +34,51 @@
 from .poll import Poller
 
 try:
     DEFAULT_PROTOCOL = pickle.DEFAULT_PROTOCOL
 except AttributeError:
     DEFAULT_PROTOCOL = pickle.HIGHEST_PROTOCOL
 
-T = TypeVar("T", bound="Socket")
+_SocketType = TypeVar("_SocketType", bound="Socket")
 
 
-class _SocketContext(Generic[T]):
+class _SocketContext(Generic[_SocketType]):
     """Context Manager for socket bind/unbind"""
 
-    socket: T
+    socket: _SocketType
     kind: str
     addr: str
 
     def __repr__(self):
         return f"<SocketContext({self.kind}={self.addr!r})>"
 
-    def __init__(self: "_SocketContext[T]", socket: T, kind: str, addr: str):
+    def __init__(
+        self: _SocketContext[_SocketType], socket: _SocketType, kind: str, addr: str
+    ):
         assert kind in {"bind", "connect"}
         self.socket = socket
         self.kind = kind
         self.addr = addr
 
-    def __enter__(self: "_SocketContext[T]") -> T:
+    def __enter__(self: _SocketContext[_SocketType]) -> _SocketType:
         return self.socket
 
     def __exit__(self, *args):
         if self.socket.closed:
             return
         if self.kind == "bind":
             self.socket.unbind(self.addr)
         elif self.kind == "connect":
             self.socket.disconnect(self.addr)
 
 
-ST = TypeVar("ST")
+SocketReturnType = TypeVar("SocketReturnType")
 
 
-class Socket(SocketBase, AttributeSetter, Generic[ST]):
+class Socket(SocketBase, AttributeSetter, Generic[SocketReturnType]):
     """The ZMQ socket object
 
     To create a Socket, first create a Context::
 
         ctx = zmq.Context.instance()
 
     then call ``ctx.socket(socket_type)``::
@@ -100,42 +100,42 @@
     _shadow = False
     _shadow_obj = None
     _monitor_socket = None
     _type_name = 'UNKNOWN'
 
     @overload
     def __init__(
-        self: "Socket[bytes]",
-        ctx_or_socket: "zmq.Context",
+        self: Socket[bytes],
+        ctx_or_socket: zmq.Context,
         socket_type: int,
         *,
-        copy_threshold: Optional[int] = None,
+        copy_threshold: int | None = None,
     ): ...
 
     @overload
     def __init__(
-        self: "Socket[bytes]",
+        self: Socket[bytes],
         *,
-        shadow: Union["Socket", int],
-        copy_threshold: Optional[int] = None,
+        shadow: Socket | int,
+        copy_threshold: int | None = None,
     ): ...
 
     @overload
     def __init__(
-        self: "Socket[bytes]",
-        ctx_or_socket: "Socket",
+        self: Socket[bytes],
+        ctx_or_socket: Socket,
     ): ...
 
     def __init__(
-        self: "Socket[bytes]",
-        ctx_or_socket: Optional[Union["zmq.Context", "Socket"]] = None,
+        self: Socket[bytes],
+        ctx_or_socket: zmq.Context | Socket | None = None,
         socket_type: int = 0,
         *,
-        shadow: Union["Socket", int] = 0,
-        copy_threshold: Optional[int] = None,
+        shadow: Socket | int = 0,
+        copy_threshold: int | None = None,
     ):
         if isinstance(ctx_or_socket, zmq.Socket):
             # positional Socket(other_socket)
             shadow = ctx_or_socket
             ctx_or_socket = None
 
         shadow_address: int = 0
@@ -194,36 +194,36 @@
             _repr_cls = f"{cls.__module__}.{cls.__name__}"
 
         closed = ' closed' if self._closed else ''
 
         return f"<{_repr_cls}(zmq.{self._type_name}) at {hex(id(self))}{closed}>"
 
     # socket as context manager:
-    def __enter__(self: T) -> T:
+    def __enter__(self: _SocketType) -> _SocketType:
         """Sockets are context managers
 
         .. versionadded:: 14.4
         """
         return self
 
     def __exit__(self, *args, **kwargs):
         self.close()
 
     # -------------------------------------------------------------------------
     # Socket creation
     # -------------------------------------------------------------------------
 
-    def __copy__(self: T, memo=None) -> T:
+    def __copy__(self: _SocketType, memo=None) -> _SocketType:
         """Copying a Socket creates a shadow copy"""
         return self.__class__.shadow(self.underlying)
 
     __deepcopy__ = __copy__
 
     @classmethod
-    def shadow(cls: Type[T], address: Union[int, "zmq.Socket"]) -> T:
+    def shadow(cls: type[_SocketType], address: int | zmq.Socket) -> _SocketType:
         """Shadow an existing libzmq socket
 
         address is a zmq.Socket or an integer (or FFI pointer)
         representing the address of the libzmq socket.
 
         .. versionadded:: 14.1
 
@@ -254,42 +254,54 @@
             self.context._rm_socket(self)
         super().close(linger=linger)
 
     # -------------------------------------------------------------------------
     # Connect/Bind context managers
     # -------------------------------------------------------------------------
 
-    def _connect_cm(self: T, addr: str) -> _SocketContext[T]:
+    def _connect_cm(self: _SocketType, addr: str) -> _SocketContext[_SocketType]:
         """Context manager to disconnect on exit
 
         .. versionadded:: 20.0
         """
         return _SocketContext(self, 'connect', addr)
 
-    def _bind_cm(self: T, addr: str) -> _SocketContext[T]:
+    def _bind_cm(self: _SocketType, addr: str) -> _SocketContext[_SocketType]:
         """Context manager to unbind on exit
 
         .. versionadded:: 20.0
         """
+        try:
+            # retrieve last_endpoint
+            # to support binding on random ports via
+            # `socket.bind('tcp://127.0.0.1:0')`
+            addr = cast(bytes, self.get(zmq.LAST_ENDPOINT)).decode("utf8")
+        except (AttributeError, ZMQError, UnicodeDecodeError):
+            pass
         return _SocketContext(self, 'bind', addr)
 
-    def bind(self: T, addr: str) -> _SocketContext[T]:
+    def bind(self: _SocketType, addr: str) -> _SocketContext[_SocketType]:
         """s.bind(addr)
 
         Bind the socket to an address.
 
         This causes the socket to listen on a network port. Sockets on the
         other side of this connection will use ``Socket.connect(addr)`` to
         connect to this socket.
 
         Returns a context manager which will call unbind on exit.
 
         .. versionadded:: 20.0
             Can be used as a context manager.
 
+        .. versionadded:: 26.0
+            binding to port 0 can be used as a context manager
+            for binding to a random port.
+            The URL can be retrieved as `socket.last_endpoint`.
+
         Parameters
         ----------
         addr : str
             The address string. This has the form 'protocol://interface:port',
             for example 'tcp://127.0.0.1:5555'. Protocols supported include
             tcp, udp, pgm, epgm, inproc and ipc. If the address is unicode, it is
             encoded to utf-8 first.
@@ -298,15 +310,15 @@
         try:
             super().bind(addr)
         except ZMQError as e:
             e.strerror += f" (addr={addr!r})"
             raise
         return self._bind_cm(addr)
 
-    def connect(self: T, addr: str) -> _SocketContext[T]:
+    def connect(self: _SocketType, addr: str) -> _SocketContext[_SocketType]:
         """s.connect(addr)
 
         Connect to a remote 0MQ socket.
 
         Returns a context manager which will call disconnect on exit.
 
         .. versionadded:: 20.0
@@ -375,26 +387,26 @@
         It is important that all available events be consumed when an event is detected,
         otherwise the read event will not trigger again.
 
         .. versionadded:: 17.0
         """
         return self.FD
 
-    def subscribe(self, topic: Union[str, bytes]) -> None:
+    def subscribe(self, topic: str | bytes) -> None:
         """Subscribe to a topic
 
         Only for SUB sockets.
 
         .. versionadded:: 15.3
         """
         if isinstance(topic, str):
             topic = topic.encode('utf8')
         self.set(zmq.SUBSCRIBE, topic)
 
-    def unsubscribe(self, topic: Union[str, bytes]) -> None:
+    def unsubscribe(self, topic: str | bytes) -> None:
         """Unsubscribe from a topic
 
         Only for SUB sockets.
 
         .. versionadded:: 15.3
         """
         if isinstance(topic, str):
@@ -442,15 +454,15 @@
         if SocketOption(option)._opt_type != _OptType.bytes:
             raise TypeError(f"option {option} will not return a string to be decoded")
         return cast(bytes, self.get(option)).decode(encoding)
 
     getsockopt_unicode = getsockopt_string = get_string
 
     def bind_to_random_port(
-        self: T,
+        self: _SocketType,
         addr: str,
         min_port: int = 49152,
         max_port: int = 65536,
         max_tries: int = 100,
     ) -> int:
         """Bind this socket to a random port in a range.
 
@@ -569,61 +581,61 @@
     def send(
         self,
         data: Any,
         flags: int = ...,
         copy: bool = ...,
         *,
         track: Literal[True],
-        routing_id: Optional[int] = ...,
-        group: Optional[str] = ...,
-    ) -> "zmq.MessageTracker": ...
+        routing_id: int | None = ...,
+        group: str | None = ...,
+    ) -> zmq.MessageTracker: ...
 
     @overload
     def send(
         self,
         data: Any,
         flags: int = ...,
         copy: bool = ...,
         *,
         track: Literal[False],
-        routing_id: Optional[int] = ...,
-        group: Optional[str] = ...,
+        routing_id: int | None = ...,
+        group: str | None = ...,
     ) -> None: ...
 
     @overload
     def send(
         self,
         data: Any,
         flags: int = ...,
         *,
         copy: bool = ...,
-        routing_id: Optional[int] = ...,
-        group: Optional[str] = ...,
+        routing_id: int | None = ...,
+        group: str | None = ...,
     ) -> None: ...
 
     @overload
     def send(
         self,
         data: Any,
         flags: int = ...,
         copy: bool = ...,
         track: bool = ...,
-        routing_id: Optional[int] = ...,
-        group: Optional[str] = ...,
-    ) -> Optional["zmq.MessageTracker"]: ...
+        routing_id: int | None = ...,
+        group: str | None = ...,
+    ) -> zmq.MessageTracker | None: ...
 
     def send(
         self,
         data: Any,
         flags: int = 0,
         copy: bool = True,
         track: bool = False,
-        routing_id: Optional[int] = None,
-        group: Optional[str] = None,
-    ) -> Optional["zmq.MessageTracker"]:
+        routing_id: int | None = None,
+        group: str | None = None,
+    ) -> zmq.MessageTracker | None:
         """Send a single zmq message frame on this socket.
 
         This queues the message to be sent by the IO thread at a later time.
 
         With flags=NOBLOCK, this raises :class:`ZMQError` if the queue is full;
         otherwise, this waits until space is available.
         See :class:`Poller` for more general non-blocking I/O.
@@ -646,16 +658,16 @@
             For use with RADIO sockets
 
         Returns
         -------
         None : if `copy` or not track
             None if message was sent, raises an exception otherwise.
         MessageTracker : if track and not copy
-            a MessageTracker object, whose `pending` property will
-            be True until the send is completed.
+            a MessageTracker object, whose `done` property will
+            be False until the send is completed.
 
         Raises
         ------
         TypeError
             If a unicode object is passed
         ValueError
             If `track=True`, but an untracked Frame is passed.
@@ -716,16 +728,16 @@
             Should the frame(s) be tracked for notification that ZMQ has
             finished with it (ignored if copy=True).
 
         Returns
         -------
         None : if copy or not track
         MessageTracker : if track and not copy
-            a MessageTracker object, whose `pending` property will
-            be True until the last send is completed.
+            a MessageTracker object, whose `done` property will
+            be False until the last send is completed.
         """
         # typecheck parts before sending:
         for i, msg in enumerate(msg_parts):
             if isinstance(msg, (zmq.Frame, bytes, memoryview)):
                 continue
             try:
                 memoryview(msg)
@@ -744,32 +756,32 @@
             self.send(msg, zmq.SNDMORE | flags, copy=copy, track=track)
         # Send the last part without the extra SNDMORE flag.
         return self.send(msg_parts[-1], flags, copy=copy, track=track)
 
     @overload
     def recv_multipart(
         self, flags: int = ..., *, copy: Literal[True], track: bool = ...
-    ) -> List[bytes]: ...
+    ) -> list[bytes]: ...
 
     @overload
     def recv_multipart(
         self, flags: int = ..., *, copy: Literal[False], track: bool = ...
-    ) -> List[zmq.Frame]: ...
+    ) -> list[zmq.Frame]: ...
 
     @overload
-    def recv_multipart(self, flags: int = ..., *, track: bool = ...) -> List[bytes]: ...
+    def recv_multipart(self, flags: int = ..., *, track: bool = ...) -> list[bytes]: ...
 
     @overload
     def recv_multipart(
         self, flags: int = 0, copy: bool = True, track: bool = False
-    ) -> Union[List[zmq.Frame], List[bytes]]: ...
+    ) -> list[zmq.Frame] | list[bytes]: ...
 
     def recv_multipart(
         self, flags: int = 0, copy: bool = True, track: bool = False
-    ) -> Union[List[zmq.Frame], List[bytes]]:
+    ) -> list[zmq.Frame] | list[bytes]:
         """Receive a multipart message as a list of bytes or Frame objects
 
         Parameters
         ----------
         flags : int, optional
             Any valid flags for :func:`Socket.recv`.
         copy : bool, optional
@@ -875,27 +887,27 @@
     def send_string(
         self,
         u: str,
         flags: int = 0,
         copy: bool = True,
         encoding: str = 'utf-8',
         **kwargs,
-    ) -> Optional["zmq.Frame"]:
+    ) -> zmq.Frame | None:
         """Send a Python unicode string as a message with an encoding.
 
         0MQ communicates with raw bytes, so you must encode/decode
         text (str) around 0MQ.
 
         Parameters
         ----------
         u : str
             The unicode string to send.
         flags : int, optional
             Any valid flags for :func:`Socket.send`.
-        encoding : str [default: 'utf-8']
+        encoding : str
             The encoding to be used
         """
         if not isinstance(u, str):
             raise TypeError("str objects only")
         return self.send(u.encode(encoding), flags=flags, copy=copy, **kwargs)
 
     send_unicode = send_string
@@ -903,35 +915,35 @@
     def recv_string(self, flags: int = 0, encoding: str = 'utf-8') -> str:
         """Receive a unicode string, as sent by send_string.
 
         Parameters
         ----------
         flags : int
             Any valid flags for :func:`Socket.recv`.
-        encoding : str [default: 'utf-8']
+        encoding : str
             The encoding to be used
 
         Returns
         -------
         s : str
             The Python unicode string that arrives as encoded bytes.
 
         Raises
         ------
         ZMQError
-            for any of the reasons :func:`~Socket.recv` might fail
+            for any of the reasons :func:`Socket.recv` might fail
         """
         msg = self.recv(flags=flags)
         return self._deserialize(msg, lambda buf: buf.decode(encoding))
 
     recv_unicode = recv_string
 
     def send_pyobj(
         self, obj: Any, flags: int = 0, protocol: int = DEFAULT_PROTOCOL, **kwargs
-    ) -> Optional[zmq.Frame]:
+    ) -> zmq.Frame | None:
         """Send a Python object as a message using pickle to serialize.
 
         Parameters
         ----------
         obj : Python object
             The Python object to send.
         flags : int
@@ -979,15 +991,15 @@
         send_kwargs = {}
         for key in ('routing_id', 'group'):
             if key in kwargs:
                 send_kwargs[key] = kwargs.pop(key)
         msg = jsonapi.dumps(obj, **kwargs)
         return self.send(msg, flags=flags, **send_kwargs)
 
-    def recv_json(self, flags: int = 0, **kwargs) -> Union[List, str, int, float, Dict]:
+    def recv_json(self, flags: int = 0, **kwargs) -> list | str | int | float | dict:
         """Receive a Python object as a message using json to serialize.
 
         Keyword arguments are passed on to json.loads
 
         Parameters
         ----------
         flags : int
@@ -1004,24 +1016,26 @@
             for any of the reasons :func:`~Socket.recv` might fail
         """
         msg = self.recv(flags)
         return self._deserialize(msg, lambda buf: jsonapi.loads(buf, **kwargs))
 
     _poller_class = Poller
 
-    def poll(self, timeout=None, flags=zmq.POLLIN) -> int:
+    def poll(self, timeout: int | None = None, flags: int = zmq.POLLIN) -> int:
         """Poll the socket for events.
+
         See :class:`Poller` to wait for multiple sockets at once.
 
         Parameters
         ----------
-        timeout : int [default: None]
+        timeout : int
             The timeout (in milliseconds) to wait for an event. If unspecified
             (or specified None), will wait forever for an event.
-        flags : int [default: POLLIN]
+        flags : int
+            default: POLLIN.
             POLLIN, POLLOUT, or POLLIN|POLLOUT. The event flags to poll for.
 
         Returns
         -------
         event_mask : int
             The poll event mask (POLLIN, POLLOUT),
             0 if the timeout was reached without an event.
@@ -1033,32 +1047,33 @@
         p = self._poller_class()
         p.register(self, flags)
         evts = dict(p.poll(timeout))
         # return 0 if no events, otherwise return event bitfield
         return evts.get(self, 0)
 
     def get_monitor_socket(
-        self: T, events: Optional[int] = None, addr: Optional[str] = None
-    ) -> T:
+        self: _SocketType, events: int | None = None, addr: str | None = None
+    ) -> _SocketType:
         """Return a connected PAIR socket ready to receive the event notifications.
 
         .. versionadded:: libzmq-4.0
         .. versionadded:: 14.0
 
         Parameters
         ----------
-        events : int [default: ZMQ_EVENT_ALL]
+        events : int
+            default: `zmq.EVENT_ALL`
             The bitmask defining which events are wanted.
-        addr :  string [default: None]
+        addr : str
             The optional endpoint for the monitoring sockets.
 
         Returns
         -------
-        socket :  (PAIR)
-            The socket is already connected and ready to receive messages.
+        socket : zmq.Socket
+            The PAIR socket, connected and ready to receive messages.
         """
         # safe-guard, method only available on libzmq >= 4
         if zmq.zmq_version_info() < (4,):
             raise NotImplementedError(
                 "get_monitor_socket requires libzmq >= 4, have %s" % zmq.zmq_version()
             )
```

### Comparing `pyzmq-26.0.0b1/zmq/sugar/stopwatch.py` & `pyzmq-26.0.0b2/zmq/sugar/stopwatch.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/sugar/tracker.py` & `pyzmq-26.0.0b2/zmq/sugar/tracker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 """Tracker for zero-copy messages with 0MQ."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
+from __future__ import annotations
+
 import time
 from threading import Event
-from typing import Set, Tuple, Union
 
 from zmq.backend import Frame
 from zmq.error import NotDone
 
 
 class MessageTracker:
-    """MessageTracker(*towatch)
-
-    A class for tracking if 0MQ is done using one or more messages.
+    """A class for tracking if 0MQ is done using one or more messages.
 
     When you send a 0MQ message, it is not sent immediately. The 0MQ IO thread
     sends the message at some later time. Often you want to know when 0MQ has
     actually sent the message though. This is complicated by the fact that
     a single 0MQ message can be sent multiple times using different sockets.
     This class allows you to track all of the 0MQ usages of a message.
 
     Parameters
     ----------
-    towatch : Event, MessageTracker, Message instances.
+    towatch : Event, MessageTracker, zmq.Frame
         This objects to track. This class can track the low-level
         Events used by the Message class, other MessageTrackers or
         actual Messages.
     """
 
-    events: Set[Event]
-    peers: Set["MessageTracker"]
+    events: set[Event]
+    peers: set[MessageTracker]
 
-    def __init__(self, *towatch: Tuple[Union["MessageTracker", Event, Frame]]):
-        """MessageTracker(*towatch)
-
-        Create a message tracker to track a set of messages.
+    def __init__(self, *towatch: tuple[MessageTracker | Event | Frame]):
+        """Create a message tracker to track a set of messages.
 
         Parameters
         ----------
         *towatch : tuple of Event, MessageTracker, Message instances.
             This list of objects to track. This class can track the low-level
             Events used by the Message class, other MessageTrackers or
             actual Messages.
@@ -66,22 +63,21 @@
             if not evt.is_set():
                 return False
         for pm in self.peers:
             if not pm.done:
                 return False
         return True
 
-    def wait(self, timeout: Union[float, int] = -1):
-        """mt.wait(timeout=-1)
-
-        Wait for 0MQ to be done with the message or until `timeout`.
+    def wait(self, timeout: float | int = -1):
+        """Wait for 0MQ to be done with the message or until `timeout`.
 
         Parameters
         ----------
-        timeout : float [default: -1, wait forever]
+        timeout : float
+            default: -1, which means wait forever.
             Maximum time in (s) to wait before raising NotDone.
 
         Returns
         -------
         None
             if done before `timeout`
```

### Comparing `pyzmq-26.0.0b1/zmq/sugar/version.py` & `pyzmq-26.0.0b2/zmq/sugar/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """PyZMQ and 0MQ version functions."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
+from __future__ import annotations
 
 import re
-from typing import Match, Tuple, Union, cast
+from typing import Match, cast
 
 from zmq.backend import zmq_version_info
 
-__version__: str = "26.0.0b1"
+__version__: str = "26.0.0b2"
 _version_pat = re.compile(r"(\d+)\.(\d+)\.(\d+)(.*)")
 _match = cast(Match, _version_pat.match(__version__))
 _version_groups = _match.groups()
 
 VERSION_MAJOR = int(_version_groups[0])
 VERSION_MINOR = int(_version_groups[1])
 VERSION_PATCH = int(_version_groups[2])
 VERSION_EXTRA = _version_groups[3].lstrip(".")
 
-version_info: Union[Tuple[int, int, int], Tuple[int, int, int, float]] = (
+version_info: tuple[int, int, int] | tuple[int, int, int, float] = (
     VERSION_MAJOR,
     VERSION_MINOR,
     VERSION_PATCH,
 )
 
 if VERSION_EXTRA:
     version_info = (
@@ -39,15 +40,15 @@
     """return the version of pyzmq as a string"""
     if __revision__:
         return '+'.join([__version__, __revision__[:6]])
     else:
         return __version__
 
 
-def pyzmq_version_info() -> Union[Tuple[int, int, int], Tuple[int, int, int, float]]:
+def pyzmq_version_info() -> tuple[int, int, int] | tuple[int, int, int, float]:
     """return the pyzmq version as a tuple of at least three numbers
 
     If pyzmq is a development version, `inf` will be appended after the third integer.
     """
     return version_info
```

### Comparing `pyzmq-26.0.0b1/zmq/tests/__init__.py` & `pyzmq-26.0.0b2/zmq/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/conftest.py` & `pyzmq-26.0.0b2/zmq/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/cython_ext.pyx` & `pyzmq-26.0.0b2/zmq/tests/cython_ext.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_asyncio.py` & `pyzmq-26.0.0b2/zmq/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_auth.py` & `pyzmq-26.0.0b2/zmq/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_cffi_backend.py` & `pyzmq-26.0.0b2/zmq/tests/test_cffi_backend.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_constants.py` & `pyzmq-26.0.0b2/zmq/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_context.py` & `pyzmq-26.0.0b2/zmq/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_cython.py` & `pyzmq-26.0.0b2/zmq/tests/test_cython.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_decorators.py` & `pyzmq-26.0.0b2/zmq/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_device.py` & `pyzmq-26.0.0b2/zmq/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_draft.py` & `pyzmq-26.0.0b2/zmq/tests/test_draft.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_error.py` & `pyzmq-26.0.0b2/zmq/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_etc.py` & `pyzmq-26.0.0b2/zmq/tests/test_etc.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_ext.py` & `pyzmq-26.0.0b2/zmq/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_future.py` & `pyzmq-26.0.0b2/zmq/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_imports.py` & `pyzmq-26.0.0b2/zmq/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_includes.py` & `pyzmq-26.0.0b2/zmq/tests/test_includes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_ioloop.py` & `pyzmq-26.0.0b2/zmq/tests/test_ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_log.py` & `pyzmq-26.0.0b2/zmq/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_message.py` & `pyzmq-26.0.0b2/zmq/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_monitor.py` & `pyzmq-26.0.0b2/zmq/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_monqueue.py` & `pyzmq-26.0.0b2/zmq/tests/test_monqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_multipart.py` & `pyzmq-26.0.0b2/zmq/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_mypy.py` & `pyzmq-26.0.0b2/zmq/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_pair.py` & `pyzmq-26.0.0b2/zmq/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_poll.py` & `pyzmq-26.0.0b2/zmq/tests/test_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_proxy_steerable.py` & `pyzmq-26.0.0b2/zmq/tests/test_proxy_steerable.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_pubsub.py` & `pyzmq-26.0.0b2/zmq/tests/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_reqrep.py` & `pyzmq-26.0.0b2/zmq/tests/test_reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_retry_eintr.py` & `pyzmq-26.0.0b2/zmq/tests/test_retry_eintr.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_security.py` & `pyzmq-26.0.0b2/zmq/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_socket.py` & `pyzmq-26.0.0b2/zmq/tests/test_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,23 @@
                 b.connect(url)
                 # Since a is unbound from url, b is not connected to anything
                 with pytest.raises(zmq.Again):
                     a.send(msg, flags=zmq.DONTWAIT)
                 with pytest.raises(zmq.Again):
                     b.recv(flags=zmq.DONTWAIT)
 
+    def test_bind_random_context(self):
+        with self.context.socket(zmq.PUSH) as push:
+            with push.bind("tcp://127.0.0.1:0"):
+                url = push.last_endpoint
+                with self.context.socket(zmq.PULL) as pull:
+                    pull.connect(url)
+                    push.send(b"msg")
+                    self.recv(pull)
+
     _repr_cls = "zmq.Socket"
 
     def test_repr(self):
         with self.context.socket(zmq.PUSH) as s:
             assert f'{self._repr_cls}(zmq.PUSH)' in repr(s)
             assert 'closed' not in repr(s)
         assert f'{self._repr_cls}(zmq.PUSH)' in repr(s)
```

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_version.py` & `pyzmq-26.0.0b2/zmq/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_win32_shim.py` & `pyzmq-26.0.0b2/zmq/tests/test_win32_shim.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_z85.py` & `pyzmq-26.0.0b2/zmq/tests/test_z85.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/tests/test_zmqstream.py` & `pyzmq-26.0.0b2/zmq/tests/test_zmqstream.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/utils/buffers.pxd` & `pyzmq-26.0.0b2/zmq/utils/buffers.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/utils/garbage.py` & `pyzmq-26.0.0b2/zmq/utils/garbage.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/utils/interop.py` & `pyzmq-26.0.0b2/zmq/utils/interop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/utils/ipcmaxlen.h` & `pyzmq-26.0.0b2/zmq/utils/ipcmaxlen.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/utils/jsonapi.py` & `pyzmq-26.0.0b2/zmq/utils/jsonapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,31 +4,32 @@
     Remove optional imports of different JSON implementations.
     Now that we require recent Python, unconditionally use the standard library.
     Custom JSON libraries can be used via custom serialization functions.
 """
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
+from __future__ import annotations
 
 import json
-from typing import Any, Dict, List, Union
+from typing import Any
 
 # backward-compatibility, unused
 jsonmod = json
 
 
 def dumps(o: Any, **kwargs) -> bytes:
     """Serialize object to JSON bytes (utf-8).
 
     Keyword arguments are passed along to :py:func:`json.dumps`.
     """
     return json.dumps(o, **kwargs).encode("utf8")
 
 
-def loads(s: Union[bytes, str], **kwargs) -> Union[Dict, List, str, int, float]:
+def loads(s: bytes | str, **kwargs) -> dict | list | str | int | float:
     """Load object from JSON bytes (utf-8).
 
     Keyword arguments are passed along to :py:func:`json.loads`.
     """
     if isinstance(s, bytes):
         s = s.decode("utf8")
     return json.loads(s, **kwargs)
```

### Comparing `pyzmq-26.0.0b1/zmq/utils/monitor.py` & `pyzmq-26.0.0b2/zmq/utils/monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Module holding utility and convenience functions for zmq event monitoring."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
+from __future__ import annotations
+
 import struct
-from typing import Awaitable, List, Union, overload
+from typing import Awaitable, overload
 
 import zmq
 import zmq.asyncio
 from zmq._typing import TypedDict
 from zmq.error import _check_version
 
 
 class _MonitorMessage(TypedDict):
     event: int
     value: int
     endpoint: bytes
 
 
-def parse_monitor_message(msg: List[bytes]) -> _MonitorMessage:
+def parse_monitor_message(msg: list[bytes]) -> _MonitorMessage:
     """decode zmq_monitor event messages.
 
     Parameters
     ----------
     msg : list(bytes)
         zmq multipart message that has arrived on a monitor PAIR socket.
 
@@ -47,63 +49,66 @@
         'value': zmq.Event(value),
         'endpoint': msg[1],
     }
     return event
 
 
 async def _parse_monitor_msg_async(
-    awaitable_msg: Awaitable[List[bytes]],
+    awaitable_msg: Awaitable[list[bytes]],
 ) -> _MonitorMessage:
     """Like parse_monitor_msg, but awaitable
 
     Given awaitable message, return awaitable for the parsed monitor message.
     """
 
     msg = await awaitable_msg
     # 4.0-style event API
     return parse_monitor_message(msg)
 
 
 @overload
 def recv_monitor_message(
-    socket: "zmq.asyncio.Socket",
+    socket: zmq.asyncio.Socket,
     flags: int = 0,
 ) -> Awaitable[_MonitorMessage]: ...
 
 
 @overload
 def recv_monitor_message(
     socket: zmq.Socket[bytes],
     flags: int = 0,
 ) -> _MonitorMessage: ...
 
 
 def recv_monitor_message(
     socket: zmq.Socket,
     flags: int = 0,
-) -> Union[_MonitorMessage, Awaitable[_MonitorMessage]]:
+) -> _MonitorMessage | Awaitable[_MonitorMessage]:
     """Receive and decode the given raw message from the monitoring socket and return a dict.
 
     Requires libzmq ≥ 4.0
 
     The returned dict will have the following entries:
-      event     : int, the event id as described in libzmq.zmq_socket_monitor
-      value     : int, the event value associated with the event, see libzmq.zmq_socket_monitor
-      endpoint  : string, the affected endpoint
+      event : int
+        the event id as described in `libzmq.zmq_socket_monitor`
+      value : int
+        the event value associated with the event, see `libzmq.zmq_socket_monitor`
+      endpoint : str
+        the affected endpoint
 
     .. versionchanged:: 23.1
         Support for async sockets added.
         When called with a async socket,
         returns an awaitable for the monitor message.
 
     Parameters
     ----------
-    socket : zmq PAIR socket
+    socket : zmq.Socket
         The PAIR socket (created by other.get_monitor_socket()) on which to recv the message
-    flags : bitfield (int)
+    flags : int
         standard zmq recv flags
 
     Returns
     -------
     event : dict
         event description as dict with the keys `event`, `value`, and `endpoint`.
     """
```

### Comparing `pyzmq-26.0.0b1/zmq/utils/mutex.h` & `pyzmq-26.0.0b2/zmq/utils/mutex.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/utils/strtypes.py` & `pyzmq-26.0.0b2/zmq/utils/strtypes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmq/utils/win32.py` & `pyzmq-26.0.0b2/zmq/utils/win32.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Win32 compatibility utilities."""
 
 # -----------------------------------------------------------------------------
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 # -----------------------------------------------------------------------------
+from __future__ import annotations
 
 import os
-from typing import Any, Callable, Optional
+from typing import Any, Callable
 
 
 class allow_interrupt:
     """Utility for fixing CTRL-C events on Windows.
 
     On Windows, the Python interpreter intercepts CTRL-C events in order to
     translate them into ``KeyboardInterrupt`` exceptions.  It (presumably)
@@ -56,15 +57,15 @@
     send message to a ``PAIR`` socket in order to interrupt your blocking
     socket polling operation.
 
     In a Tornado event loop, you can use the ``IOLoop.stop`` method to
     unblock your I/O loop.
     """
 
-    def __init__(self, action: Optional[Callable[[], Any]] = None) -> None:
+    def __init__(self, action: Callable[[], Any] | None = None) -> None:
         """Translate ``action`` into a CTRL-C handler.
 
         ``action`` is a callable that takes no arguments and returns no
         value (returned value is ignored).  It must *NEVER* raise an
         exception.
 
         If unspecified, a no-op will be used.
```

### Comparing `pyzmq-26.0.0b1/zmq/utils/z85.py` & `pyzmq-26.0.0b2/zmq/utils/z85.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 See ZMQ RFC 32 for details.
 
 
 """
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
+from __future__ import annotations
 
 import struct
 
 # Z85CHARS is the base 85 symbol table
 Z85CHARS = b"0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ.-:+=^!/*?&<>()[]{}@%$#"
 # Z85MAP maps integers in [0,84] to the appropriate character in Z85CHARS
 Z85MAP = {c: idx for idx, c in enumerate(Z85CHARS)}
```

### Comparing `pyzmq-26.0.0b1/zmq/utils/zmq_compat.h` & `pyzmq-26.0.0b2/zmq/utils/zmq_compat.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/zmqversion.py` & `pyzmq-26.0.0b2/zmqversion.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b1/PKG-INFO` & `pyzmq-26.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzmq
-Version: 26.0.0b1
+Version: 26.0.0b2
 Summary: Python bindings for 0MQ
 Author: Brian E. Granger, Min Ragan-Kelley
 Author-Email: PyZMQ Contributors <zeromq-dev@lists.zeromq.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2009-2012, Brian Granger, Min Ragan-Kelley
```

