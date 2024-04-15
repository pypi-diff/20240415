# Comparing `tmp/wowicache-1.0.8.tar.gz` & `tmp/wowicache-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowicache-1.0.8.tar", last modified: Mon Sep 25 07:07:10 2023, max compression
+gzip compressed data, was "wowicache-1.0.9.tar", last modified: Tue Oct 24 07:28:56 2023, max compression
```

## Comparing `wowicache-1.0.8.tar` & `wowicache-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-09-25 07:07:10.805142 wowicache-1.0.8/
--rw-rw-rw-   0        0        0    35818 2023-09-21 09:08:49.000000 wowicache-1.0.8/COPYING
--rw-rw-rw-   0        0        0    35818 2023-09-21 09:09:03.000000 wowicache-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1122 2023-09-25 07:07:10.804185 wowicache-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-09-25 07:07:10.805142 wowicache-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1861 2023-09-25 07:07:01.000000 wowicache-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-25 07:07:10.785141 wowicache-1.0.8/wowicache/
--rw-rw-rw-   0        0        0        0 2023-09-21 06:38:36.000000 wowicache-1.0.8/wowicache/__init__.py
--rw-rw-rw-   0        0        0        0 2023-09-21 08:10:13.000000 wowicache-1.0.8/wowicache/__main__.py
--rw-rw-rw-   0        0        0    18872 2023-09-21 09:56:43.000000 wowicache-1.0.8/wowicache/models.py
--rw-rw-rw-   0        0        0    19537 2023-09-25 07:07:01.000000 wowicache-1.0.8/wowicache/update_cache.py
-drwxrwxrwx   0        0        0        0 2023-09-25 07:07:10.803144 wowicache-1.0.8/wowicache.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-09-25 07:07:10.000000 wowicache-1.0.8/wowicache.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-09-25 07:07:10.000000 wowicache-1.0.8/wowicache.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-25 07:07:10.000000 wowicache-1.0.8/wowicache.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      383 2023-09-25 07:07:10.000000 wowicache-1.0.8/wowicache.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-09-25 07:07:10.000000 wowicache-1.0.8/wowicache.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-10-24 07:28:56.471509 wowicache-1.0.9/
+-rw-rw-rw-   0        0        0    35818 2023-09-21 09:08:49.000000 wowicache-1.0.9/COPYING
+-rw-rw-rw-   0        0        0    35818 2023-09-21 09:09:03.000000 wowicache-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-10-24 07:28:56.470509 wowicache-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-10-24 07:28:56.471509 wowicache-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1861 2023-10-24 07:27:35.000000 wowicache-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-24 07:28:56.462498 wowicache-1.0.9/wowicache/
+-rw-rw-rw-   0        0        0        0 2023-09-21 06:38:36.000000 wowicache-1.0.9/wowicache/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-09-21 08:10:13.000000 wowicache-1.0.9/wowicache/__main__.py
+-rw-rw-rw-   0        0        0    18872 2023-09-21 09:56:43.000000 wowicache-1.0.9/wowicache/models.py
+-rw-rw-rw-   0        0        0    20407 2023-10-24 07:27:12.000000 wowicache-1.0.9/wowicache/update_cache.py
+drwxrwxrwx   0        0        0        0 2023-10-24 07:28:56.469501 wowicache-1.0.9/wowicache.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-10-24 07:28:56.000000 wowicache-1.0.9/wowicache.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-10-24 07:28:56.000000 wowicache-1.0.9/wowicache.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-24 07:28:56.000000 wowicache-1.0.9/wowicache.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      383 2023-10-24 07:28:56.000000 wowicache-1.0.9/wowicache.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-10-24 07:28:56.000000 wowicache-1.0.9/wowicache.egg-info/top_level.txt
```

### Comparing `wowicache-1.0.8/COPYING` & `wowicache-1.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `wowicache-1.0.8/LICENSE` & `wowicache-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wowicache-1.0.8/PKG-INFO` & `wowicache-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowicache
-Version: 1.0.8
+Version: 1.0.9
 Summary: OPENWOWI Wowiport SQLAlchemy overlay
 Home-page: https://github.com/seb-bau/wowicache
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `wowicache-1.0.8/setup.py` & `wowicache-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wowicache',
-    version='1.0.8',
+    version='1.0.9',
     description='OPENWOWI Wowiport SQLAlchemy overlay',
     url='https://github.com/seb-bau/wowicache',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['wowicache'],
     install_requires=[
```

### Comparing `wowicache-1.0.8/wowicache/models.py` & `wowicache-1.0.9/wowicache/models.py`

 * *Files identical despite different names*

### Comparing `wowicache-1.0.8/wowicache/update_cache.py` & `wowicache-1.0.9/wowicache/update_cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,38 +97,45 @@
     session.query(UseUnit).delete()
     session.query(Building).delete()
     session.query(EconomicUnit).delete()
     session.query(District).delete()
     session.commit()
 
     if ENECONOMICUNITS in entities or ENBUILDINGS in entities:
+        sectioncount = 0
         districts = wowicon.get_districts()
         for entry in districts:
             new_entry = District(internal_id=entry.id_,
                                  name=entry.name)
             session.add(new_entry)
+            sectioncount += 1
         session.commit()
+        logger.info(f"Added {sectioncount} districts.")
 
     if ENECONOMICUNITS in entities:
+        sectioncount = 0
         economic_units = wowicon.get_economic_units(fetch_all=True)
         for entry in economic_units:
             district_id = entry.district.id_ if entry.district else None
             new_entry = EconomicUnit(internal_id=entry.id_,
                                      id_num=entry.id_num,
                                      company_id=entry.company_code.id_,
                                      name=entry.name,
                                      location=entry.location,
                                      construction_year=entry.construction_year,
                                      info=entry.info,
                                      owner_id=entry.owner.id_,
                                      district_id=district_id)
             session.add(new_entry)
+            sectioncount += 1
         session.commit()
+        logger.info(f"Added {sectioncount} economic units.")
 
     if ENBUILDINGS in entities:
+        sectioncount = 0
         buildings = wowicon.get_building_lands(fetch_all=True)
         for entry in buildings:
             district_id = entry.building.district.id_ if entry.building.district else None
             move_in_date = datetime.strptime(str(entry.building.move_in_date), "%Y-%m-%d") \
                 if entry.building.move_in_date else None
             entry_date = datetime.strptime(str(entry.entry_date), "%Y-%m-%d") \
                 if entry.entry_date else None
@@ -149,17 +156,20 @@
                                  house_number_complete=entry.estate_address.house_number_complete,
                                  construction_year=entry.building.construction_year,
                                  move_in_date=move_in_date,
                                  building_type_id=entry.building.building_type.id_,
                                  building_type_name=entry.building.building_type.name,
                                  district_id=district_id)
             session.add(new_entry)
