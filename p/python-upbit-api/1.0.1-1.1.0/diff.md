# Comparing `tmp/python-upbit-api-1.0.1.tar.gz` & `tmp/python-upbit-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jihye/PycharmProjects/python-upbit-api/dist/.tmp-iwjerw9v/python-upbit-api-1.0.1.tar", last modified: Fri May 12 04:52:31 2023, max compression
+gzip compressed data, was "/Users/jihye/PycharmProjects/python-upbit-api/dist/.tmp-zq38cxp3/python-upbit-api-1.1.0.tar", last modified: Tue May 23 09:56:58 2023, max compression
```

## Comparing `python-upbit-api-1.0.1.tar` & `python-upbit-api-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-12 04:52:31.479816 python-upbit-api-1.0.1/
--rw-r--r--   0 jihye      (501) staff       (20)     1066 2023-04-28 03:15:30.000000 python-upbit-api-1.0.1/LICENSE
--rw-r--r--   0 jihye      (501) staff       (20)     8052 2023-05-12 04:52:31.479642 python-upbit-api-1.0.1/PKG-INFO
--rw-r--r--   0 jihye      (501) staff       (20)     5762 2023-05-11 14:40:27.000000 python-upbit-api-1.0.1/README.md
--rw-r--r--   0 jihye      (501) staff       (20)     1492 2023-05-12 04:52:09.000000 python-upbit-api-1.0.1/pyproject.toml
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-12 04:52:31.477464 python-upbit-api-1.0.1/python_upbit_api.egg-info/
--rw-r--r--   0 jihye      (501) staff       (20)     8052 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/PKG-INFO
--rw-r--r--   0 jihye      (501) staff       (20)      348 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/SOURCES.txt
--rw-r--r--   0 jihye      (501) staff       (20)        1 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/dependency_links.txt
--rw-r--r--   0 jihye      (501) staff       (20)       44 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/requires.txt
--rw-r--r--   0 jihye      (501) staff       (20)        6 2023-05-12 04:52:31.000000 python-upbit-api-1.0.1/python_upbit_api.egg-info/top_level.txt
--rw-r--r--   0 jihye      (501) staff       (20)       38 2023-05-12 04:52:31.479869 python-upbit-api-1.0.1/setup.cfg
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-12 04:52:31.477881 python-upbit-api-1.0.1/tests/
--rw-r--r--   0 jihye      (501) staff       (20)     1248 2023-05-11 03:13:33.000000 python-upbit-api-1.0.1/tests/test_remaining_req.py
--rw-r--r--   0 jihye      (501) staff       (20)     3174 2023-05-12 04:51:11.000000 python-upbit-api-1.0.1/tests/test_upbit.py
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-12 04:52:31.478977 python-upbit-api-1.0.1/upbit/
--rw-r--r--   0 jihye      (501) staff       (20)      726 2023-05-10 04:44:07.000000 python-upbit-api-1.0.1/upbit/__init__.py
--rw-r--r--   0 jihye      (501) staff       (20)     3469 2023-05-11 03:13:33.000000 python-upbit-api-1.0.1/upbit/exceptions.py
--rw-r--r--   0 jihye      (501) staff       (20)     3524 2023-05-10 05:00:31.000000 python-upbit-api-1.0.1/upbit/models.py
--rw-r--r--   0 jihye      (501) staff       (20)    66010 2023-05-12 04:51:11.000000 python-upbit-api-1.0.1/upbit/upbit.py
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-23 09:56:58.133082 python-upbit-api-1.1.0/
+-rw-r--r--   0 jihye      (501) staff       (20)     1066 2023-04-28 03:15:30.000000 python-upbit-api-1.1.0/LICENSE
+-rw-r--r--   0 jihye      (501) staff       (20)     9820 2023-05-23 09:56:58.132839 python-upbit-api-1.1.0/PKG-INFO
+-rw-r--r--   0 jihye      (501) staff       (20)     7518 2023-05-22 03:07:38.000000 python-upbit-api-1.1.0/README.md
+-rw-r--r--   0 jihye      (501) staff       (20)     1504 2023-05-23 09:55:46.000000 python-upbit-api-1.1.0/pyproject.toml
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-23 09:56:58.129819 python-upbit-api-1.1.0/python_upbit_api.egg-info/
+-rw-r--r--   0 jihye      (501) staff       (20)     9820 2023-05-23 09:56:58.000000 python-upbit-api-1.1.0/python_upbit_api.egg-info/PKG-INFO
+-rw-r--r--   0 jihye      (501) staff       (20)      362 2023-05-23 09:56:58.000000 python-upbit-api-1.1.0/python_upbit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jihye      (501) staff       (20)        1 2023-05-23 09:56:58.000000 python-upbit-api-1.1.0/python_upbit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jihye      (501) staff       (20)       44 2023-05-23 09:56:58.000000 python-upbit-api-1.1.0/python_upbit_api.egg-info/requires.txt
+-rw-r--r--   0 jihye      (501) staff       (20)        6 2023-05-23 09:56:58.000000 python-upbit-api-1.1.0/python_upbit_api.egg-info/top_level.txt
+-rw-r--r--   0 jihye      (501) staff       (20)       38 2023-05-23 09:56:58.133145 python-upbit-api-1.1.0/setup.cfg
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-23 09:56:58.130698 python-upbit-api-1.1.0/tests/
+-rw-r--r--   0 jihye      (501) staff       (20)      403 2023-05-23 09:48:45.000000 python-upbit-api-1.1.0/tests/test.py
+-rw-r--r--   0 jihye      (501) staff       (20)     1248 2023-05-11 03:13:33.000000 python-upbit-api-1.1.0/tests/test_remaining_req.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3174 2023-05-12 04:51:11.000000 python-upbit-api-1.1.0/tests/test_upbit.py
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2023-05-23 09:56:58.131923 python-upbit-api-1.1.0/upbit/
+-rw-r--r--   0 jihye      (501) staff       (20)      726 2023-05-10 04:44:07.000000 python-upbit-api-1.1.0/upbit/__init__.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3469 2023-05-11 03:13:33.000000 python-upbit-api-1.1.0/upbit/exceptions.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3872 2023-05-22 03:07:38.000000 python-upbit-api-1.1.0/upbit/models.py
+-rw-r--r--   0 jihye      (501) staff       (20)    68701 2023-05-23 09:49:16.000000 python-upbit-api-1.1.0/upbit/upbit.py
```

### Comparing `python-upbit-api-1.0.1/LICENSE` & `python-upbit-api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.1/PKG-INFO` & `python-upbit-api-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-upbit-api
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python Upbit API Wrapper
 Author-email: 이지혜 Lee Jihye <ghe.lee19@gmail.com>
 Maintainer-email: 이지혜 Lee Jihye <ghe.lee19@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Lee Jihye
         
