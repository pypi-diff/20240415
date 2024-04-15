# Comparing `tmp/shippo-3.2.3.tar.gz` & `tmp/shippo-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.2.3.tar", last modified: Fri Apr 12 18:13:47 2024, max compression
+gzip compressed data, was "shippo-3.2.4.tar", last modified: Mon Apr 15 16:54:49 2024, max compression
```

## Comparing `shippo-3.2.3.tar` & `shippo-3.2.4.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.554701 shippo-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-12 18:13:47.554701 shippo-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-12 18:13:35.000000 shippo-3.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:13:47.554701 shippo-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-12 18:13:35.000000 shippo-3.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.514701 shippo-3.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.522701 shippo-3.2.3/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.522701 shippo-3.2.3/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    28983 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.522701 shippo-3.2.3/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.542701 shippo-3.2.3/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountfedexcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrieraccountwithextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/carriers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/connectexistingownupsaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/distanceunit.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/instanttransactionrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/labelfiletype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/objectstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegrouptype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    41991 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/components/weightunit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.542701 shippo-3.2.3/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/badrequestwithdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/badrequestwitherror.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.542701 shippo-3.2.3/src/shippo/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.554701 shippo-3.2.3/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15887 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.554701 shippo-3.2.3/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-12 18:13:35.000000 shippo-3.2.3/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:47.522701 shippo-3.2.3/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11400 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 18:13:47.000000 shippo-3.2.3/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.586234 shippo-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-15 16:54:49.586234 shippo-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-15 16:54:39.000000 shippo-3.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:54:49.586234 shippo-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-15 16:54:39.000000 shippo-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.550234 shippo-3.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.554234 shippo-3.2.4/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.554234 shippo-3.2.4/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28938 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.554234 shippo-3.2.4/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.574234 shippo-3.2.4/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountfedexcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/carriers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/connectexistingownaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/distanceunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/instanttransactionrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/labelfiletype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/objectstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegrouptype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41991 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/components/weightunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.574234 shippo-3.2.4/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/badrequestwithdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/badrequestwitherror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.574234 shippo-3.2.4/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.586234 shippo-3.2.4/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15887 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.586234 shippo-3.2.4/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-15 16:54:39.000000 shippo-3.2.4/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:54:49.554234 shippo-3.2.4/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 16:54:49.000000 shippo-3.2.4/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.2.3/PKG-INFO` & `shippo-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.3
+Version: 3.2.4
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.3/README.md` & `shippo-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/setup.py` & `shippo-3.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.2.3',
+    version='3.2.4',
     author='Shippo',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `shippo-3.2.3/src/shippo/_hooks/registration.py` & `shippo-3.2.4/src/shippo/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/_hooks/sdkhooks.py` & `shippo-3.2.4/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/_hooks/types.py` & `shippo-3.2.4/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/addresses.py` & `shippo-3.2.4/src/shippo/addresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/batches.py` & `shippo-3.2.4/src/shippo/batches.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/carrier_accounts.py` & `shippo-3.2.4/src/shippo/carrier_accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,22 +78,22 @@
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, shippo_api_version: Optional[str] = None, connect_existing_own_ups_account_request: Optional[components.ConnectExistingOwnUPSAccountRequest] = None) -> components.CarrierAccount:
+    def create(self, shippo_api_version: Optional[str] = None, connect_existing_own_account_request: Optional[components.ConnectExistingOwnAccountRequest] = None) -> components.CarrierAccount:
         r"""Create a new carrier account
         Creates a new carrier account or connects an existing carrier account to the Shippo account.
         """
         hook_ctx = HookContext(operation_id='CreateCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateCarrierAccountRequest(
             shippo_api_version=shippo_api_version,
-            connect_existing_own_ups_account_request=connect_existing_own_ups_account_request,
+            connect_existing_own_account_request=connect_existing_own_account_request,
         )
         
         _globals = operations.CreateCarrierAccountGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
@@ -102,15 +102,15 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCarrierAccountRequest, "connect_existing_own_ups_account_request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCarrierAccountRequest, "connect_existing_own_account_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
@@ -152,15 +152,15 @@
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, carrier_account_id: str, shippo_api_version: Optional[str] = None) -> components.CarrierAccountWithExtraInfo:
+    def get(self, carrier_account_id: str, shippo_api_version: Optional[str] = None) -> components.CarrierAccount:
         r"""Retrieve a carrier account
         Returns an existing carrier account using an object ID.
         """
         hook_ctx = HookContext(operation_id='GetCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetCarrierAccountRequest(
             carrier_account_id=carrier_account_id,
             shippo_api_version=shippo_api_version,
@@ -204,15 +204,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccountWithExtraInfo])
+                out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.2.3/src/shippo/carrier_parcel_templates.py` & `shippo-3.2.4/src/shippo/carrier_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/customs_declarations.py` & `shippo-3.2.4/src/shippo/customs_declarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/customs_items.py` & `shippo-3.2.4/src/shippo/customs_items.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/debug.py` & `shippo-3.2.4/src/shippo/debug.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/manifests.py` & `shippo-3.2.4/src/shippo/manifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/__init__.py` & `shippo-3.2.4/src/shippo/models/components/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from .carrieraccountupscreaterequest import *
 from .carrieraccountupscreaterequestparameters import *
 from .carrieraccountuspscreaterequest import *
 from .carrieraccountwithextrainfo import *
 from .carrierparceltemplate import *
 from .carriers import *
 from .cod import *
-from .connectexistingownupsaccountrequest import *
+from .connectexistingownaccountrequest import *
 from .customerreference import *
 from .customsdeclaration import *
 from .customsdeclarationcreaterequest import *
 from .customsdeclarationpaginatedlist import *
 from .customsexporteridentification import *
 from .customsinvoicedcharges import *
 from .customsitem import *
@@ -123,8 +123,8 @@
 from .upsconnectexistingownaccountparameters import *
 from .userparceltemplate import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
 from .weightunit import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","B13aFilingOption","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","Carriers","Cod","Code","ConnectExistingOwnUPSAccountRequest","ContentsType","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationCreateRequest","CustomsDeclarationCreateRequestB13aFilingOption","CustomsDeclarationCreateRequestContentsType","CustomsDeclarationCreateRequestEelPfc","CustomsDeclarationCreateRequestIncoterm","CustomsDeclarationCreateRequestNonDeliveryOption","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnit","DryIce","EelPfc","ErrorMessage","HTTPMetadata","Incoterm","InstantTransactionRequestBody","InstantTransactionRequestBodyLabelFileType","Insurance","InvoiceNumber","LabelFileType","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","NonDeliveryOption","ObjectInfo","ObjectResults","ObjectState","Order","OrderCreateRequest","OrderCreateRequestOrderStatus","OrderPaginatedList","OrderStatus","Parameters","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelObjectState","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustralia","ParcelTemplateCouriersPlease","ParcelTemplateDHLeCommerce","ParcelTemplateDPDUK","ParcelTemplateFedEx","ParcelTemplateUPS","ParcelTemplateUSPS","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupType","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostal","ServiceLevelAPG","ServiceLevelAirterra","ServiceLevelAramexAustralia","ServiceLevelAsendia","ServiceLevelAustraliaPost","ServiceLevelAxleHire","ServiceLevelBetterTrucks","ServiceLevelCDL","ServiceLevelCanadaPost","ServiceLevelChronopost","ServiceLevelColissimo","ServiceLevelCorreosEspana","ServiceLevelCouriersPlease","ServiceLevelDHLExpress","ServiceLevelDHLGermany","ServiceLevelDHLeCommerce","ServiceLevelDPDDE","ServiceLevelDPDUK","ServiceLevelDeutschePost","ServiceLevelEvriUK","ServiceLevelFedEx","ServiceLevelGLSUS","ServiceLevelGlobegistics","ServiceLevelLSO","ServiceLevelLasership","ServiceLevelMaergo","ServiceLevelMondialRelay","ServiceLevelOnTrac","ServiceLevelParcelforce","ServiceLevelPostItaliane","ServiceLevelPurolator","ServiceLevelRoyalMail","ServiceLevelSendle","ServiceLevelSwyft","ServiceLevelUDS","ServiceLevelUPS","ServiceLevelUSPS","ServiceLevelVeho","ServiceLevelePostGlobal","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnit"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","B13aFilingOption","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","Carriers","Cod","Code","ConnectExistingOwnAccountRequest","ContentsType","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationCreateRequest","CustomsDeclarationCreateRequestB13aFilingOption","CustomsDeclarationCreateRequestContentsType","CustomsDeclarationCreateRequestEelPfc","CustomsDeclarationCreateRequestIncoterm","CustomsDeclarationCreateRequestNonDeliveryOption","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnit","DryIce","EelPfc","ErrorMessage","HTTPMetadata","Incoterm","InstantTransactionRequestBody","InstantTransactionRequestBodyLabelFileType","Insurance","InvoiceNumber","LabelFileType","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","NonDeliveryOption","ObjectInfo","ObjectResults","ObjectState","Order","OrderCreateRequest","OrderCreateRequestOrderStatus","OrderPaginatedList","OrderStatus","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelObjectState","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustralia","ParcelTemplateCouriersPlease","ParcelTemplateDHLeCommerce","ParcelTemplateDPDUK","ParcelTemplateFedEx","ParcelTemplateUPS","ParcelTemplateUSPS","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupType","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostal","ServiceLevelAPG","ServiceLevelAirterra","ServiceLevelAramexAustralia","ServiceLevelAsendia","ServiceLevelAustraliaPost","ServiceLevelAxleHire","ServiceLevelBetterTrucks","ServiceLevelCDL","ServiceLevelCanadaPost","ServiceLevelChronopost","ServiceLevelColissimo","ServiceLevelCorreosEspana","ServiceLevelCouriersPlease","ServiceLevelDHLExpress","ServiceLevelDHLGermany","ServiceLevelDHLeCommerce","ServiceLevelDPDDE","ServiceLevelDPDUK","ServiceLevelDeutschePost","ServiceLevelEvriUK","ServiceLevelFedEx","ServiceLevelGLSUS","ServiceLevelGlobegistics","ServiceLevelLSO","ServiceLevelLasership","ServiceLevelMaergo","ServiceLevelMondialRelay","ServiceLevelOnTrac","ServiceLevelParcelforce","ServiceLevelPostItaliane","ServiceLevelPurolator","ServiceLevelRoyalMail","ServiceLevelSendle","ServiceLevelSwyft","ServiceLevelUDS","ServiceLevelUPS","ServiceLevelUSPS","ServiceLevelVeho","ServiceLevelePostGlobal","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnit"]
```

