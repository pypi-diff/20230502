# Comparing `tmp/Capella-1.0.3.tar.gz` & `tmp/Capella-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Capella-1.0.3.tar", last modified: Mon Nov 28 04:48:03 2022, max compression
+gzip compressed data, was "Capella-1.0.4.tar", last modified: Tue May  2 15:50:59 2023, max compression
```

## Comparing `Capella-1.0.3.tar` & `Capella-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-11-28 04:48:03.236415 Capella-1.0.3/
-drwxrwxrwx   0        0        0        0 2022-11-28 04:48:03.216761 Capella-1.0.3/Capella/
--rw-rw-rw-   0        0        0       16 2022-11-28 02:44:03.000000 Capella-1.0.3/Capella/__init__.py
--rw-rw-rw-   0        0        0    71741 2022-11-28 03:35:05.000000 Capella-1.0.3/Capella/cnav.py
--rw-rw-rw-   0        0        0    70786 2022-11-28 03:35:05.000000 Capella-1.0.3/Capella/main.py
-drwxrwxrwx   0        0        0        0 2022-11-28 04:48:03.233703 Capella-1.0.3/Capella.egg-info/
--rw-rw-rw-   0        0        0    21452 2022-11-28 04:48:03.000000 Capella-1.0.3/Capella.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2022-11-28 04:48:03.000000 Capella-1.0.3/Capella.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-28 04:48:03.000000 Capella-1.0.3/Capella.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-11-28 04:48:03.000000 Capella-1.0.3/Capella.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2022-11-28 02:47:27.000000 Capella-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    21452 2022-11-28 04:48:03.235895 Capella-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    20774 2022-11-28 03:41:03.000000 Capella-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2022-11-28 04:48:03.236916 Capella-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      628 2022-11-28 04:47:59.000000 Capella-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:50:59.406219 Capella-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-02 15:50:59.378427 Capella-1.0.4/Capella/
+-rw-rw-rw-   0        0        0       16 2022-11-28 02:44:03.000000 Capella-1.0.4/Capella/__init__.py
+-rw-rw-rw-   0        0        0    71597 2022-12-10 04:10:30.000000 Capella-1.0.4/Capella/cnav.py
+-rw-rw-rw-   0        0        0    70923 2023-05-02 00:15:25.000000 Capella-1.0.4/Capella/main.py
+drwxrwxrwx   0        0        0        0 2023-05-02 15:50:59.406219 Capella-1.0.4/Capella.egg-info/
+-rw-rw-rw-   0        0        0    26954 2023-05-02 15:50:58.000000 Capella-1.0.4/Capella.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-02 15:50:59.000000 Capella-1.0.4/Capella.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 15:50:58.000000 Capella-1.0.4/Capella.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-05-02 15:50:58.000000 Capella-1.0.4/Capella.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 15:50:58.000000 Capella-1.0.4/Capella.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2022-11-28 02:47:27.000000 Capella-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0    26954 2023-05-02 15:50:59.406219 Capella-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    26531 2023-05-02 00:42:35.000000 Capella-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 15:50:59.406219 Capella-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      954 2023-05-02 15:41:46.000000 Capella-1.0.4/setup.py
```

### Comparing `Capella-1.0.3/Capella/cnav.py` & `Capella-1.0.4/Capella/cnav.py`

 * *Files 0% similar despite different names*

```diff
@@ -1350,18 +1350,18 @@
                     self.ax11.yaxis.set_major_formatter(mticker.FuncFormatter(y_fmt))
                     self.ax11.xaxis.set_major_formatter(mdates.DateFormatter('%M:%S'))
                     self.ax11.set_facecolor('#212946')
                     self.ax11.grid(color='#2A3459')
                     plt.subplots_adjust(left=.057, bottom=.052, right=.979, top=.93, wspace=.248, hspace=.42)
 
             plt.plot(x, y)
-            # plt.scatter(time_before.minute, two)
-            # plt.scatter(time_after.minute, one)
+
+
             plt.scatter(time1, three, color='red')
-            # plt.scatter(time1.minute, four)
+
 
             p1 = np.array([datetime_to_float(time_after), one], dtype=object)
             p2 = np.array([datetime_to_float(time_before), two], dtype=object)
             p3 = np.array([datetime_to_float(time1), three], dtype=object)
             p4 = np.array([datetime_to_float(time1), four], dtype=object)
 
             d = float((np.cross(p2 - p1, p3 - p1) / np.linalg.norm(p2 - p1)) * 60)
```

### Comparing `Capella-1.0.3/Capella/main.py` & `Capella-1.0.4/Capella/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,24 +43,26 @@
         tk.Tk.__init__(self, *args, **kwargs)
 
         # create a container
         container = ttk.Frame()
         container.pack(side="top", fill="both", expand=True)
         container.grid_rowconfigure(0, weight=1)
         container.grid_columnconfigure(0, weight=1)
+
         # configure appearance
         screen_width = self.winfo_screenwidth()
         screen_height = self.winfo_screenheight()
         app_width = screen_width / 2
         app_height = screen_width / 1.68
         x = (screen_width / 2) - (app_width / 2)
         y = (screen_height / 2.2) - (app_height / 2)
         self.geometry(f'{int(app_width)}x{int(app_height)}+{int(x)}+{int(y)}')
+        
         #transparency
-        self.attributes('-alpha', 0.97)
+        self.attributes('-alpha', 1.0)
         ttk.Style("darkly")
         tk.Tk.wm_title(self, "Capella")
 
         # Add menu bar to top
         menubar = ttk.Menu(container)
         filemenu = ttk.Menu(menubar, tearoff=0)
         filemenu.add_command(label="Load Sights from Clipboard", command=lambda: load_sights_from_clipboard(), accelerator='Ctrl+l')