@@ -26,15 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/designmeme/python-upbit-api
 Project-URL: repository, https://github.com/designmeme/python-upbit-api.git
 Project-URL: changelog, https://github.com/designmeme/python-upbit-api/blob/main/CHANGELOG.md
 Project-URL: issues, https://github.com/designmeme/python-upbit-api/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -99,16 +99,53 @@
 upbit = Upbit(access_key, secret_key)
 res = upbit.get_accounts()
 data = res.json()
 ```
 
 ## Features
 
+### 업비트 REST API를 모두 메서드로 제공
+
+[업비트 REST API][upbit docs api]를 `Upbit` 클래스의 메서드로 제공합니다.
+자세한 내용은 [upbit.py](https://github.com/designmeme/python-upbit-api/blob/main/upbit/upbit.py) 파일 내 docstring 참조.
+
+|    |             | 메서드명         |
+|----|:------------|:-------------|
+| 자산 | 전체 계좌 조회    | get_accounts |
+| 주문 | 주문 가능 정보    | get_order_chance |
+|  | 개별 주문 조회    | get_order |
+|  | 주문 리스트 조회   | get_orders |
+|  | 주문 취소 접수    | delete_order |
+|  | 주문하기        | create_order |
+| 출금 | 출금 리스트 조회   | get_withdraws |
+|  | 개별 출금 조회    | get_withdraw |
+|  | 출금 가능 정보    | get_withdraw_chance |
+|  | 디지털 자산 출금하기 | create_withdraw_coin |
+|  | 원화 출금하기     | create_withdraw_krw |
+|  | 출금 허용 주소 리스트 조회 | get_withdraw_addresses |
+| 입금 | 입금 리스트 조회   | get_deposits |
+|  | 개별 입금 조회    | get_deposit |
+|  | 입금 주소 생성 요청 | create_coin_address |
+|  | 전체 입금 주소 조회 | get_coin_addresses |
+|  | 개별 입금 주소 조회 | get_coin_address |
+|  | 원화 입금하기  | create_deposit_krw |
+| 서비스 정보 | 입출금 현황 | get_wallet_status |
+|  | API 키 리스트 조회 | get_api_keys |
+| 시세 종목 조회 | 마켓 코드 조회 | get_markets |
+| 시세 캔들 조회 | 분(Minute) 캔들 | get_candles_minute |
+|  | 일(Day) 캔들 | get_candles_day |
+|  | 주(Week) 캔들 | get_candles_week |
+|  | 월(Month) 캔들 | get_candles_month |
+| 시세 체결 조회 | 최근 체결 내역 | get_trades_ticks |
+| 시세 현재가 조회 | 현재가 정보 | get_ticker |
+| 시세 호가 조회 | 호가 정보 | get_orderbook |
+
 ### Requests 사용
-[Requests][requests] 라이브러리를 이용해 모든 [업비트 REST API][upbit docs api]를 `Upbit` 클래스의 메소드로 제공합니다.
+[Requests][requests] 라이브러리를 사용합니다.
+
 
 1. `requests.Response` 객체를 그대로 반환합니다.
     
     ```python
     # example.py
     from upbit import Upbit
     
