# Comparing `tmp/openAIInsight-0.0.5-py3-none-any.whl.zip` & `tmp/openAIInsight-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5400 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     9644 b- defN 23-May-12 06:15 openAIInsight/OpenAI_PineConeVector.py
--rw-rw-r--  2.0 unx     3238 b- defN 23-May-22 07:03 openAIInsight/__init__.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      609 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      596 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/RECORD
-7 files, 15266 bytes uncompressed, 4334 bytes compressed:  71.6%
+Zip file size: 5425 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     9399 b- defN 23-May-23 06:50 openAIInsight/OpenAI_PineConeVector.py
+-rw-rw-r--  2.0 unx     3544 b- defN 23-May-23 06:53 openAIInsight/__init__.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-23 06:57 openAIInsight-0.0.6.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      609 b- defN 23-May-23 06:57 openAIInsight-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-23 06:57 openAIInsight-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-23 06:57 openAIInsight-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      596 b- defN 23-May-23 06:57 openAIInsight-0.0.6.dist-info/RECORD
+7 files, 15327 bytes uncompressed, 4359 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: openAIInsight/OpenAI_PineConeVector.py
 Comment: 
 
 Filename: openAIInsight/__init__.py
 Comment: 
 
-Filename: openAIInsight-0.0.5.dist-info/LICENCE.txt
+Filename: openAIInsight-0.0.6.dist-info/LICENCE.txt
 Comment: 
 
-Filename: openAIInsight-0.0.5.dist-info/METADATA
+Filename: openAIInsight-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: openAIInsight-0.0.5.dist-info/WHEEL
+Filename: openAIInsight-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: openAIInsight-0.0.5.dist-info/top_level.txt
+Filename: openAIInsight-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: openAIInsight-0.0.5.dist-info/RECORD
+Filename: openAIInsight-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openAIInsight/OpenAI_PineConeVector.py

```diff
@@ -1,19 +1,17 @@
 import json
 import openai
 import pinecone
-import datetime
 import traceback
 import pandas as pd
 from flask import request
 import loggerutility as logger
 import commonutility as common
 from openai.embeddings_utils import get_embedding, get_embeddings, cosine_similarity
 
-
 class OpenAI_PineConeVector:
     
     index_name      =   "" 
     openAI_apiKey   =   "" 
     pineCone_apiKey =   "" 
     queryList       =   "" 
     dfJson          =   ""
@@ -138,19 +136,17 @@
             pinecone.init(api_key=self.pineCone_apiKey, environment='us-west4-gcp')
             
             pinecone_IndexList = pinecone.list_indexes()
             
             if self.index_name in pinecone_IndexList:
                 self.my_index = pinecone.Index(index_name=self.index_name)
                 logger.log(f"self.my_index::: {self.my_index}","0")
-                logger.log(f"Pinecone execution START Time::: {datetime.datetime.now().strftime('%H:%M:%S')}","0")
                 for i in self.queryList:
                     if i != "" and i != None:
                         result.append(self.my_index.query(vector=get_embedding(i, engine=self.engineName),top_k=1, include_metadata=True))
-                logger.log(f"Pinecone execution END Time::: {datetime.datetime.now().strftime('%H:%M:%S')}","0")
                 logger.log(f"OpenAI_PineConeVector class getLookUP() Response::: \n{result}\tlen::: {len(result)}\t{type(result)}", "0")
 
                 id_list = [element["matches"][0]["id"] for element in result]
                 IdDescription_dict = dict(zip(self.queryList, id_list))
                 logger.log(f"\n\nOpenAI_PineConeVector class getLookUP() IdDescription_dict::: \n{IdDescription_dict}\tlen::: {len(IdDescription_dict)}\t{type(IdDescription_dict)}", "0")
 
                 return str(IdDescription_dict)
@@ -163,10 +159,10 @@
             
         except Exception as e:
             logger.log(f"OpenAI_PineConeVector class getLookUP() Issue::: \n{e}","0")
             trace = traceback.format_exc()
             descr = str(e)
             errorXml = common.getErrorXml(descr, trace)
             logger.log(f'\n OpenAI_PineConeVector class getLookUP() errorXml::: \n{errorXml}', "0")
-            return str(errorXml)
+            raise str(errorXml)
 
-    
+
```

## openAIInsight/__init__.py

