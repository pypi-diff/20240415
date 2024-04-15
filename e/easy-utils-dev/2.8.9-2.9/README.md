# Comparing `tmp/easy_utils_dev-2.8.9.tar.gz` & `tmp/easy_utils_dev-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.8.9.tar", last modified: Fri Apr  5 14:49:27 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.9.tar", last modified: Mon Apr 15 06:13:06 2024, max compression
```

## Comparing `easy_utils_dev-2.8.9.tar` & `easy_utils_dev-2.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:49:27.861501 easy_utils_dev-2.8.9/
--rw-rw-rw-   0        0        0      174 2024-04-05 14:49:27.856618 easy_utils_dev-2.8.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 14:49:27.788974 easy_utils_dev-2.8.9/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.8.9/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.8.9/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      367 2024-04-05 13:43:02.000000 easy_utils_dev-2.8.9/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.8.9/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.8.9/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.8.9/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7180 2024-04-05 14:49:15.000000 easy_utils_dev-2.8.9/easy_utils_dev/keycloakapi.py
--rw-rw-rw-   0        0        0     7829 2024-04-05 13:44:11.000000 easy_utils_dev-2.8.9/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.8.9/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.8.9/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.8.9/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.8.9/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.8.9/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.8.9/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.8.9/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:49:27.850760 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      174 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-05 14:49:27.000000 easy_utils_dev-2.8.9/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 14:49:27.861501 easy_utils_dev-2.8.9/setup.cfg
--rw-rw-rw-   0        0        0      317 2024-04-05 14:49:23.000000 easy_utils_dev-2.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:13:06.959288 easy_utils_dev-2.9/
+-rw-rw-rw-   0        0        0      172 2024-04-15 06:13:06.953223 easy_utils_dev-2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 06:13:06.885606 easy_utils_dev-2.9/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.9/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0    15032 2024-04-07 14:58:42.000000 easy_utils_dev-2.9/easy_utils_dev/cplib.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     7412 2024-04-15 06:10:21.000000 easy_utils_dev-2.9/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.9/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     3144 2024-04-15 05:45:40.000000 easy_utils_dev-2.9/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:13:06.948120 easy_utils_dev-2.9/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      172 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 06:13:06.959722 easy_utils_dev-2.9/setup.cfg
+-rw-rw-rw-   0        0        0      315 2024-04-15 06:13:03.000000 easy_utils_dev-2.9/setup.py
```

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.9/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/Events.py` & `easy_utils_dev-2.9/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.9/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.9/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/keycloakapi.py` & `easy_utils_dev-2.9/easy_utils_dev/keycloakapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         self.logger.info(f'Authentication response code={response.status_code}')
         self.logger.debug(f'raw response in authentication {response.text}')
         if response.status_code != 200 :
             self.logger.error(f'Authentication failed. status_code={response.status_code} {response.text}')
             raise Exception(f'Authentication Failure {response.status_code}')
         response = response.json()
         self.accessToken = response['access_token']
-        self.refreshToken = response['refresh_token']
         self.bearertoken = f"Bearer {self.accessToken}"
         if autoRefresh :
             self.logger.debug(f'auto refresh is enabled. starting auto refresh thread ..')
             t = Thread( target=self.autoRefreshToken )
             t.start()
         self.logger.debug(f'returning access token {self.accessToken}')
         return self.accessToken
@@ -106,15 +105,15 @@
         _h.update(headers)
         return _h
 
     def logout(self,userId) :
         self.logger.info('Starting to logout form KeyCloack platform ..')
         url = f'{self.baseUrl}/admin/realms/heroes/users/{userId}/logout'
         self.logger.info(f"Authentication Params: username={self.username}.")
-        payload = {'refreshToken' : self.refreshToken }
+        payload = {'refreshToken' : self.accessToken }
         headers = self.getHeaders()
         self.logger.debug(f'Logout out headers {headers}')
         self.logger.debug(f'Logout out payload {payload}')
         response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
         self.logger.debug(f'raw response in logout {response.text}')
         self.logger.info(f'Logout status code={response.status_code}')
 
@@ -131,27 +130,29 @@
             self.users = response.json()
             return self.users
         else :
             self.logger.error(f'Error getting users  {response.text}')
             self.logger.debug(f'response is not 200 , return empty array')
             self.users = []
             return []
+        
 
     def updateUser(self , user ) :
         userId=user.get('id')
         username=user.get('username')
         self.logger.info(f"Update user in KeyCloack for userId={userId} username={username}")
         url= f"{self.baseUrl}/wavesuite/common/auth/admin/realms/wavesuite/users/{userId}"
         headers = self.getHeaders()
         self.logger.debug(f'update user headers = {headers}')
-        response = requests.put(url , headers=headers, body=json.dumps(user) , verify=False)
+        self.logger.debug(f'data user payload = {user}')
+        response = requests.put(url , headers=headers, data=json.dumps(user) , verify=False)
         self.logger.info(f'update Usr response code={response.status_code}')
         self.logger.debug(f'raw response in user update {response.text}')
         if response.status_code == 204 :
-            self.logger.debug(f'response is 204 , return the json as dict and filter on data ...')
+            self.logger.debug(f'response is 204 , return True as status...')
             return True
         else :
             self.logger.error(f'Error getting users  {response.text}')
             self.logger.debug(f'response is not 204. return False error={response.text}')
             return False
         
 if __name__ == '__main__':
```

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/lralib.py` & `easy_utils_dev-2.9/easy_utils_dev/wsselib.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,32 @@
 import requests , json , subprocess , time
 import urllib3
 from threading import Thread
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 version = '1.0 build 22032024'
 