@@ -490,14 +492,17 @@
 
         canvas2.get_tk_widget().pack(side=tk.BOTTOM, fill=tk.BOTH, expand=True)
 
         toolbar = NavigationToolbar2Tk(canvas2, self)
         toolbar.update()
         canvas2._tkcanvas.pack(side=tk.TOP, fill=tk.BOTH, expand=True)
 
+        def get_canvas2(self):
+            return canvas2
+
 
 
 class PageThree(ttk.Frame, SightReduction):
 
     def __init__(self, parent, controller):
         ttk.Frame.__init__(self, parent)
         # label = tk.Label(self, text=(f'{session.fixtime.strftime("%Y-%m-%d %H:%M:%S UTC")} RUNNING FIX'), font=LARGE_FONT)
@@ -517,14 +522,18 @@
         canvas = FigureCanvasTkAgg(f, self)
         canvas.get_tk_widget().pack(side=tk.BOTTOM, fill=tk.BOTH, expand=True)
         toolbar = NavigationToolbar2Tk(canvas, self)
         toolbar.update()
         canvas._tkcanvas.pack(side=tk.TOP, fill=tk.BOTH, expand=True)
 
         return
+    
+        def get_canvas(self):
+            return canvas
+
 
         controller.bind('<Control-p', reduce_sight)
         controller.bind('<Control-l', load_sights_from_clipboard)
 
 
 # Sight Entry Page
 class PageFour(ttk.Frame, Sight, SightSession):
@@ -1338,15 +1347,14 @@
                 ent8.insert(6, f'.')
             if len(t8.get()) == 8:
                 ent8.insert(8, f'-')
 
             # autocorrects lower cases
             try:
                 if len(t8.get()) == 10 and t8.get()[-1] == 'e' or t8.get()[-1] == 'w':
-
                     if t8.get()[-1] == 'e':
                         ent8.delete(9)
                         ent8.insert(10, 'E')
                     else:
                         ent8.delete(9)
                         ent8.insert(10, 'W')
             except:
```

### Comparing `Capella-1.0.3/Capella.egg-info/PKG-INFO` & `Capella-1.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,70 @@
-Metadata-Version: 2.1
-Name: Capella
-Version: 1.0.3
-Summary: Capella Beta
-Home-page: https://github.com/AlexSpradling/Capellav.git
-Author: AlexSpradling
-Author-email: alexspradling@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Capella
 
 ## Installation
 
 `pip install Capella`
 
 ### To Run:
 Navigate to your python installation and go to `lib\site-packages` open the `Capella` directory in your terminal and run `main.py`, the GUI will open from the terminal.
 
+---
 
 ### Introduction
 
 Capella is a simple-to-use Astronavigation aid. The program will derive a celestial position from a minimum of inputs and plot the position on a chartlet, with an analysis of the accuracy of  computed position provided. The program  additionally features some helper functions for celestial observation session planning, DR computation and compass correction. 
 
+
+![](gifs/demo.gif)
+
+---
 ## Section 1: Sight Entry
 
 **DR Information**
 
 All effective navigation starts with keeping a DR. Capella is no different. For the program to work effectively, first provide a DR position, time, course and speed. 
 
 Capella uses the standard nautical conventions for time and position formatting, and all times are kept in UTC. Capella will format the input for you---just type in the numbers for the respective field and when you are finished press tab or click to advance to the next input field. If erroneous information has been inputted, the field will flag RED. 
 
+
 **Sight Entry**
 
 In the Step 2 section, complete the four required fields. All the input fields will assist with autocompletion and formatting. The fields are: 1. Body 2. Hs Value 3. Sight Date 4. Sight Time. 
 All sextant altitude corrections are handled internally, simply input the Hs value for the observation.
 
 When you have completed the four input fields, hit the *Add* button and the sight will appear in the Sight List at the top of the screen. To edit previously entered information, click on the sight in the *Sight List*, the sight's information will populate the sight entry fields under Step 2. Make any required changes and hit *Update* and the sight entry will change in the *Sight List*. To remove a sight from the *Sight List*, simply click on the sight and hit *Delete*. Multiple sight handling is easily achieved using the conventional Shift or Ctrl + click features. 
 
+
 *Averaging*
 
 If you have multiple observations of the same body, you can CTRL or SHIFT click on them in the Sight Entry area, and the average of their Hs and time/date values will appear in the Step 2-Entry area. Press the *Add* button to add the averaged sight. It is recommended you first compute the position with all sights unaveraged and use the *Fit-Slope Analysis* feature to find which values should be eschewed or kept for averaging.
 
+![](gifs/blunder_3.png)
+
+*LOP plot before fit-slope analysis and sight averaging*
+
+![](gifs/blunder_fixed.png)
+
+*LOP plot after fit-slope analysis and sight averaging*
+
 *Almanac Computation*
 
 Capella features a high-accuracy perpetual almanac valid from the years 1900-2050, with the data taken from the JPL de421 database. Once the fix is computed, all almanac data is displayed in the *Sight Data/Planning* section. 
 
 **Fix Computation**
 
 Capella will calculate a fix from the DR information provided in Step 1 and the sights added to the Sight List. A fix can be calculated from just one sight and the provided DR information, however the algorithm needs at least 2 sights to provide a more accurate fix. Once two or more sights are present in the *Sight List* and a *Fix Time* and *Fix Date* has been provided in the *Step 1* field, hit the *Compute* button or press *CTRL-l*. Capella will calculate a running fix based on the DR and *Fix Time* information provided. The calculated results as well as a DR position for the requested *Fix Time* will appear highlighted at the bottom. 
 
