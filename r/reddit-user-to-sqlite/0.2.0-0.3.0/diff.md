# Comparing `tmp/reddit-user-to-sqlite-0.2.0.tar.gz` & `tmp/reddit_user_to_sqlite-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit-user-to-sqlite-0.2.0.tar", last modified: Mon May  8 07:05:33 2023, max compression
+gzip compressed data, was "reddit_user_to_sqlite-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reddit-user-to-sqlite-0.2.0.tar` & `reddit_user_to_sqlite-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-05-01 03:22:25.344837 reddit-user-to-sqlite-0.2.0/LICENSE
--rw-r--r--   0        0        0     3797 2023-05-08 06:08:15.246487 reddit-user-to-sqlite-0.2.0/README.md
--rw-r--r--   0        0        0     1202 2023-05-08 04:41:42.994469 reddit-user-to-sqlite-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 03:19:48.457234 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-08 06:48:29.198734 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/cli.py
--rw-r--r--   0        0        0      239 2023-05-05 03:42:09.817348 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/helpers.py
--rw-r--r--   0        0        0     3141 2023-05-08 07:02:22.652956 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/reddit_api.py
--rw-r--r--   0        0        0     4750 2023-05-08 05:36:28.464858 reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/sqlite_helpers.py
--rw-r--r--   0        0        0     4894 1970-01-01 00:00:00.000000 reddit-user-to-sqlite-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-01 03:22:25.344837 reddit_user_to_sqlite-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5600 2023-05-23 19:14:45.965284 reddit_user_to_sqlite-0.3.0/README.md
+-rw-r--r--   0        0        0     1204 2023-05-23 19:13:25.850548 reddit_user_to_sqlite-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 03:19:48.457234 reddit_user_to_sqlite-0.3.0/reddit_user_to_sqlite/__init__.py
+-rw-r--r--   0        0        0     4857 2023-05-23 19:13:25.850769 reddit_user_to_sqlite-0.3.0/reddit_user_to_sqlite/cli.py
+-rw-r--r--   0        0        0     1365 2023-05-23 19:13:25.850919 reddit_user_to_sqlite-0.3.0/reddit_user_to_sqlite/csv_helpers.py
+-rw-r--r--   0        0        0     1097 2023-05-23 19:13:25.851115 reddit_user_to_sqlite-0.3.0/reddit_user_to_sqlite/helpers.py
+-rw-r--r--   0        0        0     4121 2023-05-23 19:13:25.851415 reddit_user_to_sqlite-0.3.0/reddit_user_to_sqlite/reddit_api.py
+-rw-r--r--   0        0        0     5566 2023-05-23 19:13:25.851627 reddit_user_to_sqlite-0.3.0/reddit_user_to_sqlite/sqlite_helpers.py
+-rw-r--r--   0        0        0     6699 1970-01-01 00:00:00.000000 reddit_user_to_sqlite-0.3.0/PKG-INFO
```

### Comparing `reddit-user-to-sqlite-0.2.0/LICENSE` & `reddit_user_to_sqlite-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit-user-to-sqlite-0.2.0/pyproject.toml` & `reddit_user_to_sqlite-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "reddit-user-to-sqlite"
-version = "0.2.0"
+version = "0.3.0"
 
 authors = [{ name = "David Brownman", email = "beamneocube@gmail.com" }]
 description = "Create a SQLite database containing data pulled from Reddit about a single user."
 readme = "README.md"
 license = { file = "LICENSE" }
 
 requires-python = ">=3.10"
@@ -15,15 +15,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Natural Language :: English",
 ]
 keywords = ["sqlite", "reddit", "dogsheep"]
 
 dependencies = [
-  "sqlite-utils==3.30",
+  "sqlite-utils==3.32.1",
   "click==8.1.3",
   "requests==2.29.0",
   "tqdm==4.65.0",
 ]
 
 [project.optional-dependencies]
 test = ["pytest==7.3.1", "responses==0.23.1"]
