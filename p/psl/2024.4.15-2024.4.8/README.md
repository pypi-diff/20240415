# Comparing `tmp/psl-2024.4.15.tar.gz` & `tmp/psl-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2024.4.15.tar", last modified: Mon Apr 15 13:04:33 2024, max compression
+gzip compressed data, was "psl-2024.4.8.tar", last modified: Mon Apr  8 13:04:11 2024, max compression
```

## Comparing `psl-2024.4.15.tar` & `psl-2024.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:04:33.152124 psl-2024.4.15/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-15 13:04:03.000000 psl-2024.4.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 13:04:03.000000 psl-2024.4.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-15 13:04:33.152124 psl-2024.4.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-15 13:04:03.000000 psl-2024.4.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:04:33.152124 psl-2024.4.15/psl/
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-15 13:04:11.000000 psl-2024.4.15/psl/__init__.py
--rw-------   0 runner    (1001) docker     (127)   132154 2024-04-15 13:04:11.000000 psl-2024.4.15/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:04:03.000000 psl-2024.4.15/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:04:33.152124 psl-2024.4.15/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-15 13:04:33.000000 psl-2024.4.15/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 13:04:33.000000 psl-2024.4.15/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:04:33.000000 psl-2024.4.15/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:04:23.000000 psl-2024.4.15/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 13:04:33.000000 psl-2024.4.15/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:04:33.152124 psl-2024.4.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-15 13:04:03.000000 psl-2024.4.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:04:11.621859 psl-2024.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-08 13:03:43.000000 psl-2024.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 13:03:43.000000 psl-2024.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-08 13:04:11.621859 psl-2024.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-08 13:03:43.000000 psl-2024.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:04:11.621859 psl-2024.4.8/psl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-08 13:03:50.000000 psl-2024.4.8/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (127)   131388 2024-04-08 13:03:50.000000 psl-2024.4.8/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:43.000000 psl-2024.4.8/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:04:11.621859 psl-2024.4.8/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:04:01.000000 psl-2024.4.8/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:04:11.621859 psl-2024.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-08 13:03:43.000000 psl-2024.4.8/setup.py
```

### Comparing `psl-2024.4.15/LICENSE` & `psl-2024.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2024.4.15/PKG-INFO` & `psl-2024.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.4.15
+Version: 2024.4.8
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.4.15/README.md` & `psl-2024.4.8/README.md`

 * *Files identical despite different names*

### Comparing `psl-2024.4.15/psl/__init__.py` & `psl-2024.4.8/psl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2024.4.15"
-__checksum__ = "ed3fb8b12fdb1a05d9c9e5933f952e6e9776ad91"
+__version__ = "2024.4.8"
+__checksum__ = "99c4f4f86c43fc0696efa7094e54a82ae3dec72a"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2024.4.15/psl/psl.txt` & `psl-2024.4.8/psl/psl.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7569,15 +7569,14 @@
 poivron.org
 potager.org
 sweetpepper.org
 myasustor.com
 cdn.prod.atlassian-dev.net
 translated.page
 autocode.dev
-myfritz.link
 myfritz.net
 onavstack.net
 *.awdev.ca
 *.advisor.ws
 ecommerce-shop.pl
 b-data.io
 backplaneapp.io
@@ -7693,52 +7692,36 @@
 *.cloudera.site
 cf-ipfs.com
 cloudflare-ipfs.com
 trycloudflare.com
 pages.dev
 r2.dev
 workers.dev
-cust.cloudscale.ch
-objects.lpg.cloudscale.ch
-objects.rma.cloudscale.ch
 wnext.app
 co.ca
 *.otap.co
 co.cz
-cdn77-storage.com
-rsc.contentproxy9.cz
+c.cdn77.org
 cdn77-ssl.net
 r.cdn77.net
-ssl.origin.cdn77-secure.org
-c.cdn77.org
 rsc.cdn77.org
+ssl.origin.cdn77-secure.org
 cloudns.asia
-cloudns.be
 cloudns.biz
-cloudns.cc
-cloudns.ch
-cloudns.cl
 cloudns.club