-The position calculation is provided by the robust Limited Memory-BFGS algorithm. This algorithm is robust with respect to erroneous DR information, will not converge to a local minimum and can effectively handle high altitude sights. Prudent navigation always requires the most accurate DR possible, however, the fitting algorithm is somewhat robust with respect to DR accuracy. 
+A position is calculated using a Limited Memory-BFGS algorithm. The algorithm is robust with respect to erroneous DR information, and can effectively handle high altitude sights. Prudent navigation always requires the most accurate DR possible, however, the fitting algorithm is quite robust with respect to DR accuracy. 
 
 *Example 1:*
 
 The Sight Information below yields the fix: **40-14.0-N, 049-58.0-W**.
 ```
-| DR Date   | DR Time  | DR L      | DR Î»       | Course | Speed | I.C. | H.O.E | Temp. | Press. | Fix Date  | Fix Time |
+| DR Date   | DR Time  | DR L      | DR λ       | Course | Speed | I.C. | H.O.E | Temp. | Press. | Fix Date  | Fix Time |
 | --------- | -------- | --------- | ---------- | ------ | ----- | ---- | ----- | ----- | ------ | --------- | -------- |
 | 1993-5-13 | 07:30:00 | 40-10.0-N | 050-15.0-W | 090    | 5.5   | -1.2 | 7     | 10    | 1010   | 1993-5-13 | 07:44:00 |
 
 | Body       | Hs      | Date       | Time     |
 | ---------- | ------- | ---------- | -------- |
 | Kochab     | 43-23.8 | 1993-05-13 | 07:33:45 |
 | Rasalhague | 51-05.2 | 1993-05-13 | 07:35:16 |
@@ -73,14 +75,15 @@
 ```
 by changing the DR Position to 00-00.0-N and 000-00.0-W *--a position 3673 nm away--* and keeping the same observation data, Capella yields the fix: **40-14.3-N, 049-57.8-W**. 
 
 **Systematic Error**
 
 If Capella's systematic error algorithm detects uncorrected index and personal error, a prompt will appear asking you could like to remove the error from your observations and recompute the fix. Click *Ok* and then click *Compute*. This process can be iterative and the prompt might appear multiple times, with each cycle bringing the calculated fix closer to the observer's true position. This method isn't a magic bullet, but can yield impressive results in certain circumstances. 
 
+
 **Loading and Saving Observation Records**
 
 Capella uses the computer's clipboard as a means of loading and saving observations. Rather than saving the observations in a proprietary format, the observations are copied to the clipboard as a simple markdown format table than can be pasted into any .txt file the navigator wishes to use as a sight log. 
 
 *To Save Sights*
 1. In Capella, click File-Save Sights to Clipboard or CTRL-s. 
 2. 2 markdown format tables will be saved to your computer's clipboard.
@@ -92,23 +95,26 @@
 3. In Capella, click File-Load Sights from Clipboard or CTRL-l
 
 *Why do it like this?*
 1. Simplicity. You can use one E-log for record keeping, note taking and to interact with the program. 
 2. Using the "Windows-Snap" features on a computer allows you to snap Capella to one side of the screen and snap the `.txt` sight log of choice to the other. Using the `ctrl` quick keys you can rapidly edit the observations in the `.txt` log and compute the observations in Capella side by side. 
 3. Most celestial navigation programs have UI issues that are difficult and frustrating to navigate, using this method, you can use any text editor as the primary controller of the program if you'd like. Simply use the below template:
 ```
-| DR Date    | DR Time   | DR L      | DR Î»       |   Course |   Speed |   I.C. |   H.O.E |   Temp. |   Press. | Fix Date   | Fix Time   |
+| DR Date    | DR Time   | DR L      | DR λ       |   Course |   Speed |   I.C. |   H.O.E |   Temp. |   Press. | Fix Date   | Fix Time   |
 |------------|-----------|-----------|------------|----------|---------|--------|---------|---------|----------|------------|------------|
 | 2012-07-06 | 12:30:00  | 47-25.9-N | 007-08.0-W |      208 |      17 |    0.4 |      86 |      10 |     1010 | 2012-07-06 | 12:33:22   |
  
 | Body   | Hs      | Date       | Time     |
 |--------|---------|------------|----------|
 | SunLL  | 65-03.4 | 2012-07-06 | 12:29:22 |
 ```
 
+![](gifs/saving_loading.gif)
+
+---
 
 
 ## Section 2: LOP Plot
 
 **Exploring the plot**
 
 Once the fix is computed from the *Sight Entry* page, the LOP's for the observations are automatically plotted. The plot is highly customizable with respect to  size, aspect and zoom via the buttons located in the lower right corner. Click the *NSEW arrow* icon and then left-click and drag on the plot to move the plot, the Latitude and Longitude scales will automatically change. A right-click and drag will change the plots aspect. To reset the plot back to the default at any time, click on the *House* icon. To zoom in on the plot, click the *Magnifying Glass* icon and then left-click and drag to zoom-in and right-click and drag to zoom-out. 
@@ -119,14 +125,17 @@
 
 The LOPS are automatically advanced with the course and speed information provided in the *Sight Entry* section and bodies are labeled on the plot and in the sight key area. Additionally, the computed DR position for the *Fix Time* is also plotted. If the DR is very far from the LOP plot, the plot will need to be zoomed for a better aspect, however, if a good DR is being kept, this should not be necessary in most cases. 
 
 **Fix + Confidence**
 
 The red dot on the LOP plot marks the computed position and the golden ellipse surrounding the computed fix represents an area of 95% confidence. That is, there is a 95% probability, *given the sight information provided* that the true position lies within the ellipse.
 