-class LraLib :
-    def __init__(self, address,  user, password,port=8443 ,debug_name='lralib', token_refresh_period=1700 , client_id='wp-lra-service',client_secret='c74b4dfb-4293-46da-a38a-9fd46fce23b0' ) -> None:
-        '''
-        address: string
-        token_refresh_period number , string
-        password : string
-        port : int
-        debug_name : string
-        '''
+class SeLib :
+    def __init__(self, address,  user, password, tenantId,port=28443 ,debug_name='wsselib', token_refresh_period=30) -> None:
         self.logger = DEBUGGER(debug_name)
         self.address = address
         self.port = port
-        self.baseUrl = f'https://{self.address}:{self.port}'
-        self.username = user
-        self.password = password
+        self.baseUrl = f"https://{self.address}:{self.port}/wavesuite/se/api"
+        self.seUsername = user
+        self.sePassword = password
+        self.tenantId = tenantId
         self.users = []
         self.autoRefreshTokenPeriod = token_refresh_period
-        self.client_id=client_id
-        self.client_secret = client_secret
         self.baseUrl = self.updateBaseUrl(address , port )
 
     def set_debug_level(self , level ) :
         self.logger.set_level(level)    
 
     def updateBaseUrl( self, address, port ) :
-            self.baseUrl = f"https://{address}:{port}"
+            self.baseUrl = f"https://{address}:{port}/wavesuite/se/api"
             self.logger.debug(f'baseUrl={self.baseUrl}')
             self.address = address
             self.port = port
             return self.baseUrl
 
     def disableOnScreenDebugPrint( self ) :
         self.logger.disable_print()
@@ -44,42 +36,36 @@
     
     def enableOnScreenDebugPrint( self ) :
         self.logger.enable_print()
 
     def autoRefreshToken(self) :
         self.logger.info(f'Auto refresh token started. waiting for {self.autoRefreshTokenPeriod} refresh ...')
         time.sleep(self.autoRefreshTokenPeriod )
-        self.logout()
-        self.authentication()
+        self.seLogout()
+        self.seAuthentication()
         self.logger.info(f'Auto Token refresh completed.')
 
 
