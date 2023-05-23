# Comparing `tmp/climeon-1.2.2.tar.gz` & `tmp/climeon-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climeon-1.2.2.tar", last modified: Thu Apr  6 14:40:49 2023, max compression
+gzip compressed data, was "climeon-1.3.0.tar", last modified: Tue May 23 15:03:35 2023, max compression
```

## Comparing `climeon-1.2.2.tar` & `climeon-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 14:40:49.881736 climeon-1.2.2/
--rw-rw-rw-   0        0        0      580 2023-04-06 14:40:49.879705 climeon-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-04-06 14:40:30.000000 climeon-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 14:40:49.853700 climeon-1.2.2/climeon/
--rw-rw-rw-   0        0        0       88 2023-04-06 14:40:30.000000 climeon-1.2.2/climeon/__init__.py
--rw-rw-rw-   0        0        0    27566 2023-04-06 14:40:22.000000 climeon-1.2.2/climeon/api.py
--rw-rw-rw-   0        0        0     2085 2023-04-06 14:40:22.000000 climeon-1.2.2/climeon/identifiers.py
--rw-rw-rw-   0        0        0    10921 2023-04-06 14:40:22.000000 climeon-1.2.2/climeon/plotting.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:40:49.871709 climeon-1.2.2/climeon.egg-info/
--rw-rw-rw-   0        0        0      580 2023-04-06 14:40:48.000000 climeon-1.2.2/climeon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-06 14:40:49.000000 climeon-1.2.2/climeon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 14:40:48.000000 climeon-1.2.2/climeon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-04-06 14:40:48.000000 climeon-1.2.2/climeon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-06 14:40:48.000000 climeon-1.2.2/climeon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 14:40:49.883708 climeon-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      896 2023-04-06 14:40:30.000000 climeon-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:03:35.665106 climeon-1.3.0/
+-rw-rw-rw-   0        0        0      580 2023-05-23 15:03:35.663092 climeon-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-05-23 15:03:16.000000 climeon-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 15:03:35.639536 climeon-1.3.0/climeon/
+-rw-rw-rw-   0        0        0       88 2023-05-23 15:03:16.000000 climeon-1.3.0/climeon/__init__.py
+-rw-rw-rw-   0        0        0    28844 2023-05-23 15:02:53.000000 climeon-1.3.0/climeon/api.py
+-rw-rw-rw-   0        0        0     2085 2023-05-23 15:02:53.000000 climeon-1.3.0/climeon/identifiers.py
+-rw-rw-rw-   0        0        0    10745 2023-05-23 15:02:53.000000 climeon-1.3.0/climeon/plotting.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:03:35.656873 climeon-1.3.0/climeon.egg-info/
+-rw-rw-rw-   0        0        0      580 2023-05-23 15:03:34.000000 climeon-1.3.0/climeon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-23 15:03:35.000000 climeon-1.3.0/climeon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 15:03:34.000000 climeon-1.3.0/climeon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-05-23 15:03:34.000000 climeon-1.3.0/climeon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 15:03:34.000000 climeon-1.3.0/climeon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 15:03:35.666095 climeon-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      896 2023-05-23 15:03:16.000000 climeon-1.3.0/setup.py
```

### Comparing `climeon-1.2.2/PKG-INFO` & `climeon-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climeon
-Version: 1.2.2
+Version: 1.3.0
 Summary: Climeon API client
 Home-page: UNKNOWN
 Author: Emil Hjelm
 Author-email: emil.hjelm@climeon.com
 License: MIT
 Keywords: climeon,REST,API
 Platform: UNKNOWN
```

### Comparing `climeon-1.2.2/climeon/api.py` & `climeon-1.3.0/climeon/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 import dateparser
 import msal
 import numpy as np
 import pandas as pd
 import requests
 
 # Climeon modules
-from .identifiers import powerblock, module, hp_system
+try:
+    from .identifiers import powerblock, module, hp_system
+except ImportError:
+    # Expected import error during autosummary documentation import
+    from identifiers import powerblock, module, hp_system
 
 # Check for parquet support
 try:
     pd.io.parquet.get_engine("auto")
     PARQUET_SUPPORT = True
 except ImportError:
     PARQUET_SUPPORT = False
