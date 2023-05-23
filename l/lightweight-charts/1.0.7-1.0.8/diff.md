# Comparing `tmp/lightweight_charts-1.0.7.tar.gz` & `tmp/lightweight_charts-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweight_charts-1.0.7.tar", last modified: Sun May 21 14:46:21 2023, max compression
+gzip compressed data, was "lightweight_charts-1.0.8.tar", last modified: Tue May 23 13:32:25 2023, max compression
```

## Comparing `lightweight_charts-1.0.7.tar` & `lightweight_charts-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-21 14:46:21.784977 lightweight_charts-1.0.7/
--rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.7/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)     6202 2023-05-21 14:46:21.784636 lightweight_charts-1.0.7/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     5856 2023-05-20 15:23:42.000000 lightweight_charts-1.0.7/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-21 14:46:21.781636 lightweight_charts-1.0.7/lightweight_charts/
--rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.7/lightweight_charts/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     3034 2023-05-20 21:15:48.000000 lightweight_charts-1.0.7/lightweight_charts/chart.py
--rw-r--r--   0 louis      (501) staff       (20)    23947 2023-05-21 14:30:57.000000 lightweight_charts-1.0.7/lightweight_charts/js.py
--rw-r--r--   0 louis      (501) staff       (20)   148472 2023-05-20 23:46:07.000000 lightweight_charts-1.0.7/lightweight_charts/pkg.py
--rw-r--r--   0 louis      (501) staff       (20)     2083 2023-05-21 12:37:38.000000 lightweight_charts-1.0.7/lightweight_charts/util.py
--rw-r--r--   0 louis      (501) staff       (20)     1932 2023-05-20 19:56:58.000000 lightweight_charts-1.0.7/lightweight_charts/widgets.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-21 14:46:21.784136 lightweight_charts-1.0.7/lightweight_charts.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     6202 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      402 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-21 14:46:21.785082 lightweight_charts-1.0.7/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-21 14:35:24.000000 lightweight_charts-1.0.7/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-23 13:32:25.440313 lightweight_charts-1.0.8/
+-rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.8/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)     6202 2023-05-23 13:32:25.440021 lightweight_charts-1.0.8/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     5856 2023-05-20 15:23:42.000000 lightweight_charts-1.0.8/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-23 13:32:25.437186 lightweight_charts-1.0.8/lightweight_charts/
+-rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.8/lightweight_charts/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     3110 2023-05-23 13:04:15.000000 lightweight_charts-1.0.8/lightweight_charts/chart.py
+-rw-r--r--   0 louis      (501) staff       (20)    28575 2023-05-23 13:10:38.000000 lightweight_charts-1.0.8/lightweight_charts/js.py
+-rw-r--r--   0 louis      (501) staff       (20)   148472 2023-05-20 23:46:07.000000 lightweight_charts-1.0.8/lightweight_charts/pkg.py
+-rw-r--r--   0 louis      (501) staff       (20)     2083 2023-05-21 12:37:38.000000 lightweight_charts-1.0.8/lightweight_charts/util.py
+-rw-r--r--   0 louis      (501) staff       (20)     1932 2023-05-20 19:56:58.000000 lightweight_charts-1.0.8/lightweight_charts/widgets.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-23 13:32:25.439527 lightweight_charts-1.0.8/lightweight_charts.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     6202 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      402 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-23 13:32:25.000000 lightweight_charts-1.0.8/lightweight_charts.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-23 13:32:25.440428 lightweight_charts-1.0.8/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-23 13:30:34.000000 lightweight_charts-1.0.8/setup.py
```

### Comparing `lightweight_charts-1.0.7/LICENSE` & `lightweight_charts-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.7/PKG-INFO` & `lightweight_charts-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight_charts
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `lightweight_charts-1.0.7/README.md` & `lightweight_charts-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.7/lightweight_charts/chart.py` & `lightweight_charts-1.0.8/lightweight_charts/chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, q, exit, loaded, html, js_api, width, height, x, y, on_top, debug):
         self.queue = q
         self.exit = exit
         self.loaded = loaded
         self.debug = debug
         self.js_api = js_api
         self.webview = webview.create_window('', html=html, on_top=on_top, js_api=js_api,
-                                             width=width, height=height, x=x, y=y)
+                                             width=width, height=height, x=x, y=y, background_color='#000000')
         self.webview.events.loaded += self.on_js_load
         self.loop()
 
     def loop(self):
         while 1:
             arg = self.queue.get()
             if arg in ('start', 'show', 'hide', 'exit'):
@@ -34,16 +34,16 @@
     def on_js_load(self):
         self.loaded.set(), self.loop()
 
 
 class Chart(LWC):
     def __init__(self, volume_enabled: bool = True, width: int = 800, height: int = 600, x: int = None, y: int = None,
                  on_top: bool = False, debug: bool = False,
-                 inner_width: float = 1.0, inner_height: float = 1.0):
-        super().__init__(volume_enabled, inner_width, inner_height)
+                 inner_width: float = 1.0, inner_height: float = 1.0, dynamic_loading: bool = False):
+        super().__init__(volume_enabled, inner_width, inner_height, dynamic_loading)
         self._js_api_code = 'pywebview.api.onClick'
         self._q = mp.Queue()
         self._script_func = self._q.put
         self._exit = mp.Event()
         self._loaded = mp.Event()
         self._process = mp.Process(target=PyWV, args=(self._q, self._exit, self._loaded, self._html, self._js_api,
                                                       width, height, x, y, on_top, debug,), daemon=True)
```