+![](gifs/confidence_ellipse.png)
+
+---
 ## Section 3: Fit Slope Analysis
 
 This is an implementation of Dr. David Burch's Fit Slope method. It is a means of deriving greater accuracy from our sight observations and attempting to spot any outliers or potential blunders. 
 
 **How  Fit-Slope Analysis works**
 
 The vessel is moving all the time at sea and and the celestial objects are moving all the time as well. If we take 3 observations of the Sun, how do we know which observations were accurate and which weren't? 
@@ -139,15 +148,15 @@
  
 Each plot on the *Fit-Slope* page has a fitted *slope* and a *red dot*. The *slope* represents the computed altitude at the DR Position one minute behind the DR position of the observation and the computed altitude at the DR position one minute ahead of the DR position of the observation. A red dot is the observed altitude at the time of the observation. With this information you can see if your observation was under-observed or over-observed. the *Scatter* value at the top of each plot tells you how by how many minutes of arc your observation was over or under the computed slope.  The X-axis scale is minutes after the hour of observation, and covers a 2 minute timescale. The Y-axis scale is the computed range of altitudes for the observed body over that 2 minute scale. As with the LOP Plot page, every plot is fully interactive and explorable using the buttons in the lower left corner, and the values for any point on the plot will appear in the lower right corner.
 
 *Example 2:*
 
 The following observations are taken and a fix of 21-11.0-N, 157-34.7-W is computed, the observer's actual position is: 21-12.0-N, 157-30.0-W. 
 ```
-| DR Date    | DR Time   | DR L      | DR Î»       |   Course |   Speed |   I.C. |   H.O.E |   Temp. |   Press. | Fix Date   | Fix Time   |
+| DR Date    | DR Time   | DR L      | DR λ       |   Course |   Speed |   I.C. |   H.O.E |   Temp. |   Press. | Fix Date   | Fix Time   |
 |------------|-----------|-----------|------------|----------|---------|--------|---------|---------|----------|------------|------------|
 | 1990-01-02 | 03:00:00  | 21-12.0-N | 157-30.0-W |        0 |       0 |      0 |       0 |      10 |     1010 | 1990-01-02 | 03:12:00   |
 
 | Body      | Hs      | Date       | Time     |
 | --------- | ------- | ---------- | -------- |
 | Deneb     | 50-15.0 | 1990-01-02 | 03:00:00 |
 | Fomalhaut | 38-54.0 | 1990-01-02 | 03:01:00 |
@@ -159,14 +168,24 @@
 | Fomalhaut | 38-37.0 | 1990-01-02 | 03:11:00 |
 | Aldebaran | 17-50.0 | 1990-01-02 | 03:12:00 |
 ```
 
 The fit slope analysis shows that the Aldebaran observation at 03:07:00 scatters 9.79 arc minutes under the computed slope while the other Aldebaran observations are + 0.64' and + 1.74' respectively. This observation is clearly a blunder, and the LOP plot confirms that it is far away from our other LOPS so it is removed altogether from the *Sight List* and a new position is computed: 
 21-12.0-N, 157-31.5-W. The position can be further refined, by either selecting the individual sights with the least scatter, or averaging each set since the Fit-Slope analysis confirms their normal distribution, both methods will yield a fix with a similar level of accuracy. 
 
+![](gifs/blunder.png)
+
+*Capella screens for potentially erroneous shots using statistical tests and will alert the user to a potential blunder*
+
+![](gifs/blunder_2.png)
+
+*A fit slope analysis of a sight session, we see that of the two Aldebaran observations, one scatters far off of the correct slope and is likely a blunder*
+
+---
+
 ## Section 4: Planning/Session Data
 
 
 **Sight Planning** 
 
 The *Sight Planning* utility provides a quick and convenient means of plotting a round of observations prior to a sight session. Enter a UTC date and time in the provided sight fields and then hit the *Set Time* button. Using the provided DR date/time, Lat/Long and course/speed in the *Sight Entry* page, a DR position for the selected time and will appear in the two fields below. The *Time of Phenomena*, *Body List* and *Optimal Triads* will now be populated with information. 
 
@@ -182,24 +201,24 @@
 
 A weighting algorithm will list optimal groupings of 3 celestial objects based on azimuthal distribution, magnitude and altitude and list them in a scrollable table.
 
 *Example 3:*
 
 it is 2012-07-06 at 09:00:00 UTC and we wish to plan for the day's observations. We input the below information in the *Sight Entry* DR fields. 
 ```
-| DR Date    | DR Time  | DR L      | DR Î»       | Course | Speed | I.C. | H.O.E | Temp. | Press. |
+| DR Date    | DR Time  | DR L      | DR λ       | Course | Speed | I.C. | H.O.E | Temp. | Press. |
 | ---------- | -------- | --------- | ---------- | ------ | ----- | ---- | ----- | ----- | ------ | 
 | 2012-07-06 | 09:00:00 | 48-18.4-N | 006-26.5-W | 208    | 17    | 0.4  | 86    | 10    | 1010   | 
 ```
 
 We enter the 2012-07-06, 09:00:00 UTC in the input fields in the Planning Controls tab and hit *Set Time*. We click on the time of phenomena tab and see that L.A.N. will occur at 12:33:21 UTC. and PM Nautical Twilight will be around 21:00:00 UTC. 
 
 At 12:30:00 UTC we begin a round of noon sights:
 ```
-| DR Date    | DR Time   | DR L      | DR Î»       |   Course |   Speed |   I.C. |   H.O.E |   Temp. |   Press. | Fix Date   | Fix Time   |
+| DR Date    | DR Time   | DR L      | DR λ       |   Course |   Speed |   I.C. |   H.O.E |   Temp. |   Press. | Fix Date   | Fix Time   |
 |------------|-----------|-----------|------------|----------|---------|--------|---------|---------|----------|------------|------------|
 | 2012-07-06 | 12:30:00  | 47-25.9-N | 007-08.0-W |      208 |      17 |    0.4 |      86 |      10 |     1010 | 2012-07-06 | 12:33:22   |
  
 | Body   | Hs      | Date       | Time     |
 |--------|---------|------------|----------|
 | SunLL  | 65-03.4 | 2012-07-06 | 12:29:22 |
 | SunLL  | 65-05.3 | 2012-07-06 | 12:33:22 |
@@ -229,15 +248,15 @@
 
 **Analytics**
 
 *Best Sights*
 
 A list of the observations with the lowest scatter values per body. If only one body is observed but at distinct times, then the 'best' value is computed for each block of time. For example, in the below example the 'best' values are computed for 3 distinct blocks of time, the 1993-07-07 21:00:00 and 23:00:00 sessions and the 1993-07-08, 00:30:00 session. 
 ```
