# Comparing `tmp/bandplot-0.1.5.2-py3-none-any.whl.zip` & `tmp/bandplot-0.1.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17592 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       26 b- defN 23-May-18 19:19 bandplot/__init__.py
--rw-rw-r--  2.0 unx     7096 b- defN 23-May-18 19:19 bandplot/mass.py
--rw-rw-r--  2.0 unx    25644 b- defN 23-May-18 19:19 bandplot/plots.py
--rw-rw-r--  2.0 unx    22326 b- defN 23-May-18 19:19 bandplot/pplots.py
--rw-rw-r--  2.0 unx     9321 b- defN 23-May-18 19:19 bandplot/projected.py
--rw-rw-r--  2.0 unx     6229 b- defN 23-May-18 19:19 bandplot/readdata.py
--rw-rw-r--  2.0 unx    23352 b- defN 23-May-18 19:19 bandplot/wrapper.py
--rw-rw-r--  2.0 unx     2996 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      938 b- defN 23-May-18 19:20 bandplot-0.1.5.2.dist-info/RECORD
-12 files, 98115 bytes uncompressed, 16030 bytes compressed:  83.7%
+Zip file size: 17596 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-23 01:14 bandplot/__init__.py
+-rw-rw-r--  2.0 unx     7096 b- defN 23-May-23 01:14 bandplot/mass.py
+-rw-rw-r--  2.0 unx    25644 b- defN 23-May-23 01:14 bandplot/plots.py
+-rw-rw-r--  2.0 unx    22446 b- defN 23-May-23 01:14 bandplot/pplots.py
+-rw-rw-r--  2.0 unx     9321 b- defN 23-May-23 01:14 bandplot/projected.py
+-rw-rw-r--  2.0 unx     6229 b- defN 23-May-23 01:14 bandplot/readdata.py
+-rw-rw-r--  2.0 unx    23361 b- defN 23-May-23 01:14 bandplot/wrapper.py
+-rw-rw-r--  2.0 unx     3084 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      938 b- defN 23-May-23 01:14 bandplot-0.1.5.3.dist-info/RECORD
+12 files, 98332 bytes uncompressed, 16034 bytes compressed:  83.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.5.2.dist-info/METADATA
+Filename: bandplot-0.1.5.3.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.5.2.dist-info/WHEEL
+Filename: bandplot-0.1.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.5.2.dist-info/entry_points.txt
+Filename: bandplot-0.1.5.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.5.2.dist-info/top_level.txt
+Filename: bandplot-0.1.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.5.2.dist-info/RECORD
+Filename: bandplot-0.1.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.5.2"
+__version__ = "0.1.5.3"
```

## bandplot/pplots.py

```diff
@@ -81,15 +81,15 @@
     ax1_f.axis('off')
     ax2_f = fig.add_subplot(2,1,2)
     g = ax2_f.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax2_f.set_xlim(arr[1][0], arr[1][-1])
     ax2_f.set_ylim(vertical[0], broken[0])
     ax2_f.axis('off')
 