-    def authentication(self,autoRefresh=True) :
-        self.logger.info('Starting to authenticate with LRA platform ..')
-        url = f'{self.baseUrl}/wavesuite/common/auth/realms/wavesuite/protocol/openid-connect/token'
-        self.logger.info(f"Authentication Params: username={self.username} password=********")
-        self.logger.debug(f"Authentication Params: username={self.username} password={self.password} url={url}")
+    def seAuthentication(self,autoRefresh=True) :
+        self.logger.info('Starting to authenticate with service enablement platform ..')
+        url = f'{self.baseUrl}/v1/authentication/login'
+        self.logger.info(f"Authentication Params: username={self.seUsername}  tenantId={self.tenantId} password=********")
         payload = {
-            'grant_type': 'password',
-            'username': self.username ,
-            'password': self.password,
-            'client_id': self.client_id,
-            'client_secret': self.client_secret
+            'username' : self.seUsername ,
+            'password' : self.sePassword ,
+            'tenantId' : self.tenantId
         }
-        headers = {'Content-type': 'application/x-www-form-urlencoded' }
+        headers = {'Content-type': 'application/json'}
         self.logger.debug(f'Authentication Payload: {payload}')
-        response = requests.post(url , data=payload , headers=headers , verify=False)
+        response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
         self.logger.info(f'Authentication response code={response.status_code}')
         self.logger.debug(f'raw response in authentication {response.text}')
-        if response.status_code != 200 :
-            self.logger.error(f'Authentication failed. status_code={response.status_code} {response.text}')
-            raise Exception(f'Authentication Failure {response.status_code}')
         response = response.json()
-        self.accessToken = response['access_token']
-        self.refreshToken = response['refresh_token']
+        self.accessToken = response['data']['accessToken']
+        self.refreshToken = response['data']['refreshToken']
         if autoRefresh :
             self.logger.debug(f'auto refresh is enabled. starting auto refresh thread ..')
             t = Thread( target=self.autoRefreshToken )
             t.start()
         self.logger.debug(f'returning access token {self.accessToken}')
         return self.accessToken
         
@@ -91,93 +77,104 @@
     
     def getBearerToken(self) :
         return f"Bearer {self.accessToken}"
 
     def getAuthorizationToken(self) :
         return self.getBearerToken()
 
-    def getHeaders( self , headers={}, json=True ) :
-        _h = {'Authorization' : f"Bearer {self.accessToken}"}
-        self.logger.debug(f'request headers is {_h}')
-        if json :
-            self.logger.debug(f"json content type is Enabled. adding Content-type as application/json ")
-            _h.update({'Content-type': 'application/json'})
-        _h.update(headers)
-        return _h
-
-    def logout(self) :
-        self.logger.info('Starting to logout form LRA platform ..')
-        url = f'{self.baseUrl}/wavesuite/common/auth/realms/wavesuite/protocol/openid-connect/logout'
-        self.logger.info(f"Authentication Params: username={self.username}.")
+    def seLogout(self) :
+        self.logger.info('Starting to logout form service enablement platform ..')
+        url = f'{self.baseUrl}/v1/authentication/logout'
+        self.logger.info(f"Authentication Params: username={self.seUsername} tenantId={self.tenantId}")
         payload = {'refreshToken' : self.refreshToken }
-        headers = self.getHeaders()
+        headers = self.getRequestHeader()
         self.logger.debug(f'Logout out headers {headers}')
         self.logger.debug(f'Logout out payload {payload}')
         response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
         self.logger.debug(f'raw response in logout {response.text}')
         self.logger.info(f'Logout status code={response.status_code}')
 