-| DR Date   | DR Time   | DR L    | DR Î»     |   Course |   Speed |   I.C. |   H.O.E |   Temp. |   Press. | Fix Date   | Fix Time   |
+| DR Date   | DR Time   | DR L    | DR λ     |   Course |   Speed |   I.C. |   H.O.E |   Temp. |   Press. | Fix Date   | Fix Time   |
 |-----------|-----------|---------|----------|----------|---------|--------|---------|---------|----------|------------|------------|
 | 1993-7-7  | 15:21:00  | 39-46-N | 161-20-W |      265 |       6 |   -1.5 |       9 |      10 |     1010 | 1993-7-8   | 00:33:12   |
  
 | Body  | Hs      | Date     | Time     |
 | ----- | ------- | -------- | -------- |
 | SunLL | 65-04.7 | 1993-7-7 | 21:30:17 |
 | SunLL | 65-19.7 | 1993-7-7 | 21:31:55 |
@@ -250,18 +269,66 @@
 
 *Position Errors*
 
 A table with the one and two Sigma errors for the fitting algorithm converted into nautical mile estimates. The goal is to provide the navigator with an estimate as to where their celestial fix has placed them vs. where they might actually be. However, It is important to remember that these errors are only relevant to the fit of the *information provided* and are not a magic bullet. For example, a two body fix is by definition an *exact* position, X marks the spot so to speak, and the 95% error estimate will be close to zero, however(!), the *exact* position is likely not *exactly* where you are. 
 
 Celestial Navigation under the most optimal and rigorous circumstances can provide a positional accuracy of around 1 nm, it is not a GPS. As always the prudent navigator uses more than one means of position fixing to navigate.
 
+---
+
 ## Section 5: Azimuth
 
 
 **Observation Input**
 
 In the *Observation Input* section, fill in the required input fields with the body observed, the gyro bearing and time and position of the observation. As with all other fields of their type in the program, autocompletion and format checking are provided to assist the navigator. 
 
 The output is provided in the *Compass Observations Records* field in the exact format used in the usual *Compass Observation Book* required by IMO standards. The Gyro Error, Compass Error, and Magnetic Variation and Magnetic Deviation are calculated. Magnetic Variation can be calculated for any position in the world and uses the World Magnetic Model Epoch 2020. The list of gaussian coefficients is internal to the program and is valid through 2025. 
 
+--- 
+
+# A short, true, sea story (An end-to-end example of usage)
+
+We're on a large commercial vessel steaming from the Pacific Northwest to Hawaii at a speed of 12 kts on a course of 251 True. It's 19:55 ship's time, the third mate is back on the bridge, and we've been relieved of the watch. The third mate pours a cup of coffee and jokes that the sun has just set and star time is upon us. "Show off your fancy program!" he says. "Sure!", we say. We grab the ship's sextant from under the chart table and fire up *Capella*.
+
+We enter our DR information, using 05:00:00 UTC as our DR time and choose DR coordinates we know we are within 100 NM of. We're  being deliberately vague. We know our height of eye to within 30 feet so we guess that its 158 feet. It's a big ship. 
+
+We proceed to the sight planning section and enter 05:15:00 as the time we'd like to generate sights for. We won't preset our sextant, we just want a general orientation of the evening's sky. We note the brightest and most visible stars and planets, quickly scratch them down, and then grab the sextant and head out on the bridge wing.  
+
+Once outside we find the sky is largely overcast. A quick shot of the horizon suggests the index error is around 2.0' on the arc. We look up and scan the sky. Sirius pops through the clouds and we grab 3 quick sights in succession. About 10 minutes later Rigel briefly shows up in between the clouds and we're able to grab 2 quick sights. Capella briefly emerges and we're able to get one shot, but then the clouds shroud the star and it remains hidden. Discouraged, we grab 2 quick lower limb shots of the moon and head back to the chart room. The shots were fast and likely not very precise, we don't expect much. The third mate is amused at our obvious frustration.
+
+We write everything down and look over the shots:
+
+```
+| Body    | Hs      | Date       | Time     |
+| ------- | ------- | ---------- | -------- |
+| Sirius  | 51-13.8 | 2022-03-18 | 05:04:06 |
+| Sirius  | 51-12.2 | 2022-03-18 | 05:05:44 |
+| Sirius  | 51-22.1 | 2022-03-18 | 05:07:16 |
+| Rigel   | 54-15.2 | 2022-03-18 | 05:15:48 |
+| Rigel   | 54-21.5 | 2022-03-18 | 05:17:16 |
+| Capella | 61-34.0 | 2022-03-18 | 05:13:42 |
+| MoonLL  | 11-30.5 | 2022-03-18 | 05:18:57 |
+| MoonLL  | 11-45.6 | 2022-03-18 | 05:20:25 |
+```
+
+We enter all of our sights and  calculate a fix using all of the observations. Immediately, *Capella* prompts us with a message box saying that something is likely wrong with our 05:17:16 Rigel observation. We look at the LOP plot and notice that it is an obvious blunder. 
+
+We remove the Rigel shot and re-compute the fix. We are now greeted with a message box saying that there is systematic error in our observations and are asked if we would like to recompute. We decided to first use the fit-slope analysis tool to see if any one shot is adding extra weight to the error calculation. 
+
+The fit-slope plots show that 2 of our Sirius shots scatter above the fitted line, while the middle observation scatters below. An analysis of the LOP's also suggests that our middle Sirius shot is a potential outlier. We remove the second Sirius observation and average the rest of the sights. We again calculate our position and are again greeted with a message box asking us to remove systematic error. It's clear we've overestimated our height of eye or incorrectly deduced our index error, so we click yes and remove the error and recompute our position again and receive no more messages. 
+
+The fix was calculated for 05:18:00 and we get the following prediction: 21-51.5 N, 155-41.0 W. We go back to the LOP plot section and note a nice tight cocked hat and small confidence ellipse -- with a small amount of logical deduction we've turned a fairly messy fix into what looks like a pretty good one. We note the ship's GPS log and see that our 05:18:00 UTC position was 21-51.2, 155-41.4, *we were only .55 NM off*. Pleased, we wink at the third mate, put the sextant back in the box and stroll off of the bridge, only to hurry down the ladderwell to our stateroom--*we have to be back on watch in 5 hours*.
+
+### Above Steps Demonstrated
+
+![](gifs/poa_shots.gif)
+
+---
+#### Disclaimer:
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+---
 