-    L = ax2.legend([], frameon=False, loc='upper left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax2.legend([], frameon=False, loc='best', bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax2.add_artist(L)
     ax2.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Broken3(arr, fre, ticks, labels, broken, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[fig_p.height_ratio, 1-fig_p.height_ratio], figsize=fig_p.size)
     fig.subplots_adjust(hspace=0.0)
@@ -146,15 +146,15 @@
     ax1_g.axis('off')
     ax2_g = fig.add_subplot(2,1,2)
     h = ax2_g.plot(arr[2], fre[2].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     ax2_g.set_xlim(arr[2][0], arr[2][-1])
     ax2_g.set_ylim(vertical[0], broken[0])
     ax2_g.axis('off')
 
-    L = ax2.legend([], frameon=False, loc='upper left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = ax2.legend([], frameon=False, loc='best', bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     ax2.add_artist(L)
     ax2.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Nobroken(arr, fre, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r']
@@ -200,15 +200,15 @@
     plt.ylabel('Frequency (THz)')
     ax = plt.axes()
     g = ax.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     ax.set_xlim(arr[1][0], arr[1][-1])
     ax.set_ylim(ylim)
     ax.axis('off')
 
-    L = plt.legend([], frameon=False, loc='upper left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
     plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Nobroken3(arr, fre, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k', 'b']
@@ -240,15 +240,15 @@
 
     af = plt.axes()
     h = af.plot(arr[2], fre[2].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     af.set_xlim(arr[2][0], arr[2][-1])
     af.set_ylim(ylim)
     af.axis('off')
 
-    L = plt.legend([], frameon=False, loc='upper left', title=legend[0], title_fontproperties={'size':'medium'})
+    L = plt.legend([], frameon=False, loc='best', bbox_to_anchor=(0., 0.5, 0.5, 0.5), title=legend[0], title_fontproperties={'size':'medium'})
     plt.gca().add_artist(L)
     plt.legend([f[0], g[0], h[0]], [legend[1], legend[2], legend[3]], frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 
 def BrokenWd(arr, fre, ticks, labels, broken, darr, dele, elements, legend, fig_p):
     fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2, height_ratios=[fig_p.height_ratio, 1-fig_p.height_ratio],
```

## bandplot/wrapper.py

```diff
@@ -1,8 +1,8 @@
-import argparse, os, re, platform, glob
+import ast, argparse, os, re, platform, glob
 import matplotlib.pyplot as plt
 from bandplot import plots, pplots, readdata
 from bandplot import __version__
 
 plt.rcParams['xtick.direction'] = 'in'
 plt.rcParams['ytick.direction'] = 'in'
 plt.rcParams['ytick.minor.visible'] = True
@@ -33,63 +33,56 @@
                                                                              'center left', 'center right', 'lower center', 'upper center', 'center'],
                                                                     help="arrange the legend location, default: best", default='best')
     parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
                                                                                     "k, black; w, white", default=[])
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
                                                                                     default=[])
     parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
-    parser.add_argument('-m', "--mass",       action='store_true',  help='calculate the effective masses')
-    parser.add_argument('-M', "--scale",      type=float,           help='the scale of data for effective masses calculation, default: 0.15', default=0.15)
+    parser.add_argument('-m', "--mass",       type=float,           nargs='*', help='calculate the effective masses, default: 0.15', default=None)
     parser.add_argument('-r', "--projected",  action='store_true',  help='plot the projected band structure')
     parser.add_argument('-i', "--input",      type=str,             nargs='+', help="plot figure from .dat file, default: BAND.dat", default=["BAND.dat"])
     parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
     parser.add_argument('-j', "--klabels",    type=str,             help="filename of KLABELS, default: KLABELS", default="KLABELS")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             nargs='+', default=[], help="plot DOS from .dat file, or file list")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of DOS")
     parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d, or symbol-s,p,d')
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-W', "--wratios",    type=float,           help='width ratio for DOS subplot')
-    parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
-    parser.add_argument('-Z', "--alpha",      type=float,           help='alpha value for filling region, default=0.2', default=0.2)
+    parser.add_argument('-z', "--fill",       type=float,           nargs='*', help='fill a shaded region between PDOS and axis, default: 0.2', default=None)
     parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
     dosfiles = [f for i in args.dos for f in glob.glob(i)]
 
     color = []
     for i in args.color:
         j = i.split('*')
         if len(j) == 2:
-            color = color + [j[0]] * int(j[1])
+            color += [ast.literal_eval(j[0])] * int(j[1]) if '(' in j[0] and ')' in j[0] else [j[0]] * int(j[1])
         else:
-            color.append(i)
+            color += [ast.literal_eval(i)] if '(' in i and ')' in i else [i]
 
     linestyle = []
     for i in args.linestyle:
-        if len(i) > 2 and i[0] == '(' and i[-1] == ')':
-            linestyle.append(eval(i))
-        elif len(i.split('*')) == 2:
-            j = i.split('*')
-            linestyle = linestyle + [j[0]] * int(j[1])
+        j = i.split('*')
+        if len(j) == 2:
+            linestyle += [ast.literal_eval(j[0])] * int(j[1]) if '(' in j[0] and ')' in j[0] else [j[0]] * int(j[1])
         else:
-            linestyle.append(i)
+            linestyle += [ast.literal_eval(i)] if '(' in i and ')' in i else [i]
 
     linewidth = []
     for i in args.linewidth:
-        if len(i.split('*')) == 2:
-            j = i.split('*')
-            linewidth = linewidth + [float(j[0])] * int(j[1])
-        else:
-            linewidth.append(float(i))
+        j = i.split('*')
+        linewidth += [float(j[0])] * int(j[1]) if len(j) == 2 else [float(i)]
 
     plt.rcParams['font.family'] = '%s'%args.font
 
     pltname = os.path.split(os.getcwd())[-1]
     formula = ''
     if os.path.exists('POSCAR'):
         symbol, factor = readdata.symbols('POSCAR')
@@ -118,37 +111,38 @@
 
     width_ratios = args.wratios or (0.3 if args.divided else 0.5)
 
     fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
                     color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi,
                     width_ratios=width_ratios, exchange=args.exchange, fill=args.fill)
 # calculate the effective masses
-    if args.mass:
+    if args.mass is not None:
         if not fig_p.vertical:
             fig_p.vertical = [-5.0, 5.0]
+        scale = 0.15 if args.mass == [] else args.mass[0]
         from bandplot import mass
         if os.path.exists("BAND_GAP"):
             lumo, homo, homo_c, filename = mass.get_vbm_cbm("BAND_GAP")
             Extension = [len(lumo), len(homo), len(homo_c), len(filename)]
             if all(x == 1 for x in Extension):
                 data = mass.bs_dat_read(filename)
-                calM = mass.dat_read(data[0], lumo[0], homo[0], homo_c[0], args.scale)
+                calM = mass.dat_read(data[0], lumo[0], homo[0], homo_c[0], scale)
                 pltlabel = mass.npfit(calM)
                 mass.plot(data[0], calM, pltlabel, ticks, labels, legend, fig_p)
                 print("{:<8}{:<8}{:<8}{:<8}{:<8}{:<8}".format("e_x","e_y","h1_x","h1_y","h2_x","h2_y"))
                 for i in pltlabel:
                     if isinstance(i, float):
                         print("{:<8.3f}".format(i), end='')
                     else:
                         print("{:<8s}".format('-'), end='')
                 print()
             elif all(x == 2 for x in Extension):
                 data = mass.bs_dat_read(filename)
-                calM_u = mass.dat_read(data[0], lumo[0], homo[0], homo_c[0], args.scale)
-                calM_d = mass.dat_read(data[1], lumo[1], homo[1], homo_c[1], args.scale)
+                calM_u = mass.dat_read(data[0], lumo[0], homo[0], homo_c[0], scale)
+                calM_d = mass.dat_read(data[1], lumo[1], homo[1], homo_c[1], scale)
                 pltlabel_u = mass.npfit(calM_u)
                 pltlabel_d = mass.npfit(calM_d)
                 mass.plot2(data, calM_u, pltlabel_u, calM_d, pltlabel_d, ticks, labels, legend, fig_p)
                 print("{:<8}{:<8}{:<8}{:<8}{:<8}{:<8}".format("e_x","e_y","h1_x","h1_y","h2_x","h2_y"))
                 for i in pltlabel_u:
                     if isinstance(i, float):
                         print("{:<8.3f}".format(i), end='')
@@ -201,16 +195,16 @@
                 elif ispin == "Ispin" and args.divided:
                     plots.Dispin(arr, bands, ticks, labels, legend, fig_p)
             else:
                 darr, dele, s_elements = readdata.dos(args.dos)
                 index_f, labels_elements = readdata.select(s_elements, args.partial)
                 if not elements:
                     elements = labels_elements
-                if fig_p.fill:
-                    fig_p.fill = args.alpha
+                if fig_p.fill is not None:
+                    fig_p.fill = 0.2 if fig_p.fill == [] else fig_p.fill[0]
 
                 if ispin == "Noneispin":
                     plots.NoneispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p)
                 elif ispin == "Ispin" and not args.divided:
                     plots.IspinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p)
                 elif ispin == "Ispin" and args.divided:
                     plots.DispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, legend, fig_p)