+    def seUpdateUserGroup(self , user , group ) :
+        username = user.get('userName')
+        self.logger.info(f'Starting to update {username} with group {group} ...')
+        url= f"{self.baseUrl}/v1/tenants/users/{username}/update"
+        payload = {
+            'email' : user.get('email') ,
+            'externallyManaged' : True , 
+            'firstName' : user.get('firstName'),
+            'lastName' : user.get('lastName') ,
+            'roleName' : group 
+        }
+        self.logger.debug(f'Updating using form {payload}')
+        headers = self.getRequestHeader()
+        response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
+        self.logger.debug(f'raw response {response.text}')
+        self.logger.info(f'Update user {username} status code={response.status_code}')
+
+    def seDeleteUser(self , user ) :
+        username = user.get('userName')
+        self.logger.info(f'Starting to remove {username} ...')
+        url= f"{self.baseUrl}/v1/tenants/users/{username}"
+        headers = self.getRequestHeader()
+        response = requests.delete(url, headers=headers , verify=False)
+        self.logger.debug(f'raw response  {response.text}')
+        self.logger.info(f'remove user {username} status code={response.status_code}')
+
+    def seLockUser(self , user ) :
+        username = user.get('userName')
+        self.logger.info(f'Starting to lock {username} ...')
+        url= f"{self.baseUrl}/v1/tenants/users/{username}/lock"
+        headers = self.getRequestHeader()
+        response = requests.post(url, headers=headers , verify=False)
+        self.logger.debug(f'raw response  {response.text}')
+        self.logger.info(f'lock user {username} status code={response.status_code}')
+
+    def seUnlockUser(self , user ) :
+        username = user.get('userName')
+        self.logger.info(f'Starting to unlock {username} ...')
+        url= f"{self.baseUrl}/v1/tenants/users/{username}/unlock"
+        headers = self.getRequestHeader()
+        response = requests.post(url, headers=headers , verify=False)
+        self.logger.debug(f'raw response {response.text}')
+        self.logger.info(f'unlock user {username} status code={response.status_code}')
+
+    def getRequestHeader( self , extra_header={}) :
+        headers = {'Content-type': 'application/json' , 'authorization': f"Bearer {self.accessToken}"}
+        headers.update(extra_header)
+        return headers
+
+    def getLicense(self) :
+        self.logger.info(f'Getting license information...')
+        url= f"{self.baseUrl}/v1/license"
+        headers = self.getRequestHeader()
+        response = requests.get(url, headers=headers , verify=False)
+        self.logger.debug(f'raw response {response.text}')
+        self.logger.info(f'requesting license status code={response.status_code}')
+        if response.status_code == 200 :
+            return response.json()
+        else :
+            return {}
+        
+
     def getUsers(self) :
-        self.logger.info(f"Get users from LRA ...")
-        url= f"{self.baseUrl}/lra-rest/users"
-        headers = self.getHeaders()
+        self.logger.info(f"Get users from SE ...")
+        url= f"{self.baseUrl}/v1/tenants/users"
+        headers = self.getRequestHeader()
         self.logger.debug(f'Get users headers = {headers}')
         response = requests.get(url , headers=headers , verify=False)
         self.logger.info(f'Get Usr response code={response.status_code}')
         self.logger.debug(f'raw response in authentication {response.text}')
         if response.status_code == 200 :
             self.logger.debug(f'response is 200 , return the json as dict and filter on data ...')
-            self.users = response.json().get('items')
+            self.users = response.json().get('data')
             return self.users
         else :
             self.logger.error(f'Error getting users  {response.text}')
             self.logger.debug(f'response is not 200 , return empty array')
             self.users = []
             return []
 