+            sectioncount += 1
         session.commit()
+        logger.info(f"Added {sectioncount} buildings.")
 
     if ENUSEUNITS in entities:
+        sectioncount = 0
         use_units = wowicon.get_use_units(fetch_all=True)
         for entry in use_units:
             move_in_date = datetime.strptime(str(entry.move_in_date), "%Y-%m-%d") \
                 if entry.move_in_date else None
             entry_date = datetime.strptime(str(entry.entry_date), "%Y-%m-%d") \
                 if entry.entry_date else None
             exit_date = datetime.strptime(str(entry.exit_date), "%Y-%m-%d") \
@@ -208,21 +218,24 @@
                                 exit_date=exit_date,
                                 position_id=position_id,
                                 position=position,
                                 floor_id=floor_id,
                                 floor_name=floor_name,
                                 floor_level=floor_level)
             session.add(new_entry)
+            sectioncount += 1
         session.commit()
+        logger.info(f"Added {sectioncount} use units.")
 
     # Für Contractors benötigen wir auch Personen
     if ENCONTRACTORS in entities and ENPERSONS not in entities:
         entities.append(ENPERSONS)
 
     if ENPERSONS in entities:
+        sectioncount = 0
         persons = wowicon.get_persons(fetch_all=True)
         for entry in persons:
             valid_from = datetime.strptime(str(entry.valid_from), "%Y-%m-%d") \
                 if entry.valid_from else None
             valid_to = datetime.strptime(str(entry.valid_to), "%Y-%m-%d") \
                 if entry.valid_to else None
             birth_date = datetime.strptime(str(entry.natural_person.birth_date), "%Y-%m-%d") \
