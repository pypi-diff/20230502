# Comparing `tmp/exergenics-2.6.0.tar.gz` & `tmp/exergenics-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-2.6.0.tar", last modified: Wed Apr 26 01:25:10 2023, max compression
+gzip compressed data, was "exergenics-2.7.0.tar", last modified: Tue May  2 08:58:06 2023, max compression
```

## Comparing `exergenics-2.6.0.tar` & `exergenics-2.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 01:25:10.543620 exergenics-2.6.0/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-26 01:25:10.543620 exergenics-2.6.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 01:25:10.539620 exergenics-2.6.0/exergenics/
--rw-rw-r--   0 root         (0) root         (0)       37 2023-04-26 01:23:52.000000 exergenics-2.6.0/exergenics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    59324 2023-04-26 01:23:52.000000 exergenics-2.6.0/exergenics/exergenics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 01:25:10.543620 exergenics-2.6.0/exergenics.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-26 01:25:10.000000 exergenics-2.6.0/exergenics.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 01:25:10.543620 exergenics-2.6.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      672 2023-04-26 01:25:08.000000 exergenics-2.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:58:06.951701 exergenics-2.7.0/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-02 08:58:06.951701 exergenics-2.7.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:58:06.951701 exergenics-2.7.0/exergenics/
+-rw-rw-r--   0 root         (0) root         (0)       37 2023-05-02 08:56:50.000000 exergenics-2.7.0/exergenics/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    60098 2023-05-02 08:56:50.000000 exergenics-2.7.0/exergenics/exergenics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 08:58:06.951701 exergenics-2.7.0/exergenics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-02 08:58:06.000000 exergenics-2.7.0/exergenics.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 08:58:06.951701 exergenics-2.7.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      672 2023-05-02 08:58:04.000000 exergenics-2.7.0/setup.py
```

### Comparing `exergenics-2.6.0/exergenics/exergenics.py` & `exergenics-2.7.0/exergenics/exergenics.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,35 +297,35 @@
         return True
 
     # function  : getBuilding
     # param     : buildingCode
     def getWeather(self, buildingCode, distance=20):
 
         subDomain = "staging"
-        if self.mode=="production":
-            subDomain  = "app"
+        if self.mode == "production":
+            subDomain = "app"
 
-        req =  "https://"+subDomain+".exergenicsportal.com/api/ex/index.php?I_AM_LAMBDA=eyJraWQiOiJpRlwvb0dLamdOTjdLMlEwMWNFRndXUkFROWFZWWdKZ3BBZlNOdDJyWWFIQT0iLCJhbGciOiJSUzI1NiJ9&path=/getWeather/"+buildingCode+"&httpMethod=GET&awsSubscriptionKey=7b786790-6e4e-4310-bfc7-d30aec6beb02&queryStringParameters={\"distance\":" + \
-             str(distance) + \
-             "}&postParams=&whoAmI=getWeatherProduction&"
+        req = "https://" + subDomain + ".exergenicsportal.com/api/ex/index.php?I_AM_LAMBDA=eyJraWQiOiJpRlwvb0dLamdOTjdLMlEwMWNFRndXUkFROWFZWWdKZ3BBZlNOdDJyWWFIQT0iLCJhbGciOiJSUzI1NiJ9&path=/getWeather/" + buildingCode + "&httpMethod=GET&awsSubscriptionKey=7b786790-6e4e-4310-bfc7-d30aec6beb02&queryStringParameters={\"distance\":" + \
+              str(distance) + \
+              "}&postParams=&whoAmI=getWeatherProduction&"
         request = requests.get(req)
-        return  request.json()["body"]
-
+        return request.json()["body"]
 
     def setEquipmentVariableValue(self, plantCode, equipmentTag, variableName, variableValue):
         activityUrl = "{}/{}/{}/?variableName={}&variableValue={}".format(self.ex__setEquipmentVariableValue, plantCode,
                                                                           equipmentTag, variableName, variableValue)
         self.lastStatus, self.lastResponse = self.doRequest(
             self.getExchangeEndpoint(), activityUrl, {})
         if self.noResponse():
             return False
         return self.lastResponse
 
     def getEquipmentVariableValue(self, plantCode, equipmentTag, variableName):