-    def createUser(self, user : dict , group ) :
-        username = user.get('userName')
-        self.logger.info(f'Starting to create {username}  with group {group} ...')
-        url= f"{self.baseUrl}/lra-rest/users"
-        self.logger.debug(f'creating user {username} using url {url} with POST')
-        if group == 'ROLE_ADMIN' :
-            lra_operatorRole = False 
-            adminRole  = True 
-            lra_viewerRole = False
-        elif group == 'ROLE_LRA_OPERATOR' :
-            lra_operatorRole = True 
-            adminRole  = False 
-            lra_viewerRole = False
-        elif group == 'ROLE_LRA_VIEWER' :
-            lra_operatorRole = False 
-            adminRole  = False 
-            lra_viewerRole = True
-        payload = {
-            'address' : '' ,
-            'adminRole' : adminRole ,
-            'contact' : '' ,
-            'email' : user.get('email') ,
-            'enabled' : True  ,
-            'disabled' : False ,
-            'localUser' : False , 
-            'loginAttemptLocked' : False,
-            'lra_operatorRole' : lra_operatorRole , 
-            'lra_viewerRole' : lra_viewerRole , 
-            'name' : user.get('name') ,
-            'phoneNumber' : '' ,
-            'roles' : [group] ,
-            'userSource' : False,
-            'username' : user.get('email') # yes this must be email.    
-        }
-        self.logger.debug(f'Creating {username} using form {payload}')
-        headers = self.getHeaders()
-        response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
-        self.logger.debug(f'raw response {response.text}')
-        self.logger.info(f'create user {username} status code={response.status_code}')
-        return response
-
-
 if __name__ == '__main__':
     pass
```

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.9/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.9/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.9/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.9/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/utils.py` & `easy_utils_dev-2.9/easy_utils_dev/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,8 +65,51 @@
     return path
 
 def getScriptDirInMachine(f= __file__):
     '''
     THis functions aims to return the script dir.
     '''
     return os.path.dirname(os.path.abspath(f))
-    
+
+
+
+def is_packed():
+    # Check if the script is running from an executable produced by PyInstaller
+    if getattr(sys, 'frozen', False):
+        return True
+    # Check if the 'bundle' directory exists
+    elif hasattr(sys, '_MEIPASS') and os.path.exists(os.path.join(sys._MEIPASS, 'bundle')):
+        return True
+    else:
+        return False
+
+def get_executable_path(file=__file__) :
+    if is_packed():
+        return os.path.dirname(os.path.realpath(sys.argv[0]))
+    return os.path.dirname(os.path.realpath(file))
+
+def isArgsEmpty(args) :
+    if True in args.__dict__.values() :
+        return False
+    else :
+        return True
+    
+def convert_bytes_to_mb(bytes_size,rounded=True):
+    """Convert bytes to megabytes (MB)."""
+    if rounded :
+        # print(f'''
+        # {bytes_size} =>>> {round(float(bytes_size))}
+        # ''')
+        return round(float(bytes_size / (1024 * 1024)))
+    return bytes_size / (1024 * 1024)
+
+def convert_bytes_to_kb(bytes_size,rounded=True):
+    """Convert bytes to kilobytes (KB)."""
+    if rounded :
+        return round(float(bytes_size / 1024))
+    return bytes_size / 1024
+
+def convert_mb_to_bytes(mb_size):
+    return mb_size * 1024 * 1024
+
+if __name__ == "__main__":
+    pass
```

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.9/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.9/easy_utils_dev/lralib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 
 from easy_utils_dev.debugger import DEBUGGER
 import requests , json , subprocess , time
 import urllib3
 from threading import Thread
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+from easy_utils_dev.cplib import *
 
 version = '1.0 build 22032024'
 
-class SeLib :
-    def __init__(self, address,  user, password, tenantId,port=28443 ,debug_name='wsselib', token_refresh_period=30) -> None:
+class LraLib :
+    def __init__(self, address,  user, password,port=8443 ,debug_name='lralib', token_refresh_period=1700 , client_id='wp-lra-service',client_secret='c74b4dfb-4293-46da-a38a-9fd46fce23b0' ) -> None:
+        '''
+        address: string
+        token_refresh_period number , string
+        password : string
+        port : int
+        debug_name : string
+        '''
         self.logger = DEBUGGER(debug_name)
         self.address = address
         self.port = port
-        self.baseUrl = f"https://{self.address}:{self.port}/wavesuite/se/api"
-        self.seUsername = user
-        self.sePassword = password
-        self.tenantId = tenantId
+        self.baseUrl = f'https://{self.address}:{self.port}'
+        self.username = user
+        self.password = password
         self.users = []
         self.autoRefreshTokenPeriod = token_refresh_period