@@ -243,14 +256,15 @@
                                 commercial_register_town=entry.legal_person.commercial_register_town,
                                 first_name=entry.natural_person.first_name,
                                 last_name=entry.natural_person.last_name,
                                 birth_date=birth_date,
                                 gender_id=gender_id,
                                 gender_name=gender_name)
             session.add(new_person)
+            sectioncount += 1
 
             if entry.addresses is not None:
                 for address_entry in entry.addresses:
                     address_valid_from = datetime.strptime(str(address_entry.valid_from), "%Y-%m-%d") \
                         if address_entry.valid_from else None
                     address_valid_to = datetime.strptime(str(address_entry.valid_to), "%Y-%m-%d") \
                         if address_entry.valid_to else None
@@ -292,20 +306,22 @@
                                              content=comm_entry.content,
                                              explanation=comm_entry.explanation,
                                              communication_type_id=comm_entry.communication_type.id_,
                                              communication_type=comm_entry.communication_type.name,
                                              person_id=new_person.internal_id)
                     session.add(new_comm)
         session.commit()
+        logger.info(f"Added {sectioncount} persons.")
 
     # Für Contractors brauchen wir auch Contracts
     if ENCONTRACTORS in entities and ENCONTRACTS not in entities:
         entities.append(ENCONTRACTS)
 
     if ENCONTRACTS in entities:
+        sectioncount = 0
         contracts = wowicon.get_license_agreements(fetch_all=True)
         for entry in contracts:
             contract_start = datetime.strptime(str(entry.start_contract), "%Y-%m-%d") \
                 if entry.start_contract else None
             contract_end = datetime.strptime(str(entry.end_of_contract), "%Y-%m-%d") \
                 if entry.end_of_contract else None
             new_entry = Contract(internal_id=entry.id_,
@@ -317,17 +333,20 @@
                                  status_id=entry.status_contract.id_,
                                  status_name=entry.status_contract.name,
                                  life_id=entry.life_of_contract.id_,
                                  life_name=entry.life_of_contract.name,
                                  contract_start=contract_start,
                                  contract_end=contract_end)
             session.add(new_entry)
+            sectioncount += 1
         session.commit()
+        logger.info(f"Added {sectioncount} contracts.")
 
     if ENCONTRACTORS in entities:
+        sectioncount = 0
         contractors = wowicon.get_contractors(fetch_all=True)
         for entry in contractors:
             # end_contract = datetime.strptime(str(entry.end_of_contract), "%Y-%m-%d") \
             #     if entry.end_of_contract else None
             # if end_contract is not None:
             #     print(f"ID: {entry.id_}")
             #     # print(end_contract)
@@ -347,19 +366,23 @@
                                    type_id=entry.contractor_type.id_,
                                    type_name=entry.contractor_type.name,
                                    valid_from=valid_from,
                                    valid_to=valid_to)
             try:
                 session.add(new_entry)
                 session.commit()
+                sectioncount += 1
             except sqlalchemy.exc.IntegrityError:
-                print("Rolling back...")
+                logger.warning(f"Rolling back contractor")
                 session.rollback()
 
+        logger.info(f"Added {sectioncount} contractors.")
+
     session.close()
+    logger.info("Cache update complete.")
 
 
 if __name__ == '__main__':
     if len(sys.argv) < 2:
         print("Missing env-File argument")
         exit()
```

### Comparing `wowicache-1.0.8/wowicache.egg-info/PKG-INFO` & `wowicache-1.0.9/wowicache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowicache
-Version: 1.0.8
+Version: 1.0.9
 Summary: OPENWOWI Wowiport SQLAlchemy overlay
 Home-page: https://github.com/seb-bau/wowicache
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

