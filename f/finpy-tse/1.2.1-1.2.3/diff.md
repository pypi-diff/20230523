# Comparing `tmp/finpy_tse-1.2.1.tar.gz` & `tmp/finpy_tse-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finpy_tse-1.2.1.tar", last modified: Sun May 14 08:02:36 2023, max compression
+gzip compressed data, was "finpy_tse-1.2.3.tar", last modified: Tue May 23 07:15:37 2023, max compression
```

## Comparing `finpy_tse-1.2.1.tar` & `finpy_tse-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-14 08:02:05.000000 finpy_tse-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-05-14 08:02:05.000000 finpy_tse-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/finpy_tse/
--rw-r--r--   0 runner    (1001) docker     (123)   163676 2023-05-14 08:02:05.000000 finpy_tse-1.2.1/finpy_tse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/finpy_tse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 08:02:36.000000 finpy_tse-1.2.1/finpy_tse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 08:02:36.417531 finpy_tse-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-14 08:02:05.000000 finpy_tse-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:15:37.248397 finpy_tse-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-23 07:15:25.000000 finpy_tse-1.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-23 07:15:37.248397 finpy_tse-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-05-23 07:15:25.000000 finpy_tse-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:15:37.244397 finpy_tse-1.2.3/finpy_tse/
+-rw-r--r--   0 runner    (1001) docker     (123)   163676 2023-05-23 07:15:25.000000 finpy_tse-1.2.3/finpy_tse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:15:37.244397 finpy_tse-1.2.3/finpy_tse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-23 07:15:37.000000 finpy_tse-1.2.3/finpy_tse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-23 07:15:37.000000 finpy_tse-1.2.3/finpy_tse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:15:37.000000 finpy_tse-1.2.3/finpy_tse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-23 07:15:37.000000 finpy_tse-1.2.3/finpy_tse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 07:15:37.000000 finpy_tse-1.2.3/finpy_tse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 07:15:37.248397 finpy_tse-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 07:15:25.000000 finpy_tse-1.2.3/setup.py
```

### Comparing `finpy_tse-1.2.1/LICENSE.txt` & `finpy_tse-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finpy_tse-1.2.1/PKG-INFO` & `finpy_tse-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finpy_tse
-Version: 1.2.1
+Version: 1.2.3
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -104,22 +104,23 @@
 ```python
 fpy.Get_RI_History(
     stock='خودرو',
     start_date='1400-01-01',
     end_date='1401-01-01',
     ignore_date=False,
     show_weekday=False,
-    double_date=False)
+    double_date=False,
+    alt=False)
 ```
 
 <p>&nbsp;</p>
 
 <div dir="rtl" align="right">
 
-# دریافت سابقه اطلاعات درون‌ریز یک نماد
+# دریافت سابقه اطلاعات درون‌روز یک نماد
 <hr style="border:2px solid gray"> </hr>
 
 
 ### : دریافت سابقه ریز معاملات
 
 </div>
```

### Comparing `finpy_tse-1.2.1/README.md` & `finpy_tse-1.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -94,22 +94,23 @@
 ```python
 fpy.Get_RI_History(
     stock='خودرو',
     start_date='1400-01-01',
     end_date='1401-01-01',
     ignore_date=False,
     show_weekday=False,
-    double_date=False)
+    double_date=False,
+    alt=False)
 ```
 
 <p>&nbsp;</p>
 
 <div dir="rtl" align="right">
 
-# دریافت سابقه اطلاعات درون‌ریز یک نماد
+# دریافت سابقه اطلاعات درون‌روز یک نماد
 <hr style="border:2px solid gray"> </hr>
 
 
 ### : دریافت سابقه ریز معاملات
 
 </div>
```

### Comparing `finpy_tse-1.2.1/finpy_tse/__init__.py` & `finpy_tse-1.2.3/finpy_tse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             
 ################################################################################################################################################################################
 ################################################################################################################################################################################
 
 def __Get_TSE_WebID__(stock):
     # search TSE function ------------------------------------------------------------------------------------------------------------
     def request(name):
-        page = requests.get(f'http://www.tsetmc.com/tsev2/data/search.aspx?skey={name}', headers=headers)
+        page = requests.get(f'http://old.tsetmc.com/tsev2/data/search.aspx?skey={name}', headers=headers)
         data = []
         for i in page.text.split(';') :
             try :
                 i = i.split(',')
                 data.append([i[0],i[1],i[2],i[7],i[-1]])
             except :
                 pass