@@ -44,14 +48,15 @@
 CLIENT_ID = "fe8152ab-d22c-4f61-9a24-17bb397bee75"
 AUTHORITY = "https://climeonlive.b2clogin.com/climeonlive.onmicrosoft.com/"
 POLICY_ROPC = "B2C_1_ropc"
 POLICY_SIGN_IN = "B2C_1_SignIn"
 AUTHORITY_SIGN_IN = AUTHORITY + POLICY_SIGN_IN
 AUTHORITY_ROPC = AUTHORITY + POLICY_ROPC
 MSAL_SCOPE = ["https://climeonlive.onmicrosoft.com/backend/read"]
+MSAL_TOKEN = ""
 
 # Offline cache settings
 BASE_FOLDER = getenv("APPDATA", gettempdir())
 OFFLINE_FOLDER = path.join(BASE_FOLDER, "ClimeonLive")
 OFFLINE_NAME = "%s_%s_%s_%s_%s"
 FOLDER_SIZE_LIMIT = 2*1024*1024*1024
 
@@ -95,26 +100,31 @@
     # pylint: disable=too-many-public-methods
 
     def __init__(self, user=None, passwd=None, prod=True, plotly=True):
         self.logger = getLogger(__name__)
         self.user = user or getenv("API_USER")
         self.passwd = passwd or getenv("API_PASS")
         self.url = PROD_URL if prod else DEV_URL
-        self.headers = {"authorization": ""}
+        self.session = requests.Session()
         ropc = self.user and self.passwd
         authority = AUTHORITY_ROPC if ropc else AUTHORITY_SIGN_IN
         self.app = msal.PublicClientApplication(CLIENT_ID,
                                                 authority=authority,
                                                 validate_authority=False)
         if plotly:
             pd.options.plotting.backend = "plotly"
-        self.login()
+        if MSAL_TOKEN:
+            self.headers = {"authorization": MSAL_TOKEN}
+        else:
+            self.headers = {"authorization": ""}
+            self.login()
 
     def login(self):
         """Logs in the user to Climeon API."""
+        global MSAL_TOKEN # pylint: disable=global-statement
         result = None
         if self.user and self.passwd:
             self.logger.debug("Logging in with user %s", self.user)
             result = self.app.acquire_token_by_username_password(self.user,
                                                                  self.passwd,
                                                                  MSAL_SCOPE)
         else:
@@ -135,14 +145,15 @@
                 disable(0) # Enable logging again
                 self.fallback_login()
                 return
         if "error" in result:
             raise Exception(result["error_description"])
         token = result["access_token"]
         auth = f"Bearer {token}"
+        MSAL_TOKEN = auth
         self.headers = {"authorization": auth}
 
     def fallback_login(self):
         """Fallback in case interactive MSAL login can't be used."""
         self.logger.warning("Falling back on python input")
         self.user = input("Climeon live user email: ")
         self.passwd = getpass("Password: ")
@@ -152,53 +163,52 @@
         self.login()
 
     def _http(self, method, endpoint, body, retry):
         headers = self.headers
         if body:
             headers["Content-Type"] = "application/json-patch+json"
             headers["accept"] = "text/plain"
-        res = method(endpoint, headers=headers, data=body)
+        res = self.session.request(method, endpoint, headers=headers, data=body)
         auth_fail = res.text.startswith(AUTH_FAIL) or res.status_code == 401
         if auth_fail and retry:
             self.login()
             return self._http(method, endpoint, body, False)
         if not res.ok:
             raise Exception(res.text)
         return res
 
     def get(self, endpoint):
         """General purpose GET method."""
         req_url = self.url + endpoint
-        return self._http(requests.get, req_url, None, True)
+        return self._http("GET", req_url, None, True)
 
     def post(self, endpoint, body):
         """General purpose POST method."""
         req_url = self.url + endpoint
         json_body = json.dumps(body)