### Comparing `lightweight_charts-1.0.7/lightweight_charts/js.py` & `lightweight_charts-1.0.8/lightweight_charts/js.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,41 +3,154 @@
 from typing import Union, Literal
 
 from lightweight_charts.pkg import LWC_4_0_1
 from lightweight_charts.util import LINE_STYLE, MARKER_POSITION, MARKER_SHAPE, CROSSHAIR_MODE, _crosshair_mode, _line_style, \
     MissingColumn, _js_bool, _price_scale_mode, PRICE_SCALE_MODE, _marker_position, _marker_shape, IDGen
 
 
-class Line:
+class SeriesCommon:
+    def _set_interval(self, df: pd.DataFrame):
+        common_interval = pd.to_datetime(df['time']).diff().value_counts()
+        self._interval = common_interval.index[0]
+
+    def _df_datetime_format(self, df: pd.DataFrame):
+        if 'date' in df.columns:
+            df = df.rename(columns={'date': 'time'})
+        self._set_interval(df)
+        # df['time'] = df['time'].apply(self._datetime_format)
+        df['time'] = self._datetime_format(df['time'])
+        return df
+
+    def _series_datetime_format(self, series):
+        if 'date' in series.keys():
+            series = series.rename({'date': 'time'})
+        series['time'] = self._datetime_format(series['time'])
+        return series
+
+    def _datetime_format(self, arg):
+        arg = pd.to_datetime(arg)
+        if self._interval != timedelta(days=1):
+            arg = arg.astype('int64') // 10 ** 9 if isinstance(arg, pd.Series) else arg.timestamp()
+            arg = self._interval.total_seconds() * (arg // self._interval.total_seconds())
+        else:
+            arg = arg.dt.strftime('%Y-%m-%d') if isinstance(arg, pd.Series) else arg.strftime('%Y-%m-%d')
+        return arg
+
+    def marker(self, time: datetime = None, position: MARKER_POSITION = 'below', shape: MARKER_SHAPE = 'arrow_up',
+               color: str = '#2196F3', text: str = '') -> str:
+        """
+        Creates a new marker.\n
+        :param time: The time that the marker will be placed at. If no time is given, it will be placed at the last bar.
+        :param position: The position of the marker.
+        :param color: The color of the marker (rgb, rgba or hex).
+        :param shape: The shape of the marker.
+        :param text: The text to be placed with the marker.
+        :return: The id of the marker placed.
+        """
+        try:
+            time = self._last_bar['time'] if not time else self._datetime_format(time)
+        except TypeError:
+            raise TypeError('Chart marker created before data was set.')
+        marker_id = self._rand.generate()
+        self.run_script(f"""
+            {self.id}.markers.push({{
+                time: {time if isinstance(time, float) else f"'{time}'"},
+                position: '{_marker_position(position)}',
+                color: '{color}',
+                shape: '{_marker_shape(shape)}',
+                text: '{text}',
+                id: '{marker_id}'
+                }});
+            {self.id}.series.setMarkers({self.id}.markers)""")
+        return marker_id
+
+    def remove_marker(self, marker_id: str):
+        """
+        Removes the marker with the given id.\n
+        """
+        self.run_script(f'''
+           {self.id}.markers.forEach(function (marker) {{
+               if ('{marker_id}' === marker.id) {{
+                   {self.id}.markers.splice({self.id}.markers.indexOf(marker), 1)
+                   {self.id}.series.setMarkers({self.id}.markers)
+                   }}
+               }});''')
+
+    def horizontal_line(self, price: Union[float, int], color: str = 'rgb(122, 146, 202)', width: int = 1,
+                        style: LINE_STYLE = 'solid', text: str = '', axis_label_visible=True):
+        """
+        Creates a horizontal line at the given price.\n
+        """
+        var = self._rand.generate()
+        self.run_script(f"""
+           let priceLine{var} = {{
+               price: {price},
+               color: '{color}',
+               lineWidth: {width},
+               lineStyle: {_line_style(style)},
+               axisLabelVisible: {_js_bool(axis_label_visible)},
+               title: '{text}',
+           }};
+           let line{var} = {{
+               line: {self.id}.series.createPriceLine(priceLine{var}),
+               price: {price},
+           }};
+           {self.id}.horizontal_lines.push(line{var})""")
+
+    def remove_horizontal_line(self, price: Union[float, int]):
+        """
+        Removes a horizontal line at the given price.
+        """
+        self.run_script(f'''
+           {self.id}.horizontal_lines.forEach(function (line) {{
+           if ({price} === line.price) {{
+               {self.id}.series.removePriceLine(line.line);
+               {self.id}.horizontal_lines.splice({self.id}.horizontal_lines.indexOf(line), 1)
+               }}
+           }});''')
+
+    def title(self, title: str):
+        self.run_script(f'{self.id}.series.applyOptions({{title: "{title}"}})')
+
+
+class Line(SeriesCommon):
     def __init__(self, parent, color, width):
         self._parent = parent
-        self.id = self._parent._rand.generate()
+        self._rand = self._parent._rand
+        self.id = self._rand.generate()
+        self.run_script = self._parent.run_script
+
         self._parent.run_script(f'''
-            var {self.id} = {self._parent.id}.chart.addLineSeries({{
-                color: '{color}',
-                lineWidth: {width},
-            }})''')
+            var {self.id} = {{
+                series: {self._parent.id}.chart.addLineSeries({{
+                    color: '{color}',
+                    lineWidth: {width},
+                }}),
+                markers: [],
+                horizontal_lines: [],
+            }}
+        ''')
 
     def set(self, data: pd.DataFrame):
         """
         Sets the line data.\n
         :param data: columns: date/time, value
         """
         df = self._parent._df_datetime_format(data)
-        self._parent.run_script(f'{self.id}.setData({df.to_dict("records")})')
+        self._last_bar = df.iloc[-1]
+        self.run_script(f'{self.id}.series.setData({df.to_dict("records")})')
 
     def update(self, series: pd.Series):
         """
         Updates the line data.\n
         :param series: labels: date/time, value
         """
         series = self._parent._series_datetime_format(series)
-        self._parent.run_script(f'{self.id}.update({series.to_dict()})')
-
-    def marker(self): pass
+        self._last_bar = series
+        self.run_script(f'{self.id}.series.update({series.to_dict()})')
 
 
 class API:
     def __init__(self):
         self.click_funcs = {}
 
     def onClick(self, data):
@@ -45,60 +158,37 @@
         if isinstance(data['time'], int):
             data['time'] = datetime.fromtimestamp(data['time'])
         else:
             data['time'] = datetime.strptime(data['time'], '%Y-%m-%d')
         click_func(data) if click_func else None
 
 
-class LWC:
-    def __init__(self, volume_enabled: bool = True, inner_width: float = 1.0, inner_height: float = 1.0):
+class LWC(SeriesCommon):
+    def __init__(self, volume_enabled: bool = True, inner_width: float = 1.0, inner_height: float = 1.0, dynamic_loading: bool = False):
         self._volume_enabled = volume_enabled
         self._inner_width = inner_width
         self._inner_height = inner_height
-        self._position = 'left'
-        self.loaded = False
+        self._dynamic_loading = dynamic_loading
+
         self._rand = IDGen()
         self.id = self._rand.generate()
+        self._position = 'left'
+        self.loaded = False
+        self._html = HTML
         self._append_js = f'document.body.append({self.id}.div)'
         self._scripts = []
         self._script_func = None
-        self._html = HTML
         self._last_bar = None
         self._interval = None
-        self._background_color = '#000000'
-        self._volume_up_color = 'rgba(83,141,131,0.8)'
-        self._volume_down_color = 'rgba(200,127,130,0.8)'
         self._js_api = API()
         self._js_api_code = None
 
-    def _set_interval(self, df: pd.DataFrame):
-        common_interval = pd.to_datetime(df['time']).diff().value_counts()
-        self._interval = common_interval.index[0]
-
-    def _df_datetime_format(self, df: pd.DataFrame):
-        if 'date' in df.columns:
-            df = df.rename(columns={'date': 'time'})
-        self._set_interval(df)
-        df['time'] = df['time'].apply(self._datetime_format)
-        return df
-
-    def _series_datetime_format(self, series):
-        if 'date' in series.keys():
-            series = series.rename({'date': 'time'})
-        series['time'] = self._datetime_format(series['time'])
-        return series
-
-    def _datetime_format(self, string):
-        string = pd.to_datetime(string)
-        if self._interval != timedelta(days=1):
-            string = string.timestamp()
-            string = self._interval.total_seconds() * (string // self._interval.total_seconds())
-        else:
-            string = string.strftime('%Y-%m-%d')
-        return string
+        self._background_color = '#000000'
+        self._volume_up_color = 'rgba(83,141,131,0.8)'
+        self._volume_down_color = 'rgba(200,127,130,0.8)'
 
     def _on_js_load(self):
         self.loaded = True
         for script in self._scripts:
             self.run_script(script)
 
     def _create_chart(self):
@@ -131,15 +221,51 @@
             volume = bars.drop(columns=['open', 'high', 'low', 'close']).rename(columns={'volume': 'value'})
             volume['color'] = self._volume_down_color
             volume.loc[bars['close'] > bars['open'], 'color'] = self._volume_up_color
             self.run_script(f'{self.id}.volumeSeries.setData({volume.to_dict(orient="records")})')
             bars = bars.drop(columns=['volume'])
 
         bars = bars.to_dict(orient='records')
-        self.run_script(f'{self.id}.series.setData({bars})')
+        self.run_script(f'''
+            {self.id}.candleData = {bars}
+            {self.id}.shownData = ({self.id}.candleData.length >= 190) ? {self.id}.candleData.slice(-190) : {self.id}.candleData
+            {self.id}.series.setData({self.id}.shownData);
+            
+            var timer = null;
+            {self.id}.chart.timeScale().subscribeVisibleLogicalRangeChange(() => {{
+                if (timer !== null) {{
+                    return;
+                }}
+                timer = setTimeout(() => {{
+                let chart = {self.id}
+                let logicalRange = chart.chart.timeScale().getVisibleLogicalRange();
+                if (logicalRange !== null) {{
+                    let barsInfo = chart.series.barsInLogicalRange(logicalRange);
+                    if (barsInfo === null || barsInfo.barsBefore === null || barsInfo.barsAfter === null) {{return}}
+                    if (barsInfo !== null && barsInfo.barsBefore < 20 || barsInfo.barsAfter < 20) {{
+                        let newBeginning = chart.candleData.indexOf(chart.shownData[0])+Math.round(barsInfo.barsBefore)-20
+                        let newEnd = chart.candleData.indexOf(chart.shownData[chart.shownData.length-2])-Math.round(barsInfo.barsAfter)+20
+                        if (newBeginning < 0) {{
+                            newBeginning = 0
+                        }}
+                        chart.shownData = chart.candleData.slice(newBeginning, newEnd)
+                        if (newEnd-17 <= chart.candleData.length-1) {{
+                            chart.shownData[chart.shownData.length - 1] = Object.assign({{}}, chart.shownData[chart.shownData.length - 1]);
+                            chart.shownData[chart.shownData.length - 1].open = chart.candleData[chart.candleData.length - 1].close;
+                            chart.shownData[chart.shownData.length - 1].high = chart.candleData[chart.candleData.length - 1].close;
+                            chart.shownData[chart.shownData.length - 1].low = chart.candleData[chart.candleData.length - 1].close;
+                            chart.shownData[chart.shownData.length - 1].close = chart.candleData[chart.candleData.length - 1].close;
+                            }}
+                        chart.series.setData(chart.shownData);
+                    }}
+                }}
+                timer = null;
+                }}, 50);
+            }});
+        ''') if self._dynamic_loading else self.run_script(f'{self.id}.series.setData({bars})')
 
     def update(self, series, from_tick=False):
         """
         Updates the data from a bar;
         if series['time'] is the same time as the last bar, the last bar will be overwritten.\n
         :param series: labels: date/time, open, high, low, close, volume (if volume enabled).
         """
@@ -149,15 +275,37 @@
             if 'volume' not in series:
                 raise MissingColumn("Volume enabled, but 'volume' column was not found.")
 
             volume = series.drop(['open', 'high', 'low', 'close']).rename({'volume': 'value'})
             volume['color'] = self._volume_up_color if series['close'] > series['open'] else self._volume_down_color
             self.run_script(f'{self.id}.volumeSeries.update({volume.to_dict()})')
             series = series.drop(['volume'])
-        self.run_script(f'{self.id}.series.update({series.to_dict()})')
+        bar = series.to_dict()
+        self.run_script(f'''
+        
+            let logicalRange = {self.id}.chart.timeScale().getVisibleLogicalRange();
+            let barsInfo = {self.id}.series.barsInLogicalRange(logicalRange);
+                
+            if ({self.id}.candleData[{self.id}.candleData.length-1].time === {bar['time']}) {{
+            
+                {self.id}.shownData[{self.id}.shownData.length-1] = {bar}
+                {self.id}.candleData[{self.id}.candleData.length-1] = {bar}
+            }}
+            else {{
+                if (barsInfo.barsAfter > 0) {{
+                    {self.id}.shownData[{self.id}.shownData.length-1] = {bar}
+                }}
+                else {{
+                    {self.id}.shownData.push({bar})
+                }}
+                
+            {self.id}.candleData.push({bar})
+            }}
+            {self.id}.series.update({self.id}.shownData[{self.id}.shownData.length-1])
+            ''') if self._dynamic_loading else self.run_script(f'{self.id}.series.update({bar})')
 
     def update_from_tick(self, series):
         """
         Updates the data from a tick.\n
         :param series: labels: date/time, price, volume (if volume enabled).
         """
         series = self._series_datetime_format(series)
@@ -180,113 +328,46 @@
 
     def create_line(self, color: str = 'rgba(214, 237, 255, 0.6)', width: int = 2):
         """
         Creates and returns a Line object.)\n
         """
         return Line(self, color, width)
 
-    def marker(self, time: datetime = None, position: MARKER_POSITION = 'below', shape: MARKER_SHAPE = 'arrow_up',
-               color: str = '#2196F3', text: str = '') -> str:
-        """
-        Creates a new marker.\n
-        :param time: The time that the marker will be placed at. If no time is given, it will be placed at the last bar.
-        :param position: The position of the marker.
-        :param color: The color of the marker (rgb, rgba or hex).
-        :param shape: The shape of the marker.
-        :param text: The text to be placed with the marker.
-        :return: The id of the marker placed.
-        """
-        try:
-            time = self._last_bar['time'] if not time else self._datetime_format(time)
-        except TypeError:
-            raise TypeError('Chart marker created before data was set.')
-        marker_id = self._rand.generate()
-        self.run_script(f"""
-            markers.push({{
-                time: {time if isinstance(time, float) else f"'{time}'"},
-                position: '{_marker_position(position)}',
-                color: '{color}',
-                shape: '{_marker_shape(shape)}',
-                text: '{text}',
-                id: '{marker_id}'
-                }});
-            {self.id}.series.setMarkers(markers)""")
-        return marker_id
-
-    def remove_marker(self, marker_id: str):
-        """
-        Removes the marker with the given id.\n
-        """
-        self.run_script(f'''
-           markers.forEach(function (marker) {{
-               if ('{marker_id}' === marker.id) {{
-                   markers.splice(markers.indexOf(marker), 1)
-                   {self.id}.series.setMarkers(markers)
-                   }}
-               }});''')
-
-    def horizontal_line(self, price: Union[float, int], color: str = 'rgb(122, 146, 202)', width: int = 1,
-                        style: LINE_STYLE = 'solid', text: str = '', axis_label_visible=True):
-        """
-        Creates a horizontal line at the given price.\n
-        """
-        var = self._rand.generate()
-        self.run_script(f"""
-           let priceLine{var} = {{
-               price: {price},
-               color: '{color}',
-               lineWidth: {width},
-               lineStyle: {_line_style(style)},
-               axisLabelVisible: {_js_bool(axis_label_visible)},
-               title: '{text}',
-           }};
-           let line{var} = {{
-               line: {self.id}.series.createPriceLine(priceLine{var}),
-               price: {price},
-           }};
-           horizontal_lines.push(line{var})""")
-
-    def remove_horizontal_line(self, price: Union[float, int]):
-        """
-        Removes a horizontal line at the given price.
-        """
+    def price_scale(self, mode: PRICE_SCALE_MODE = 'normal', align_labels: bool = True, border_visible: bool = False,
+                    border_color: str = None, text_color: str = None, entire_text_only: bool = False, ticks_visible: bool = False):
         self.run_script(f'''
-           horizontal_lines.forEach(function (line) {{
-           if ({price} === line.price) {{
-               {self.id}.series.removePriceLine(line.line);
-               horizontal_lines.splice(horizontal_lines.indexOf(line), 1)
-               }}
-           }});''')
-
-    def config(self, mode: PRICE_SCALE_MODE = 'normal', title: str = None, right_padding: float = None):
-        """
-        :param mode: Chart price scale mode.
-        :param title: Last price label text.
-        :param right_padding: How many bars of empty space to the right of the last bar.
-        """
-        self.run_script(f'{self.id}.chart.timeScale().scrollToPosition({right_padding}, false)') if right_padding is not None else None
-        self.run_script(f'{self.id}.series.applyOptions({{title: "{title}"}})') if title else None
-        self.run_script(f"{self.id}.chart.priceScale().applyOptions({{mode: {_price_scale_mode(mode)}}})")
+            {self.id}.chart.priceScale('right').applyOptions({{
+                mode: {_price_scale_mode(mode)},
+                alignLabels: {_js_bool(align_labels)},
+                borderVisible: {_js_bool(border_visible)},
+                {f'borderColor: "{border_color}",' if border_color else ''}
+                {f'textColor: "{text_color}",' if text_color else ''}
+                entireTextOnly: {_js_bool(entire_text_only)},
+                ticksVisible: {_js_bool(ticks_visible)},
+            }})''')
 