### Comparing `shippo-3.2.3/src/shippo/models/components/address.py` & `shippo-3.2.4/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/addressimporter.py` & `shippo-3.2.4/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.2.4/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.2.4/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/alcohol.py` & `shippo-3.2.4/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/batch.py` & `shippo-3.2.4/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/batchshipment.py` & `shippo-3.2.4/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.2.4/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/billing.py` & `shippo-3.2.4/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccount.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccount.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .carrieraccountservicelevel import CarrierAccountServiceLevel
+from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CarrierAccount:
     account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
     r"""Unique identifier of the account. Please check the <a href=\\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\\">carrier accounts tutorial</a>
@@ -20,19 +21,15 @@
     r"""Carrier token, see <a href=\\"#tag/Carriers\\">Carriers</a><br>
     Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for all supported carriers.
     """
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     r"""Determines whether the account is active. When creating a shipment, if no `carrier_accounts` are explicitly
     passed Shippo will query all carrier accounts that have this field set. By default, this is set to True.
     """
-    parameters: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
-    r"""An array of additional parameters for the account, such as e.g. password or token.
-    Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for the parameters per carrier.<br> 
-    To protect account information, this field will be masked in any API response.
-    """
+    parameters: Optional[Union[Dict[str, Any], UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
     carrier_name: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_name'), 'exclude': lambda f: f is None }})
     r"""Carrier name, see <a href=\\"#tag/Carriers\\">Carriers</a><br>"""
     is_shippo_account: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_shippo_account'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the carrier account object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountbase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CarrierAccountBase:
     account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
     r"""Unique identifier of the account. Please check the <a href=\\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\\">carrier accounts tutorial</a>