@@ -219,16 +213,16 @@
             if dosfiles:
                 if fig_p.output == "BAND.png":
                     fig_p.output = "DOS.png"
                 darr, dele, s_elements = readdata.dos(dosfiles)
                 index_f, labels_elements = readdata.select(s_elements, args.partial)
                 if not elements:
                     elements = labels_elements
-                if fig_p.fill:
-                    fig_p.fill = args.alpha
+                if fig_p.fill is not None:
+                    fig_p.fill = 0.2 if fig_p.fill == [] else fig_p.fill[0]
 
                 plots.pdosfiles(darr, dele, index_f, elements, legend, fig_p)
             else:
                 print("ERROR: No *.dat file.")
 # compare two Band Structures
         elif len_bandfile == 2:
             if not fig_p.vertical:
@@ -293,47 +287,41 @@
     parser.add_argument('-j', "--bandconf",   type=str,             help="filename of band setting file, default: band.conf", default="band.conf")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             help="plot Phonon DOS from .dat file")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Phonon density of states range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of Phonon DOS")
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-W', "--wratios",    type=float,           help='width ratio for DOS subplot, default 0.5', default=0.5)
-    parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
-    parser.add_argument('-Z', "--alpha",      type=float,           help='alpha value for filling region, default=0.2', default=0.2)
+    parser.add_argument('-z', "--fill",       type=float,           nargs='*', help='fill a shaded region between PDOS and axis, default: 0.2', default=None)
     parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