-    def time_scale(self, visible: bool = True, time_visible: bool = True, seconds_visible: bool = False):
+    def time_scale(self, right_offset: int = 0, min_bar_spacing: float = 0.5,
+                   visible: bool = True, time_visible: bool = True, seconds_visible: bool = False,
+                   border_visible: bool = True, border_color: str = None):
         """
         Options for the time scale of the chart.
-        :param visible: Time scale visibility control.
-        :param time_visible: Time visibility control.
-        :param seconds_visible: Seconds visibility control.
-        :return:
         """
         self.run_script(f'''
-           {self.id}.chart.applyOptions({{
-               timeScale: {{
-               visible: {_js_bool(visible)},
-               timeVisible: {_js_bool(time_visible)},
-               secondsVisible: {_js_bool(seconds_visible)},
-               }}
-           }})''')
+            {self.id}.chart.applyOptions({{
+                timeScale: {{
+                    rightOffset: {right_offset},
+                    minBarSpacing: {min_bar_spacing},
+                    visible: {_js_bool(visible)},
+                    timeVisible: {_js_bool(time_visible)},
+                    secondsVisible: {_js_bool(seconds_visible)},
+                    borderVisible: {_js_bool(border_visible)},
+                    {f'borderColor: "{border_color}",' if border_color else ''}
+                    
+                }}
+            }})''')
 
     def layout(self, background_color: str = None, text_color: str = None, font_size: int = None,
                font_family: str = None):
         """
         Global layout options for the chart.
         """
         self._background_color = background_color if background_color else self._background_color
@@ -466,41 +547,45 @@
         self._parent = parent
         self._position = position
         self._rand = self._chart._rand
         self.id = f'window.{self._rand.generate()}'
         self._append_js = f'{self._parent.id}.div.parentNode.insertBefore({self.id}.div, {self._parent.id}.div.nextSibling)'
         self._js_api = self._chart._js_api
         self._js_api_code = self._chart._js_api_code
-
+        self.run_script = self._chart.run_script
         self._create_chart()
         if not sync:
             return
         sync_parent_var = self._parent.id if isinstance(sync, bool) else sync
         self.run_script(f'''
             {sync_parent_var}.chart.timeScale().subscribeVisibleLogicalRangeChange((timeRange) => {{
                 {self.id}.chart.timeScale().setVisibleLogicalRange(timeRange)
-                }});''')
-
-    def run_script(self, script): self._chart.run_script(script)
+            }});
+        ''')
 
 
 SCRIPT = """
 document.body.style.backgroundColor = '#000000'
-const markers = []
-const horizontal_lines = []
 const up = 'rgba(39, 157, 130, 100)'
 const down = 'rgba(200, 97, 100, 100)'
 
+const wrapper = document.createElement('div')
+document.body.appendChild(wrapper)
+
 function makeChart(innerWidth, innerHeight) {
-    let chart = {}
-    chart.scale = {
-        width: innerWidth,
-        height: innerHeight
+    let chart = {
+        markers: [],
+        horizontal_lines: [],
+        div: document.createElement('div'),
+        legend: document.createElement('div'),
+        scale: {
+            width: innerWidth,
+            height: innerHeight
+        },
     }
-    chart.div = document.createElement('div')
     chart.chart = LightweightCharts.createChart(chart.div, {
         width: window.innerWidth*innerWidth,
         height: window.innerHeight*innerHeight,
         layout: {
             textColor: '#d1d4dc',
             background: {
                 color:'#000000',
@@ -531,28 +616,26 @@
                                         downColor: down, borderDownColor: down, wickDownColor: down, lineWidth: 2,
                                         })
     chart.volumeSeries = chart.chart.addHistogramSeries({
                         color: '#26a69a',
                         priceFormat: {type: 'volume'},
                         priceScaleId: '',
                         })
-    chart.legend = document.createElement('div')
+    chart.chart.priceScale('').applyOptions({
+        scaleMargins: {top: 0.8, bottom: 0},
+        });
     chart.legend.style.position = 'absolute'
     chart.legend.style.zIndex = 1000
     chart.legend.style.width = `${(chart.scale.width*100)-8}vw`
     chart.legend.style.top = '10px'
     chart.legend.style.left = '10px'
     chart.legend.style.fontFamily = 'Monaco'
     chart.legend.style.fontSize = '11px'
     chart.legend.style.color = 'rgb(191, 195, 203)'
     chart.div.appendChild(chart.legend)
-    
-    chart.chart.priceScale('').applyOptions({
-        scaleMargins: {top: 0.8, bottom: 0}
-        });
     return chart
 }
 function legendItemFormat(num) {
 return num.toFixed(2).toString().padStart(8, ' ')
 }
 """
```

### Comparing `lightweight_charts-1.0.7/lightweight_charts/pkg.py` & `lightweight_charts-1.0.8/lightweight_charts/pkg.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.7/lightweight_charts/util.py` & `lightweight_charts-1.0.8/lightweight_charts/util.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.7/lightweight_charts/widgets.py` & `lightweight_charts-1.0.8/lightweight_charts/widgets.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.7/lightweight_charts.egg-info/PKG-INFO` & `lightweight_charts-1.0.8/lightweight_charts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight-charts
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `lightweight_charts-1.0.7/setup.py` & `lightweight_charts-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='lightweight_charts',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'pandas',
         'pywebview',
     ],
     author='louisnw',
```