-        activityUrl = "{}/{}/{}/?variableName={}".format(self.ex__getEquipmentVariableValue, plantCode, equipmentTag, variableName)
+        activityUrl = "{}/{}/{}/?variableName={}".format(self.ex__getEquipmentVariableValue, plantCode, equipmentTag,
+                                                         variableName)
         self.lastStatus, self.lastResponse = self.doRequest(
             self.getExchangeEndpoint(), activityUrl, {})
         if self.noResponse():
             return False
         return self.lastResponse
 
     def jobLogInfo(self, jobId, message):
@@ -540,18 +540,26 @@
         client = boto3.client(
             's3',
             region_name='ap-southeast-2',
             aws_access_key_id=AWS_ACCESS_KEY_ID,
             aws_secret_access_key=AWS_SECRET_ACCESS_KEY
         )
         today = date.today()
+
+        extraArgs = {'ContentType': contentType}
+        if contentType == "text/html" or contentType == "html":
+            extraArgs = {
+                'ContentType': 'text/html',
+                'ContentDisposition': 'inline'
+            }
+
         saveAs = "{}/{}/{}/{}__{}".format(today.year, today.month,
                                           today.day, uuid.uuid4().hex, localFile)
         client.upload_file(Filename=localFile, Bucket=self.aws_bucketName, Key=saveAs,
-                           ExtraArgs={'ContentType': contentType})
+                           ExtraArgs=extraArgs)
         return "{}{}".format(self.aws_bucketRoot, saveAs)
 
     def getJobs(self, stage, status="completed"):
         activityUrl = "{}/{}/{}".format(self.ex__getJobs, stage, status)
 
         self.lastStatus, self.lastResponse = self.doRequest(
             self.getExchangeEndpoint(), activityUrl, {})
@@ -990,15 +998,15 @@
                                             chartWidth, chartHeight, backgroundColor, fontSize, fontFamily,
                                             fontColor, legendFamily, legendSize, legendColor, legendBg, titleFont,
                                             titleColor)
         self.putFile(plantCode, urlToChart, portalCategory,
                      chartName, equipCode, jobId)
         return urlToChart
 