@@ -153,15 +190,15 @@
 # example.py
 from upbit import Upbit, TooManyRequests, UpbitClientError, UpbitServerError
 
 upbit = Upbit()
 try:
     res = upbit.get_markets()
 except TooManyRequests as e:
-    status_code = e.response.status_code  # 423
+    status_code = e.response.status_code  # 429
     # ...예외 처리 코드
 except UpbitClientError as e:
     res = e.response
     # ...예외 처리 코드
 except UpbitServerError as e:
     res = e.response
     # ...예외 처리 코드
```

### Comparing `python-upbit-api-1.0.1/pyproject.toml` & `python-upbit-api-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 #where = ["src"]  # ["."] by default
 include = ["upbit*"]  # ["*"] by default
 #exclude = ["tests*"]  # empty by default
 #namespaces = true  # true by default
 
 [project]
 name = "python-upbit-api"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
     {name = "이지혜 Lee Jihye", email = "ghe.lee19@gmail.com"},
 ]
 maintainers = [
     {name = "이지혜 Lee Jihye", email = "ghe.lee19@gmail.com"},
 ]
 description = "Python Upbit API Wrapper"
 readme = "README.md"
 requires-python = ">=3.8"
 #keywords = ["one", "two"]
 license = {file = "LICENSE"}
 classifiers = [
     # 참고: https://pypi.org/classifiers/
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `python-upbit-api-1.0.1/python_upbit_api.egg-info/PKG-INFO` & `python-upbit-api-1.1.0/python_upbit_api.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-upbit-api
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python Upbit API Wrapper
 Author-email: 이지혜 Lee Jihye <ghe.lee19@gmail.com>
 Maintainer-email: 이지혜 Lee Jihye <ghe.lee19@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Lee Jihye
         
@@ -26,15 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/designmeme/python-upbit-api
 Project-URL: repository, https://github.com/designmeme/python-upbit-api.git
 Project-URL: changelog, https://github.com/designmeme/python-upbit-api/blob/main/CHANGELOG.md
 Project-URL: issues, https://github.com/designmeme/python-upbit-api/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -99,16 +99,53 @@
 upbit = Upbit(access_key, secret_key)
 res = upbit.get_accounts()
 data = res.json()
 ```
 
 ## Features
 
+### 업비트 REST API를 모두 메서드로 제공
+
+[업비트 REST API][upbit docs api]를 `Upbit` 클래스의 메서드로 제공합니다.
+자세한 내용은 [upbit.py](https://github.com/designmeme/python-upbit-api/blob/main/upbit/upbit.py) 파일 내 docstring 참조.
+
+|    |             | 메서드명         |
+|----|:------------|:-------------|
+| 자산 | 전체 계좌 조회    | get_accounts |
+| 주문 | 주문 가능 정보    | get_order_chance |
+|  | 개별 주문 조회    | get_order |
+|  | 주문 리스트 조회   | get_orders |
+|  | 주문 취소 접수    | delete_order |
+|  | 주문하기        | create_order |
+| 출금 | 출금 리스트 조회   | get_withdraws |
+|  | 개별 출금 조회    | get_withdraw |
+|  | 출금 가능 정보    | get_withdraw_chance |
+|  | 디지털 자산 출금하기 | create_withdraw_coin |
+|  | 원화 출금하기     | create_withdraw_krw |
+|  | 출금 허용 주소 리스트 조회 | get_withdraw_addresses |
+| 입금 | 입금 리스트 조회   | get_deposits |
+|  | 개별 입금 조회    | get_deposit |
+|  | 입금 주소 생성 요청 | create_coin_address |
+|  | 전체 입금 주소 조회 | get_coin_addresses |
+|  | 개별 입금 주소 조회 | get_coin_address |
+|  | 원화 입금하기  | create_deposit_krw |
+| 서비스 정보 | 입출금 현황 | get_wallet_status |
+|  | API 키 리스트 조회 | get_api_keys |
+| 시세 종목 조회 | 마켓 코드 조회 | get_markets |
+| 시세 캔들 조회 | 분(Minute) 캔들 | get_candles_minute |
+|  | 일(Day) 캔들 | get_candles_day |
+|  | 주(Week) 캔들 | get_candles_week |
+|  | 월(Month) 캔들 | get_candles_month |
+| 시세 체결 조회 | 최근 체결 내역 | get_trades_ticks |
+| 시세 현재가 조회 | 현재가 정보 | get_ticker |
+| 시세 호가 조회 | 호가 정보 | get_orderbook |
+
 ### Requests 사용
-[Requests][requests] 라이브러리를 이용해 모든 [업비트 REST API][upbit docs api]를 `Upbit` 클래스의 메소드로 제공합니다.
+[Requests][requests] 라이브러리를 사용합니다.
+
 
 1. `requests.Response` 객체를 그대로 반환합니다.
     
     ```python
     # example.py
     from upbit import Upbit
     
@@ -153,15 +190,15 @@
 # example.py
 from upbit import Upbit, TooManyRequests, UpbitClientError, UpbitServerError
 
 upbit = Upbit()
 try:
     res = upbit.get_markets()
 except TooManyRequests as e:
-    status_code = e.response.status_code  # 423
+    status_code = e.response.status_code  # 429
     # ...예외 처리 코드
 except UpbitClientError as e:
     res = e.response
     # ...예외 처리 코드
 except UpbitServerError as e:
     res = e.response
     # ...예외 처리 코드
```

### Comparing `python-upbit-api-1.0.1/tests/test_remaining_req.py` & `python-upbit-api-1.1.0/tests/test_remaining_req.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.1/tests/test_upbit.py` & `python-upbit-api-1.1.0/tests/test_upbit.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.1/upbit/__init__.py` & `python-upbit-api-1.1.0/upbit/__init__.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.1/upbit/exceptions.py` & `python-upbit-api-1.1.0/upbit/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.0.1/upbit/models.py` & `python-upbit-api-1.1.0/upbit/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,25 +31,37 @@
 """주문 타입
 
 - limit: 지정가 주문
 - price: 시장가 주문(매수)
 - market: 시장가 주문(매도)
 """
 
-TransactionStatus = Literal['WAITING', 'PROCESSING', 'DONE', 'FAILED', 'CANCELLED', 'REJECTED']
-"""입출금 상태
+WithdrawState = Literal['WAITING', 'PROCESSING', 'DONE', 'FAILED', 'CANCELLED', 'REJECTED']
+"""출금 상태
 
 - WAITING: 대기중
 - PROCESSING: 진행중
 - DONE: 완료
 - FAILED: 실패
 - CANCELLED: 취소됨
 - REJECTED: 거절됨
 """
 
+DepositState = Literal['PROCESSING', 'ACCEPTED', 'CANCELLED', 'REJECTED', 'TRAVEL_RULE_SUSPECTED', 'REFUNDING', 'REFUNDED']
+"""입금 상태
+
+- PROCESSING: 진행중
+- ACCEPTED: 완료
+- CANCELLED: 취소됨
+- REJECTED: 거절됨
+- TRAVEL_RULE_SUSPECTED: 트래블룰 추가 인증 대기중
+- REFUNDING: 반환절차 진행중
+- REFUNDED: 반환됨
+"""
+
 TransactionType = Literal['default', 'internal']
 """입출금 유형
 
 - default: 일반
 - internal: 바로
 """
```

### Comparing `python-upbit-api-1.0.1/upbit/upbit.py` & `python-upbit-api-1.1.0/upbit/upbit.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     InvalidRemainingReq,
 )
 from .models import (
     OrderBy,
     OrderState,
     OrderSide,
     OrderType,
-    TransactionStatus,
+    WithdrawState,
+    DepositState,
     TwoFactorType,
     TransactionType,
     MinuteUnit,
     RequestGroup,
     RemainingReq,
 )
 
@@ -75,15 +76,15 @@
     def _request_wrapper(func: Callable) -> Callable:
         """
         업비트 API 요청 래퍼
 
         1) 잔여 요청수 처리
         2) HTTPError를 UpbitError로 변환
 