@@ -19,14 +20,10 @@
     r"""Carrier token, see <a href=\\"#tag/Carriers\\">Carriers</a><br>
     Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for all supported carriers.
     """
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     r"""Determines whether the account is active. When creating a shipment, if no `carrier_accounts` are explicitly
     passed Shippo will query all carrier accounts that have this field set. By default, this is set to True.
     """
-    parameters: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
-    r"""An array of additional parameters for the account, such as e.g. password or token.
-    Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for the parameters per carrier.<br> 
-    To protect account information, this field will be masked in any API response.
-    """
+    parameters: Optional[Union[Dict[str, Any], UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 
 
 @dataclasses.dataclass
-class Parameters:
+class CarrierAccountChronopostCreateRequestParameters:
     pass
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CarrierAccountChronopostCreateRequest:
     carrier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier') }})
-    parameters: Parameters = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters') }})
+    parameters: CarrierAccountChronopostCreateRequestParameters = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters') }})
```

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountfedexcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountfedexcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carrieraccountwithextrainfo.py` & `shippo-3.2.4/src/shippo/models/components/carrieraccountwithextrainfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .carrieraccountservicelevel import CarrierAccountServiceLevel
+from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 class CarrierAccountWithExtraInfoType(str, Enum):
     r"""Authentication method used by this account."""
     DEFAULT = 'default'
     OAUTH = 'oauth'
 
 class CarrierAccountWithExtraInfoStatus(str, Enum):
@@ -52,19 +53,15 @@
     r"""Carrier token, see <a href=\\"#tag/Carriers\\">Carriers</a><br>
     Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for all supported carriers.
     """
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     r"""Determines whether the account is active. When creating a shipment, if no `carrier_accounts` are explicitly
     passed Shippo will query all carrier accounts that have this field set. By default, this is set to True.
     """
-    parameters: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
-    r"""An array of additional parameters for the account, such as e.g. password or token.
-    Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for the parameters per carrier.<br> 
-    To protect account information, this field will be masked in any API response.
-    """
+    parameters: Optional[Union[Dict[str, Any], UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
     carrier_name: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_name'), 'exclude': lambda f: f is None }})
     r"""Carrier name, see <a href=\\"#tag/Carriers\\">Carriers</a><br>"""
     is_shippo_account: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_shippo_account'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the carrier account object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.3/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.2.4/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/carriers.py` & `shippo-3.2.4/src/shippo/models/components/carriers.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/cod.py` & `shippo-3.2.4/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/connectexistingownupsaccountrequest.py` & `shippo-3.2.4/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
+from .distanceunit import DistanceUnit
+from .weightunit import WeightUnit
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ConnectExistingOwnUPSAccountRequest:
-    account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
-    r"""This field is required as input to the API, but is not used for UPS. Use the empty string."""
-    active: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active') }})
-    parameters: UPSConnectExistingOwnAccountParameters = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters') }})
-    r"""An array of additional parameters for the account, such as e.g. password or token.
-    Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for the parameters per carrier.<br> 
-    To protect account information, this field will be masked in any API response.
-    """
-    carrier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier'), 'exclude': lambda f: f is None }})
-    metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
+class UserParcelTemplateUpdateRequest:
+    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    r"""The measure unit used for length, width and height."""
+    height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
+    r"""The height of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
+    length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
+    r"""The length of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    r"""The name of the User Parcel Template"""
+    width: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width') }})
+    r"""The width of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
+    weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
+    r"""The weight of the package, in units specified by the weight_unit attribute."""
+    weight_unit: Optional[WeightUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight_unit'), 'exclude': lambda f: f is None }})
+    r"""The unit used for weight."""
```

### Comparing `shippo-3.2.3/src/shippo/models/components/customerreference.py` & `shippo-3.2.4/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/customsdeclaration.py` & `shippo-3.2.4/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.2.4/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.2.4/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/customsitem.py` & `shippo-3.2.4/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/customsitembase.py` & `shippo-3.2.4/src/shippo/models/components/customsitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/customstaxidentification.py` & `shippo-3.2.4/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.2.4/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.2.4/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.2.4/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.2.4/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.2.4/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/departmentnumber.py` & `shippo-3.2.4/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/dryice.py` & `shippo-3.2.4/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/errormessage.py` & `shippo-3.2.4/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/httpmetadata.py` & `shippo-3.2.4/src/shippo/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/instanttransactionrequestbody.py` & `shippo-3.2.4/src/shippo/models/components/instanttransactionrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/insurance.py` & `shippo-3.2.4/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/invoicenumber.py` & `shippo-3.2.4/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/labelfiletype.py` & `shippo-3.2.4/src/shippo/models/components/labelfiletype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/lineitem.py` & `shippo-3.2.4/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/lineitembase.py` & `shippo-3.2.4/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/liverate.py` & `shippo-3.2.4/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/location.py` & `shippo-3.2.4/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/manifest.py` & `shippo-3.2.4/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/order.py` & `shippo-3.2.4/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/parcel.py` & `shippo-3.2.4/src/shippo/models/components/parcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/parcelcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/parcelextra.py` & `shippo-3.2.4/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/parcelinsurance.py` & `shippo-3.2.4/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/parcelrequest.py` & `shippo-3.2.4/src/shippo/models/components/parcelrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.2.4/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/pickup.py` & `shippo-3.2.4/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/pickupbase.py` & `shippo-3.2.4/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/ponumber.py` & `shippo-3.2.4/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/rate.py` & `shippo-3.2.4/src/shippo/models/components/rate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/ratemessage.py` & `shippo-3.2.4/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/refund.py` & `shippo-3.2.4/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/refundrequestbody.py` & `shippo-3.2.4/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/rmanumber.py` & `shippo-3.2.4/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/servicegroup.py` & `shippo-3.2.4/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.2.4/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/servicegrouptype.py` & `shippo-3.2.4/src/shippo/models/components/servicegrouptype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.2.4/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/servicelevel.py` & `shippo-3.2.4/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.2.4/src/shippo/models/components/servicelevelenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/shipment.py` & `shippo-3.2.4/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/shipmentextra.py` & `shippo-3.2.4/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/shippoaccount.py` & `shippo-3.2.4/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.2.4/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/track.py` & `shippo-3.2.4/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/trackingstatus.py` & `shippo-3.2.4/src/shippo/models/components/trackingstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.2.4/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.2.4/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/tracksrequest.py` & `shippo-3.2.4/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/transaction.py` & `shippo-3.2.4/src/shippo/models/components/transaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/transactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.2.4/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.2.4/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/userparceltemplate.py` & `shippo-3.2.4/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.2.4/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UserParcelTemplateUpdateRequest:
+class UserParcelTemplateWithoutCarrierTemplateCreateRequest:
     distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
     r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""The height of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""The length of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
```

### Comparing `shippo-3.2.3/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.2.4/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/errors/badrequestwithdetail.py` & `shippo-3.2.4/src/shippo/models/errors/badrequestwithdetail.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/errors/badrequestwitherror.py` & `shippo-3.2.4/src/shippo/models/errors/badrequestwitherror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/errors/initiateoauth2signin.py` & `shippo-3.2.4/src/shippo/models/errors/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/errors/sdkerror.py` & `shippo-3.2.4/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/__init__.py` & `shippo-3.2.4/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.2.4/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createaddress.py` & `shippo-3.2.4/src/shippo/models/operations/createaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createbatch.py` & `shippo-3.2.4/src/shippo/models/operations/createbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createcarrieraccount.py` & `shippo-3.2.4/src/shippo/models/operations/createcarrieraccount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import connectexistingownupsaccountrequest as components_connectexistingownupsaccountrequest
+from ...models.components import connectexistingownaccountrequest as components_connectexistingownaccountrequest
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateCarrierAccountGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
@@ -14,11 +14,11 @@
 
 
 
 @dataclasses.dataclass
 class CreateCarrierAccountRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    connect_existing_own_ups_account_request: Optional[components_connectexistingownupsaccountrequest.ConnectExistingOwnUPSAccountRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    connect_existing_own_account_request: Optional[components_connectexistingownaccountrequest.ConnectExistingOwnAccountRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Examples."""
```

### Comparing `shippo-3.2.3/src/shippo/models/operations/createcustomsdeclaration.py` & `shippo-3.2.4/src/shippo/models/operations/createcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createcustomsitem.py` & `shippo-3.2.4/src/shippo/models/operations/createcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createliverate.py` & `shippo-3.2.4/src/shippo/models/operations/createliverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createmanifest.py` & `shippo-3.2.4/src/shippo/models/operations/createmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createorder.py` & `shippo-3.2.4/src/shippo/models/operations/createorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createparcel.py` & `shippo-3.2.4/src/shippo/models/operations/createparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createpickup.py` & `shippo-3.2.4/src/shippo/models/operations/createpickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createrefund.py` & `shippo-3.2.4/src/shippo/models/operations/createrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createservicegroup.py` & `shippo-3.2.4/src/shippo/models/operations/createservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createshipment.py` & `shippo-3.2.4/src/shippo/models/operations/createshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createshippoaccount.py` & `shippo-3.2.4/src/shippo/models/operations/createshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createtrack.py` & `shippo-3.2.4/src/shippo/models/operations/createtrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createtransaction.py` & `shippo-3.2.4/src/shippo/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/createuserparceltemplate.py` & `shippo-3.2.4/src/shippo/models/operations/createuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.2.4/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.2.4/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.2.4/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getaddress.py` & `shippo-3.2.4/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getbatch.py` & `shippo-3.2.4/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.2.4/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.2.4/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.2.4/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.2.4/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.2.4/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getdefaultparceltemplate.py` & `shippo-3.2.4/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getmanifest.py` & `shippo-3.2.4/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getorder.py` & `shippo-3.2.4/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getparcel.py` & `shippo-3.2.4/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getrate.py` & `shippo-3.2.4/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getrefund.py` & `shippo-3.2.4/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getshipment.py` & `shippo-3.2.4/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.2.4/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/gettrack.py` & `shippo-3.2.4/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/gettransaction.py` & `shippo-3.2.4/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.2.4/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/initiateoauth2signin.py` & `shippo-3.2.4/src/shippo/models/operations/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listaddresses.py` & `shippo-3.2.4/src/shippo/models/operations/listparcels.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListAddressesGlobals:
+class ListParcelsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListAddressesRequest:
+class ListParcelsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.3/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.2.4/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.2.4/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.2.4/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 
 
 
 @dataclasses.dataclass
 class ListCustomsDeclarationsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100)"""
+    results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
+    r"""The number of results to return per page (max 100, default 5)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.3/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.2.4/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listmanifests.py` & `shippo-3.2.4/src/shippo/models/operations/listmanifests.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 
 
 
 @dataclasses.dataclass
 class ListManifestsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100)"""
+    results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
+    r"""The number of results to return per page (max 100, default 5)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.3/src/shippo/models/operations/listorders.py` & `shippo-3.2.4/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listparcels.py` & `shippo-3.2.4/src/shippo/models/operations/listshipments.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListParcelsGlobals:
+class ListShipmentsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListParcelsRequest:
+class ListShipmentsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.3/src/shippo/models/operations/listrefunds.py` & `shippo-3.2.4/src/shippo/models/operations/listrefunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listservicegroups.py` & `shippo-3.2.4/src/shippo/models/operations/listservicegroups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.2.4/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.2.4/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listshipments.py` & `shippo-3.2.4/src/shippo/models/operations/listshippoaccounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListShipmentsGlobals:
+class ListShippoAccountsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListShipmentsRequest:
+class ListShippoAccountsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.3/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.2.4/src/shippo/models/operations/listaddresses.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListShippoAccountsGlobals:
+class ListAddressesGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListShippoAccountsRequest:
+class ListAddressesRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100)"""
+    results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
+    r"""The number of results to return per page (max 100, default 5)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.3/src/shippo/models/operations/listtransactions.py` & `shippo-3.2.4/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/listuserparceltemplates.py` & `shippo-3.2.4/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/purchasebatch.py` & `shippo-3.2.4/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/registercarrieraccount.py` & `shippo-3.2.4/src/shippo/models/operations/registercarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.2.4/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.2.4/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/updatedefaultparceltemplate.py` & `shippo-3.2.4/src/shippo/models/operations/updatedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/updateservicegroup.py` & `shippo-3.2.4/src/shippo/models/operations/updateservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.2.4/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.2.4/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/models/operations/validateaddress.py` & `shippo-3.2.4/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/orders.py` & `shippo-3.2.4/src/shippo/orders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/parcels.py` & `shippo-3.2.4/src/shippo/parcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/pickups.py` & `shippo-3.2.4/src/shippo/pickups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/rates.py` & `shippo-3.2.4/src/shippo/rates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/rates_at_checkout.py` & `shippo-3.2.4/src/shippo/rates_at_checkout.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/refunds.py` & `shippo-3.2.4/src/shippo/refunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/sdk.py` & `shippo-3.2.4/src/shippo/sdk.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/sdkconfiguration.py` & `shippo-3.2.4/src/shippo/sdkconfiguration.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.2.3'
-    gen_version: str = '2.304.1'
-    user_agent: str = 'speakeasy-sdk/python 3.2.3 2.304.1 2018-02-08 shippo'
+    sdk_version: str = '3.2.4'
+    gen_version: str = '2.306.0'
+    user_agent: str = 'speakeasy-sdk/python 3.2.4 2.306.0 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `shippo-3.2.3/src/shippo/service_groups.py` & `shippo-3.2.4/src/shippo/service_groups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/shipments.py` & `shippo-3.2.4/src/shippo/shipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/shippo_accounts.py` & `shippo-3.2.4/src/shippo/shippo_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/tracking_status.py` & `shippo-3.2.4/src/shippo/tracking_status.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/transactions.py` & `shippo-3.2.4/src/shippo/transactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/user_parcel_templates.py` & `shippo-3.2.4/src/shippo/user_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/utils/retries.py` & `shippo-3.2.4/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo/utils/utils.py` & `shippo-3.2.4/src/shippo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.3/src/shippo.egg-info/PKG-INFO` & `shippo-3.2.4/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.3
+Version: 3.2.4
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.2.3/src/shippo.egg-info/SOURCES.txt` & `shippo-3.2.4/src/shippo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 src/shippo/models/components/carrieraccountupscreaterequest.py
 src/shippo/models/components/carrieraccountupscreaterequestparameters.py
 src/shippo/models/components/carrieraccountuspscreaterequest.py
 src/shippo/models/components/carrieraccountwithextrainfo.py
 src/shippo/models/components/carrierparceltemplate.py
 src/shippo/models/components/carriers.py
 src/shippo/models/components/cod.py
-src/shippo/models/components/connectexistingownupsaccountrequest.py
+src/shippo/models/components/connectexistingownaccountrequest.py
 src/shippo/models/components/customerreference.py
 src/shippo/models/components/customsdeclaration.py
 src/shippo/models/components/customsdeclarationcreaterequest.py
 src/shippo/models/components/customsdeclarationpaginatedlist.py
 src/shippo/models/components/customsexporteridentification.py
 src/shippo/models/components/customsinvoicedcharges.py
 src/shippo/models/components/customsitem.py
```

