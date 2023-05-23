# Comparing `tmp/meesee-1.0.0.tar.gz` & `tmp/meesee-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/meneer/Development/meesee/dist/tmpvci4kwh9/meesee-1.0.0.tar", last modified: Tue Apr  6 11:23:45 2021, max compression
+gzip compressed data, was "meesee-1.1.0.tar", last modified: Tue May 23 12:48:28 2023, max compression
```

## Comparing `meesee-1.0.0.tar` & `meesee-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 meneer    (1000) meneer    (1000)        0 2021-04-06 11:23:45.068929 meesee-1.0.0/
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     2838 2021-04-06 11:23:45.068929 meesee-1.0.0/PKG-INFO
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     1403 2021-04-06 09:18:15.000000 meesee-1.0.0/README.md
-drwxrwxr-x   0 meneer    (1000) meneer    (1000)        0 2021-04-06 11:23:45.068929 meesee-1.0.0/meesee.egg-info/
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     2838 2021-04-06 11:23:45.000000 meesee-1.0.0/meesee.egg-info/PKG-INFO
--rw-rw-r--   0 meneer    (1000) meneer    (1000)      177 2021-04-06 11:23:45.000000 meesee-1.0.0/meesee.egg-info/SOURCES.txt
--rw-rw-r--   0 meneer    (1000) meneer    (1000)        1 2021-04-06 11:23:45.000000 meesee-1.0.0/meesee.egg-info/dependency_links.txt
--rw-rw-r--   0 meneer    (1000) meneer    (1000)       13 2021-04-06 11:23:45.000000 meesee-1.0.0/meesee.egg-info/requires.txt
--rw-rw-r--   0 meneer    (1000) meneer    (1000)        7 2021-04-06 11:23:45.000000 meesee-1.0.0/meesee.egg-info/top_level.txt
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     4972 2021-04-06 09:18:15.000000 meesee-1.0.0/meesee.py
--rw-rw-r--   0 meneer    (1000) meneer    (1000)       38 2021-04-06 11:23:45.068929 meesee-1.0.0/setup.cfg
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     1097 2021-04-06 11:23:33.000000 meesee-1.0.0/setup.py
+drwxrwxr-x   0 meneer    (1000) meneer    (1000)        0 2023-05-23 12:48:28.953574 meesee-1.1.0/
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)     1071 2023-05-23 12:07:33.000000 meesee-1.1.0/LICENSE
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)     3444 2023-05-23 12:48:28.953574 meesee-1.1.0/PKG-INFO
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)     2474 2023-05-23 12:07:33.000000 meesee-1.1.0/README.md
+drwxrwxr-x   0 meneer    (1000) meneer    (1000)        0 2023-05-23 12:48:28.953574 meesee-1.1.0/meesee.egg-info/
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)     3444 2023-05-23 12:48:28.000000 meesee-1.1.0/meesee.egg-info/PKG-INFO
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)      185 2023-05-23 12:48:28.000000 meesee-1.1.0/meesee.egg-info/SOURCES.txt
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)        1 2023-05-23 12:48:28.000000 meesee-1.1.0/meesee.egg-info/dependency_links.txt
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)       13 2023-05-23 12:48:28.000000 meesee-1.1.0/meesee.egg-info/requires.txt
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)        7 2023-05-23 12:48:28.000000 meesee-1.1.0/meesee.egg-info/top_level.txt
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)     4972 2023-05-23 12:07:33.000000 meesee-1.1.0/meesee.py
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)       38 2023-05-23 12:48:28.953574 meesee-1.1.0/setup.cfg
+-rw-rw-r--   0 meneer    (1000) meneer    (1000)     1246 2023-05-23 12:27:37.000000 meesee-1.1.0/setup.py
```

### Comparing `meesee-1.0.0/PKG-INFO` & `meesee-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,121 @@
 Metadata-Version: 2.1
 Name: meesee
-Version: 1.0.0
+Version: 1.1.0
 Summary: Task queue, Long lived workers process parallelization, with Redis as backend
 Home-page: https://github.com/Attumm/meesee
 Author: Melvin Bijman
 Author-email: bijman.m.m@gmail.com
 License: MIT