-    color  = []
+    color = []
     for i in args.color:
         j = i.split('*')
         if len(j) == 2:
-            color = color + [j[0]] * int(j[1])
+            color += [ast.literal_eval(j[0])] * int(j[1]) if '(' in j[0] and ')' in j[0] else [j[0]] * int(j[1])
         else:
-            color.append(i)
+            color += [ast.literal_eval(i)] if '(' in i and ')' in i else [i]
 
     linestyle = []
     for i in args.linestyle:
-        if len(i) > 2 and i[0] == '(' and i[-1] == ')':
-            linestyle.append(eval(i))
-        elif len(i.split('*')) == 2:
-            j = i.split('*')
-            linestyle = linestyle + [j[0]] * int(j[1])
+        j = i.split('*')
+        if len(j) == 2:
+            linestyle += [ast.literal_eval(j[0])] * int(j[1]) if '(' in j[0] and ')' in j[0] else [j[0]] * int(j[1])
         else:
-            linestyle.append(i)
+            linestyle += [ast.literal_eval(i)] if '(' in i and ')' in i else [i]
 
     linewidth = []
     for i in args.linewidth:
-        if len(i.split('*')) == 2:
-            j = i.split('*')
-            linewidth = linewidth + [float(j[0])] * int(j[1])
-        else:
-            linewidth.append(float(i))
+        j = i.split('*')
+        linewidth += [float(j[0])] * int(j[1]) if len(j) == 2 else [float(i)]
 
     plt.rcParams['font.family'] = '%s'%args.font
     pltname = os.path.split(os.getcwd())[-1]
     s_ele = []
     formula = ''
     if os.path.exists('POSCAR-unitcell'):
         symbol, factor = readdata.symbols('POSCAR-unitcell')
@@ -377,28 +365,28 @@
         if args.dos is None:
             if args.broken is None:
                 pplots.Nobroken(arr, fre, ticks, labels, legend, fig_p)
             else:
                 pplots.Broken(arr, fre, ticks, labels, broken, legend, fig_p)
         elif os.path.exists(args.dos):
             darr, dele = readdata.pdos(args.dos)
-            if fig_p.fill:
-                fig_p.fill = args.alpha
+            if fig_p.fill is not None:
+                fig_p.fill = 0.2 if fig_p.fill == [] else fig_p.fill[0]
             if args.broken is None:
                 pplots.NobrokenWd(arr, fre, ticks, labels, darr, dele, elements, legend, fig_p)
             else:
                 pplots.BrokenWd(arr, fre, ticks, labels, broken, darr, dele, elements, legend, fig_p)
 # plot Phonon DOS
     elif len_bandfile == 0:
         if args.dos and os.path.exists(args.dos):
             if fig_p.output == "BAND.png":
                     fig_p.output = "DOS.png"
             darr, dele = readdata.pdos(args.dos)