-    def plotlyBowlChart2D(self, data, optimalPointX="optimalPointX", optimalPointY="optimalPointY", title="title", 
+    def plotlyBowlChart2D(self, data, optimalPointX="optimalPointX", optimalPointY="optimalPointY", title="title",
                           legendTitle="legendTitle", xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle",
                           yAxis2Title="yAxis2Title", outputType="html", backgroundColor="white",
                           chartWidth=800, chartHeight=600, fontSize=12, fontFamily="TimesNewRoman", fontColor="black",
                           legendFamily="Courier", legendSize=12, legendColor="black", legendBg="LightSteelBlue",
                           titleFont="Arial", titleColor="black"):
 
         return self.plotlyRequest("bowlchart2D", {
@@ -1026,19 +1034,21 @@
         }, "urlToBowlChart2D")
 
     def portalChart_bowlChart2D(self, plantCode, chartName, portalCategory, data, optimalPointX="optimalPointX",
                                 optimalPointY="optimalPointY", title="title", legendTitle="legendTitle",
                                 xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle", yAxis2Title="yAxis2Title",
                                 outputType="html", backgroundColor="white", chartWidth=800, chartHeight=600,
                                 fontSize=12, fontFamily="TimesNewRoman", fontColor="black", legendFamily="Courier",
-                                legendSize=12, legendColor="black",legendBg="LightSteelBlue", titleFont="Arial",
+                                legendSize=12, legendColor="black", legendBg="LightSteelBlue", titleFont="Arial",
                                 titleColor="black", equipCode="", jobId=""):
-        urlToChart = self.plotlyBowlChart2D(data, optimalPointX, optimalPointY, title, legendTitle, xAxisTitle, yAxisTitle,
+        urlToChart = self.plotlyBowlChart2D(data, optimalPointX, optimalPointY, title, legendTitle, xAxisTitle,
+                                            yAxisTitle,
                                             yAxis2Title, outputType, backgroundColor, chartWidth, chartHeight, fontSize,
-                                            fontFamily, fontColor, legendFamily, legendSize, legendColor, legendBg, titleFont,
+                                            fontFamily, fontColor, legendFamily, legendSize, legendColor, legendBg,
+                                            titleFont,
                                             titleColor)
         self.putFile(plantCode, urlToChart, portalCategory,
                      chartName, equipCode, jobId)
         return urlToChart
 
     def plotlyBowlChart3D(self, point, x, y, z, title="title", legendTitle="legendTitle", xAxisTitle="xAxisTitle",
                           yAxisTitle="yAxisTitle", zAxisTitle="zAxisTitle", outputType="html", backgroundColor="white",
@@ -1083,18 +1093,20 @@
                                             fontColor, legendFamily, legendSize, legendColor, legendBg, titleFont,
                                             titleColor)
         self.putFile(plantCode, urlToChart, portalCategory,
                      chartName, equipCode, jobId)
         return urlToChart
 
     def plotlyDynamicBowlChart2D(self, data, legendTitle="legendTitle", xAxisTitle="xAxisTitle",
-                          yAxisTitle="yAxisTitle", yAxis2Title="yAxis2Title", outputType="html", backgroundColor="white",
-                          chartWidth=800, chartHeight=600, fontSize=12, fontFamily="TimesNewRoman", fontColor="black",
-                          legendFamily="Courier", legendSize=12, legendColor="black", legendBg="LightSteelBlue",
-                          titleFont="Arial", titleColor="black"):
+                                 yAxisTitle="yAxisTitle", yAxis2Title="yAxis2Title", outputType="html",
+                                 backgroundColor="white",
+                                 chartWidth=800, chartHeight=600, fontSize=12, fontFamily="TimesNewRoman",
+                                 fontColor="black",
+                                 legendFamily="Courier", legendSize=12, legendColor="black", legendBg="LightSteelBlue",
+                                 titleFont="Arial", titleColor="black"):
 
         return self.plotlyRequest("dynamicbowlchart2D", {
             "dataJSON": data,
             "legendTitle": legendTitle,
             "xAxisTitle": xAxisTitle,
             "yAxisTitle": yAxisTitle,
             "yAxis2Title": yAxis2Title,
@@ -1109,35 +1121,36 @@
             "legendSize": legendSize,
             "legendColor": legendColor,
             "legendBg": legendBg,
             "titleFont": titleFont,
             "titleColor": titleColor
         }, "urlToDynamicBowlChart2D")
 
-
     def portalChart_dynamicBowlChart2D(self, plantCode, chartName, portalCategory, data,
-                                legendTitle="legendTitle", xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle",
-                                yAxis2Title="yAxis2Title", outputType="html", backgroundColor="white",
-                                chartWidth=800, chartHeight=600, fontSize=12, fontFamily="TimesNewRoman",
-                                fontColor="black", legendFamily="Courier", legendSize=12, legendColor="black",
-                                legendBg="LightSteelBlue", titleFont="Arial", titleColor="black", equipCode="",
-                                jobId=""):
+                                       legendTitle="legendTitle", xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle",
+                                       yAxis2Title="yAxis2Title", outputType="html", backgroundColor="white",
+                                       chartWidth=800, chartHeight=600, fontSize=12, fontFamily="TimesNewRoman",
+                                       fontColor="black", legendFamily="Courier", legendSize=12, legendColor="black",
+                                       legendBg="LightSteelBlue", titleFont="Arial", titleColor="black", equipCode="",
+                                       jobId=""):
         urlToChart = self.plotlyDynamicBowlChart2D(data, legendTitle, xAxisTitle, yAxisTitle, yAxis2Title,
-                                            outputType, backgroundColor, chartWidth, chartHeight, fontSize, fontFamily,
-                                            fontColor, legendFamily, legendSize, legendColor, legendBg, titleFont,
-                                            titleColor)
+                                                   outputType, backgroundColor, chartWidth, chartHeight, fontSize,
+                                                   fontFamily,
+                                                   fontColor, legendFamily, legendSize, legendColor, legendBg,
+                                                   titleFont,
+                                                   titleColor)
         self.putFile(plantCode, urlToChart, portalCategory,
                      chartName, equipCode, jobId)
         return urlToChart
 
     def plotlyDynamicBarChart2D(self, data, legendTitle="legendTitle", xAxisTitle="xAxisTitle",
-                          yAxisTitle="yAxisTitle", outputType="html", backgroundColor="white",
-                          chartWidth=800, chartHeight=600, fontSize=16, fontFamily="Verdana", fontColor="black",
-                          legendFamily="Verdana", legendSize=15, legendColor="black", legendBg="LightSteelBlue",
-                          titleFont="Arial", titleColor="black"):
+                                yAxisTitle="yAxisTitle", outputType="html", backgroundColor="white",
+                                chartWidth=800, chartHeight=600, fontSize=16, fontFamily="Verdana", fontColor="black",
+                                legendFamily="Verdana", legendSize=15, legendColor="black", legendBg="LightSteelBlue",
+                                titleFont="Arial", titleColor="black"):
 
         return self.plotlyRequest("dynamicbarchart2D", {
             "dataJSON": data,
             "legendTitle": legendTitle,
             "xAxisTitle": xAxisTitle,
             "yAxisTitle": yAxisTitle,
             "outputType": outputType,
@@ -1152,23 +1165,24 @@
             "legendColor": legendColor,
             "legendBg": legendBg,
             "titleFont": titleFont,
             "titleColor": titleColor
         }, "urlToDynamicBarChart2D")
 
     def portalChart_dynamicBarChart2D(self, plantCode, chartName, portalCategory, data,
-                                legendTitle="legendTitle", xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle",
-                                outputType="html", backgroundColor="white", chartWidth=800, chartHeight=600,
-                                fontSize=16, fontFamily="Verdana", fontColor="black", legendFamily="Verdana",
-                                legendSize=15, legendColor="black", legendBg="LightSteelBlue",
-                                titleFont="Arial", titleColor="black", equipCode="", jobId=""):
+                                      legendTitle="legendTitle", xAxisTitle="xAxisTitle", yAxisTitle="yAxisTitle",
+                                      outputType="html", backgroundColor="white", chartWidth=800, chartHeight=600,
+                                      fontSize=16, fontFamily="Verdana", fontColor="black", legendFamily="Verdana",
+                                      legendSize=15, legendColor="black", legendBg="LightSteelBlue",
+                                      titleFont="Arial", titleColor="black", equipCode="", jobId=""):
         urlToChart = self.plotlyDynamicBarChart2D(data, legendTitle, xAxisTitle, yAxisTitle,
-                                            outputType, backgroundColor, chartWidth, chartHeight, fontSize, fontFamily,
-                                            fontColor, legendFamily, legendSize, legendColor, legendBg, titleFont,
-                                            titleColor)
+                                                  outputType, backgroundColor, chartWidth, chartHeight, fontSize,
+                                                  fontFamily,
+                                                  fontColor, legendFamily, legendSize, legendColor, legendBg, titleFont,
+                                                  titleColor)
         self.putFile(plantCode, urlToChart, portalCategory,
                      chartName, equipCode, jobId)
         return urlToChart
 
 
 '''
 *****************************
@@ -1176,15 +1190,15 @@
 *****************************
 
 N.WONG FEB 2023
 Implements exergenics internal application logging by providing a Logtail interface
 '''
 
 
-class Singleton (type):
+class Singleton(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(
                 Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
@@ -1211,15 +1225,16 @@
     In sub-functions:
 
     logger = Logger()
     logger.info('message')
 
     """
 
-    def __init__(self, loggerName: str,  component: str = '', subComponent: str = '', jobId: str = '', environment: str = ''):
+    def __init__(self, loggerName: str, component: str = '', subComponent: str = '', jobId: str = '',
+                 environment: str = ''):
         """Initialise the logger object
 
         Parameters
         ----------
         loggerName : str
             Logger name in string format.
         component : str
@@ -1335,8 +1350,7 @@
 
         Returns
         -------
         str
             Logger version in string
         """
         return str(self._version)
-
```

### Comparing `exergenics-2.6.0/setup.py` & `exergenics-2.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='exergenics',
-    version='2.6.0',
+    version='2.7.0',
     author="John Christian",
     author_email='john.christian@exergenics.com',
     packages=['exergenics'],
     long_description="",
     long_description_content_type="text/markdown",
     # package_dir={'': 'src'},
     url='https://github.com/Exergenics/internal-portal-api',
```