-dnsabr.com
-cloudns.cx
+cloudns.cc
 cloudns.eu
 cloudns.in
 cloudns.info
-dns-cloud.net
-dns-dynamic.net
-cloudns.nz
 cloudns.org
-cloudns.ph
 cloudns.pro
 cloudns.pw
 cloudns.us
 cnpy.gdn
 codeberg.page
-csb.app
-preview.csb.app
 co.nl
 co.no
 webhosting.be
 hosting-cluster.nl
 convex.site
 ac.ru
 edu.ru
@@ -7787,15 +7770,14 @@
 firm.dk
 reg.dk
 store.dk
 dyndns.dappnode.io
 *.dapps.earth
 *.bzz.dapps.earth
 builtwithdark.com
-darklang.io
 demo.datadetect.com
 instance.datadetect.com
 edgestack.me
 ddns5.com
 debian.net
 deno.dev
 deno-staging.dev
@@ -8132,16 +8114,14 @@
 myddns.rocks
 blogsite.xyz
 dynv6.net
 e4.cz
 easypanel.app
 easypanel.host
 *.ewp.live
-at.emf.camp
-rt.ht
 elementor.cloud
 elementor.cool
 en-root.fr
 mytuleap.com
 tuleap-partners.com
 encr.app
 encoreapi.com
@@ -8336,15 +8316,14 @@
 flutterflow.app
 fly.dev
 edgeapp.net
 shw.io
 flynnhosting.net
 forgeblocks.com
 id.forgerock.io
-framer.ai
 framer.app
 framercanvas.com
 framer.media
 framer.photos
 framer.website
 framer.wiki
 *.frusky.de
@@ -8355,29 +8334,14 @@
 fbx-os.fr
 fbxos.fr
 freebox-os.fr
 freeboxos.fr
 freedesktop.org
 freemyip.com
 wien.funkfeuer.at
-daemon.asia
-dix.asia
-mydns.bz
-0am.jp
-0g0.jp
-0j0.jp
-0t0.jp
-mydns.jp
-pgw.jp
-wjg.jp
-keyword-on.net
-live-on.net
-server-on.net
-mydns.tw
-mydns.vc
 *.futurecms.at
 *.ex.futurecms.at
 *.in.futurecms.at
 futurehosting.at
 futuremailing.at
 *.ex.ortsinfo.at
 *.kunden.ortsinfo.at
@@ -8395,17 +8359,14 @@
 api.gov.uk
 gehirn.ne.jp
 usercontent.jp
 gentapps.com
 gentlentapis.com
 lab.ms
 cdn-edges.net
-localcert.net
-localhostcert.net
-corpnet.work
 ghost.io
 gsj.bz
 githubusercontent.com
 githubpreview.dev
 github.io
 gitlab.io
 gitapp.si
@@ -8616,36 +8577,34 @@
 blogspot.sn
 blogspot.td
 blogspot.tw
 blogspot.ug
 blogspot.vn
 goupile.fr
 gov.nl
-grayjayleagues.com
 awsmppl.com
 xn--gnstigbestellen-zvb.de
 xn--gnstigliefern-wob.de
 fin.ci
 free.hr
 caa.li
 ua.rs
 conf.se
 hs.zone
 hs.run
 hashbang.sh
 hasura.app
 hasura-app.io
 pages.it.hs-heilbronn.de
-helioho.st
-heliohost.us
 hepforge.org
 herokuapp.com
 herokussl.com
 ravendb.cloud
 ravendb.community
+ravendb.me
 development.run
 ravendb.run
 homesklep.pl
 *.kin.one
 *.id.pub
 *.kin.pub
 secaas.hk
@@ -8714,15 +8673,14 @@
 se.leg.br
 sp.leg.br
 to.leg.br
 pixolino.com
 na4u.ru
 iopsys.se
 ipifony.net
-is-a.dev
 ir.md
 iservschule.de
 mein-iserv.de
 schulplattform.de
 schulserver.de
 test-iserv.de
 iserv.dev