-        :raises upbit.exceptions.TooManyRequests: 상태 코드가 423인 경우 발생
+        :raises upbit.exceptions.TooManyRequests: 상태 코드가 429인 경우 발생
         :raises upbit.exceptions.CreateAskError: 상태 코드가 400이고 인 오류 코드가 'create_ask_error' 인 경우 발생
         :raises upbit.exceptions.CreateBidError: 상태 코드가 400이고 인 오류 코드가 'create_bid_error' 인 경우 발생
         :raises upbit.exceptions.InsufficientFundsAsk: 상태 코드가 400이고 인 오류 코드가 'insufficient_funds_ask' 인 경우 발생
         :raises upbit.exceptions.InsufficientFundsBid: 상태 코드가 400이고 인 오류 코드가 'insufficient_funds_bid' 인 경우 발생
         :raises upbit.exceptions.UnderMinTotalAsk: 상태 코드가 400이고 인 오류 코드가 'under_min_total_ask' 인 경우 발생
         :raises upbit.exceptions.UnderMinTotalAsk: 상태 코드가 400이고 인 오류 코드가 'under_min_total_ask' 인 경우 발생
         :raises upbit.exceptions.UnderMinTotalBid: 상태 코드가 400이고 인 오류 코드가 'under_min_total_bid' 인 경우 발생