-            if fig_p.fill:
-                fig_p.fill = args.alpha
+            if fig_p.fill is not None:
+                fig_p.fill = 0.2 if fig_p.fill == [] else fig_p.fill[0]
             pplots.dosfile(darr, dele, elements, legend, fig_p)
         else:
             print('No *.dat file.')
 # compare two Phonon Band Structures
     elif len_bandfile == 2:
         arr = [''] * 2
         fre = [''] * 2
```

## Comparing `bandplot-0.1.5.2.dist-info/METADATA` & `bandplot-0.1.5.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: numpy (>=1.22.0)
 Requires-Dist: matplotlib (>=3.4.0)
 
 [![bandplot](https://img.shields.io/pypi/v/bandplot?style=flat-square)](https://pypi.org/project/bandplot/)
 [![bandplot](https://img.shields.io/pypi/pyversions/bandplot?style=flat-square)](https://pypi.org/project/bandplot/)
@@ -40,14 +41,15 @@
 * To execute <b style="color:blue;"><i>bandplot</b></i> <b style="color:red;"><i>\-h</b></i> for the parameters to use.
 * Example:
 ```bash
 bandplot -h
 bandplot -i BAND.dat -o BAND.png -l g m k g -d PDOS* -z
 bandplot -i BAND1.dat BAND2.dat -g TiO\$_2\$ PBE HSE
 bandplot -b -l g m k g -y -3 3
+bandplot -r -i PBAND*.dat -p C,O-s,p
 ```
 ***
 <b style="color:blue;"><i>pbandplot</b></i>
 * To execute <b style="color:blue;"><i>pbandplot</b></i> <b style="color:red;"><i>\-h</b></i> for the parameters to use.
 * Example:
 ```bash
 pbandplot -h
```

## Comparing `bandplot-0.1.5.2.dist-info/RECORD` & `bandplot-0.1.5.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-bandplot/__init__.py,sha256=yiXFBxUCS9aDTfIRgk_qZR73uu9Nneq4eiQfb6LCJg4,26
+bandplot/__init__.py,sha256=mFp-25ZLsKGYdenSxIDCsdXd-NbUGoaCoouHW35dmf4,26
 bandplot/mass.py,sha256=Sh3Eq-K8z7WNnUkDbPOcZKGruvEphlAqHYgr01-vpXE,7096
 bandplot/plots.py,sha256=yWFTG29hkF2NgHnnMn-Dg1_51Jra7zTwk2vzaNxicpM,25644
-bandplot/pplots.py,sha256=hWxpyVZiMRTHHmRfos4VXQ0-bLYAqeync0WE4CexCE4,22326
+bandplot/pplots.py,sha256=brKpvhhoB63uK3zUywgzDA9pml3U6C8YySui6g5MqFw,22446
 bandplot/projected.py,sha256=EketFLm4KUusA3wVslVVJke7HJIbCvhwyiiW-x3eslI,9321
 bandplot/readdata.py,sha256=vrxY7d4V8ONemimNxANrWkvXtt0raZyAbyRN1i8eoLM,6229
-bandplot/wrapper.py,sha256=JfPhmcAq4E9qqh_mRGkgKAnTEeyRjfXS5y7kK7UhMyA,23352
-bandplot-0.1.5.2.dist-info/METADATA,sha256=xZzLEvkWa8UUNgz1gNY92-Xoo4tNZt1HiKYmKP-JNJY,2996
-bandplot-0.1.5.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bandplot-0.1.5.2.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
-bandplot-0.1.5.2.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
-bandplot-0.1.5.2.dist-info/RECORD,,
+bandplot/wrapper.py,sha256=wKlgDGtBpIeKiLHQrshZxXXGTBreCz1vVZA_DqObqx8,23361
+bandplot-0.1.5.3.dist-info/METADATA,sha256=HoRXJ32ss_V9EcDnLQXTKdPDtLROiTDpZ4x8N9RQEGg,3084
+bandplot-0.1.5.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bandplot-0.1.5.3.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
+bandplot-0.1.5.3.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
+bandplot-0.1.5.3.dist-info/RECORD,,
```