+        self.client_id=client_id
+        self.client_secret = client_secret
         self.baseUrl = self.updateBaseUrl(address , port )
+        self.debug=False
 
     def set_debug_level(self , level ) :
-        self.logger.set_level(level)    
+        self.logger.set_level(level) 
+        self.debug = True
 
     def updateBaseUrl( self, address, port ) :
-            self.baseUrl = f"https://{address}:{port}/wavesuite/se/api"
+            self.baseUrl = f"https://{address}:{port}"
             self.logger.debug(f'baseUrl={self.baseUrl}')
             self.address = address
             self.port = port
             return self.baseUrl
 
     def disableOnScreenDebugPrint( self ) :
         self.logger.disable_print()
@@ -36,145 +47,146 @@
     
     def enableOnScreenDebugPrint( self ) :
         self.logger.enable_print()
 
     def autoRefreshToken(self) :
         self.logger.info(f'Auto refresh token started. waiting for {self.autoRefreshTokenPeriod} refresh ...')
         time.sleep(self.autoRefreshTokenPeriod )
-        self.seLogout()
-        self.seAuthentication()
+        self.logout()
+        self.authentication()
         self.logger.info(f'Auto Token refresh completed.')
 
 
-    def seAuthentication(self,autoRefresh=True) :
-        self.logger.info('Starting to authenticate with service enablement platform ..')
-        url = f'{self.baseUrl}/v1/authentication/login'
-        self.logger.info(f"Authentication Params: username={self.seUsername}  tenantId={self.tenantId} password=********")
-        payload = {
-            'username' : self.seUsername ,
-            'password' : self.sePassword ,
-            'tenantId' : self.tenantId
-        }
-        headers = {'Content-type': 'application/json'}
-        self.logger.debug(f'Authentication Payload: {payload}')
-        response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
-        self.logger.info(f'Authentication response code={response.status_code}')
-        self.logger.debug(f'raw response in authentication {response.text}')
-        response = response.json()
-        self.accessToken = response['data']['accessToken']
-        self.refreshToken = response['data']['refreshToken']
-        if autoRefresh :
-            self.logger.debug(f'auto refresh is enabled. starting auto refresh thread ..')
-            t = Thread( target=self.autoRefreshToken )
-            t.start()
-        self.logger.debug(f'returning access token {self.accessToken}')
-        return self.accessToken
+    def authentication(self,autoRefresh=True) :
+        self.logger.info('Starting to authenticate with LRA platform ..')
+        # url = f'{self.baseUrl}/wavesuite/common/auth/realms/wavesuite/protocol/openid-connect/token'
+        # self.logger.info(f"Authentication Params: username={self.username} password=********")
+        # self.logger.debug(f"Authentication Params: username={self.username} password={self.password} url={url}")
+        # payload = {
+        #     'grant_type': 'password',
+        #     'username': self.username ,
+        #     'password': self.password,
+        #     'client_id': self.client_id,
+        #     'client_secret': self.client_secret
+        # }
+        # headers = {'Content-type': 'application/x-www-form-urlencoded' }
+        # self.logger.debug(f'Authentication Payload: {payload}')
+        # response = requests.post(url , data=payload , headers=headers , verify=False)
+        # self.logger.info(f'Authentication response code={response.status_code}')
+        # self.logger.debug(f'raw response in authentication {response.text}')
+        # if response.status_code != 200 :
+        #     self.logger.error(f'Authentication failed. status_code={response.status_code} {response.text}')
+        #     raise Exception(f'Authentication Failure {response.status_code}')
+        # response = response.json()
+        # self.accessToken = response['access_token']
+        # self.refreshToken = response['refresh_token']
+        # if autoRefresh :
+        #     self.logger.debug(f'auto refresh is enabled. starting auto refresh thread ..')
+        #     t = Thread( target=self.autoRefreshToken )
+        #     t.start()
+        # self.logger.debug(f'returning access token {self.accessToken}')
+        self.cp = cp = CommonPlatformLib(
+            address=self.address,
+            port=self.port,
+            username=self.username,
+            password=self.password,
+            token_refresh_period=self.autoRefreshTokenPeriod,
+        )
+        if self.debug :
+            cp.logger.set_level('debug')
+        cp.authentication(autoRefresh=autoRefresh)
+        self.accessToken = cp.accessToken
+        self.refreshToken = cp.refreshToken
+        self.logger.info('Authenticate with LRA platform Completed')
+        return cp.accessToken
         
     def getAccessToken(self) :
         return self.accessToken
     
     def getRefreshToken(self) :
         return self.accessToken
     
     def getBearerToken(self) :
         return f"Bearer {self.accessToken}"
 
     def getAuthorizationToken(self) :
         return self.getBearerToken()
 