@@ -154,15 +154,15 @@
     دریافت سابقه قیمت یک سهم در روزهای معاملاتی بین تاریخ شروع و پایان
     قابلیت دریافت همه سابقه قیمت بدون توجه به تاریخ شروع و پایان
     قابلیت تعدیل قیمت برای سود نقدی و افزایش سرمایه با احتساب آورده
     قابلیت ارائه تاریخ میلادی علاوه بر تاریخ شمسی، قابلیت نمایش روزهای هفته
     """
     # a function to get price data from a given page ----------------------------------------------------------------------------------
     def get_price_data(ticker_no,ticker,name, data_part):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={ticker_no}&Top=999999&A=0', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={ticker_no}&Top=999999&A=0', headers=headers)
         df_history=pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Final','Close','Open','Y-Final','Value','Volume','No']
         #split data into defined columns
         df_history[columns] = df_history[0].str.split("@",expand=True)
         # drop old column 0
         df_history.drop(columns=[0],inplace=True)
         df_history.dropna(inplace=True)
@@ -1521,30 +1521,30 @@
 
 ################################################################################################################################################################################
 ################################################################################################################################################################################
 def Get_MarketWatch(save_excel = True, save_path = 'D:/FinPy-TSE Data/MarketWatch'):
     #--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     # GET MARKET RETAIL AND INSTITUTIONAL DATA
     #--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-    r = requests.get('http://www.tsetmc.com/tsev2/data/ClientTypeAll.aspx', headers=headers)
+    r = requests.get('http://old.tsetmc.com/tsev2/data/ClientTypeAll.aspx', headers=headers)
     Mkt_RI_df = pd.DataFrame(r.text.split(';'))
     Mkt_RI_df = Mkt_RI_df[0].str.split(",",expand=True)
     # assign names to columns:
     Mkt_RI_df.columns = ['WEB-ID','No_Buy_R','No_Buy_I','Vol_Buy_R','Vol_Buy_I','No_Sell_R','No_Sell_I','Vol_Sell_R','Vol_Sell_I']
     # convert columns to numeric type:
     cols = ['No_Buy_R','No_Buy_I','Vol_Buy_R','Vol_Buy_I','No_Sell_R','No_Sell_I','Vol_Sell_R','Vol_Sell_I']
     Mkt_RI_df[cols] = Mkt_RI_df[cols].apply(pd.to_numeric, axis=1)
     Mkt_RI_df['WEB-ID'] = Mkt_RI_df['WEB-ID'].apply(lambda x: x.strip())
     Mkt_RI_df = Mkt_RI_df.set_index('WEB-ID')
     # re-arrange the order of columns:
     Mkt_RI_df = Mkt_RI_df[['No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R','Vol_Sell_I']]
     #--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     # GET MARKET WATCH PRICE AND OB DATA
     #--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-    r = requests.get('http://www.tsetmc.com/tsev2/data/MarketWatchPlus.aspx', headers=headers)
+    r = requests.get('http://old.tsetmc.com/tsev2/data/MarketWatchPlus.aspx', headers=headers)
     main_text = r.text
     Mkt_df = pd.DataFrame((main_text.split('@')[2]).split(';'))
     Mkt_df = Mkt_df[0].str.split(",",expand=True)
     Mkt_df = Mkt_df.iloc[:,:23]
     Mkt_df.columns = ['WEB-ID','Ticker-Code','Ticker','Name','Time','Open','Final','Close','No','Volume','Value',
                       'Low','High','Y-Final','EPS','Base-Vol','Unknown1','Unknown2','Sector','Day_UL','Day_LL','Share-No','Mkt-ID']
     # re-arrange columns and drop some columns:
@@ -1552,15 +1552,15 @@
                       'Low','High','Y-Final','EPS','Base-Vol','Sector','Day_UL','Day_LL','Share-No','Mkt-ID']]
     # Just keep: 300 Bourse, 303 Fara-Bourse, 305 Sandoogh, 309 Payeh, 400 H-Bourse, 403 H-FaraBourse, 404 H-Payeh
     Mkt_ID_list = ['300','303','305','309','400','403','404']
     Mkt_df = Mkt_df[Mkt_df['Mkt-ID'].isin(Mkt_ID_list)]
     Mkt_df['Market'] = Mkt_df['Mkt-ID'].map({'300':'بورس','303':'فرابورس','305':'صندوق قابل معامله','309':'پایه','400':'حق تقدم بورس','403':'حق تقدم فرابورس','404':'حق تقدم پایه'})
     Mkt_df.drop(columns=['Mkt-ID'],inplace=True)   # we do not need Mkt-ID column anymore
     # assign sector names:
-    r = requests.get('http://www.tsetmc.com/Loader.aspx?ParTree=111C1213', headers=headers)
+    r = requests.get('http://old.tsetmc.com/Loader.aspx?ParTree=111C1213', headers=headers)
     sectro_lookup = (pd.read_html(r.text)[0]).iloc[1:,:]
     # convert from Arabic to Farsi and remove half-space
     sectro_lookup[1] = sectro_lookup[1].apply(lambda x: (str(x).replace('ي','ی')).replace('ك','ک'))
     sectro_lookup[1] = sectro_lookup[1].apply(lambda x: x.replace('\u200c',' '))
     sectro_lookup[1] = sectro_lookup[1].apply(lambda x: x.strip())
     Mkt_df['Sector'] = Mkt_df['Sector'].map(dict(sectro_lookup[[0, 1]].values))
     # modify format of columns:
@@ -1730,15 +1730,15 @@
     http = urllib3.PoolManager()
     look_up = pd.DataFrame({'Ticker':[],'Name':[],'WEB-ID':[],'Market':[]})
     # --------------------------------------------------------------------------------------------------
     if(bourse):
         if(show_progress):
             clear_output(wait=True)
             print('Gathering Bourse market stock list ...')
-        r = http.request('GET', "http://www.tsetmc.com/Loader.aspx?ParTree=15131J&i=32097828799138957") 
+        r = http.request('GET', "http://old.tsetmc.com/Loader.aspx?ParTree=15131J&i=32097828799138957") 
         soup = BeautifulSoup(r.data.decode('utf-8'), 'html.parser')
         table = soup.findAll("table", {"class": "table1"})
         stock_list = table[0].find_all('a')
         ticker = []
         web_id = []
         name = []
         for stock in stock_list:
@@ -1749,15 +1749,15 @@
         bourse_lookup['Market'] = 'بورس'
         look_up = pd.concat([look_up,bourse_lookup],axis=0)
     # --------------------------------------------------------------------------------------------------
     if(farabourse):
         if(show_progress):
             clear_output(wait=True)
             print('Gathering Fara-Bourse market stock list ...')
-        r = http.request('GET', 'http://www.tsetmc.com/Loader.aspx?ParTree=15131J&i=43685683301327984') 
+        r = http.request('GET', 'http://old.tsetmc.com/Loader.aspx?ParTree=15131J&i=43685683301327984') 
         soup = BeautifulSoup(r.data.decode('utf-8'), 'html.parser')
         table = soup.findAll("table", {"class": "table1"})
         stock_list = table[0].find_all('a')
         ticker = []
         web_id = []
         name = []
         for stock in stock_list:
@@ -1811,15 +1811,15 @@
         look_up = look_up.set_index('Ticker')
         look_up = look_up[['Name','Market','WEB-ID']]
         if(payeh):
             # some minor changes in payeh_lookup
             payeh_lookup['Ticker'] = payeh_lookup['Ticker'].apply(lambda x: characters.ar_to_fa(x))
             payeh_lookup = payeh_lookup.set_index('Ticker')
             # look for payeh market web-ids from market watch
-            r = requests.get('http://www.tsetmc.com/tsev2/data/MarketWatchPlus.aspx', headers=headers)
+            r = requests.get('http://old.tsetmc.com/tsev2/data/MarketWatchPlus.aspx', headers=headers)
             mkt_watch = pd.DataFrame((r.text.split('@')[2]).split(';'))
             mkt_watch = mkt_watch[0].str.split(",",expand=True)
             mkt_watch = mkt_watch[[0,2]]
             mkt_watch.columns = ['WEB-ID','Ticker']
             mkt_watch['Ticker'] = mkt_watch['Ticker'].apply(lambda x: characters.ar_to_fa(x))
             mkt_watch = mkt_watch.set_index('Ticker')
             # join based on payeh_lookup
@@ -1868,15 +1868,15 @@
                         if (counter==1):
                             df_final = i.copy()
                         else:
                             df_final = pd.concat([df_final,i])
                         counter+=1
                 return df_final
             async def get_session(session, code):
-                url = f'http://www.tsetmc.com/Loader.aspx?Partree=15131M&i={code}'
+                url = f'http://old.tsetmc.com/Loader.aspx?Partree=15131M&i={code}'
                 async with session.get(url, headers=headers) as response:
                     try:
                         data_text = await response.text()
                         soup = BeautifulSoup(data_text, 'html.parser')
                         table = soup.findAll("table", {"class": "table1"})
                         df_id = pd.read_html(str(table[0]))[0]
                         # rotate data frame:
```

### Comparing `finpy_tse-1.2.1/finpy_tse.egg-info/PKG-INFO` & `finpy_tse-1.2.3/finpy_tse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finpy-tse
-Version: 1.2.1
+Version: 1.2.3
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -104,22 +104,23 @@
 ```python
 fpy.Get_RI_History(
     stock='خودرو',
     start_date='1400-01-01',
     end_date='1401-01-01',
     ignore_date=False,
     show_weekday=False,
-    double_date=False)
+    double_date=False,
+    alt=False)
 ```
 
 <p>&nbsp;</p>
 
 <div dir="rtl" align="right">
 
-# دریافت سابقه اطلاعات درون‌ریز یک نماد
+# دریافت سابقه اطلاعات درون‌روز یک نماد
 <hr style="border:2px solid gray"> </hr>
 
 
 ### : دریافت سابقه ریز معاملات
 
 </div>
```

### Comparing `finpy_tse-1.2.1/setup.py` & `finpy_tse-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='finpy_tse',                           # should match the package folder
     packages=['finpy_tse'],                     # should match the package folder
-    version='1.2.1',                                # important for updates
+    version='1.2.3',                            # important for updates
     license='BSD (3-clause)',                                  # should match your chosen license
     description='A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='ALI RAHIMI  AND  RASOOL GHAFOURI',
     author_email='a.rahimi.aut@gmail.com',
     install_requires=['requests','jdatetime','pandas','numpy','requests','bs4','asyncio','urllib3','aiohttp','unsync','IPython','persiantools','datetime','XlsxWriter','lxml'],                  # list all packages that your package uses
```