```

### Comparing `reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/reddit_api.py` & `reddit_user_to_sqlite-0.3.0/reddit_user_to_sqlite/reddit_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from typing import Literal, Optional, Sequence, TypedDict, final
+from typing import Any, Literal, NotRequired, Optional, Sequence, TypedDict, final
 
 import requests
-from tqdm import tqdm
+from tqdm import tqdm, trange
+
+from reddit_user_to_sqlite.helpers import batched
 
 USER_AGENT = "reddit-to-sqlite"
 
 
 class SubredditFragment(TypedDict):
     ## SUBREDDIT
     # "consoledeals"
@@ -16,15 +18,15 @@
     subreddit_type: str
 
 
 class UserFragment(TypedDict):
     # comment author username
     author: str
     # comment author prefixed id
-    author_fullname: str
+    author_fullname: NotRequired[str]
 
 
 class Comment(SubredditFragment, UserFragment):
     # this is only the relevant fields from the response
 
     ## COMMENT
     # short ID
@@ -82,14 +84,18 @@
     num_comments: int
     over_18: bool
 
     # timestamp
     created: float
 
 
+# class Subreddit(TypedDict):
+#     should_archive_posts: bool
+
+
 @final
 class ResourceWrapper(TypedDict):
     kind: str
     data: Comment | Post
 
 
 @final
@@ -114,30 +120,42 @@
     error: int
 
 
 # max page size is 100
 PAGE_SIZE = 100
 
 
+def _raise_reddit_error(response):
+    if "error" in response:
+        raise ValueError(
+            f'Received API error from Reddit (code {response["error"]}): {response["message"]}'
+        )
+
+
+def _call_reddit_api(url: str, params: dict[str, Any] | None = None) -> SuccessResponse:
+    response = requests.get(
+        url,
+        {"limit": PAGE_SIZE, "raw_json": 1, **(params or {})},
+        headers={"user-agent": USER_AGENT},
+    ).json()
+
+    _raise_reddit_error(response)
+
+    return response
+
+
 def _load_paged_resource(resource: Literal["comments", "submitted"], username: str):
     result = []
     after = None
     # max number of pages we can fetch
-    for _ in tqdm(range(10)):
-        response: SuccessResponse | ErorrResponse = requests.get(
+    for _ in trange(10):
+        response = _call_reddit_api(
             f"https://www.reddit.com/user/{username}/{resource}.json",
-            {"limit": PAGE_SIZE, "raw_json": 1, "after": after},
-            headers={"user-agent": USER_AGENT},
-        ).json()
-
-        if "error" in response:
-            raise ValueError(
-                f'Received API error from Reddit (code {response["error"]}): {response["message"]}'
-            )
-
+            params={"after": after},
+        )
         result += [c["data"] for c in response["data"]["children"]]
         after = response["data"]["after"]
 
         if len(response["data"]["children"]) < PAGE_SIZE:
             break
 
     return result
@@ -145,7 +163,30 @@
 
 def load_comments_for_user(username: str) -> list[Comment]:
     return _load_paged_resource("comments", username)
 
 
 def load_posts_for_user(username: str) -> list[Post]:
     return _load_paged_resource("submitted", username)
+
+
+def load_info(resources: Sequence[str]) -> list[Comment | Post]:
+    result = []
+
+    for batch in batched(tqdm(resources), PAGE_SIZE):
+        response = _call_reddit_api(
+            "https://www.reddit.com/api/info.json", params={"id": ",".join(batch)}
+        )
+        result += [c["data"] for c in response["data"]["children"]]
+
+    return result
+
+
+def get_user_id(username: str) -> str:
+    response = requests.get(
+        f"https://www.reddit.com/user/{username}/about.json",
+        headers={"user-agent": USER_AGENT},
+    ).json()
+
+    _raise_reddit_error(response)
+
+    return response["data"]["id"]
```

### Comparing `reddit-user-to-sqlite-0.2.0/reddit_user_to_sqlite/sqlite_helpers.py` & `reddit_user_to_sqlite-0.3.0/reddit_user_to_sqlite/sqlite_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Sequence, TypedDict, cast
+from typing import Callable, Iterable, TypedDict, TypeVar
 
 from sqlite_utils import Database
 
 from reddit_user_to_sqlite.reddit_api import (
     Comment,
     Post,
     SubredditFragment,
@@ -10,84 +10,102 @@
 )
 
 
 class SubredditRow(TypedDict):
     id: str
     name: str
     type: str