-    def seLogout(self) :
-        self.logger.info('Starting to logout form service enablement platform ..')
-        url = f'{self.baseUrl}/v1/authentication/logout'
-        self.logger.info(f"Authentication Params: username={self.seUsername} tenantId={self.tenantId}")
-        payload = {'refreshToken' : self.refreshToken }
-        headers = self.getRequestHeader()
-        self.logger.debug(f'Logout out headers {headers}')
-        self.logger.debug(f'Logout out payload {payload}')
-        response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
-        self.logger.debug(f'raw response in logout {response.text}')
-        self.logger.info(f'Logout status code={response.status_code}')
-
-    def seUpdateUserGroup(self , user , group ) :
-        username = user.get('userName')
-        self.logger.info(f'Starting to update {username} with group {group} ...')
-        url= f"{self.baseUrl}/v1/tenants/users/{username}/update"
-        payload = {
-            'email' : user.get('email') ,
-            'externallyManaged' : True , 
-            'firstName' : user.get('firstName'),
-            'lastName' : user.get('lastName') ,
-            'roleName' : group 
-        }
-        self.logger.debug(f'Updating using form {payload}')
-        headers = self.getRequestHeader()
-        response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
-        self.logger.debug(f'raw response {response.text}')
-        self.logger.info(f'Update user {username} status code={response.status_code}')
-
-    def seDeleteUser(self , user ) :
-        username = user.get('userName')
-        self.logger.info(f'Starting to remove {username} ...')
-        url= f"{self.baseUrl}/v1/tenants/users/{username}"
-        headers = self.getRequestHeader()
-        response = requests.delete(url, headers=headers , verify=False)
-        self.logger.debug(f'raw response  {response.text}')
-        self.logger.info(f'remove user {username} status code={response.status_code}')
-
-    def seLockUser(self , user ) :
-        username = user.get('userName')
-        self.logger.info(f'Starting to lock {username} ...')
-        url= f"{self.baseUrl}/v1/tenants/users/{username}/lock"
-        headers = self.getRequestHeader()
-        response = requests.post(url, headers=headers , verify=False)
-        self.logger.debug(f'raw response  {response.text}')
-        self.logger.info(f'lock user {username} status code={response.status_code}')
-
-    def seUnlockUser(self , user ) :
-        username = user.get('userName')
-        self.logger.info(f'Starting to unlock {username} ...')
-        url= f"{self.baseUrl}/v1/tenants/users/{username}/unlock"
-        headers = self.getRequestHeader()
-        response = requests.post(url, headers=headers , verify=False)
-        self.logger.debug(f'raw response {response.text}')
-        self.logger.info(f'unlock user {username} status code={response.status_code}')
-
-    def getRequestHeader( self , extra_header={}) :
-        headers = {'Content-type': 'application/json' , 'authorization': f"Bearer {self.accessToken}"}
-        headers.update(extra_header)
-        return headers
-
-    def getLicense(self) :
-        self.logger.info(f'Getting license information...')
-        url= f"{self.baseUrl}/v1/license"
-        headers = self.getRequestHeader()
-        response = requests.get(url, headers=headers , verify=False)
-        self.logger.debug(f'raw response {response.text}')
-        self.logger.info(f'requesting license status code={response.status_code}')
-        if response.status_code == 200 :
-            return response.json()
-        else :
-            return {}
-        
+    def getHeaders( self , headers={}, json=True ) :
+        _h = {'Authorization' : f"Bearer {self.accessToken}"}
+        self.logger.debug(f'request headers is {_h}')
+        if json :
+            self.logger.debug(f"json content type is Enabled. adding Content-type as application/json ")
+            _h.update({'Content-type': 'application/json'})
+        _h.update(headers)
+        return _h
+
+    def logout(self) :
+        self.logger.info('Starting to logout form LRA platform ..')
+        self.cp.logout()
+        self.logger.info('Logout form LRA platform Completed')
 
     def getUsers(self) :
