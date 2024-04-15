# Comparing `tmp/ActiveCollab-2.tar.gz` & `tmp/activecollab-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ActiveCollab-2.tar", last modified: Thu Apr 11 09:47:53 2024, max compression
+gzip compressed data, was "activecollab-2.1.tar", last modified: Mon Apr 15 03:35:35 2024, max compression
```

## Comparing `ActiveCollab-2.tar` & `activecollab-2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:47:53.976348 ActiveCollab-2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:47:53.972348 ActiveCollab-2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:47:53.972348 ActiveCollab-2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-11 09:47:46.000000 ActiveCollab-2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 09:47:46.000000 ActiveCollab-2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:47:53.972348 ActiveCollab-2/ActiveCollab/
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-04-11 09:47:46.000000 ActiveCollab-2/ActiveCollab/ActiveCollab.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 09:47:46.000000 ActiveCollab-2/ActiveCollab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:47:53.972348 ActiveCollab-2/ActiveCollab/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-11 09:47:46.000000 ActiveCollab-2/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:47:53.976348 ActiveCollab-2/ActiveCollab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-11 09:47:53.000000 ActiveCollab-2/ActiveCollab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-11 09:47:53.000000 ActiveCollab-2/ActiveCollab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:47:53.000000 ActiveCollab-2/ActiveCollab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 09:47:53.000000 ActiveCollab-2/ActiveCollab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 09:47:53.000000 ActiveCollab-2/ActiveCollab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-11 09:47:46.000000 ActiveCollab-2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-11 09:47:53.976348 ActiveCollab-2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-11 09:47:46.000000 ActiveCollab-2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-11 09:47:46.000000 ActiveCollab-2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:47:53.976348 ActiveCollab-2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 09:47:46.000000 ActiveCollab-2/setup.py_bck
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:35:35.929556 activecollab-2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:35:35.929556 activecollab-2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:35:35.929556 activecollab-2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-15 03:35:30.000000 activecollab-2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 03:35:30.000000 activecollab-2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:35:35.929556 activecollab-2.1/ActiveCollab/
+-rw-r--r--   0 runner    (1001) docker     (127)    13031 2024-04-15 03:35:30.000000 activecollab-2.1/ActiveCollab/ActiveCollab.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 03:35:30.000000 activecollab-2.1/ActiveCollab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:35:35.929556 activecollab-2.1/ActiveCollab/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-15 03:35:30.000000 activecollab-2.1/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:35:35.929556 activecollab-2.1/ActiveCollab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-15 03:35:35.000000 activecollab-2.1/ActiveCollab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-15 03:35:35.000000 activecollab-2.1/ActiveCollab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:35:35.000000 activecollab-2.1/ActiveCollab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 03:35:35.000000 activecollab-2.1/ActiveCollab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 03:35:35.000000 activecollab-2.1/ActiveCollab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 03:35:30.000000 activecollab-2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-15 03:35:35.929556 activecollab-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-15 03:35:30.000000 activecollab-2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 03:35:30.000000 activecollab-2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 03:35:35.929556 activecollab-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-15 03:35:30.000000 activecollab-2.1/setup.py_bck
```

### Comparing `ActiveCollab-2/.github/workflows/publish.yml` & `activecollab-2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ActiveCollab-2/ActiveCollab/ActiveCollab.py` & `activecollab-2.1/ActiveCollab/ActiveCollab.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         ]
         for option in options:
             chrome_options.add_argument(option)
 
         driver = webdriver.Chrome(service=chrome_service , options=chrome_options)
         self.wait_30 = WebDriverWait(driver , 30)
         self.wait_10 = WebDriverWait(driver , 10)
-        self.wait_5 = WebDriverWait(driver , 5)
+        self.wait_2 = WebDriverWait(driver , 2)
         driver.get(host_url)
         time.sleep(5)
 
         try:
             if self.wait_10.until(EC.presence_of_element_located(
                     (By.XPATH , '//*[@id="projects"]/div/div/h1'))).text == 'Sign in to ActiveCollab':
                 self.driver = driver
@@ -66,21 +66,21 @@
 
     def list_projects(self):
         """
         :return: list of all projects you have with their project number
         """
         self.driver.get(f'{self.host_url}/projects')
         try:
-            if self.wait_5.until(EC.presence_of_element_located(
+            if self.wait_2.until(EC.presence_of_element_located(
                     (By.XPATH , '//*[@id="projects"]/div/div/h1'))).text == 'Sign in to ActiveCollab':
                 print('You are not logged in')
         except:
             pass
         try:
-            if self.wait_5.until(EC.presence_of_element_located(
+            if self.wait_2.until(EC.presence_of_element_located(
                     (By.XPATH , '//*[@id="main_message_inner"]/span'))).text:
                 print(self.driver.find_element(By.XPATH,value='//*[@id="main_message_inner"]/span').text)
         except:
             pass
         project_list = {}
         time.sleep(2)
         all_projects = self.driver.find_elements(By.CLASS_NAME , value="list-item")
@@ -93,21 +93,21 @@
 
     def list_users(self):
         """
         :return: list of all users
         """
         self.driver.get(f'{self.host_url}/people')
         try:
-            if self.wait_5.until(EC.presence_of_element_located(
+            if self.wait_2.until(EC.presence_of_element_located(
                     (By.XPATH , '//*[@id="projects"]/div/div/h1'))).text == 'Sign in to ActiveCollab':
                 print('You are not logged in')
         except:
             pass
         try:
-            if self.wait_5.until(EC.presence_of_element_located(
+            if self.wait_2.until(EC.presence_of_element_located(
                     (By.XPATH , '//*[@id="main_message_inner"]/span'))).text:
                 print(self.driver.find_element(By.XPATH,value='//*[@id="main_message_inner"]/span').text)
         except:
             pass
         user_list = []
         time.sleep(2)
         all_users = self.driver.find_elements(By.CLASS_NAME , value="col_name")
@@ -122,21 +122,21 @@
     def list_users_in_project(self , project_id):
         """
         :param project_id: Project id you want to search user from
         :return: List of users in passed project id
         """
         self.driver.get(f'{self.host_url}/projects/{project_id}/members')
         try:
-            if self.wait_5.until(EC.presence_of_element_located(
+            if self.wait_2.until(EC.presence_of_element_located(
                     (By.XPATH , '//*[@id="projects"]/div/div/h1'))).text == 'Sign in to ActiveCollab':
                 print('You are not logged in')
         except:
             pass
         try:
-            if self.wait_5.until(EC.presence_of_element_located(
+            if self.wait_2.until(EC.presence_of_element_located(
                     (By.XPATH , '//*[@id="main_message_inner"]/span'))).text:
                 print(self.driver.find_element(By.XPATH,value='//*[@id="main_message_inner"]/span').text)
         except:
             pass
         users_list_in_project = {}
         time.sleep(2)
         all_users = self.driver.find_elements(By.CLASS_NAME,value="people_list_name")
@@ -147,25 +147,25 @@
         return users_list_in_project
 
     def add_user_in_project(self,project_id,user_name_or_user_email):
         """
 
         :param project_id: Project id in which you want to add the user
         :param user_name_or_user_email: User name or email that you want to add, Make sure to use full name to avoid
-        :return: User added OR something went wrong
+        :return: User added
         """
         self.driver.get(f'{self.host_url}/projects/{project_id}/members')
         try:
-            if self.wait_5.until(EC.presence_of_element_located(
+            if self.wait_2.until(EC.presence_of_element_located(
                     (By.XPATH , '//*[@id="projects"]/div/div/h1'))).text == 'Sign in to ActiveCollab':
                 print('You are not logged in')
         except:
             pass
         try:
-            if self.wait_5.until(EC.presence_of_element_located(
+            if self.wait_2.until(EC.presence_of_element_located(
                     (By.XPATH , '//*[@id="main_message_inner"]/span'))).text:
                 print(self.driver.find_element(By.XPATH,value='//*[@id="main_message_inner"]/span').text)
         except:
             pass
         current_member_count = self.driver.find_element(By.XPATH,value='//*[@id="project_people"]/div/div[2]/div/div/div/div[1]/h3').text.split(' (')[1].split(')')[0]
         print(current_member_count)
         try:
@@ -181,11 +181,98 @@
                 return print(f"User: {user_name_or_user_email} added in project {project_id}")
         except Exception as e:
             print('Something went wrong.')
             print(e)
             self.driver.close()
             self.driver.quit()
 
+    def add_note_in_project(self,project_id,note_title,note_content):
+        """
+        :param note_title: Title of your note
+        :param note_content: content of the note
+        :param project_id: Project id in which you want to add the user
+        :return: Notes added with note URL
+        """
+        self.driver.get(f'{self.host_url}/projects/{project_id}/notes/add')
+        try:
+            if self.wait_2.until(EC.presence_of_element_located(
+                    (By.XPATH , '//*[@id="projects"]/div/div/h1'))).text == 'Sign in to ActiveCollab':
+                print('You are not logged in')
+        except:
+            pass
+        try:
+            if self.wait_2.until(EC.presence_of_element_located(
+                    (By.XPATH , '//*[@id="main_message_inner"]/span'))).text:
+                print(self.driver.find_element(By.XPATH,value='//*[@id="main_message_inner"]/span').text)
+        except:
+            pass
+        try:
+            self.wait_2.until((EC.presence_of_element_located((By.XPATH,"//input[@placeholder='Title of the note']")))).send_keys(note_title)
+            # self.wait_10.until((EC.presence_of_element_located((By.XPATH,"//input[@placeholder='Title of the note']")))).send_keys(Keys.TAB)
+            # init = input('wait..')
+            self.wait_2.until((EC.presence_of_element_located((By.XPATH,'/html/body/div[1]/section/div/div/div/form/div/div/div/div[1]/div/div[2]/div/div[2]')))).send_keys(note_content)
+            self.wait_2.until((EC.presence_of_element_located((By.XPATH,"//button[@type='submit']")))).click()
+            if self.wait_10.until(EC.presence_of_element_located((By.CLASS_NAME,"project_object_location"))):
+                return print(f'Note created: {self.driver.current_url}')
+        except Exception as e:
+            print('Something went wrong.')
+            print(e)
+            self.driver.close()
+            self.driver.quit()
+
+
+    def add_task_in_project(self,project_id,task_title,task_description,task_assignee):
+
+        global task_id
+        self.driver.get(f'{self.host_url}/projects/{project_id}/')
+        try:
+            if self.wait_2.until(EC.presence_of_element_located(
+                    (By.XPATH , '//*[@id="projects"]/div/div/h1'))).text == 'Sign in to ActiveCollab':
+                print('You are not logged in')
+        except:
+            pass
+        try:
+            if self.wait_2.until(EC.presence_of_element_located(
+                    (By.XPATH , '//*[@id="main_message_inner"]/span'))).text:
+                print(self.driver.find_element(By.XPATH,value='//*[@id="main_message_inner"]/span').text)
+        except:
+            pass
+        try:
+            self.wait_10.until(EC.presence_of_element_located((By.CLASS_NAME,"SortableListItem")))
+            current_task_ids = self.driver.find_elements(By.CLASS_NAME,value="SortableListItem")
+            current_task_list = []
+            updated_task_list = []
+            for i in current_task_ids:
+                current_task_list.append(i.get_attribute('data-id'))
+            self.driver.find_elements(By.CLASS_NAME,value="add-icon")[0].click()
+            self.driver.find_element(By.XPATH,value="//input[@id='taskNameInput']").send_keys(task_title)
+            self.driver.find_element(By.CLASS_NAME,value="mce-content-body").send_keys(task_description)
+            self.driver.find_element(By.XPATH,value="//span[@class='slim_control_label on-focus']").click()
+            self.wait_2.until(EC.presence_of_element_located((By.XPATH,"//input[@placeholder='Choose an assignee']"))).send_keys(str(task_assignee).strip())
+            # time.sleep(0.2)
+            self.driver.find_element(By.XPATH,value="//input[@placeholder='Choose an assignee']").send_keys(Keys.ENTER)
+            self.driver.find_element(By.XPATH,value="//button[normalize-space()='Add Task']").click()
+            time.sleep(3)
+            updated_task_ids = self.driver.find_elements(By.CLASS_NAME,value="SortableListItem")
+            for i in updated_task_ids:
+                updated_task_list.append(i.get_attribute('data-id'))
+            if len(current_task_ids)<len(updated_task_ids):
+                for i in updated_task_list:
+                    if i not in current_task_list:
+                        task_id = i
+                return print(f"Task created: {self.host_url}/projects/{project_id}?modal=Task-{task_id}-{project_id}")
+            else:
+                return print('Task not created')
+        except Exception as e:
+            print('Something went wrong.')
+            print(e)
+            self.driver.close()
+            self.driver.quit()
+
+
+
+
+
```

### Comparing `ActiveCollab-2/ActiveCollab.egg-info/PKG-INFO` & `activecollab-2.1/ActiveCollab.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 2
+Version: 2.1
 Summary: A Python module to interact with ActiveCollab and perform certain actions
 Author-email: Ankushtpss <ankushkumartpss@gmail.com>
 Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
 Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,55 +16,67 @@
 
 # ActiveCollab
 
 ## Overview
 This project aims to build a headless interaction with your active collab using Selenium WebDriver.
 
 
+## Download stats
+[![Downloads](https://static.pepy.tech/badge/ActiveCollab)](https://pepy.tech/project/ActiveCollab) <br>
+[![Downloads](https://static.pepy.tech/badge/ActiveCollab/week)](https://pepy.tech/project/ActiveCollab) <br>
+[![Downloads](https://static.pepy.tech/badge/ActiveCollab/month)](https://pepy.tech/project/ActiveCollab)
+
+
 ## Installation
 
 ```console
 pip install ActiveCollab
 ```
-
 whatsapp-auto officially supports Python 3.8+.
 
 ## Usage
 
 ### Default
-
 ```python
 import ActiveCollab
 
 host_url = 'host_url' # Active Collab hosted URL  
 
 user_name = 'your_username_or_email' # Active Collab username or email
 
 password = 'your_password' # Active Collab Password
 
 ac = ActiveCollab.Connect(host_url,user_name,password)  # Login to Active Collab
 ```
 
 
-### List all projects
 
+### List all projects
 ```python
 ac.list_projects()  # List out all project assigned to logged in user
 ```
 
 ### List all users
-
 ```python
 ac.list_users()  # List out all users in your organization with id, name and email
 ```
 
-### List users in a project
-
+### List Users in a Project
 ```python
 ac.list_users_in_project(project_id)  # List out all users in the project (project_id)
 ```
 
-### add user in a project
-
+### + Add User in a Project
 ```python
 ac.add_user_in_project(project_id,user_name_or_user_email)  # Add user in provided project_id
 ```
+
+
+### + Add Task in a Project
+```python
+ac.add_task_in_project(project_id,task_title,task_description,task_assignee)  # Add task in the provided project_id
+```
+
+### + Add Note in a Project
+```python
+ac.add_note_in_project(project_id,note_title,note_content)  # Add note in the provided project_id
+```
```

### Comparing `ActiveCollab-2/LICENSE` & `activecollab-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ActiveCollab-2/PKG-INFO` & `activecollab-2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 2
+Version: 2.1
 Summary: A Python module to interact with ActiveCollab and perform certain actions
 Author-email: Ankushtpss <ankushkumartpss@gmail.com>
 Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
 Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,55 +16,67 @@
 
 # ActiveCollab
 
 ## Overview
 This project aims to build a headless interaction with your active collab using Selenium WebDriver.
 
 
+## Download stats
+[![Downloads](https://static.pepy.tech/badge/ActiveCollab)](https://pepy.tech/project/ActiveCollab) <br>
+[![Downloads](https://static.pepy.tech/badge/ActiveCollab/week)](https://pepy.tech/project/ActiveCollab) <br>
+[![Downloads](https://static.pepy.tech/badge/ActiveCollab/month)](https://pepy.tech/project/ActiveCollab)
+
+
 ## Installation
 
 ```console
 pip install ActiveCollab
 ```
-
 whatsapp-auto officially supports Python 3.8+.
 
 ## Usage
 
 ### Default
-
 ```python
 import ActiveCollab
 
 host_url = 'host_url' # Active Collab hosted URL  
 
 user_name = 'your_username_or_email' # Active Collab username or email
 
 password = 'your_password' # Active Collab Password
 
 ac = ActiveCollab.Connect(host_url,user_name,password)  # Login to Active Collab
 ```
 
 
-### List all projects
 
+### List all projects
 ```python
 ac.list_projects()  # List out all project assigned to logged in user
 ```
 
 ### List all users
-
 ```python
 ac.list_users()  # List out all users in your organization with id, name and email
 ```
 
-### List users in a project
-
+### List Users in a Project
 ```python
 ac.list_users_in_project(project_id)  # List out all users in the project (project_id)
 ```
 
-### add user in a project
-
+### + Add User in a Project
 ```python
 ac.add_user_in_project(project_id,user_name_or_user_email)  # Add user in provided project_id
 ```
+
+
+### + Add Task in a Project
+```python
+ac.add_task_in_project(project_id,task_title,task_description,task_assignee)  # Add task in the provided project_id
+```
+
+### + Add Note in a Project
+```python
+ac.add_note_in_project(project_id,note_title,note_content)  # Add note in the provided project_id
+```
```

### Comparing `ActiveCollab-2/pyproject.toml` & `activecollab-2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 dependencies = [
     "selenium",
     "webdriver_manager",
 ]
 
-version = "2"
+version = "2.1"
 
 [tool.setuptools_scm]
 
 [project.urls]
 "Homepage" = "https://github.com/Ankushtpss/ActiveCollab"
 "Bug Tracker" = "https://github.com/Ankushtpss/ActiveCollab/issues"
```

### Comparing `ActiveCollab-2/setup.py_bck` & `activecollab-2.1/setup.py_bck`

 * *Files identical despite different names*