@@ -335,14 +336,15 @@
             "market": market,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, params=params, **kwargs)
 
     def get_order(self,
+                  *,
                   uuid: Optional[str] = None,
                   identifier: Optional[str] = None,
                   **kwargs) -> Response:
         """개별 주문 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%A3%BC%EB%AC%B8-%EC%A1%B0%ED%9A%8C>`_
@@ -358,15 +360,15 @@
         :return: API 서버 응답
 
         Usage::
 
             access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
-            res = upbit.get_order('d7c96420-a9ab-4ae8-a461-3db412427fb3')
+            res = upbit.get_order(uuid='d7c96420-a9ab-4ae8-a461-3db412427fb3')
             print(res.json())
 
             {
                 'created_at': '2023-02-06T11:00:45+09:00',
                 'executed_volume': '132.99843443',
                 'locked': '0',
                 'market': 'KRW-STRAX',
@@ -396,14 +398,15 @@
             "identifier": identifier,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, params=params, **kwargs)
 
     def get_orders(self,
+                   *,
                    market: Optional[str] = None,
                    uuids: Optional[list[str]] = None,
                    identifiers: Optional[list[str]] = None,
                    state: OrderState = 'wait',
                    states: Optional[list[OrderState]] = None,
                    page: int = 1,
                    limit: int = 100,
@@ -465,14 +468,15 @@
             "order_by": order_by,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, params=params, **kwargs)
 
     def delete_order(self,
+                     *,
                      uuid: Optional[str] = None,
                      identifier: Optional[str] = None,
                      **kwargs) -> Response:
         """주문 취소 접수
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EC%A3%BC%EB%AC%B8-%EC%B7%A8%EC%86%8C>`_
@@ -488,15 +492,15 @@
         :return: API 서버 응답
 
         Usage::
 
             access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
-            res = upbit.delete_order('cdd92199-2897-4e14-9448-f923320408ad')
+            res = upbit.delete_order(uuid='cdd92199-2897-4e14-9448-f923320408ad')
             print(res.json())
 
             {
                 "uuid": "cdd92199-2897-4e14-9448-f923320408ad",
                 "side": "bid",
                 "ord_type": "limit",
                 "price": "100.0",
@@ -519,17 +523,18 @@
             "identifier": identifier,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('delete', url, headers=headers, params=params, **kwargs)
 
     def create_order(self,
-                     market: str, 
-                     side: OrderSide, 
+                     market: str,
+                     side: OrderSide,
                      ord_type: OrderType,
+                     *,
                      volume: Optional[str] = None,
                      price: Optional[str] = None,
                      identifier: Optional[str] = None,
                      **kwargs) -> Response:
         """주문하기
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
@@ -588,16 +593,17 @@
         return self._request('post', url, headers=headers, params=params, **kwargs)
 
     # --------------------------------------------------------------------------
     # Exchange API > 출금
     # --------------------------------------------------------------------------
 
     def get_withdraws(self,
+                      *,
                       currency: Optional[str] = None,
-                      state: Optional[TransactionStatus] = None,
+                      state: Optional[WithdrawState] = None,
                       uuids: Optional[list[str]] = None,
                       txids: Optional[list[str]] = None,
                       page: int = 1,
                       limit: int = 100,
                       order_by: OrderBy = 'desc',
                       **kwargs) -> Response:
         """출금 리스트 조회
@@ -626,14 +632,15 @@
             res = upbit.get_withdraws(currency='XRP', state='DONE')
             print(res.json())
 
             [{
                 "type": "withdraw",
                 "uuid": "35a4f1dc-1db5-4d6b-89b5-7ec137875956",
                 "currency": "XRP",
+                "net_type": "XRP",
                 "txid": "98c15999f0bdc4ae0e8a-ed35868bb0c204fe6ec29e4058a3451e-88636d1040f4baddf943274ce37cf9cc",
                 "state": "DONE",
                 "created_at": "2019-02-28T15:17:51+09:00",
                 "done_at": "2019-02-28T15:22:12+09:00",
                 "amount": "1.00",
                 "fee": "0.0",
                 "transaction_type": "default"
@@ -650,14 +657,15 @@
             "order_by": order_by,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, params=params, **kwargs)
 
     def get_withdraw(self,
+                     *,
                      uuid: Optional[str] = None,
                      txid: Optional[str] = None,
                      currency: Optional[str] = None,
                      **kwargs) -> Response:
         """개별 출금 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
@@ -673,21 +681,22 @@
         :return: API 서버 응답
 
         Usage::
 
             access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
-            res = upbit.get_withdraw('9f432943-54e0-40b7-825f-b6fec8b42b79')
+            res = upbit.get_withdraw(uuid='9f432943-54e0-40b7-825f-b6fec8b42b79')
             print(res.json())
 
             {
                 "type": "withdraw",
                 "uuid": "9f432943-54e0-40b7-825f-b6fec8b42b79",
                 "currency": "BTC",
+                "net_type": "BTC",
                 "txid": null,
                 "state": "processing",
                 "created_at": "2018-04-13T11:24:01+09:00",
                 "done_at": null,
                 "amount": "0.01",
                 "fee": "0.0",
                 "transaction_type": "default"
@@ -701,33 +710,36 @@
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, params=params, **kwargs)
 
     def get_withdraw_chance(self,
                             currency: str,
+                            *,
+                            net_type: str,
                             **kwargs) -> Response:
         """출금 가능 정보 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EC%B6%9C%EA%B8%88-%EA%B0%80%EB%8A%A5-%EC%A0%95%EB%B3%B4>`_
 
         :param currency: Currency 코드
