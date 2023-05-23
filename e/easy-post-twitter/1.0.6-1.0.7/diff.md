# Comparing `tmp/easy_post_twitter-1.0.6.tar.gz` & `tmp/easy_post_twitter-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_post_twitter-1.0.6.tar", max compression
+gzip compressed data, was "easy_post_twitter-1.0.7.tar", max compression
```

## Comparing `easy_post_twitter-1.0.6.tar` & `easy_post_twitter-1.0.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       22 2023-05-09 13:37:39.194682 easy_post_twitter-1.0.6/easy_post_twitter/__init__.py
--rw-r--r--   0        0        0    10361 2023-05-19 14:28:46.273859 easy_post_twitter-1.0.6/easy_post_twitter/twitter.py
--rw-r--r--   0        0        0      415 2023-05-17 21:00:36.173097 easy_post_twitter-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 easy_post_twitter-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-09 13:37:39.194682 easy_post_twitter-1.0.7/easy_post_twitter/__init__.py
+-rw-r--r--   0        0        0    11800 2023-05-21 21:35:18.594562 easy_post_twitter-1.0.7/easy_post_twitter/twitter.py
+-rw-r--r--   0        0        0      415 2023-05-23 12:20:17.184434 easy_post_twitter-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 easy_post_twitter-1.0.7/PKG-INFO
```

### Comparing `easy_post_twitter-1.0.6/easy_post_twitter/twitter.py` & `easy_post_twitter-1.0.7/easy_post_twitter/twitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,15 +219,51 @@
         else:
             try:
                 response = client.create_tweet(text=text)
                 log.info(f'Tweet created successfully. ID: {response.data["id"]}')
                 return response
             except Exception as e:
                 log.error(f'Error creating tweet. Error: {e}')
-            
-        
+
+
+    def tweetIt(self, text, img, isThread, id):
+        ''' This method do not use twitter's api search to determine if
+        a tweet is the day's opening one or a response to an early one. 
+        Tweets with or without images.
+        '''
+        # with image
+        if img != '':
+          if isThread:
+              api = self.__get_api()
+              media = api.media_upload(img)
+              response = api.update_status(status=text, media_ids=[media.media_id], in_reply_to_status_id=id)
+              return response
+          else:
+              api = self.__get_api()
+              media = api.media_upload(img)
+              response = api.update_status(status=text, media_ids=[media.media_id])
+              return response
+
+        # no image
+        else:          
+          client = self.__get_client()
+          if isThread:
+              try:
+                  print('Thread. Last tweet id:',id)
+                  response = client.create_tweet(text=text, in_reply_to_tweet_id=id)
+                  return response
+              except Exception as e:
+                  log.error(f'Error creating thread. Error: {e}')
+          else:
+              try:
+                  response = client.create_tweet(text=text)
+                  log.info(f'Tweet created successfully. ID: {response.data["id"]}')
+                  return response
+              except Exception as e:
+                  log.error(f'Error creating tweet. Error: {e}')
+
 
 if __name__ == '__main__':
     img = '/home/drakon/Documents/DEV/projetos/easy_post_twitter/imgs/market1.png'
     tw = Twitter(with_images=True)
     status = 'B3 interbank deposit futures: today and a month ago #FuturodoCDI #mercadofinanceiro'
     tw.tweet_to_publish_with_image(text=status, imgs=img, sequential=False)
```