@@ -8835,15 +8793,14 @@
 git-repos.de
 lcube-server.de
 svn-repos.de
 leadpages.co
 lpages.co
 lpusercontent.com
 lelux.site
-runcontainers.dev
 co.business
 co.education
 co.events
 co.financial
 co.network
 co.place
 co.technology
@@ -8985,15 +8942,14 @@
 jp.ngrok.io
 sa.ngrok.io
 us.ngrok.io
 ngrok.pizza
 ngrok.pro
 torun.pl
 nh-serv.co.uk
-nimsite.uk
 nfshost.com
 ipfs.nftstorage.link
 *.developer.app
 noop.app
 *.northflank.app
 *.build.run
 *.code.run
@@ -9123,37 +9079,33 @@
 123hjemmeside.dk
 123hjemmeside.no
 123homepage.it
 123kotisivu.fi
 123minsida.se
 123miweb.es
 123paginaweb.pt
+123sait.ru
 123siteweb.fr
 123webseite.at
 123webseite.de
 123website.be
 123website.ch
 123website.lu
 123website.nl
 service.one
 simplesite.com
 simplesite.com.br
 simplesite.gr
 simplesite.pl
 nid.io
-is-cool.dev
-is-not-a.dev
-localplayer.dev
-is-local.org
 opensocial.site
 opencraft.hosting
 orsites.com
 operaunite.com
 tech.orange
-can.re
 authgear-staging.com
 authgearapps.com
 skygearapp.com
 outsystemscloud.com
 *.webpaas.ovh.net
 *.hosting.ovh.net
 ownprovider.com
@@ -9161,22 +9113,18 @@
 *.owo.codes
 ox.rs
 oy.lc
 pgfog.com
 pagefrontapp.com
 pagexl.com
 *.paywhirl.com
-*.xmit.co
 bar0.net
 bar1.net
 bar2.net
 rdv.to
-srv.us
-gh.srv.us
-gl.srv.us
 art.pl
 gliwice.pl
 krakow.pl
 poznan.pl
 wroc.pl
 zakopane.pl
 pantheonsite.io
@@ -9381,15 +9329,14 @@
 scalebook.scw.cloud
 smartlabeling.scw.cloud
 dedibox.fr
 schokokeks.net
 gov.scot
 service.gov.scot
 scrysec.com
-client.scrypted.io
 firewall-gateway.com
 firewall-gateway.de
 my-gateway.de
 my-router.de
 spdns.de
 spdns.eu
 firewall-gateway.net
@@ -9429,23 +9376,20 @@
 medecin.fr
 notaires.fr
 pharmacien.fr
 port.fr
 veterinaire.fr
 small-web.org
 vp4.me
-*.snowflake.app
-*.privatelink.snowflake.app
+snowflake.app
+privatelink.snowflake.app
 streamlit.app
 streamlitapp.com
 try-snowplow.com
 srht.site
-w-corp-staticblitz.com
-w-credentialless-staticblitz.com
-w-staticblitz.com
 stackhero-network.com
 runs.onstackit.cloud
 stackit.gg
 stackit.rocks
 stackit.run
 stackit.zone
 musician.io
@@ -9604,15 +9548,14 @@
 uber.space
 *.uberspace.de
 hk.com
 hk.org
 ltd.hk
 inc.hk
 it.com
-unison-services.cloud
 name.pm
 sch.tf
 biz.wf
 sch.wf
 org.yt
 virtualuser.de
 virtual-user.de
@@ -9671,15 +9614,14 @@
 webflow.io
 webflowtest.io
 *.webhare.dev
 reserve-online.net
 reserve-online.com
 bookonline.app
 hotelwithflight.com
-*.wadl.top
 wedeploy.io
 wedeploy.me
 wedeploy.sh
 remotewd.com
 pages.wiardweb.com
 wmflabs.org
 toolforge.org
```

### Comparing `psl-2024.4.15/psl.egg-info/PKG-INFO` & `psl-2024.4.8/psl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.4.15
+Version: 2024.4.8
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.4.15/setup.py` & `psl-2024.4.8/setup.py`

 * *Files identical despite different names*