+    # TODO: handle archiving and updating
+    # archives_posts: bool
 
 
-def comment_to_subreddit_row(comment: SubredditFragment) -> SubredditRow:
+def item_to_subreddit_row(item: SubredditFragment) -> SubredditRow:
     return {
-        "id": comment["subreddit_id"][3:],
-        "name": comment["subreddit"],
-        "type": comment["subreddit_type"],
+        "id": item["subreddit_id"][3:],
+        "name": item["subreddit"],
+        "type": item["subreddit_type"],
     }
 
 
-def insert_subreddits(db: Database, subreddits: Sequence[SubredditFragment]):
-    db["subreddits"].insert_all(  # type: ignore
-        map(comment_to_subreddit_row, subreddits),
-        ignore=True,  # type: ignore
+def insert_subreddits(db: Database, subreddits: Iterable[SubredditFragment]):
+    # https://github.com/simonw/sqlite-utils/issues/554
+    db["subreddits"].upsert_all(  # type: ignore
+        map(item_to_subreddit_row, subreddits),
+        # ignore=True,  # type: ignore
         # only relevant if creating the table
         pk="id",  # type: ignore
         not_null=["id", "name"],  # type: ignore
     )
 
 
 class UserRow(TypedDict):
     id: str
     username: str
 
 
-def comment_to_user_row(comment: UserFragment) -> UserRow:
-    return {"id": comment["author_fullname"][3:], "username": comment["author"]}
+def item_to_user_row(item: UserFragment) -> dict[str, str] | None:
+    if "author_fullname" in item:
+        return {"id": item["author_fullname"][3:], "username": item["author"]}
 
 
 def insert_user(db: Database, user: UserFragment):
-    db["users"].insert(  # type: ignore
-        cast(dict[str, Any], comment_to_user_row(user)),
-        # ignore any write error
-        ignore=True,
-        # only relevant if creating the table
-        pk="id",  # type: ignore
-        not_null=["id", "username"],
-    )
+    if user_row := item_to_user_row(user):
+        # don't really want to upsert, but I get errors from sqlite when I `insert` after an insert_all
+        # https://github.com/simonw/sqlite-utils/issues/554
+        db["users"].upsert(  # type: ignore
+            user_row,
+            # ignore any write error
+            # ignore=True,
+            # only relevant if creating the table
+            pk="id",  # type: ignore
+            not_null=["id", "username"],  # type: ignore
+        )
 
 
 class CommentRow(TypedDict):
     id: str
     timestamp: int
     score: int
     text: str
     user: str
     is_submitter: int
     subreddit: str
     permalink: str
     controversiality: int
 
 
-def comment_to_comment_row(comment: Comment) -> CommentRow:
+def comment_to_comment_row(comment: Comment) -> CommentRow | None:
+    if "author_fullname" not in comment:
+        return
+
     return {
         "id": comment["id"],
         "timestamp": int(comment["created"]),
         "score": comment["score"],
         "text": comment["body"],
         "user": comment["author_fullname"][3:],  # strip leading t2_
         "subreddit": comment["subreddit_id"][3:],  # strip leading t5_
         "permalink": f'https://old.reddit.com{comment["permalink"]}?context=10',
         "is_submitter": int(comment["is_submitter"]),
         "controversiality": comment["controversiality"],
     }
 
 
-def upsert_comments(db: Database, comments: list[Comment]):
-    db["comments"].insert_all(  # type: ignore
-        map(comment_to_comment_row, comments),
-        upsert=True,
+T = TypeVar("T")
+U = TypeVar("U")
+
+
+def apply_and_filter(filterer: Callable[[T], U | None], items: Iterable[T]) -> list[U]:
+    return [c for c in map(filterer, items) if c]
+
+
+def upsert_comments(db: Database, comments: Iterable[Comment]) -> int:
+    comment_rows = apply_and_filter(comment_to_comment_row, comments)
+    db["comments"].upsert_all(  # type: ignore
+        comment_rows,
         pk="id",  # type: ignore
         # update the schema - needed if user does archive first
         alter=True,  # type: ignore
         foreign_keys=[  # type: ignore
             (
                 "subreddit",
                 "subreddits",
@@ -99,14 +117,15 @@
                 "id",
             ),
         ],
         # can re-add or assert this later, but the rows aren't created if this is present
         # see: https://github.com/simonw/sqlite-utils/issues/538
         # not_null=["id", "timestamp", "text", "user", "subreddit", "permalink"],
     )
+    return len(comment_rows)
 
 
 class PostRow(TypedDict):
     id: str
     timestamp: int
     score: int
     title: str
@@ -118,15 +137,18 @@
     upvote_ratio: float
     score: int
     num_comments: int
     num_awards: int
     is_removed: int
 
 
-def post_to_post_row(post: Post) -> PostRow:
+def post_to_post_row(post: Post) -> PostRow | None:
+    if "author_fullname" not in post:
+        return
+
     return {
         "id": post["id"],
         "timestamp": int(post["created"]),
         "score": post["score"],
         "num_comments": post["num_comments"],
         "title": post["title"],
         "text": post["selftext"],
@@ -137,17 +159,18 @@
         "upvote_ratio": post["upvote_ratio"],
         "score": post["score"],
         "num_awards": post["total_awards_received"],
         "is_removed": int(post["selftext"] == "[removed]"),
     }
 
 
-def upsert_posts(db: Database, posts: list[Post]):
+def upsert_posts(db: Database, posts: Iterable[Post]) -> int:
+    post_rows = apply_and_filter(post_to_post_row, posts)
     db["posts"].insert_all(  # type: ignore
-        map(post_to_post_row, posts),
+        post_rows,
         upsert=True,
         pk="id",  # type: ignore
         alter=True,  # type: ignore
         foreign_keys=[  # type: ignore
             (
                 "subreddit",
                 "subreddits",
@@ -156,14 +179,15 @@
             (
                 "user",
                 "users",
                 "id",
             ),
         ],
     )
+    return len(post_rows)
 
 
 def ensure_fts(db: Database):
     table_names = set(db.table_names())
     if "comments" in table_names and "comments_fts" not in table_names:
         db["comments"].enable_fts(["text"], create_triggers=True)
     if "posts" in table_names and "posts_fts" not in table_names:
```

### Comparing `reddit-user-to-sqlite-0.2.0/PKG-INFO` & `reddit_user_to_sqlite-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: reddit-user-to-sqlite
-Version: 0.2.0
-Summary: Create a SQLite database containing data pulled from Reddit about a single user.
-Keywords: sqlite,reddit,dogsheep
-Author-email: David Brownman <beamneocube@gmail.com>
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Requires-Dist: sqlite-utils==3.30
-Requires-Dist: click==8.1.3
-Requires-Dist: requests==2.29.0
-Requires-Dist: tqdm==4.65.0
-Requires-Dist: pytest==7.3.1 ; extra == "test"
-Requires-Dist: responses==0.23.1 ; extra == "test"
-Project-URL: Author, https://xavd.id
-Project-URL: Bug Tracker, https://github.com/xavdid/reddit-user-to-sqlite/issues
-Project-URL: Changelog, https://github.com/xavdid/reddit-user-to-sqlite/blob/main/CHANGELOG.md
-Project-URL: Homepage, https://github.com/xavdid/reddit-user-to-sqlite
-Provides-Extra: test
-
 # reddit-user-to-sqlite
 
 Stores all the content from a specific user in a SQLite database. This includes their comments and their posts.
 
 ## Install
 
 The PyPI package is `reddit-user-to-sqlite` ([PyPI Link](https://pypi.org/project/reddit-user-to-sqlite/)). Install it globally using [pipx](https://pypa.github.io/pipx/):
@@ -49,20 +23,29 @@
 reddit-user-to-sqlite user your_username --db my-reddit-data.db
 ```
 
 #### Params
 
 > Note: the argument order is reversed from most dogsheep packages (which take db_path first). This method allows for use of a default db name, so I prefer it.
 
-1. `username`: a case-insensitive string. The leading `/u/` is optional (and ignored if supplied)
+1. `username`: a case-insensitive string. The leading `/u/` is optional (and ignored if supplied).
 2. (optional) `--db`: the path to a sqlite file, which will be created or updated as needed. Defaults to `reddit.db`.
 
-### A Note on Stored Data
+### archive
 
-While most [Dogsheep](https://github.com/dogsheep) projects grab the raw JSON output of their source APIs, Reddit's API has a lot of junk in it. So, I opted for a slimmed down approach.
+Reads the output of a [Reddit GDPR archive](https://support.reddithelp.com/hc/en-us/articles/360043048352-How-do-I-request-a-copy-of-my-Reddit-data-and-information-) and fetches additional info from the Reddit API (where possible). This allows you to store more than 1k posts/comments.
+
+> FYI: this behavior is built with the assumption that the archive that Reddit provides has the same format regardless of if you select `GDPR` or `CCPA` as the request type. But, just to be on the safe side, I recommend selecting `GDPR` during the export process until I'm able to confirm.
+
+#### Params
+
+> Note: the argument order is reversed from most dogsheep packages (which take db_path first). This method allows for use of a default db name, so I prefer it.
+
+1. `archive_path`: the path to the (unzipped) archive directory on your machine. Don't rename/move the files that Reddit gives you.
+2. (optional) `--db`: the path to a sqlite file, which will be created or updated as needed. Defaults to `reddit.db`.
 
 ## Viewing Data
 
 The resulting SQLite database pairs well with [Datasette](https://datasette.io/), a tool for viewing SQLite in the web. Below is my recommended configuration.
 
 First, install `datasette`:
 
@@ -132,15 +115,15 @@
 
 When in a virtual environment, run the following:
 
 ```bash
 pip install -e '.[test]'
 ```
 
-This installs the package in `--edit` mode and makes its dependencies available.
+This installs the package in `--edit` mode and makes its dependencies available. You can now run `reddit-user-to-sqlite` to invoke the CLI.
 
 ### Running Tests
 
 In your virtual environment, a simple `pytest` should run the unit test suite.
 
 ## Motivation
 
@@ -148,12 +131,29 @@
 
 ## FAQs
 
 ### Why do some of my posts say `[removed]` even though I can see them?
 
 If a post is removed, only the mods and the user who posted it can see its text. Since this tool currently runs without any authentication, those removed posts can't be fetched via the API.
 
+To fetch data about your own removed posts, use the GDPR archive import
 This will be fixed in a future release, either by:
 
-- (planned) being able to pull data from a GDPR archive
-- (maybe) adding support for authentication, so you can see your own posts
+### Why is the database missing data returned by the Reddit API?
+
+While most [Dogsheep](https://github.com/dogsheep) projects grab the raw JSON output of their source APIs, Reddit's API has a lot of junk in it. So, I opted for a slimmed down approach.
+
+If there's a field missing that you think would be useful, feel free to open an issue!
+
+### Does this tool refetch old data?
+
+When running the `user` command, yes. It fetches and updates up to 1k each of comments and posts and updates the local copy.
+
+When running the `archive` command, no. To cut down on API requests, it only fetches data about comments/posts that aren't yet in the database (since the archive may include many items).
+
+Both of these may change in the future to be more in line with [Reddit's per-subreddit archiving guidelines](https://www.reddit.com/r/modnews/comments/py2xy2/voting_commenting_on_archived_posts/).
+
+## Releasing New Versions
+
+> these notes are mostly for myself (or other contributors)
 
+1. ensure tests pass
```