+### About
 
+Capt. Alex Spradling holds 1600 Ton Master Oceans, and 2nd Mate Unlimited Tonnage Oceans Licenses and actively sails as a deck officer in the U.S. Merchant Marine. He is a graduate of SUNY Maritime College.
```

### Comparing `Capella-1.0.3/LICENSE` & `Capella-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Capella-1.0.3/PKG-INFO` & `Capella-1.0.4/Capella.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Capella
-Version: 1.0.3
+Version: 1.0.4
 Summary: Capella Beta
-Home-page: https://github.com/AlexSpradling/Capellav.git
+Home-page: https://github.com/AlexSpradling/Capella.git
 Author: AlexSpradling
 Author-email: alexspradling@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,47 +16,62 @@
 ## Installation
 
 `pip install Capella`
 
 ### To Run:
 Navigate to your python installation and go to `lib\site-packages` open the `Capella` directory in your terminal and run `main.py`, the GUI will open from the terminal.
 
+---
 
 ### Introduction
 
 Capella is a simple-to-use Astronavigation aid. The program will derive a celestial position from a minimum of inputs and plot the position on a chartlet, with an analysis of the accuracy of  computed position provided. The program  additionally features some helper functions for celestial observation session planning, DR computation and compass correction. 
 
+
+![](gifs/demo.gif)
+
+---
 ## Section 1: Sight Entry
 
 **DR Information**
 
 All effective navigation starts with keeping a DR. Capella is no different. For the program to work effectively, first provide a DR position, time, course and speed. 
 
 Capella uses the standard nautical conventions for time and position formatting, and all times are kept in UTC. Capella will format the input for you---just type in the numbers for the respective field and when you are finished press tab or click to advance to the next input field. If erroneous information has been inputted, the field will flag RED. 
 
+
 **Sight Entry**
 
 In the Step 2 section, complete the four required fields. All the input fields will assist with autocompletion and formatting. The fields are: 1. Body 2. Hs Value 3. Sight Date 4. Sight Time. 
 All sextant altitude corrections are handled internally, simply input the Hs value for the observation.
 
 When you have completed the four input fields, hit the *Add* button and the sight will appear in the Sight List at the top of the screen. To edit previously entered information, click on the sight in the *Sight List*, the sight's information will populate the sight entry fields under Step 2. Make any required changes and hit *Update* and the sight entry will change in the *Sight List*. To remove a sight from the *Sight List*, simply click on the sight and hit *Delete*. Multiple sight handling is easily achieved using the conventional Shift or Ctrl + click features. 
 
+
 *Averaging*
 
 If you have multiple observations of the same body, you can CTRL or SHIFT click on them in the Sight Entry area, and the average of their Hs and time/date values will appear in the Step 2-Entry area. Press the *Add* button to add the averaged sight. It is recommended you first compute the position with all sights unaveraged and use the *Fit-Slope Analysis* feature to find which values should be eschewed or kept for averaging.
 
+![](gifs/blunder_3.png)
+
+*LOP plot before fit-slope analysis and sight averaging*
+
+![](gifs/blunder_fixed.png)
+
+*LOP plot after fit-slope analysis and sight averaging*
+
 *Almanac Computation*
 
 Capella features a high-accuracy perpetual almanac valid from the years 1900-2050, with the data taken from the JPL de421 database. Once the fix is computed, all almanac data is displayed in the *Sight Data/Planning* section. 
 
 **Fix Computation**
 
 Capella will calculate a fix from the DR information provided in Step 1 and the sights added to the Sight List. A fix can be calculated from just one sight and the provided DR information, however the algorithm needs at least 2 sights to provide a more accurate fix. Once two or more sights are present in the *Sight List* and a *Fix Time* and *Fix Date* has been provided in the *Step 1* field, hit the *Compute* button or press *CTRL-l*. Capella will calculate a running fix based on the DR and *Fix Time* information provided. The calculated results as well as a DR position for the requested *Fix Time* will appear highlighted at the bottom. 
 