+        :param net_type: 출금 네트워크
         :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
 
         :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
 
         :return: API 서버 응답
 
         Usage::
 
             access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
-            res = upbit.get_withdraw_chance('BTC')
+            res = upbit.get_withdraw_chance('BTC', net_type='BTC')
             print(res.json())
 
             {
                 "member_level": {
                     "security_level": 3,
                     "fee_level": 0,
                     "email_verified": true,
@@ -766,32 +778,36 @@
                     "can_withdraw": true
                 }
             }
         """
         url = self._endpoint + "/withdraws/chance"
         params = {
             "currency": currency,
+            "net_type": net_type,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, params=params, **kwargs)
 
     def create_withdraw_coin(self,
                              currency: str,
+                             *,
+                             net_type: str,
                              amount: str,
                              address: str,
                              secondary_address: Optional[str] = None,
                              transaction_type: TransactionType = 'default',
                              **kwargs) -> Response:
-        """코인 출금하기
+        """디지털 자산 출금하기
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EC%BD%94%EC%9D%B8-%EC%B6%9C%EA%B8%88%ED%95%98%EA%B8%B0>`_
 
         :param currency: Currency 코드
+        :param net_type: 출금 네트워크
         :param amount: 출금 수량
         :param address: 출금 가능 주소에 등록된 출금 주소
         :param secondary_address: 2차 출금 주소 (필요한 코인에 한해서)
         :param transaction_type: 출금 유형. default: 일반출금, internal: 바로출금
         :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
 
         :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
@@ -799,45 +815,48 @@
         :return: API 서버 응답
 
         Usage::
 
             access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
-            res = upbit.create_withdraw_coin('BTC', '0.01', '1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa')
+            res = upbit.create_withdraw_coin('BTC', net_type='BTC', amount='0.01', address='1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa')
             print(res.json())
 
             {
                 "type": "withdraw",
                 "uuid": "9f432943-54e0-40b7-825f-b6fec8b42b79",
                 "currency": "BTC",
+                "net_type": "BTC",
                 "txid": "ebe6937b-130e-4066-8ac6-4b0e67f28adc",
                 "state": "processing",
                 "created_at": "2018-04-13T11:24:01+09:00",
                 "done_at": null,
                 "amount": "0.01",
                 "fee": "0.0",
                 "krw_amount": "80420.0",
                 "transaction_type": "default"
             }
         """
         url = self._endpoint + "/withdraws/coin"
         params = {
             "currency": currency,
+            "net_type": net_type,
             "amount": amount,
             "address": address,
             "secondary_address": secondary_address,
             "transaction_type": transaction_type,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('post', url, headers=headers, json=params, **kwargs)
 
     def create_withdraw_krw(self,
                             amount: str,
+                            *,
                             two_factor_type: TwoFactorType = 'kakao_pay',
                             **kwargs) -> Response:
         """원화 출금하기
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EC%9B%90%ED%99%94-%EC%B6%9C%EA%B8%88%ED%95%98%EA%B8%B0>`_
 
@@ -875,36 +894,70 @@
             "amount": amount,
             "two_factor_type": two_factor_type,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('post', url, headers=headers, json=params, **kwargs)
 
+    def get_withdraw_addresses(self,
+                               **kwargs) -> Response:
+        """출금 허용 주소 리스트 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%EC%B6%9C%EA%B8%88%ED%97%88%EC%9A%A9%EC%A3%BC%EC%86%8C-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%A1%B0%ED%9A%8C>`_
+
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_withdraw_addresses()
+            print(res.json())
+
+            [{
+                "currency": "BTC",
+                "net_type": "BTC",
+                "withdraw_address": "1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa",
+                "secondary_address": null
+            }, ...]
+        """
+        url = self._endpoint + "/withdraws/coin_addresses"
+        headers = self._get_request_headers(headers=kwargs.pop('headers', None))
+
+        return self._request('get', url, headers=headers, **kwargs)
+
     # --------------------------------------------------------------------------
     # Exchange API > 입금
     # --------------------------------------------------------------------------
 
     def get_deposits(self,
+                     *,
                      currency: Optional[str] = None,
-                     state: Optional[TransactionStatus] = None,
+                     state: Optional[DepositState] = None,
                      uuids: Optional[list[str]] = None,
                      txids: Optional[list[str]] = None,
                      page: int = 1,
                      limit: int = 100,
                      order_by: OrderBy = 'desc',
                      **kwargs) -> Response:
         """입금 리스트 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EC%9E%85%EA%B8%88-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%A1%B0%ED%9A%8C>`_
 
         :param currency: Currency 코드
-        :param state: 출금 상태
-        :param uuids: 출금 UUID 리스트
-        :param txids: 출금 TXID 리스트
+        :param state: 입금 상태
+        :param uuids: 입금 UUID 리스트
+        :param txids: 입금 TXID 리스트
         :param page: 페이지 수
         :param limit: 개수 제한 (default: 100, max: 100)
         :param order_by: 정렬 방식
         :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
 
         :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
 
@@ -918,14 +971,15 @@
             res = upbit.get_deposits(currency='KRW')
             print(res.json())
 
             [{
                 "type": "deposit",
                 "uuid": "94332e99-3a87-4a35-ad98-28b0c969f830",
                 "currency": "KRW",
+                "net_type": None,
                 "txid": "9e37c537-6849-4c8b-a134-57313f5dfc5a",
                 "state": "ACCEPTED",
                 "created_at": "2017-12-08T15:38:02+09:00",
                 "done_at": "2017-12-08T15:38:02+09:00",
                 "amount": "100000.0",
                 "fee": "0.0",
                 "transaction_type": "default"
@@ -942,14 +996,15 @@
             "order_by": order_by,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, params=params, **kwargs)
 
     def get_deposit(self,
+                    *,
                     uuid: Optional[str] = None,
                     txid: Optional[str] = None,
                     currency: Optional[str] = None,
                     **kwargs) -> Response:
         """개별 입금 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
@@ -965,21 +1020,22 @@
         :return: API 서버 응답
 
         Usage::
 
             access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
-            res = upbit.get_deposit('94332e99-3a87-4a35-ad98-28b0c969f830')
+            res = upbit.get_deposit(uuid='94332e99-3a87-4a35-ad98-28b0c969f830')
             print(res.json())
 
             {
                 "type": "deposit",
                 "uuid": "94332e99-3a87-4a35-ad98-28b0c969f830",
                 "currency": "KRW",
+                "net_type": None,
                 "txid": "9e37c537-6849-4c8b-a134-57313f5dfc5a",
                 "state": "ACCEPTED",
                 "created_at": "2017-12-08T15:38:02+09:00",
                 "done_at": "2017-12-08T15:38:02+09:00",
                 "amount": "100000.0",
                 "fee": "0.0",
                 "transaction_type": "default"
@@ -993,43 +1049,47 @@
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, params=params, **kwargs)
 
     def create_coin_address(self,
                             currency: str,
+                            *,
+                            net_type: str,
                             **kwargs) -> Response:
         """입금 주소 생성 요청
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EC%9E%85%EA%B8%88-%EC%A3%BC%EC%86%8C-%EC%83%9D%EC%84%B1-%EC%9A%94%EC%B2%AD>`_
 
         :param currency: Currency 코드
+        :param net_type: 입금 네트워크
         :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
 
         :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
 
         :return: API 서버 응답
 
         Usage::
 
             access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
-            res = upbit.create_coin_address('BTC')
+            res = upbit.create_coin_address('BTC', net_type='BTC')
             print(res.json())
 
             {
               "success": true,
               "message": "BTC 입금주소를 생성중입니다."
             }
         """
         url = self._endpoint + "/deposits/generate_coin_address"
         params = {
             "currency": currency,
+            "net_type": net_type,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('post', url, headers=headers, json=params, **kwargs)
 
     def get_coin_addresses(self,
                            **kwargs) -> Response:
@@ -1050,62 +1110,69 @@
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
             res = upbit.get_coin_addresses()
             print(res.json())
 
             [{
                 "currency": "BTC",
+                "net_type": "BTC",
                 "deposit_address": "3EusRwybuZUhVDeHL7gh3HSLmbhLcy7NqD",
                 "secondary_address": null
             }, ...]
         """
         url = self._endpoint + "/deposits/coin_addresses"
         headers = self._get_request_headers(headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, **kwargs)
 
     def get_coin_address(self,
                          currency: str,
+                         *,
+                         net_type: str,
                          **kwargs) -> Response:
         """개별 입금 주소 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EA%B0%9C%EB%B3%84-%EC%9E%85%EA%B8%88-%EC%A3%BC%EC%86%8C-%EC%A1%B0%ED%9A%8C>`_
 
         :param currency: Currency 코드
+        :param net_type: 입금 네트워크
         :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
 
         :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
 
         :return: API 서버 응답
 
         Usage::
 
             access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
-            res = upbit.get_coin_address('BTC')
+            res = upbit.get_coin_address('BTC', net_type='BTC')
             print(res.json())
 
             {
                 "currency": "BTC",
+                "net_type": "BTC",
                 "deposit_address": "3EusRwybuZUhVDeHL7gh3HSLmbhLcy7NqD",
                 "secondary_address": null
             }
         """
         url = self._endpoint + "/deposits/coin_address"
         params = {
             "currency": currency,
+            "net_type": net_type,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('get', url, headers=headers, params=params, **kwargs)
 
     def create_deposit_krw(self,
                            amount: str,
+                           *,
                            two_factor_type: TwoFactorType = 'kakao_pay',
                            **kwargs) -> Response:
         """원화 입금하기
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EC%9B%90%ED%99%94-%EC%9E%85%EA%B8%88%ED%95%98%EA%B8%B0>`_
 
@@ -1170,14 +1237,15 @@
             secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
             upbit = Upbit(access_key, secret_key)
             res = upbit.get_wallet_status()
             print(res.json())
 
             [{
                 'currency': 'BTC',
+                'net_type': 'BTC',
                 'wallet_state': 'working',
                 'block_state': 'normal',
                 'block_height': 776512,
                 'block_updated_at': '2023-02-14T13:37:39.806+00:00',
                 'block_elapsed_minutes': 12
             }, ...]
         """
@@ -1220,15 +1288,15 @@
     # --------------------------------------------------------------------------
     # Quotation API > 시세 종목 조회
     # --------------------------------------------------------------------------
 
     def get_markets(self,
                     is_detail: bool = False,
                     **kwargs) -> Response:
-        """거래 가능한 마켓 목록 조회
+        """마켓 코드 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EB%A7%88%EC%BC%93-%EC%BD%94%EB%93%9C-%EC%A1%B0%ED%9A%8C>`_
 
         :param is_detail: 유의종목 필드과 같은 상세 정보 노출 여부
         :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
 
@@ -1257,14 +1325,15 @@
     # --------------------------------------------------------------------------
     # Quotation API > 시세 캔들 조회
     # --------------------------------------------------------------------------
 
     def get_candles_minute(self,
                            unit: MinuteUnit,
                            market: str,
+                           *,
                            to: Optional[str] = None,
                            count: Optional[int] = None,
                            **kwargs) -> Response:
         """분(Minute) 캔들 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EB%B6%84minute-%EC%BA%94%EB%93%A4-1>`_
@@ -1304,14 +1373,15 @@
             "count": count,
         }
 
         return self._request('get', url, params=params, **kwargs)
 
     def get_candles_day(self,
                         market: str,
+                        *,
                         to: Optional[str] = None,
                         count: Optional[int] = None,
                         converting_price_unit: Optional[str] = None,
                         **kwargs) -> Response:
         """일(Day) 캔들 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
@@ -1356,14 +1426,15 @@
             "convertingPriceUnit": converting_price_unit,
         }
 
         return self._request('get', url, params=params, **kwargs)
 
     def get_candles_week(self,
                          market: str,
+                         *,
                          to: Optional[str] = None,
                          count: Optional[int] = None,
                          **kwargs) -> Response:
         """주(Week) 캔들 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EC%A3%BCweek-%EC%BA%94%EB%93%A4-1>`_
@@ -1402,14 +1473,15 @@
             "count": count,
         }
 
         return self._request('get', url, params=params, **kwargs)
 
     def get_candles_month(self,
                           market: str,
+                          *,
                           to: Optional[str] = None,
                           count: Optional[int] = None,
                           **kwargs) -> Response:
         """월(Month) 캔들 조회
 
         API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
         `Upbit API Doc <https://docs.upbit.com/reference/%EC%9B%94month-%EC%BA%94%EB%93%A4-1>`_
@@ -1452,14 +1524,15 @@
 
     # --------------------------------------------------------------------------
     # Quotation API > 시세 체결 조회
     # --------------------------------------------------------------------------
 
     def get_trades_ticks(self,
                          market: str,
+                         *,
                          to: Optional[str] = None,
                          count: Optional[int] = None,
                          cursor: Optional[str] = None,
                          days_ago: Optional[Literal[1, 2, 3, 4, 5, 6, 7]] = None,
                          **kwargs) -> Response:
         """최근 체결 내역 조회
```