-        return self._http(requests.post, req_url, json_body, True)
+        return self._http("POST", req_url, json_body, True)
 
 
     # Analytics
 
     def analytics(self, machine_id, date_from, date_to, variables=None, interval=None):
         """Get aggregated logfile data from the Analytics database.
 
         Parameters:
-            machine_id (str): module or powerblock id e.g. "0100000016".
+            machine_id (str): Module or powerblock id e.g. "0100000016".
             date_from (str, datetime): Datetime to get data from.
             date_to (str, datetime): Datetime to get data to.
             variables (list, optional): Variables to get. Defaults to all
                                         available variables.
             interval (str, optional): Interval size specified in ISO-8601
                                       duration format:
                                       https://en.wikipedia.org/wiki/ISO_8601
                                       Defaults to a reasonable interval.
                                       Can be any of
-                                      ``["PT1S", "PT10S", "PT1M", "PT10M", \
-                                         "PT1H", "PT12H", "PT24H"]``.
+                                      ``"PT1S", "PT10S", "PT1M", "PT10M", "PT1H", "PT12H", "PT24H"``
 
         Returns:
             DataFrame: A Pandas DataFrame.
         """
         # pylint: disable=too-many-arguments,too-many-locals
         date_from = parse_datetime(date_from)
         date_to = parse_datetime(date_to)
@@ -234,17 +244,20 @@
         raw_data = response.json()
         dataframe = json_to_dataframe(raw_data[machine_id])
         if dataframe.empty:
             self.logger.warning("No data found for %s between %s and %s",
                                 machine_id, date_from, date_to)
             return dataframe
         dataframe = format_dataframe(dataframe, date_from.tzinfo, False)
-        rec_int = (dataframe.index[1] - dataframe.index[0]).total_seconds()
+        if len(dataframe.index) > 1:
+            rec_int = (dataframe.index[1] - dataframe.index[0]).total_seconds()
+        else:
+            rec_int = SQL_INTERVALS[interval]
         if SQL_INTERVALS[interval] < rec_int:
-            int_str = next(i for i, v in SQL_INTERVALS.items() if v >= rec_int)
+            int_str = next((i for i, v in SQL_INTERVALS.items() if v >= rec_int), "PT24H")
             self.logger.warning("Requested interval %s could not be fetched, "
                                 "got interval %s instead. Use logfile data to "
                                 "get higher resolution.", interval, int_str)
         else:
             int_str = interval
         pandas_interval = int_str[2:].replace("M", "T")
         dataframe = dataframe.resample(pandas_interval).first()
@@ -347,14 +360,31 @@
             var = instance_type["variables"]
         else:
             var = {k: v for k, v in instance_type["variables"].items() if k in variables}
         interval = interval or default_tsi_interval(date_from, date_to)
         return self.tsi_query(machine_id, date_from, date_to, var, interval)
 
 
+    # Config
+
+    def config_query(self, query):
+        """Get config history for a specific module/powerblock or config name."""
+        endpoint = f"/Config/{query}"
+        response = self.get(endpoint)
+        return response.json()
+
+    def config_changes(self, machine_id=None):
+        """Get config changes for specified machine."""
+        endpoint = "/Config/changes"
+        if machine_id:
+            endpoint += f"/{machine_id}"
+        response = self.get(endpoint)
+        return response.json()
+
+
     # Modules
 
     def modules(self):
         """Get info for all registered modules."""
         response = self.get("/Modules")
         return response.json()
 
@@ -497,40 +527,43 @@
         """Get logfile for a machine/date.
 
         Parameters:
             machine_id (str): module or powerblock id e.g. "0100000016".
             date_from (str, datetime): Datetime to get data from.
             date_to (str, datetime, optional): Datetime to get data to.
             variables (list, optional): List of strings with variable names.
+                                        Defaults to all available variables.
                                         Any other variables will be dropped.
                                         Useful if a long timerange is used to
                                         not exhaust memory.
 
         Returns:
             DataFrame: A Pandas DataFrame.
         """
         date_from = parse_datetime(date_from)
         date_to = parse_datetime(date_to)
-        date_to = date_to or date_from + timedelta(days=1)
-        if date_to.date() <= date_from.date():
+        if date_to is None or date_to.date() == date_from.date():
+            date_to = date_from + timedelta(days=1)
+        if date_to.date() < date_from.date():
             raise ValueError("Start date must be earlier than end date.")
         filename = offline_name(machine_id, date_from.date(), date_to.date(),
                                 variables, "")
         dataframe = load_dataframe(filename)
         if not dataframe is None:
             return dataframe
         if variables is not None:
             variables = list(set(variables + ["Timestamp", "Timestamp UTC [-]"]))
         diff = date_to - date_from
         date_list = [date_from + timedelta(days=d) for d in range(diff.days)]
         for date in date_list:
             try:
                 data_str = self.logfile_raw(machine_id, date)
             except Exception: # pylint: disable=broad-except