-The position calculation is provided by the robust Limited Memory-BFGS algorithm. This algorithm is robust with respect to erroneous DR information, will not converge to a local minimum and can effectively handle high altitude sights. Prudent navigation always requires the most accurate DR possible, however, the fitting algorithm is somewhat robust with respect to DR accuracy. 
+A position is calculated using a Limited Memory-BFGS algorithm. The algorithm is robust with respect to erroneous DR information, and can effectively handle high altitude sights. Prudent navigation always requires the most accurate DR possible, however, the fitting algorithm is quite robust with respect to DR accuracy. 
 
 *Example 1:*
 
 The Sight Information below yields the fix: **40-14.0-N, 049-58.0-W**.
 ```
 | DR Date   | DR Time  | DR L      | DR Î»       | Course | Speed | I.C. | H.O.E | Temp. | Press. | Fix Date  | Fix Time |
 | --------- | -------- | --------- | ---------- | ------ | ----- | ---- | ----- | ----- | ------ | --------- | -------- |
@@ -73,14 +88,15 @@
 ```
 by changing the DR Position to 00-00.0-N and 000-00.0-W *--a position 3673 nm away--* and keeping the same observation data, Capella yields the fix: **40-14.3-N, 049-57.8-W**. 
 
 **Systematic Error**
 
 If Capella's systematic error algorithm detects uncorrected index and personal error, a prompt will appear asking you could like to remove the error from your observations and recompute the fix. Click *Ok* and then click *Compute*. This process can be iterative and the prompt might appear multiple times, with each cycle bringing the calculated fix closer to the observer's true position. This method isn't a magic bullet, but can yield impressive results in certain circumstances. 
 
+
 **Loading and Saving Observation Records**
 
 Capella uses the computer's clipboard as a means of loading and saving observations. Rather than saving the observations in a proprietary format, the observations are copied to the clipboard as a simple markdown format table than can be pasted into any .txt file the navigator wishes to use as a sight log. 
 
 *To Save Sights*
 1. In Capella, click File-Save Sights to Clipboard or CTRL-s. 
 2. 2 markdown format tables will be saved to your computer's clipboard.
@@ -101,14 +117,17 @@
 | 2012-07-06 | 12:30:00  | 47-25.9-N | 007-08.0-W |      208 |      17 |    0.4 |      86 |      10 |     1010 | 2012-07-06 | 12:33:22   |
  
 | Body   | Hs      | Date       | Time     |
 |--------|---------|------------|----------|
 | SunLL  | 65-03.4 | 2012-07-06 | 12:29:22 |
 ```
 
+![](gifs/saving_loading.gif)
+
+---
 
 
 ## Section 2: LOP Plot
 
 **Exploring the plot**
 
 Once the fix is computed from the *Sight Entry* page, the LOP's for the observations are automatically plotted. The plot is highly customizable with respect to  size, aspect and zoom via the buttons located in the lower right corner. Click the *NSEW arrow* icon and then left-click and drag on the plot to move the plot, the Latitude and Longitude scales will automatically change. A right-click and drag will change the plots aspect. To reset the plot back to the default at any time, click on the *House* icon. To zoom in on the plot, click the *Magnifying Glass* icon and then left-click and drag to zoom-in and right-click and drag to zoom-out. 
@@ -119,14 +138,17 @@
 
 The LOPS are automatically advanced with the course and speed information provided in the *Sight Entry* section and bodies are labeled on the plot and in the sight key area. Additionally, the computed DR position for the *Fix Time* is also plotted. If the DR is very far from the LOP plot, the plot will need to be zoomed for a better aspect, however, if a good DR is being kept, this should not be necessary in most cases. 
 
 **Fix + Confidence**
 
 The red dot on the LOP plot marks the computed position and the golden ellipse surrounding the computed fix represents an area of 95% confidence. That is, there is a 95% probability, *given the sight information provided* that the true position lies within the ellipse.
 
+![](gifs/confidence_ellipse.png)
+
+---
 ## Section 3: Fit Slope Analysis
 
 This is an implementation of Dr. David Burch's Fit Slope method. It is a means of deriving greater accuracy from our sight observations and attempting to spot any outliers or potential blunders. 
 
 **How  Fit-Slope Analysis works**
 
 The vessel is moving all the time at sea and and the celestial objects are moving all the time as well. If we take 3 observations of the Sun, how do we know which observations were accurate and which weren't? 
@@ -159,14 +181,24 @@
 | Fomalhaut | 38-37.0 | 1990-01-02 | 03:11:00 |
 | Aldebaran | 17-50.0 | 1990-01-02 | 03:12:00 |
 ```
 
 The fit slope analysis shows that the Aldebaran observation at 03:07:00 scatters 9.79 arc minutes under the computed slope while the other Aldebaran observations are + 0.64' and + 1.74' respectively. This observation is clearly a blunder, and the LOP plot confirms that it is far away from our other LOPS so it is removed altogether from the *Sight List* and a new position is computed: 
 21-12.0-N, 157-31.5-W. The position can be further refined, by either selecting the individual sights with the least scatter, or averaging each set since the Fit-Slope analysis confirms their normal distribution, both methods will yield a fix with a similar level of accuracy. 
 
+![](gifs/blunder.png)
+
+*Capella screens for potentially erroneous shots using statistical tests and will alert the user to a potential blunder*
+
+![](gifs/blunder_2.png)
+
+*A fit slope analysis of a sight session, we see that of the two Aldebaran observations, one scatters far off of the correct slope and is likely a blunder*
+
+---
+
 ## Section 4: Planning/Session Data
 
 
 **Sight Planning** 
 
 The *Sight Planning* utility provides a quick and convenient means of plotting a round of observations prior to a sight session. Enter a UTC date and time in the provided sight fields and then hit the *Set Time* button. Using the provided DR date/time, Lat/Long and course/speed in the *Sight Entry* page, a DR position for the selected time and will appear in the two fields below. The *Time of Phenomena*, *Body List* and *Optimal Triads* will now be populated with information. 
 