-Description: # Meesee
-        [![Build Status](https://travis-ci.org/Attumm/meesee.svg?branch=master)](https://travis-ci.org/Attumm/meesee)
-        
-        Task queue, Long lived workers process parallelization, with Redis as backend.
-        The project is still used in production and has to knowlegde been used in 3 companies in production setting.
-        
-        ## Examples
-        
-        Create my_func that will 
-        1. print starting message.
-        2. Sleep 1 second.
-        3. print a ending message.
-        
-        Let's start 10 of those.
-        
-        
-        ```python
-        import time
-        from meesee import startapp
-        
-        def my_func(item, worker_id):
-            print("hello, look at me")
-            time.sleep(1)
-            print('finished item', locals())
-        
-        
-        startapp(my_func, workers=10)
-        ```
-        
-        Open another terminal, Let's produce some tasks
-        ```python
-        from meesee import RedisQueue, config
-        
-        def produce(items):
-            r = RedisQueue(**config)
-            for i in range(items):
-                r.send(i)
-        
-        produce(10)
-        
-        ```
-        
-        Great, the placement of both scripts can be on any machine with connectivity to the redis instance.
-        
-        ### Prerequisites
-        
-        #### Redis
-        
-        For Debian, Ubuntu
-        ```
-        sudo apt-get install redis-server
-        ```
-        For Centos, Red Hat
-        ```
-        sudo yum install redis
-        ```
-        
-        ### Installing
-        
-        Create a virtualenv for your project.
-        Install meesee:
-        
-        ```
-        $ . /path/to/virtualenv/bin/activate
-        $  pip install meesee
-        ```
-        
-        ## Authors
-        
-        * **Melvin Bijman** 
-        * **Mark Moes**
-        
-        ## License
-        
-        This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Distributed Computing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Meesee
+[![Build Status](https://travis-ci.com/Attumm/meesee.svg?branch=main)](https://travis-ci.com/Attumm/meesee)
+
+Task queue, Long lived workers process parallelization, with Redis as backend.
+The project is used in production by three different companies.
+There are Meesee instances that have been running without maintenance or restarts for more than one year.
+
+Since the scope of the project is laser focussed on providing the following usecases.
+There are no outstanding feature requests, the project is stable and no code are needed at the moment.
+For feature request or additional information, an issue could be raised.
+For examples on how to use Meesee there are [examples](https://github.com/Attumm/meesee/tree/main/examples) available.
+
+
+1. Should be able to run for long periods, without maintenance or restarts.
+2. Restarting the service for maintenance or deployments, should not lead to missing messages.
+3. Should be reasonable fast and minimal amount of memory overhead for client and Redis instance.
+4. Should be able to schedule messages when workers are offline during deployment.
+5. Should not skip messages during certain scenario's such as heavy load.
+6. Should try to be as simple as possible to use, without a big learning curve. Distributed computing is hard enough by itself.
+
+## Examples
+
+Create my_func that will 
+1. print starting message.
+2. Sleep 1 second.
+3. print a ending message.
+
+Let's start 10 of those.
+
+
+```python
+import time
+from meesee import startapp
+
+def my_func(item, worker_id):
+    print("hello, look at me")
+    time.sleep(1)
+    print('finished item', locals())
+
+
+startapp(my_func, workers=10)
+```
+
+Open another terminal, Let's produce some tasks
+```python
+from meesee import RedisQueue, config
+
+def produce(items):
+    r = RedisQueue(**config)
+    for i in range(items):
+        r.send(i)
+
+produce(10)
+
+```
+
+Great, the placement of both scripts can be on any machine with connectivity to the redis instance.
+
+
+### Installing
+
+Create a virtualenv for your project.
+Install meesee:
+
+```
+$ . /path/to/virtualenv/bin/activate
+$  pip install meesee
+```
+
+### Prerequisites
+
+#### Redis instance
+
+For Docker
+```
+$ docker run --name some-redis -d redis
+```
+
+For Debian, Ubuntu
+```
+$ sudo apt-get install redis-server
+```
+For Centos, Red Hat
+```
+$ sudo yum install redis
+```
+
+## Authors
+
+* **Melvin Bijman** 
+* **Mark Moes**
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+
```

### Comparing `meesee-1.0.0/meesee.egg-info/PKG-INFO` & `meesee-1.1.0/meesee.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,121 @@
 Metadata-Version: 2.1
 Name: meesee
-Version: 1.0.0
+Version: 1.1.0
 Summary: Task queue, Long lived workers process parallelization, with Redis as backend
 Home-page: https://github.com/Attumm/meesee
 Author: Melvin Bijman
 Author-email: bijman.m.m@gmail.com
 License: MIT
-Description: # Meesee
-        [![Build Status](https://travis-ci.org/Attumm/meesee.svg?branch=master)](https://travis-ci.org/Attumm/meesee)
-        
-        Task queue, Long lived workers process parallelization, with Redis as backend.
-        The project is still used in production and has to knowlegde been used in 3 companies in production setting.
-        
-        ## Examples
-        
-        Create my_func that will 
-        1. print starting message.
-        2. Sleep 1 second.
-        3. print a ending message.
-        
-        Let's start 10 of those.
-        
-        
-        ```python
-        import time
-        from meesee import startapp
-        
-        def my_func(item, worker_id):
-            print("hello, look at me")
-            time.sleep(1)
-            print('finished item', locals())
-        
-        
-        startapp(my_func, workers=10)
-        ```
-        
-        Open another terminal, Let's produce some tasks
-        ```python
-        from meesee import RedisQueue, config
-        
-        def produce(items):
-            r = RedisQueue(**config)
-            for i in range(items):
-                r.send(i)
-        
-        produce(10)
-        
-        ```
-        
-        Great, the placement of both scripts can be on any machine with connectivity to the redis instance.
-        
-        ### Prerequisites
-        
-        #### Redis
-        
-        For Debian, Ubuntu
-        ```
-        sudo apt-get install redis-server
-        ```
-        For Centos, Red Hat
-        ```
-        sudo yum install redis
-        ```
-        
-        ### Installing
-        
-        Create a virtualenv for your project.
-        Install meesee:
-        
-        ```
-        $ . /path/to/virtualenv/bin/activate
-        $  pip install meesee
-        ```
-        
-        ## Authors
-        
-        * **Melvin Bijman** 
-        * **Mark Moes**
-        
-        ## License
-        
-        This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Distributed Computing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Meesee
+[![Build Status](https://travis-ci.com/Attumm/meesee.svg?branch=main)](https://travis-ci.com/Attumm/meesee)
+
+Task queue, Long lived workers process parallelization, with Redis as backend.
+The project is used in production by three different companies.
+There are Meesee instances that have been running without maintenance or restarts for more than one year.
+
+Since the scope of the project is laser focussed on providing the following usecases.
+There are no outstanding feature requests, the project is stable and no code are needed at the moment.
+For feature request or additional information, an issue could be raised.
+For examples on how to use Meesee there are [examples](https://github.com/Attumm/meesee/tree/main/examples) available.
+
+
+1. Should be able to run for long periods, without maintenance or restarts.
+2. Restarting the service for maintenance or deployments, should not lead to missing messages.
+3. Should be reasonable fast and minimal amount of memory overhead for client and Redis instance.
+4. Should be able to schedule messages when workers are offline during deployment.
+5. Should not skip messages during certain scenario's such as heavy load.
+6. Should try to be as simple as possible to use, without a big learning curve. Distributed computing is hard enough by itself.
+
+## Examples
+
+Create my_func that will 
+1. print starting message.
+2. Sleep 1 second.
+3. print a ending message.
+
+Let's start 10 of those.
+
+
+```python
+import time
+from meesee import startapp
+
+def my_func(item, worker_id):
+    print("hello, look at me")
+    time.sleep(1)
+    print('finished item', locals())
+
+
+startapp(my_func, workers=10)
+```
+
+Open another terminal, Let's produce some tasks
+```python
+from meesee import RedisQueue, config
+
+def produce(items):
+    r = RedisQueue(**config)
+    for i in range(items):
+        r.send(i)
+
+produce(10)
+
+```
+
+Great, the placement of both scripts can be on any machine with connectivity to the redis instance.
+
+
+### Installing
+
+Create a virtualenv for your project.
+Install meesee:
+
+```
+$ . /path/to/virtualenv/bin/activate
+$  pip install meesee
+```
+
+### Prerequisites
+
+#### Redis instance
+
+For Docker
+```
+$ docker run --name some-redis -d redis
+```
+
+For Debian, Ubuntu
+```
+$ sudo apt-get install redis-server
+```
+For Centos, Red Hat
+```
+$ sudo yum install redis
+```
+
+## Authors
+
+* **Melvin Bijman** 
+* **Mark Moes**
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+
```

### Comparing `meesee-1.0.0/meesee.py` & `meesee-1.1.0/meesee.py`

 * *Files identical despite different names*

### Comparing `meesee-1.0.0/setup.py` & `meesee-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     author='Melvin Bijman',
     author_email='bijman.m.m@gmail.com',
 
     description='Task queue, Long lived workers process parallelization, with Redis as backend',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
-    version='1.0.0',
+    version='1.1.0',
     py_modules=['meesee'],
-    install_requires=['redis==3.5.3'],
+    install_requires=['redis==4.5.5'],
     python_requires='>3.5',
     license='MIT',
 
     url='https://github.com/Attumm/meesee',
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
@@ -32,9 +32,12 @@
         'License :: OSI Approved :: MIT License',
 
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