-        self.logger.info(f"Get users from SE ...")
-        url= f"{self.baseUrl}/v1/tenants/users"
-        headers = self.getRequestHeader()
+        self.logger.info(f"Get users from LRA ...")
+        url= f"{self.baseUrl}/lra-rest/users"
+        headers = self.getHeaders()
         self.logger.debug(f'Get users headers = {headers}')
         response = requests.get(url , headers=headers , verify=False)
         self.logger.info(f'Get Usr response code={response.status_code}')
         self.logger.debug(f'raw response in authentication {response.text}')
         if response.status_code == 200 :
             self.logger.debug(f'response is 200 , return the json as dict and filter on data ...')
-            self.users = response.json().get('data')
+            self.users = response.json().get('items')
             return self.users
         else :
             self.logger.error(f'Error getting users  {response.text}')
             self.logger.debug(f'response is not 200 , return empty array')
             self.users = []
             return []
 
+    def createUser(self, user : dict , group ) :
+        username = user.get('userName')
+        self.logger.info(f'Starting to create {username}  with group {group} ...')
+        url= f"{self.baseUrl}/lra-rest/users"
+        self.logger.debug(f'creating user {username} using url {url} with POST')
+        if group == 'ROLE_ADMIN' :
+            lra_operatorRole = False 
+            adminRole  = True 
+            lra_viewerRole = False
+        elif group == 'ROLE_LRA_OPERATOR' :
+            lra_operatorRole = True 
+            adminRole  = False 
+            lra_viewerRole = False
+        elif group == 'ROLE_LRA_VIEWER' :
+            lra_operatorRole = False 
+            adminRole  = False 
+            lra_viewerRole = True
+        payload = {
+            'address' : '' ,
+            'adminRole' : adminRole ,
+            'contact' : '' ,
+            'email' : user.get('email') ,
+            'enabled' : True  ,
+            'disabled' : False ,
+            'localUser' : False , 
+            'loginAttemptLocked' : False,
+            'lra_operatorRole' : lra_operatorRole , 
+            'lra_viewerRole' : lra_viewerRole , 
+            'name' : username ,
+            'phoneNumber' : '' ,
+            'roles' : [group] ,
+            'userSource' : False,
+            'username' : user.get('email') # yes this must be email.    
+        }
+        self.logger.debug(f'Creating {username} using form {payload}')
+        headers = self.getHeaders()
+        response = requests.post(url , data=json.dumps(payload) , headers=headers , verify=False)
+        self.logger.debug(f'raw response {response.text}')
+        self.logger.info(f'create user {username} status code={response.status_code}')
+        return response
+
+
 if __name__ == '__main__':
     pass
```

### Comparing `easy_utils_dev-2.8.9/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.9/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 setup.py
 easy_utils_dev/EasySsh.py
 easy_utils_dev/Events.py
 easy_utils_dev/__init__.py
+easy_utils_dev/cplib.py
 easy_utils_dev/custom_env.py
 easy_utils_dev/debugger.py
 easy_utils_dev/encryptor.py
 easy_utils_dev/keycloakapi.py
 easy_utils_dev/lralib.py
 easy_utils_dev/ne1830PSS.py
 easy_utils_dev/optics_utils.py
```