```diff
@@ -6,18 +6,23 @@
 class openAI:
     def getCompletionEndpoint(self):
         try:
             jsonData = request.get_data('jsonData', None)
             jsonData = json.loads(jsonData[9:])
             logger.log(f"\njsonData openAI class::: {jsonData}","0")
 
-            licenseKey   = jsonData['license_key']
-            insightInput = jsonData['insight_input']
+            licenseKey      = jsonData['license_key']
+            insightInput    = jsonData['insight_input']
+            enterpriseName  = jsonData['enterprise']     # eg. APPVIS, DEMOVIS
+            fileName        = enterpriseName + "_insightData.txt"
+            logger.log(f"\n\njsonData openAI class fileName::: \t{fileName}\n","0")
+
             openai.api_key = licenseKey
-            openAI_trainingData = open("openAI_trainingData.txt","r").read()
+            # openAI_trainingData = open("openAI_trainingData.txt","r").read()  # original
+            openAI_trainingData = open(fileName,"r").read()
             
             # response = openai.Completion.create(
             # model="code-davinci-001",
             # prompt= openAI_trainingData + insightInput,
             # temperature=0.25,
             # max_tokens=198,
             # top_p=0.5,
@@ -27,15 +32,15 @@
             # )
 
             # logger.log(f"Response openAI completion endpoint::::: {response}","0")
             # finalResult=str(response["choices"][0]["text"])
             # logger.log(f"OpenAI completion endpoint finalResult ::::: {finalResult}","0")
             # return finalResult
         
-            logger.log(f"\n\nopenAI_trainingData before conversion :::::: {type(openAI_trainingData)} \n{openAI_trainingData}","0")
+            logger.log(f"\n\nopenAI_trainingData before conversion :::::: {type(openAI_trainingData)} \n{openAI_trainingData}\n","0")
             openAI_trainingData = openAI_trainingData.replace("<insight_input>", insightInput)
             logger.log(f"\n\nopenAI_trainingData after replacing <insight_input> :::::: \n{openAI_trainingData} \n{type(openAI_trainingData)}","0")
             messageList = json.loads(openAI_trainingData)
             logger.log(f"\n\nmessageList after conversion :::::: {messageList} \n{type(messageList)}","0")
             
             logger.log(f"\n\nfinal messageList :::::: {messageList}","0")
 
@@ -56,11 +61,9 @@
         except Exception as e:
             logger.log(f'\n In getCompletionEndpoint exception stacktrace : ', "1")
             trace = traceback.format_exc()
             descr = str(e)
             returnErr = common.getErrorXml(descr, trace)
             logger.log(f'\n Print exception returnSring inside getCompletionEndpoint : {returnErr}', "0")
             return str(returnErr)
-
-    
-
         
+
```

## Comparing `openAIInsight-0.0.5.dist-info/LICENCE.txt` & `openAIInsight-0.0.6.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `openAIInsight-0.0.5.dist-info/METADATA` & `openAIInsight-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openAIInsight
-Version: 0.0.5
+Version: 0.0.6
 Summary: Proteus openAI File
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

## Comparing `openAIInsight-0.0.5.dist-info/RECORD` & `openAIInsight-0.0.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-openAIInsight/OpenAI_PineConeVector.py,sha256=6NJjIvgAEcZyn8SUOnt2tITaZFbdFlV0SVzlV2eVLEA,9644
-openAIInsight/__init__.py,sha256=u1bKMu3xE0nmf-QZjGIhUI0Reg5Wu5XE0kLh0ewKKu8,3238
-openAIInsight-0.0.5.dist-info/LICENCE.txt,sha256=2qX9IkEUBx0VJp1Vh9O2dsRwE-IpYId0lXDyn7OVsJ8,1073
-openAIInsight-0.0.5.dist-info/METADATA,sha256=t7-rIKWsGcxX6XBdViIQj_INpht1_9ae6szgcooDi8U,609
-openAIInsight-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-openAIInsight-0.0.5.dist-info/top_level.txt,sha256=YzsKehORjpmF7-8r3ivEG7yh7VoqXMt2TfYbfHovmfg,14
-openAIInsight-0.0.5.dist-info/RECORD,,
+openAIInsight/OpenAI_PineConeVector.py,sha256=wpq7-kfFQJkTGAhUWzbAGNb94GSST8QuTkMYWfB2ugA,9399
+openAIInsight/__init__.py,sha256=TmQBHxDJ8OtGXakRbGkdQUkYAydvBOFaq5sOmsw6Lr8,3544
+openAIInsight-0.0.6.dist-info/LICENCE.txt,sha256=2qX9IkEUBx0VJp1Vh9O2dsRwE-IpYId0lXDyn7OVsJ8,1073
+openAIInsight-0.0.6.dist-info/METADATA,sha256=ZjIPT2kkT6mj6DrJQc3LSf7MuOcyY8VyTfxL3ekoWCI,609
+openAIInsight-0.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+openAIInsight-0.0.6.dist-info/top_level.txt,sha256=YzsKehORjpmF7-8r3ivEG7yh7VoqXMt2TfYbfHovmfg,14
+openAIInsight-0.0.6.dist-info/RECORD,,
```