@@ -250,18 +282,66 @@
 
 *Position Errors*
 
 A table with the one and two Sigma errors for the fitting algorithm converted into nautical mile estimates. The goal is to provide the navigator with an estimate as to where their celestial fix has placed them vs. where they might actually be. However, It is important to remember that these errors are only relevant to the fit of the *information provided* and are not a magic bullet. For example, a two body fix is by definition an *exact* position, X marks the spot so to speak, and the 95% error estimate will be close to zero, however(!), the *exact* position is likely not *exactly* where you are. 
 
 Celestial Navigation under the most optimal and rigorous circumstances can provide a positional accuracy of around 1 nm, it is not a GPS. As always the prudent navigator uses more than one means of position fixing to navigate.
 
+---
+
 ## Section 5: Azimuth
 
 
 **Observation Input**
 
 In the *Observation Input* section, fill in the required input fields with the body observed, the gyro bearing and time and position of the observation. As with all other fields of their type in the program, autocompletion and format checking are provided to assist the navigator. 
 
 The output is provided in the *Compass Observations Records* field in the exact format used in the usual *Compass Observation Book* required by IMO standards. The Gyro Error, Compass Error, and Magnetic Variation and Magnetic Deviation are calculated. Magnetic Variation can be calculated for any position in the world and uses the World Magnetic Model Epoch 2020. The list of gaussian coefficients is internal to the program and is valid through 2025. 
 
+--- 
+
+# A short, true, sea story (An end-to-end example of usage)
+
+We're on a large commercial vessel steaming from the Pacific Northwest to Hawaii at a speed of 12 kts on a course of 251 True. It's 19:55 ship's time, the third mate is back on the bridge, and we've been relieved of the watch. The third mate pours a cup of coffee and jokes that the sun has just set and star time is upon us. "Show off your fancy program!" he says. "Sure!", we say. We grab the ship's sextant from under the chart table and fire up *Capella*.
+
+We enter our DR information, using 05:00:00 UTC as our DR time and choose DR coordinates we know we are within 100 NM of. We're  being deliberately vague. We know our height of eye to within 30 feet so we guess that its 158 feet. It's a big ship. 
+
+We proceed to the sight planning section and enter 05:15:00 as the time we'd like to generate sights for. We won't preset our sextant, we just want a general orientation of the evening's sky. We note the brightest and most visible stars and planets, quickly scratch them down, and then grab the sextant and head out on the bridge wing.  
+
+Once outside we find the sky is largely overcast. A quick shot of the horizon suggests the index error is around 2.0' on the arc. We look up and scan the sky. Sirius pops through the clouds and we grab 3 quick sights in succession. About 10 minutes later Rigel briefly shows up in between the clouds and we're able to grab 2 quick sights. Capella briefly emerges and we're able to get one shot, but then the clouds shroud the star and it remains hidden. Discouraged, we grab 2 quick lower limb shots of the moon and head back to the chart room. The shots were fast and likely not very precise, we don't expect much. The third mate is amused at our obvious frustration.
+
+We write everything down and look over the shots:
+
+```
+| Body    | Hs      | Date       | Time     |
+| ------- | ------- | ---------- | -------- |
+| Sirius  | 51-13.8 | 2022-03-18 | 05:04:06 |
+| Sirius  | 51-12.2 | 2022-03-18 | 05:05:44 |
+| Sirius  | 51-22.1 | 2022-03-18 | 05:07:16 |
+| Rigel   | 54-15.2 | 2022-03-18 | 05:15:48 |
+| Rigel   | 54-21.5 | 2022-03-18 | 05:17:16 |
+| Capella | 61-34.0 | 2022-03-18 | 05:13:42 |
+| MoonLL  | 11-30.5 | 2022-03-18 | 05:18:57 |
+| MoonLL  | 11-45.6 | 2022-03-18 | 05:20:25 |
+```
+
+We enter all of our sights and  calculate a fix using all of the observations. Immediately, *Capella* prompts us with a message box saying that something is likely wrong with our 05:17:16 Rigel observation. We look at the LOP plot and notice that it is an obvious blunder. 
+
+We remove the Rigel shot and re-compute the fix. We are now greeted with a message box saying that there is systematic error in our observations and are asked if we would like to recompute. We decided to first use the fit-slope analysis tool to see if any one shot is adding extra weight to the error calculation. 
+
+The fit-slope plots show that 2 of our Sirius shots scatter above the fitted line, while the middle observation scatters below. An analysis of the LOP's also suggests that our middle Sirius shot is a potential outlier. We remove the second Sirius observation and average the rest of the sights. We again calculate our position and are again greeted with a message box asking us to remove systematic error. It's clear we've overestimated our height of eye or incorrectly deduced our index error, so we click yes and remove the error and recompute our position again and receive no more messages. 
+
+The fix was calculated for 05:18:00 and we get the following prediction: 21-51.5 N, 155-41.0 W. We go back to the LOP plot section and note a nice tight cocked hat and small confidence ellipse -- with a small amount of logical deduction we've turned a fairly messy fix into what looks like a pretty good one. We note the ship's GPS log and see that our 05:18:00 UTC position was 21-51.2, 155-41.4, *we were only .55 NM off*. Pleased, we wink at the third mate, put the sextant back in the box and stroll off of the bridge, only to hurry down the ladderwell to our stateroom--*we have to be back on watch in 5 hours*.
+
+### Above Steps Demonstrated
+
+![](gifs/poa_shots.gif)
+
+---
+#### Disclaimer:
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+---
 
+### About
 
+Capt. Alex Spradling holds 1600 Ton Master Oceans, and 2nd Mate Unlimited Tonnage Oceans Licenses and actively sails as a deck officer in the U.S. Merchant Marine. He is a graduate of SUNY Maritime College.
```