-                self.logger.warning("No logfile found for date %s", date)
+                self.logger.warning("No logfile found for %s on date %s",
+                                    machine_id, date.date())
                 continue
             header_idx = data_str.index("Timestamp")
             dateframe = pd.read_csv(StringIO(data_str[header_idx:]))
             if variables:
                 drop_var = [c for c in dateframe.columns if c not in variables]
                 dateframe = dateframe.drop(drop_var, axis=1)
             dateframe = format_dataframe(dateframe, date_from.tzinfo)
@@ -611,16 +644,16 @@
     dataframe = pd.DataFrame(data, columns=columns)
     return dataframe
 
 def format_dataframe(dataframe, original_tz, resample=True):
     """Clean up and properly timestamp dataframe."""
     dataframe = dataframe.loc[:, ~dataframe.columns.str.contains("^Unnamed")]
     ts_1 = parse_datetime(dataframe["Timestamp"][0])
-    ts_2 = parse_datetime(dataframe["Timestamp"][1])
-    if ts_2 - ts_1 < timedelta(seconds=0.5):
+    ts_2 = parse_datetime(dataframe["Timestamp"][1]) if len(dataframe.index) > 1 else None
+    if ts_2 is not None and ts_2 - ts_1 < timedelta(seconds=0.5):
         # Blackbox file, need to use Timestamp column to maintain resolution
         utc_1 = parse_datetime(dataframe["Timestamp UTC [-]"][0])
         utc_offset = ts_1 - utc_1
         dataframe["Timestamp"] = pd.to_datetime(dataframe["Timestamp"])
         dataframe["Timestamp"] = dataframe["Timestamp"] + utc_offset
     elif "Timestamp UTC [-]" in dataframe:
         dataframe["Timestamp"] = pd.to_datetime(dataframe["Timestamp UTC [-]"],
```

### Comparing `climeon-1.2.2/climeon/identifiers.py` & `climeon-1.3.0/climeon/identifiers.py`

 * *Files identical despite different names*

### Comparing `climeon-1.2.2/climeon/plotting.py` & `climeon-1.3.0/climeon/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # External modules
 from pandas import DataFrame
 from plotly.graph_objects import Scattergl
 from plotly.subplots import make_subplots
 from plotly_resampler import FigureResampler, FigureWidgetResampler, \
     EveryNthPoint
 
+DEFAULT_HEIGHT = 900
+
 STATES = [
     "INIT",
     "IDLE",
     "READY",
     "START",
     "RUNNING",
     "STOP",
@@ -74,20 +76,26 @@
     "", # EXHAUST_VALVE_OPEN
     "", # VACANT
     "", # VACANT
     "", # VACANT
     "REMOTE_CONTROL"
 ]
 
-def add_transition(fig, data, variable, color, states, template, pos):
+STATE_MAP = {
+    "State [-]": STATES,
+    "StartState [-]": START_STATES,
+    "StatusWord [-]": STATUS_WORD
+}
+
+def add_transition(fig, data, variable, color="blue", template="%s", pos=1):
     """Add status transitions for a specific variable in a plotly figure."""
     # pylint: disable=too-many-arguments
     if variable not in data:
         return
-    template = template or "%s"
+    states = STATE_MAP[variable] if variable in STATE_MAP else None
     edges = data[abs(data[variable].diff()) > 0][variable].astype(int)
     for idx, (timestamp, state) in enumerate(zip(edges.index, edges)):
         if state == 0:
             continue
         if variable in ["StatusWord [-]", "SecondaryStatusWord [-]"] and idx > 0:
             bit = int(state ^ edges[idx-1]).bit_length() - 1
             if not (state >> bit) & 1 or not states[bit]:
@@ -108,24 +116,21 @@
     """Add all possible state transitions.
 
     Parameters:
         fig (figure):       A plotly figure.
         data (DataFrame):   A pandas dataframe with data.
     """
     # pylint: disable=too-many-arguments
-    add_transition(fig, data, "State [-]", "blue", STATES, None, 0.96)
-    #add_transition(fig, data, "StartState [-]", "green", START_STATES, None, 0.96)
-    add_transition(fig, data, "AlarmCode [-]", "red", None, "AlarmCode %s", 1.04)
-    add_transition(fig, data, "NoOfGreasingCyclesFrontBearing [-]", "blue",
-                   None, "Front greasing", 1)
-    add_transition(fig, data, "NoOfGreasingCyclesRearBearing [-]", "blue",
-                   None, "Rear greasing", 1)
-    add_transition(fig, data, "NoOfAtuCycles [-]", "green", None, "ATU", 1)
+    add_transition(fig, data, "State [-]", pos=0.96)
+    add_transition(fig, data, "AlarmCode [-]", "red", "AlarmCode %s", 1.04)
+    add_transition(fig, data, "NoOfGreasingCyclesFrontBearing [-]", template="Front greasing")
+    add_transition(fig, data, "NoOfGreasingCyclesRearBearing [-]", template="Rear greasing")
+    add_transition(fig, data, "NoOfAtuCycles [-]", "green", "ATU", 1.02)
     if "State [-]" not in data:
-        add_transition(fig, data, "StatusWord [-]", "blue", STATUS_WORD, None, 0.96)
+        add_transition(fig, data, "StatusWord [-]", pos=0.96)
     if "Wetgas detected [-]" in data:
         color_code(fig, data["Wetgas detected [-]"], [None, "red"])
     elif "SecondaryStatusWord [-]" in data:
         wet_gas = (data["SecondaryStatusWord [-]"].dropna().astype(int) & (1 << 10) > 0) * 1
         color_code(fig, wet_gas, [None, "red"])
 
 def color_code(fig, state, colors, text=""):
@@ -138,20 +143,20 @@
         else:
             end_idx = state_changes.index[idx + 1]
         color = colors[int(state_changes[timestamp])]
         if color is not None:
             fig.add_vrect(timestamp, end_idx, annotation_text=text,
                           fillcolor=color, opacity=0.2, line_width=0)
 
-def get_figure(rows=1, secondary_y=True, resampler=True, height=900):
+def get_figure(rows=1, secondary_y=True, resampler=False, height=DEFAULT_HEIGHT):
     """Convenience function for creating a plotly figure.
 
     Parameters:
         rows (int): Amount of plot rows to include (subplots).
-        secondary_y (bool):
+        secondary_y (bool): Indicates if secondary y-axis should be enabled.
         resampler (bool): Indicates if resampling should be done dynamically
                           to improve loading times.
         height (int): Figure height.
     """
     specs = [[{"secondary_y": secondary_y}] for _ in range(rows)]
     fig = make_subplots(rows, 1, shared_xaxes=True, vertical_spacing=0.02, specs=specs)
     if resampler:
@@ -159,33 +164,29 @@
             fig = FigureWidgetResampler(fig)
         else:
             fig = FigureResampler(fig)
     fig.update_layout(hovermode="x", height=height)
     fig.update_traces(mode="lines", hovertemplate=None)
     return fig
 
-def standard_plot(data, resampler=True):
+def standard_plot(data, resampler=True, height=DEFAULT_HEIGHT):
     """Create a plot with state transitions and useful variables."""
     # pylint: disable=too-many-statements
-    fig = get_figure(rows=2, resampler=resampler)
-    fig.update_layout(hovermode="x", height=900)
-    fig.update_traces(mode="lines", hovertemplate=None)
+    fig = get_figure(rows=2, resampler=resampler, height=height)
 
     # 1st plot: Power and Control with state transitions
-    # 1st axis [kW], [krpm]
+    # 1st axis [kW], [%]
     add_trace(fig, data, "PowerOutput [kW]", 1)
-    if "TurbSpeed [rpm]" in data:
-        data["TurbSpeed [krpm]"] = data["TurbSpeed [rpm]"] / 1000
-        add_trace(fig, data, "TurbSpeed [krpm]", 1)
-
-    # 2nd axis [%]
-    add_trace(fig, data, "AV25Pos [%]", 1, secondary_y=True)
-    add_trace(fig, data, "AV26Pos [%]", 1, secondary_y=True)
-    add_trace(fig, data, "Fcp91Speed [%]", 1, secondary_y=True)
-    add_trace(fig, data, "Fcp92Speed [%]", 1, secondary_y=True)
+    add_trace(fig, data, "AV25Pos [%]", 1)
+    add_trace(fig, data, "AV26Pos [%]", 1)
+    add_trace(fig, data, "Fcp91Speed [%]", 1)
+    add_trace(fig, data, "Fcp92Speed [%]", 1)
+
+    # 2nd axis [rpm]
+    add_trace(fig, data, "TurbSpeed [rpm]", 1, secondary_y=True)
 
     # 2nd plot: Variables galore
     # 1st axis [deg C]
 
     # Hot side
     add_trace(fig, data, "T38 [deg C]", 2, visible="legendonly")
     add_trace(fig, data, "T39 [deg C]", 2, visible="legendonly")
@@ -236,27 +237,27 @@
     add_trace(fig, data, "Cushion [bar]", 2, visible="legendonly", secondary_y=True)
     add_trace(fig, data, "P71 [bar]", 2, visible="legendonly", secondary_y=True)
     add_trace(fig, data, "CX DP water [bar]", 2, visible="legendonly", secondary_y=True)
     add_trace(fig, data, "CX DP media [bar]", 2, visible="legendonly", secondary_y=True)
     add_trace(fig, data, "FCP91 DP [bar]", 2, visible="legendonly", secondary_y=True)
     add_trace(fig, data, "Condenser DP [bar]", 2, visible="legendonly", secondary_y=True)
 
-    fig["layout"]["yaxis"]["title"] = "[kW], [krpm]"
-    fig["layout"]["yaxis2"]["title"] = "[%]"
+    fig["layout"]["yaxis"]["title"] = "[kW], [%]"
+    fig["layout"]["yaxis2"]["title"] = "[rpm]"
     fig["layout"]["yaxis2"]["showgrid"] = False
     fig["layout"]["yaxis2"]["zeroline"] = False
     fig["layout"]["yaxis3"]["title"] = "[deg C]"
     fig["layout"]["yaxis4"]["title"] = "[bar], [-]"
     fig["layout"]["yaxis4"]["showgrid"] = False
     fig["layout"]["yaxis4"]["zeroline"] = False
 
     add_transitions(fig, data)
     return fig
 
-def add_trace(fig, data, variable, row, visible=None, secondary_y=False):
+def add_trace(fig, data, variable, row=1, visible=None, secondary_y=False):
     """Add a trace to a resampled plotly figure."""
     # pylint: disable=too-many-arguments
     if not variable in data:
         return
     if isinstance(fig, FigureWidgetResampler):
         trace = Scattergl(name=variable, visible=visible)
         fig.add_trace(trace, row=row, col=1, secondary_y=secondary_y,
```

### Comparing `climeon-1.2.2/climeon.egg-info/PKG-INFO` & `climeon-1.3.0/climeon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climeon
-Version: 1.2.2
+Version: 1.3.0
 Summary: Climeon API client
 Home-page: UNKNOWN
 Author: Emil Hjelm
 Author-email: emil.hjelm@climeon.com
 License: MIT
 Keywords: climeon,REST,API
 Platform: UNKNOWN
```

### Comparing `climeon-1.2.2/setup.py` & `climeon-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
 00000010: 7320 696d 706f 7274 2073 6574 7570 2c20  s import setup, 
 00000020: 6669 6e64 5f70 6163 6b61 6765 730d 0a0d  find_packages...
 00000030: 0a73 6574 7570 280d 0a20 2020 206e 616d  .setup(..    nam
 00000040: 653d 2263 6c69 6d65 6f6e 222c 0d0a 2020  e="climeon",..  
 00000050: 2020 7061 636b 6167 6573 3d66 696e 645f    packages=find_
 00000060: 7061 636b 6167 6573 2829 2c0d 0a20 2020  packages(),..   
-00000070: 2076 6572 7369 6f6e 3d22 312e 322e 3222   version="1.2.2"
+00000070: 2076 6572 7369 6f6e 3d22 312e 332e 3022   version="1.3.0"
 00000080: 2c0d 0a20 2020 206c 6963 656e 7365 3d22  ,..    license="
 00000090: 4d49 5422 2c0d 0a20 2020 2064 6573 6372  MIT",..    descr
 000000a0: 6970 7469 6f6e 3d22 436c 696d 656f 6e20  iption="Climeon 
 000000b0: 4150 4920 636c 6965 6e74 222c 0d0a 2020  API client",..  
 000000c0: 2020 6c6f 6e67 5f64 6573 6372 6970 7469    long_descripti
 000000d0: 6f6e 3d22 436c 696d 656f 6e20 4150 4920  on="Climeon API 
 000000e0: 636c 6965 6e74 222c 0d0a 2020 2020 6175  client",..    au
```

