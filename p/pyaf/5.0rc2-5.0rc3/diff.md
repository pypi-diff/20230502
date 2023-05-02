# Comparing `tmp/pyaf-5.0rc2-py2.py3-none-any.whl.zip` & `tmp/pyaf-5.0rc3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,53 @@
-Zip file size: 137643 bytes, number of entries: 55
--rw-r--r--  2.0 unx     2601 b- defN 22-Jul-12 18:14 pyaf/ForecastEngine.py
--rw-r--r--  2.0 unx     4288 b- defN 22-Jul-12 18:14 pyaf/HierarchicalForecastEngine.py
--rw-r--r--  2.0 unx      475 b- defN 23-Mar-18 03:44 pyaf/__init__.py
+Zip file size: 130774 bytes, number of entries: 51
+-rw-r--r--  2.0 unx     2286 b- defN 23-Apr-06 21:36 pyaf/ForecastEngine.py
+-rw-r--r--  2.0 unx     3972 b- defN 23-Apr-06 21:36 pyaf/HierarchicalForecastEngine.py
+-rw-r--r--  2.0 unx      576 b- defN 23-May-02 12:06 pyaf/__init__.py
 -rw-r--r--  2.0 unx      559 b- defN 22-Jul-12 18:14 pyaf/Bench/Artificial.py
--rw-r--r--  2.0 unx    19020 b- defN 23-Mar-23 11:09 pyaf/Bench/GenericBenchmark.py
+-rw-r--r--  2.0 unx    18471 b- defN 23-Apr-06 21:38 pyaf/Bench/GenericBenchmark.py
 -rw-r--r--  2.0 unx      773 b- defN 22-Jul-12 18:14 pyaf/Bench/MComp.py
 -rw-r--r--  2.0 unx      693 b- defN 22-Jul-12 18:14 pyaf/Bench/NN3.py
--rw-r--r--  2.0 unx    38915 b- defN 23-Mar-22 10:56 pyaf/Bench/TS_datasets.py
+-rw-r--r--  2.0 unx    39004 b- defN 23-Mar-31 09:19 pyaf/Bench/TS_datasets.py
 -rw-r--r--  2.0 unx      516 b- defN 22-Jul-12 18:14 pyaf/Bench/YahooStocks.py
 -rw-r--r--  2.0 unx        0 b- defN 22-May-14 18:26 pyaf/Bench/__init__.py
 -rw-r--r--  2.0 unx      341 b- defN 22-Jul-12 18:14 pyaf/Bench/download_all_stock_prices.py
 -rw-r--r--  2.0 unx    69054 b- defN 22-May-14 18:26 pyaf/Bench/stocks_symbol_list.py
--rw-r--r--  2.0 unx    47821 b- defN 22-Jul-12 18:14 pyaf/CodeGen/TS_CodeGen_Objects.py
--rw-r--r--  2.0 unx     1877 b- defN 22-Jul-12 18:14 pyaf/CodeGen/TS_CodeGenerator.py
--rw-r--r--  2.0 unx        0 b- defN 22-May-14 18:26 pyaf/CodeGen/__init__.py
--rw-r--r--  2.0 unx      510 b- defN 23-Mar-15 23:58 pyaf/TS/Complexity.py
--rw-r--r--  2.0 unx     6748 b- defN 23-Mar-18 11:31 pyaf/TS/DateTime_Functions.py
--rw-r--r--  2.0 unx     6232 b- defN 22-Jul-12 18:14 pyaf/TS/Exogenous.py
--rw-r--r--  2.0 unx     6430 b- defN 23-Mar-15 23:59 pyaf/TS/Intermittent_Models.py
--rw-r--r--  2.0 unx     6757 b- defN 23-Mar-15 23:58 pyaf/TS/Keras_Models.py
--rw-r--r--  2.0 unx     4387 b- defN 22-Jul-12 18:14 pyaf/TS/MissingData.py
--rw-r--r--  2.0 unx     7378 b- defN 23-Mar-15 23:58 pyaf/TS/ModelSelection_Legacy.py
--rw-r--r--  2.0 unx    11568 b- defN 23-Mar-23 07:43 pyaf/TS/ModelSelection_Voting.py
--rw-r--r--  2.0 unx    12893 b- defN 23-Mar-22 18:14 pyaf/TS/Options.py
--rw-r--r--  2.0 unx    16910 b- defN 23-Mar-23 07:41 pyaf/TS/Perf.py
--rw-r--r--  2.0 unx    12670 b- defN 23-Mar-18 03:44 pyaf/TS/Plots.py
--rw-r--r--  2.0 unx     4542 b- defN 23-Mar-23 07:42 pyaf/TS/PredictionIntervals.py
--rw-r--r--  2.0 unx     8405 b- defN 23-Mar-15 23:58 pyaf/TS/Pytorch_Models.py
--rw-r--r--  2.0 unx    10020 b- defN 23-Mar-18 03:44 pyaf/TS/Scikit_Models.py
--rw-r--r--  2.0 unx     7280 b- defN 23-Mar-21 11:34 pyaf/TS/SignalDecomposition.py
--rw-r--r--  2.0 unx    18240 b- defN 23-Mar-21 11:34 pyaf/TS/SignalDecomposition_AR.py
--rw-r--r--  2.0 unx    27054 b- defN 23-Mar-21 11:35 pyaf/TS/SignalDecomposition_Cycle.py
--rw-r--r--  2.0 unx     3383 b- defN 23-Mar-15 23:59 pyaf/TS/SignalDecomposition_Forecaster.py
--rw-r--r--  2.0 unx      886 b- defN 22-Jul-12 18:14 pyaf/TS/SignalDecomposition_Quant.py
--rw-r--r--  2.0 unx    16395 b- defN 23-Mar-21 11:33 pyaf/TS/SignalDecomposition_Trainer.py
--rw-r--r--  2.0 unx    13987 b- defN 23-Mar-22 09:11 pyaf/TS/SignalDecomposition_Trend.py
--rw-r--r--  2.0 unx    25147 b- defN 23-Mar-15 23:59 pyaf/TS/SignalHierarchy.py
--rw-r--r--  2.0 unx     3158 b- defN 22-Jul-12 18:14 pyaf/TS/Signal_Grouping.py
--rw-r--r--  2.0 unx    16930 b- defN 23-Mar-23 09:20 pyaf/TS/Signal_Transformation.py
--rw-r--r--  2.0 unx     7269 b- defN 22-Jul-12 18:14 pyaf/TS/Temporal_Hierarchy.py
--rw-r--r--  2.0 unx     7913 b- defN 23-Mar-21 15:13 pyaf/TS/Time.py
--rw-r--r--  2.0 unx    29365 b- defN 23-Mar-21 11:35 pyaf/TS/TimeSeriesModel.py
--rw-r--r--  2.0 unx     4279 b- defN 23-Mar-23 07:42 pyaf/TS/TimeSeries_Cutting.py
--rw-r--r--  2.0 unx     3677 b- defN 23-Mar-15 23:58 pyaf/TS/Utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-May-14 18:26 pyaf/TS/__init__.py
+-rw-r--r--  2.0 unx      510 b- defN 23-Mar-26 14:57 pyaf/TS/Complexity.py
+-rw-r--r--  2.0 unx     7339 b- defN 23-Apr-02 19:54 pyaf/TS/DateTime_Functions.py
+-rw-r--r--  2.0 unx     9827 b- defN 23-Mar-31 18:23 pyaf/TS/Exogenous.py
+-rw-r--r--  2.0 unx     6715 b- defN 23-Mar-26 14:57 pyaf/TS/Intermittent_Models.py
+-rw-r--r--  2.0 unx     6757 b- defN 23-Mar-26 14:57 pyaf/TS/Keras_Models.py
+-rw-r--r--  2.0 unx     4876 b- defN 23-Apr-19 13:33 pyaf/TS/MissingData.py
+-rw-r--r--  2.0 unx     7727 b- defN 23-Mar-26 18:39 pyaf/TS/ModelSelection_Legacy.py
+-rw-r--r--  2.0 unx    11293 b- defN 23-Apr-06 16:47 pyaf/TS/ModelSelection_Voting.py
+-rw-r--r--  2.0 unx    12097 b- defN 23-Apr-14 15:49 pyaf/TS/Options.py
+-rw-r--r--  2.0 unx    17092 b- defN 23-Apr-09 01:03 pyaf/TS/Perf.py
+-rw-r--r--  2.0 unx    13535 b- defN 23-May-02 11:56 pyaf/TS/Plots.py
+-rw-r--r--  2.0 unx     8552 b- defN 23-Apr-09 19:38 pyaf/TS/PredictionIntervals.py
+-rw-r--r--  2.0 unx     8405 b- defN 23-Mar-26 14:57 pyaf/TS/Pytorch_Models.py
+-rw-r--r--  2.0 unx    10555 b- defN 23-Apr-06 15:07 pyaf/TS/Scikit_Models.py
+-rw-r--r--  2.0 unx     7719 b- defN 23-Apr-06 17:12 pyaf/TS/SignalDecomposition.py
+-rw-r--r--  2.0 unx    18596 b- defN 23-Apr-08 03:10 pyaf/TS/SignalDecomposition_AR.py
+-rw-r--r--  2.0 unx    27307 b- defN 23-Apr-08 01:50 pyaf/TS/SignalDecomposition_Cycle.py
+-rw-r--r--  2.0 unx     3383 b- defN 23-Mar-26 14:57 pyaf/TS/SignalDecomposition_Forecaster.py
+-rw-r--r--  2.0 unx    18323 b- defN 23-Apr-06 15:59 pyaf/TS/SignalDecomposition_Trainer.py
+-rw-r--r--  2.0 unx    13834 b- defN 23-Apr-08 01:45 pyaf/TS/SignalDecomposition_Trend.py
+-rw-r--r--  2.0 unx    27008 b- defN 23-Apr-19 13:28 pyaf/TS/SignalHierarchy.py
+-rw-r--r--  2.0 unx     3314 b- defN 23-Mar-27 14:22 pyaf/TS/Signal_Grouping.py
+-rw-r--r--  2.0 unx    18016 b- defN 23-Apr-06 17:26 pyaf/TS/Signal_Transformation.py
+-rw-r--r--  2.0 unx     7373 b- defN 23-Mar-26 14:57 pyaf/TS/Temporal_Hierarchy.py
+-rw-r--r--  2.0 unx     8867 b- defN 23-Apr-13 07:48 pyaf/TS/Time.py
+-rw-r--r--  2.0 unx    32048 b- defN 23-Apr-19 23:31 pyaf/TS/TimeSeriesModel.py
+-rw-r--r--  2.0 unx     4784 b- defN 23-Apr-22 22:10 pyaf/TS/TimeSeries_Cutting.py
+-rw-r--r--  2.0 unx     4091 b- defN 23-Apr-02 12:05 pyaf/TS/Utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-26 14:57 pyaf/TS/__init__.py
 -rw-r--r--  2.0 unx    13735 b- defN 23-Mar-15 23:58 pyaf/WS/WS_Backend.py
 -rw-r--r--  2.0 unx     3518 b- defN 22-Jul-12 18:14 pyaf/WS/WS_REST_Flask.py
 -rw-r--r--  2.0 unx        0 b- defN 22-May-14 18:26 pyaf/WS/__init__.py
 -rw-r--r--  2.0 unx      926 b- defN 22-May-14 18:26 pyaf/WS/test_heroku_web_service.py
--rw-r--r--  2.0 unx      320 b- defN 23-Mar-24 09:30 pyaf-5.0rc2.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx     1541 b- defN 23-Mar-24 09:30 pyaf-5.0rc2.dist-info/LICENSE
--rw-r--r--  2.0 unx    13869 b- defN 23-Mar-24 09:30 pyaf-5.0rc2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-24 09:30 pyaf-5.0rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-24 09:30 pyaf-5.0rc2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4553 b- defN 23-Mar-24 09:30 pyaf-5.0rc2.dist-info/RECORD
-55 files, 525923 bytes uncompressed, 130481 bytes compressed:  75.2%
+-rw-r--r--  2.0 unx      320 b- defN 23-May-02 20:09 pyaf-5.0rc3.dist-info/AUTHORS.rst
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-02 20:09 pyaf-5.0rc3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13853 b- defN 23-May-02 20:09 pyaf-5.0rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-02 20:09 pyaf-5.0rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-02 20:09 pyaf-5.0rc3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4202 b- defN 23-May-02 20:09 pyaf-5.0rc3.dist-info/RECORD
+51 files, 494398 bytes uncompressed, 124168 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -30,23 +30,14 @@
 
 Filename: pyaf/Bench/download_all_stock_prices.py
 Comment: 
 
 Filename: pyaf/Bench/stocks_symbol_list.py
 Comment: 
 
-Filename: pyaf/CodeGen/TS_CodeGen_Objects.py
-Comment: 
-
-Filename: pyaf/CodeGen/TS_CodeGenerator.py
-Comment: 
-
-Filename: pyaf/CodeGen/__init__.py
-Comment: 
-
 Filename: pyaf/TS/Complexity.py
 Comment: 
 
 Filename: pyaf/TS/DateTime_Functions.py
 Comment: 
 
 Filename: pyaf/TS/Exogenous.py
@@ -93,17 +84,14 @@
 
 Filename: pyaf/TS/SignalDecomposition_Cycle.py
 Comment: 
 
 Filename: pyaf/TS/SignalDecomposition_Forecaster.py
 Comment: 
 
-Filename: pyaf/TS/SignalDecomposition_Quant.py
-Comment: 
-
 Filename: pyaf/TS/SignalDecomposition_Trainer.py
 Comment: 
 
 Filename: pyaf/TS/SignalDecomposition_Trend.py
 Comment: 
 
 Filename: pyaf/TS/SignalHierarchy.py
@@ -141,26 +129,26 @@
 
 Filename: pyaf/WS/__init__.py
 Comment: 
 
 Filename: pyaf/WS/test_heroku_web_service.py
 Comment: 
 
-Filename: pyaf-5.0rc2.dist-info/AUTHORS.rst
+Filename: pyaf-5.0rc3.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: pyaf-5.0rc2.dist-info/LICENSE
+Filename: pyaf-5.0rc3.dist-info/LICENSE
 Comment: 
 
-Filename: pyaf-5.0rc2.dist-info/METADATA
+Filename: pyaf-5.0rc3.dist-info/METADATA
 Comment: 
 
-Filename: pyaf-5.0rc2.dist-info/WHEEL
+Filename: pyaf-5.0rc3.dist-info/WHEEL
 Comment: 
 
-Filename: pyaf-5.0rc2.dist-info/top_level.txt
+Filename: pyaf-5.0rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyaf-5.0rc2.dist-info/RECORD
+Filename: pyaf-5.0rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyaf/ForecastEngine.py

```diff
@@ -59,13 +59,7 @@
         return json.dumps(lDict, default = lambda o: o.__dict__, indent=4, sort_keys=True);
 
     def computePerf(self, actual, predicted , name):
         lForecastPerf =  tsperf.cPerf();
         lForecastPerf.compute(actual, predicted, name);
         return lForecastPerf;
 
-    def generateCode(self, iDSN = None, iDialect = None):
-        from CodeGen import TS_CodeGen_Objects as tscodegen
-        lCodeGenerator = tscodegen.cDecompositionCodeGenObject(iDSN, iDialect);
-        lSQL = lCodeGenerator.generateCode(self);
-        # print("GENERATED_SQL_CODE" , lSQL);
-        return lSQL;
```

## pyaf/HierarchicalForecastEngine.py

```diff
@@ -58,21 +58,14 @@
 
     def computePerf(self, actual, predicted , name):
         from .TS import Perf as tsperf
         lForecastPerf =  tsperf.cPerf();
         lForecastPerf.compute(actual, predicted, name);
         return lForecastPerf;
 
-    def generateCode(self, iDSN = None, iDialect = None):
-        from CodeGen import TS_CodeGen_Objects as tscodegen
-        lCodeGenerator = tscodegen.cDecompositionCodeGenObject(iDSN, iDialect);
-        lSQL = lCodeGenerator.generateCode(self);
-        # print("GENERATED_SQL_CODE" , lSQL);
-        return lSQL;
-
     def create_signal_hierarchy(self , iInputDS, iTime, iSignal, iHorizon, iHierarchy, iExogenousData = None):
         lSignalHierarchy = None;
         if(iHierarchy['Type'] == "Grouped"):
             from .TS import Signal_Grouping as siggroup
             lSignalHierarchy = siggroup.cSignalGrouping();
         elif(iHierarchy['Type'] == "Temporal"):
             from .TS import Temporal_Hierarchy as temphier
```

## pyaf/__init__.py

```diff
@@ -10,10 +10,13 @@
         raise Exception("PYAF_ERROR_PYTHON_2_NOT_SUPPORTED")
 
 
 check_python_version_for_pyaf()
 
 from . import ForecastEngine, HierarchicalForecastEngine
 
-__version__ = '5.0-rc2'
+__version__ = '5.0-rc3'
 
+def activate_timer_logging():
+    import pyaf.TS.Utils as tsutil
+    tsutil.activate_timer_logging()
```

## pyaf/Bench/GenericBenchmark.py

```diff
@@ -63,15 +63,14 @@
             
             sys.stdout = logfile    
             sys.stderr = logfile
             set_pyaf_logger(logfilename)
         set_process_name(a.getName())
         tester = cGeneric_OneSignal_Tester(a.mTSSpec , a.mBenchName);
         a.mResult = tester;
-        tester.mTestCodeGeneration = False;
         tester.mParallelMode = a.mParallelMode
         tester.testSignal(a.mSignal, a.mHorizon)
         print("BENCHMARK_SUCCESS '" + a.getName() + "'");
     except cBenchmarkError as error:
         print("BENCHMARKING_ERROR '" + a.getName() + "' : " + str(error));
     except MemoryError:
         print("BENCHMARK_MEMORY_FAILURE '" + a.getName() + "'");
@@ -111,15 +110,14 @@
         self.mTSSpec = tsspec;
         self.mTrainDataset = {};
         self.mAutoForecastBySignal = {}
         self.mTrainPerfData = {}
         self.mTestPerfData = {}
         self.mTrainTime = {};
         self.mBenchName = bench_name;
-        self.mTestCodeGeneration = False;
         self.mTestIdempotency = False;
         self.mParallelMode = True;
         self.mPlot = None
 
     def reportTrainingDataInfo(self, iSignal, iHorizon):
         df = self.mTrainDataset[iSignal  + "_" + str(iHorizon)];
         lDate = self.mTSSpec.mTimeVar
@@ -248,34 +246,25 @@
         import pickle
         output = pickle.dumps(iModel)
         lReloadedObject = pickle.loads(output)
         output2 = pickle.dumps(lReloadedObject)    
         assert(iModel.to_json() == lReloadedObject.to_json())
         return lReloadedObject;
 
-    def generateCode(self, iSignal, iHorizon):
-        from  pyaf.CodeGen import TS_CodeGenerator as tscodegen
-        lAutoF = self.mAutoForecastBySignal[iSignal  + "_" + str(iHorizon)]
-        lCodeGenerator = tscodegen.cTimeSeriesCodeGenerator();
-        lSQL = lCodeGenerator.testGeneration(lAutoF);
-        del lCodeGenerator;
-
     def getTestPerfs(self, iSignal, iHorizon):
         self.getApplyInDatset(iSignal, iHorizon);
         self.applyModel(iSignal, iHorizon);
         lSignalDataset = self.mTSSpec.mFullDataset;
         lFullDF = lSignalDataset[iSignal].dropna()
         self.mActual = lFullDF.tail(iHorizon).reset_index(drop = True);
         self.mPredicted = self.mApplyOut[iSignal + '_Forecast'].tail(iHorizon).reset_index(drop = True);
         print(iHorizon , self.mActual.head(iHorizon));
         print(iHorizon , self.mPredicted.head(iHorizon));
         self.reportActualAndPredictedData(iSignal, iHorizon);
         self.computePerfOnForecasts(iSignal, iHorizon);
-        if(self.mTestCodeGeneration):
-            self.generateCode(iSignal, iHorizon);
         
     def dumpForecastPerfs(self, iSignal, iHorizon):
         lAutoF1 = self.mAutoForecastBySignal[iSignal  + "_" + str(iHorizon)]
         lPerf = self.mTestPerfData[iSignal  + "_" + str(iHorizon)];
         print("BENCHMARK_PERF_DETAIL_SIGNAL_HORIZON", self.mTSSpec.mName , iSignal,
               self.mTrainDataset[iSignal  + "_" + str(iHorizon)].shape[0] ,
               iHorizon);
@@ -374,15 +363,14 @@
     test a collection of signals
     '''
 
     def __init__(self , tsspec, bench_name):
         # print("BENCH_DATA" , bench_name, tsspec)
         self.mTSSpec = tsspec;
         self.mBenchName = bench_name;
-        self.mTestCodeGeneration = False;
         self.mTestIdempotency = False;
         self.mType = "OneDataFramePerSignal";
         if(hasattr(self.mTSSpec , "mFullDataset")):
             self.mType = "OneDataFrameForAllSignals";
         print("BENCH_TYPE" , bench_name, self.mType);
         self.fillSignalInfo();
```

## pyaf/Bench/TS_datasets.py

```diff
@@ -47,22 +47,22 @@
     def getFutureData(self):
         return self.mFutureData;
 
     def getHorizon(self):
         return self.mHorizon;
 
     def save_dataset(self, iFileNamePrefix):
-        self.mFullDataset.to_csv(iFileNamePrefix + "_training.csv")
+        self.mFullDataset.to_csv(iFileNamePrefix + "_training.csv", index = False)
         if(self.mExogenousDataFrame is not None):
-            self.mExogenousDataFrame.to_csv(iFileNamePrefix + "_exogenous.csv")
+            self.mExogenousDataFrame.to_csv(iFileNamePrefix + "_exogenous.csv", index= False)
         
     def load_dataset_if_possible(self, iFileNamePrefix):
         self.mFullDataset = pd.read_csv(iFileNamePrefix + "_training.csv")
         if(os.path.isfile(iFileNamePrefix + "_exogenous.csv")):
-            self.mExogenousDataFrame = pd.read_csv(iFileNamePrefix + "_exogenous.csv")
+            self.mExogenousDataFrame = pd.read_csv(iFileNamePrefix + "_exogenous.csv", dtype=object)
             self.mExogenousVariables = [x for x in self.mExogenousDataFrame.columns if x.startswith('exog_')]
         
     
 # @profile    
 def load_airline_passengers() :
     tsspec = cTimeSeriesDatasetSpec();
     tsspec.mName = "AirLine_Passengers"
@@ -288,14 +288,15 @@
     tr = tstransf.create_tranformation(transform , arg)
     transformed = None
     if(tr is None):
         transformed = apply_old_transform(signal, transform)
     else :
         tr.fit(signal)
         transformed = tr.invert(signal)
+        transformed = transformed["rescaled"]
         # print(signal.head())
         # print(transformed.head())
     transformed = transformed.astype(np.float64)
     return transformed
 
 def generate_random_TS_name(N , FREQ, seed, trendtype, cycle_length, transform, sigma = 1.0, exog_count = 20, ar_order = 0) :
     lName = "Signal_" + str(N) + "_" + str(FREQ) +  "_" + str(seed)  + "_" + str(trendtype) +  "_" + str(cycle_length)   + "_" + str(transform)   + "_" + str(sigma) + "_" + str(exog_count) ;
```

## pyaf/TS/DateTime_Functions.py

```diff
@@ -77,15 +77,15 @@
     def __init__(self):
         pass
 
     def apply_date_time_computer(self, iDatePart, series):
         # Future Warning regarding DateTime_Functions - series.dt.weekofyear #153
         lComputer = cDateTime_Helper.get_date_time_computer(iDatePart)
         if(lComputer is None):
-            print("apply_date_time_computer_failures" , iDatePart)
+            tsutil.print_pyaf_detailed_info("apply_date_time_computer_failures" , iDatePart)
         assert(lComputer is not None)
         lOut = lComputer(series)
         return lOut
 
     def guess_time_resolution(self, iEstimTime):
         lEstimSecond = self.apply_date_time_computer(eDatePart.Second, iEstimTime)
         if(lEstimSecond.nunique() > 1.0):
@@ -102,25 +102,35 @@
         lEstimMonth = self.apply_date_time_computer(eDatePart.MonthOfYear, iEstimTime)
         if(lEstimMonth.nunique() > 1.0):
             return eTimeResolution.MONTH;
         # fallback
         return eTimeResolution.YEAR;
 
     
-    def get_lags_for_time_resolution(self):
+    def get_lags_for_time_resolution(self, iResolution):
         # self.mOptions.mMaxAROrder is set to 64 by default, Which covers all these resolutions.
         if(not self.isPhysicalTime()):
             return None;
         lARORder = {}
         lARORder[eTimeResolution.SECOND] = 60
         lARORder[eTimeResolution.MINUTE] = 60
         lARORder[eTimeResolution.HOUR] = 24
         lARORder[eTimeResolution.DAY] = 31
         lARORder[eTimeResolution.MONTH] = 12
-        return lARORder.get(self.mResolution , None)
+        return lARORder.get(iResolution , None)
+
+    def get_moving_window_lengths_for_time_resolution(self, iResolution):
+        # self.mOptions.mMovingAverageLengths self.mOptions.mMovingMedianLengths 
+        lWindows = {}
+        lWindows[eTimeResolution.SECOND] = [60] # Minute
+        lWindows[eTimeResolution.MINUTE] = [60] # Hour
+        lWindows[eTimeResolution.HOUR] = [12, 24] # Half-Day, Day
+        lWindows[eTimeResolution.DAY] = [5, 7, 30] # Business Week, Week, Month
+        lWindows[eTimeResolution.MONTH] = [3, 6, 12] # 3, 6 and 12 months
+        return lWindows.get(iResolution , [])
 
 
     def adaptTimeDeltaToTimeResolution(self, iResolution, iTimeDelta):
         if(eTimeResolution.SECOND == iResolution):
             lTimeDelta = pd.DateOffset(seconds=round(iTimeDelta / np.timedelta64(1,'s')))
             return lTimeDelta
         if(eTimeResolution.MINUTE == iResolution):
```

## pyaf/TS/Exogenous.py

```diff
@@ -19,24 +19,81 @@
         self.mEncodedExogenous = None;
         self.mExogenousVariableCategories = None;
         self.mExogenousDataFrame = None;
         self.mExogenousData = None;        
         self.mDateVariable = None;
         self.mContExogenousStats = None;
         self.mExcluded = [];
+
+    def long_list_to_str(self, iList):
+        lList_str = ""
+        if(len(iList) > 10):
+            lList_str = str(iList[:5]) + " ... " + str(iList[-5:])
+        else:
+            lList_str = str(iList)
+        return lList_str
+
+    def decode_used_vars(self, used):
+        used_vars = used
+        if(used is not None):
+            used_vars = [x.split("=")[0] for x in used]
+            used_vars = [x for x in used_vars if x in self.mExogenousVariables]
+            used_vars = list(set(used_vars))
+        return used_vars
+
+
+    def info(self, used = None):
+        logger = tsutil.get_pyaf_logger();
+        lDict = self.to_dict(used)
+        logger.info("EXOGENOUS_VARIABLE_DETAIL_START")
+        for exog in lDict["Categorical_Variables"].keys():
+            lList = lDict["Categorical_Variables"][exog]
+            lUsed_cat = lDict["Categorical_Variables_Usage"][exog]
+            logger.info("EXOGENOUS_VARIABLE_DETAIL_CATEGORICAL_FREQUENCIES '" + exog + "' " + str(lList))
+            logger.info("EXOGENOUS_VARIABLE_DETAIL_CATEGORICAL_USED '" + exog + "' " + str(lUsed_cat))
+        lExcluded_cat = lDict["Categorical_Variables_Excluded"]
+        logger.info("EXOGENOUS_VARIABLE_DETAIL_CATEGORICAL_EXCLUDED " + str(len(lExcluded_cat)) + " " + self.long_list_to_str(lExcluded_cat))
+        for (exog, lStats) in lDict["Continuous_Variables"].items():
+            logger.info("EXOGENOUS_VARIABLE_DETAIL_CONTINUOUS '" + exog + "' " + str(lStats))
+        lExcluded_cont = lDict["Continuous_Variables_Excluded"]
+        logger.info("EXOGENOUS_VARIABLE_DETAIL_CONTINUOUS_EXCLUDED " + str(len(lExcluded_cont)) + " " + self.long_list_to_str(lExcluded_cont))
         
-    def info(self):
-        lStr2 = "ExogenousVariables = '" + self.mExogD +"'";
-        return lStr2;
+        logger.info("EXOGENOUS_VARIABLE_DETAIL_END")
 
 
-    def to_dict(self):
+    def to_dict(self, used = None):
+        used_vars = self.decode_used_vars(used)
         dict1 = {};
+        lExcluded_cat = []
+        dict1 ["Categorical_Variables"] = {}
+        dict1 ["Categorical_Variables_Usage"] = {}
+        for (exog, lList) in self.mExogenousVariableCategories.items():
+            if(used_vars is not None and (exog in used_vars)):
+                lUsed_cat = []
+                for (cat, freq) in lList:
+                    lUsed_cat_i = [x for x in used if x.startswith(exog + "=" + str(cat))]
+                    if(len(lUsed_cat_i) > 0):
+                        lUsed_cat = lUsed_cat + [exog + "=" + str(cat)]
+                dict1 ["Categorical_Variables"][exog] = dict([(np.array([x[0]]).item(), x[1].item()) for x in lList])
+                dict1 ["Categorical_Variables_Usage"][exog] = lUsed_cat
+            else:
+                lExcluded_cat = lExcluded_cat + [exog]
+        dict1 ["Categorical_Variables_Excluded"] = lExcluded_cat
+        dict1 ["Continuous_Variables"] = {}
+        lExcluded_cont = []
+        for exog in self.mContExogenousStats.keys():
+            if(used_vars is not None and (exog in used_vars)):
+                lExogStats = self.mContExogenousStats[exog];
+                dict1 ["Continuous_Variables"][exog] = {"Mean" : lExogStats[0], "StdDev" : lExogStats[1]}
+            else:
+                lExcluded_cont = lExcluded_cont + [exog]
+        dict1 ["Continuous_Variables_Excluded"] = lExcluded_cont
         return dict1;
 
+
     def check(self):
         if(self.mExogenousData is not None):
             lExogenousDataFrame = self.mExogenousData[0];
             lExogenousVariables = self.mExogenousData[1];
             if(self.mDateVariable not in lExogenousDataFrame.columns):
                 raise tsutil.PyAF_Error("PYAF_ERROR_TIME_COLUMN_NOT_FOUND_IN_EXOGENOUS " + str(self.mDateVariable));
             for exog in lExogenousVariables:
@@ -44,18 +101,18 @@
                     raise tsutil.PyAF_Error("PYAF_ERROR_EXOGENOUS_VARIABLE_NOT_FOUND " + str(exog));
                     
     def fit(self):
         self.mExogenousDataFrame = self.mExogenousData[0];
         self.mExogenousVariables = self.mExogenousData[1];
         self.mDateVariable = self.mTimeInfo.mTime;
         self.check()
-        # print("preProcessExogenousVariables , columns", self.mExogenousVariables);
+        # tsutil.print_pyaf_detailed_info("preProcessExogenousVariables , columns", self.mExogenousVariables);
         self.updateExogenousVariableInfo();
         self.createEncodedExogenous();
-        # print("preProcessExogenousVariables , dummy columns", self.mEncodedExogenous);
+        # tsutil.print_pyaf_detailed_info("preProcessExogenousVariables , dummy columns", self.mEncodedExogenous);
 
     def addVars(self, df):
         lExogDate = self.mDateVariable;
         N = df.shape[0]
         df1 = df[[self.mDateVariable]];
         lCompleteEncoded = df1.merge(self.mEncodedExogenousDataFrame,
                                      how='left',
@@ -69,72 +126,88 @@
                        left_on=self.mDateVariable,
                        right_on=lExogDate);
         return df2;
 
     def transformDataset(self, df):
         df1 = self.addVars(df);
         return df1;
+
+    def encode_exogenous_categorical(self, exog):
+        lSeries = self.mExogenousDataFrame[exog]
+        lList = self.mExogenousVariableCategories[exog];
+        lEncodedVars = {}
+        assert(lList is not None)
+        for lCat in lList:
+            lDummyName = exog + "=" + str(lCat[0]);
+            lEncodedVars[lDummyName] = np.where(lSeries == lCat[0] , np.int8(1), np.int8(0));
+        return lEncodedVars
         
+    def encode_exogenous_continuous(self, exog):
+        lSeries = self.mExogenousDataFrame[exog]
+        lEncodedVars = {}
+        lExogStats = self.mContExogenousStats[exog];
+        # single precision here ...
+        lStandardized = (lSeries - lExogStats[0])/ lExogStats[1];
+        lStandardized = lStandardized.astype(np.float32);
+        lStandardized.fillna(np.float32(0.0), inplace=True);
+        lEncodedVars[exog] = lStandardized
+        return lEncodedVars
+
+    
     def createEncodedExogenous(self):
         self.mEncodedExogenous = [];
         lEncodedVars = {self.mDateVariable : self.mExogenousDataFrame[self.mDateVariable]}
-        for exog in self.mExogenousVariables:
-            if(exog not in self.mExcluded):
-                lSeries = self.mExogenousDataFrame[exog]
-                lList = self.mExogenousVariableCategories[exog];
-                if(lList is not None):
-                    for lCat in lList:
-                        lDummyName = exog + "=" + str(lCat);
-                        lEncodedVars[lDummyName] = np.where(lSeries == lCat , np.int8(1), np.int8(0));
-                        self.mEncodedExogenous = self.mEncodedExogenous + [lDummyName];
-                else:
-                    lExogStats = self.mContExogenousStats[exog];
-                    # single precision here ...
-                    lStandardized = (lSeries - lExogStats[0])/ lExogStats[1];
-                    lStandardized = lStandardized.astype(np.float32);
-                    lStandardized.fillna(np.float32(0.0), inplace=True);
-                    lEncodedVars[exog] = lStandardized
-                    self.mEncodedExogenous = self.mEncodedExogenous + [exog];
-            else:
-                # print("EXCLUDED" , exog);
-                pass
+        lEncodedVars_exog = {}
+        for exog in self.mExogenousVariableCategories.keys():
+            lEncodedVars_exog_cat = self.encode_exogenous_categorical(exog)
+            lEncodedVars_exog.update(lEncodedVars_exog_cat)
+        for exog in self.mContExogenousStats.keys():
+            lEncodedVars_exog_cont = self.encode_exogenous_continuous(exog)
+            lEncodedVars_exog.update(lEncodedVars_exog_cont)
+        for(lName, lEncodedSeries) in lEncodedVars_exog.items():
+            lEncodedVars[lName] = lEncodedSeries
+            self.mEncodedExogenous = self.mEncodedExogenous + [lName];
         self.mEncodedExogenousDataFrame = pd.DataFrame(lEncodedVars,
                                                        index = self.mExogenousDataFrame.index);
         # self.mEncodedExogenousDataFrame.info()
 
+    def updateExogenousVariableInfo_Categorical(self, exog, series):
+        NCat = self.mOptions.mMaxExogenousCategories;
+        # use nan as a category
+        lValues, lCounts = np.unique(series, return_counts=True)
+        lValueCounts = zip([x for x in lValues], [x for x in lCounts])
+        lValueCounts_Significant = [x for x in lValueCounts if(x[1] > 5)]
+        lValueCounts_ordered = sorted(lValueCounts_Significant, key = lambda x : (-x[1], x[0]))
+        lList = lValueCounts_ordered[:NCat]
+        lList = [(x[0], x[1]) for x in lList]
+        if(len(lList) <= 1):
+            self.mExcluded.append(exog);
+        else:
+            self.mExogenousVariableCategories[exog] = lList;
+        
+    def updateExogenousVariableInfo_Continuous(self, exog, series):
+        stat_exog = (series.mean(), series.std());
+        if(stat_exog[1] > 1e-5):
+            self.mContExogenousStats[exog] = stat_exog;
+        else:
+            self.mExcluded.append(exog);
+        
+        
     def updateExogenousVariableInfo(self):
         # self.mExogenousDataFrame.info()
-        # print(self.mExogenousDataFrame.describe());
+        # tsutil.print_pyaf_detailed_info(self.mExogenousDataFrame.describe());
         self.mExogenousVariableCategories = {};
         self.mContExogenousStats = {};
         # Compute these stats only on the estimation part.
         (lTimeMin , lTimeMax) = (self.mTimeInfo.mTimeMin , self.mTimeInfo.mTimeMax)
         if(self.mTimeInfo.isPhysicalTime()):
             (lTimeMin , lTimeMax) = (pd.Timestamp(self.mTimeInfo.mTimeMin) , pd.Timestamp(self.mTimeInfo.mTimeMax))
             
         lEstimFrame = self.mExogenousDataFrame[self.mExogenousDataFrame[self.mDateVariable] >= lTimeMin]
         lEstimFrame = lEstimFrame[lEstimFrame[self.mDateVariable] <= lTimeMax]
         for exog in self.mExogenousVariables:
             lType = self.mExogenousDataFrame[exog].dtype
-            # print("EXOG_DTYPE" , exog, lType)
+            # tsutil.print_pyaf_detailed_info("EXOG_DTYPE" , exog, lType)
             if((lType == object) or (lType.name == 'category')):
-                # use nan as a category
-                lVC = lEstimFrame[exog].value_counts(dropna = False, sort=False);
-                lVC = lVC[lVC > 5]
-                lVC = lVC.reset_index().sort_values(by=[exog, 'index'], ascending=[False, True]);
-                NCat = self.mOptions.mMaxExogenousCategories;
-                lVC = lVC.head(NCat)
-                # print("EXOGENOUS_DATA", exog, lVC.columns, lVC.head(NCat));
-                lList = lVC['index'].values
-                lList = sorted(lList.tolist());
-                # print("most_frequent_categories_for" , exog, lList);
-                if(len(lList) <= 1):
-                    self.mExcluded.append(exog);
-                else:
-                    self.mExogenousVariableCategories[exog] = lList;
+                self.updateExogenousVariableInfo_Categorical(exog, lEstimFrame[exog])
             else:
-                self.mExogenousVariableCategories[exog] = None;
-                stat_exog = (lEstimFrame[exog].mean(), lEstimFrame[exog].std());
-                if(stat_exog[1] > 1e-5):
-                    self.mContExogenousStats[exog] = stat_exog;
-                else:
-                    self.mExcluded.append(exog);
+                self.updateExogenousVariableInfo_Continuous(exog, lEstimFrame[exog])
```

## pyaf/TS/Intermittent_Models.py

```diff
@@ -38,15 +38,15 @@
         elif(croston_type == "SBJ"):
             return (1.0 - alpha/(2.0-alpha))
         # default : any other value is the legacy croston method
         return 1.0
 
 
     def estimate_alpha(self, df):
-        # print("CROSTON_OPTIONS" , self.mOptions.mCrostonOptions.__dict__)
+        # tsutil.print_pyaf_detailed_info("CROSTON_OPTIONS" , self.mOptions.mCrostonOptions.__dict__)
         method = self.mOptions.mCrostonOptions.mMethod
         if(self.mOptions.mCrostonOptions.mAlpha is not None):
             self.mAlpha = self.mOptions.mCrostonOptions.mAlpha
             return 
         else:
             # choose the best alpha based on L2
             lPerfs = {}
@@ -56,16 +56,16 @@
                 lPerf = tsperf.cPerf();
                 lDict = lPerf.computeCriterionValues(forecast_df[self.mCycleResidueName] ,
                                                      forecast_df[lForecastColumnName] ,
                                                      [self.mOptions.mCrostonOptions.mAlphaCriterion],
                                                      "CROSTON_SEL_" + '_Fit_' + str(alpha))
                 lPerfs[alpha] = lDict[self.mOptions.mCrostonOptions.mAlphaCriterion]
             self.mAlpha = min(lPerfs, key=lPerfs.get)
-            # print(lPerfs)
-            # print("CROSTON_OPTIMIZED_ALPHA" , self.mAlpha)
+            # tsutil.print_pyaf_detailed_info(lPerfs)
+            # tsutil.print_pyaf_detailed_info("CROSTON_OPTIMIZED_ALPHA" , self.mAlpha)
             return
     
     def croston(self, df, horizon_index = 1):
         alpha =  self.mAlpha
         method = self.mOptions.mCrostonOptions.mMethod
         df = self.compute_forecast(df, alpha , method , horizon_index)
         return df
@@ -77,25 +77,25 @@
             return x.mean() + np.zeros_like(x)
         from statsmodels.tsa.api import SimpleExpSmoothing
         lSES = SimpleExpSmoothing(x).fit(smoothing_level=alpha, optimized=False)
         y = lSES.fittedvalues
         return y
 
     def compute_forecast(self, df, alpha, method, horizon_index = 1):
-        # print(df.shape)
-        # print(df.columns)
-        # print(df[['Date', 'Signal', '_Signal', 'row_number', '_Signal_ConstantTrend_residue_zeroCycle_residue']].tail(12))
+        # tsutil.print_pyaf_detailed_info(df.shape)
+        # tsutil.print_pyaf_detailed_info(df.columns)
+        # tsutil.print_pyaf_detailed_info(df[['Date', 'Signal', '_Signal', 'row_number', '_Signal_ConstantTrend_residue_zeroCycle_residue']].tail(12))
         lCounts_df = df[[self.mTime, self.mCycleResidueName]].copy()
         lCounts_df['index'] = np.arange(lCounts_df.shape[0])
         df1 = lCounts_df.reset_index()
 
         counts = lCounts_df[self.mCycleResidueName] - self.mOffset
         counts = counts[:-(horizon_index)]
-        # print(list(counts.unique()))
-        # print(counts.describe())
+        # tsutil.print_pyaf_detailed_info(list(counts.unique()))
+        # tsutil.print_pyaf_detailed_info(counts.describe())
         # assert(not np.isnan(counts[:-1]).any())
         #  q is often called the “demand” and a the “inter-arrival time”.
         q = counts[abs(counts) > 1e-8]
         if(q.shape[0] == 0):
             df1['forecast'] = self.mOffset
             return df1
         assert(q.shape[0] > 0)
@@ -119,33 +119,33 @@
         while(np.isnan(df4.loc[i , 'forecast'])):
             df4.loc[i , 'forecast'] = 0.0
             i = i + 1
         df4['forecast'] = df4['forecast'] + self.mOffset
         return df4
         
     def fit(self):
-        #  print("ESTIMATE_CROSTON_MODEL_START" , self.mCycleResidueName);
+        # tsutil.print_pyaf_detailed_info("ESTIMATE_CROSTON_MODEL_START" , self.mCycleResidueName);
 
         self.set_name();
         
         series = self.mCycleResidueName; 
         self.mTime = self.mTimeInfo.mTime;
         self.mSignal = self.mTimeInfo.mSignal;
         lAREstimFrame = self.mSplit.getEstimPart(self.mARFrame)
         self.mOffset = lAREstimFrame[self.mCycleResidueName].min()
-        # print("OFFSET", (self.mCycleResidueName, self.mOffset))
+        # tsutil.print_pyaf_detailed_info("OFFSET", (self.mCycleResidueName, self.mOffset))
         self.estimate_alpha(lAREstimFrame)
         self.mFeatureSelector =  None;
         self.mInputNamesAfterSelection = self.mInputNames;
 
         lPredicted = self.croston(self.mARFrame);
         self.mARFrame[self.mOutName] = lPredicted['forecast']
         self.compute_ar_residue(self.mARFrame)
 
-        # print("ESTIMATE_CROSTON_MODEL_END" , self.mOutName);
+        # tsutil.print_pyaf_detailed_info("ESTIMATE_CROSTON_MODEL_END" , self.mOutName);
 
 
     def transformDataset(self, df, horizon_index = 1):
         series = self.mCycleResidueName;
         pred = self.croston(df, horizon_index)
         df[self.mOutName] = pred['forecast'];
         self.compute_ar_residue(df)
```

## pyaf/TS/MissingData.py

```diff
@@ -1,19 +1,20 @@
 # Copyright (C) 2016 Antoine Carme <Antoine.Carme@outlook.com>
 # All rights reserved.
 
 # This file is part of the Python Automatic Forecasting (PyAF) library and is made available under
 # the terms of the 3 Clause BSD license
 
-
-
 import pandas as pd
 import numpy as np
 import datetime
 
+from . import Utils as tsutil
+
+
 # this is a specialized missing data imputer for the time and signal
 # it performs a simple interpolation (for the moment)
 
 class cMissingDataImputer:
 
     def __init__(self):
         self.mOptions = None;
@@ -29,72 +30,84 @@
 
     def apply_time_imputation_method(self, iInputDS, iTime):
         if(self.mOptions.mMissingDataOptions.mTimeMissingDataImputation is None):
             return iInputDS
         
         if(not self.has_missing_data(iInputDS[iTime])):
             return iInputDS
+
+        lMethod = self.mOptions.mMissingDataOptions.mTimeMissingDataImputation
+        lTimer = tsutil.cTimer(("MISSING_DATA_APPLY_TIME_IMPUTATION", {"Time" : iTime, "Method" : lMethod}))
+        if(not lMethod in ["DiscardRow" , 'Interpolate']):
+            raise tsutil.PyAF_Error("PYAF_ERROR_UNKNOWN_TIME_MISSING_VALUE_IMPUTATION_METHOD '" + str(lMethod) + "'");
         
-        elif(self.mOptions.mMissingDataOptions.mTimeMissingDataImputation == "DiscardRow"):
+        if(lMethod == "DiscardRow"):
             iInputDS = iInputDS[iInputDS[iTime].notnull()]
 
-        elif(self.mOptions.mMissingDataOptions.mTimeMissingDataImputation == "Interpolate"):
+        elif(lMethod == "Interpolate"):
             lTime = self.interpolate_time_if_needed(iInputDS , iTime)
             iInputDS[iTime] = lTime
 
         return iInputDS
         
     def apply_signal_imputation_method(self, iInputDS, iSignal):
         if(self.mOptions.mMissingDataOptions.mSignalMissingDataImputation is None):
             return iInputDS
             
         if(not self.has_missing_data(iInputDS[iSignal])):
             return iInputDS
-        elif(self.mOptions.mMissingDataOptions.mSignalMissingDataImputation == "DiscardRow"):
+
+        lMethod = self.mOptions.mMissingDataOptions.mSignalMissingDataImputation
+        lTimer = tsutil.cTimer(("MISSING_DATA_APPLY_SIGNAL_IMPUTATION", {"Signal" : iSignal, "Method" : lMethod}))
+        if(not lMethod in ["DiscardRow" , 'Interpolate' , 'Constant' , 'Mean', 'Median', 'PreviousValue']):
+            raise tsutil.PyAF_Error("PYAF_ERROR_UNKNOWN_SIGNAL_MISSING_VALUE_IMPUTATION_METHOD '" + str(lMethod) + "'");
+
+
+        if(lMethod == "DiscardRow"):
             iInputDS = iInputDS[iInputDS[iSignal].notnull()]
 
-        elif(self.mOptions.mMissingDataOptions.mSignalMissingDataImputation == "Interpolate"):
+        elif(lMethod == "Interpolate"):
             lSignal = self.interpolate_signal_if_needed(iInputDS , iSignal)
             iInputDS[iSignal] = lSignal
             
-        elif(self.mOptions.mMissingDataOptions.mSignalMissingDataImputation == "Constant"):
+        elif(lMethod == "Constant"):
             lSignal = iInputDS[iSignal].fillna(self.mOptions.mMissingDataOptions.mConstant, method=None)
             iInputDS[iSignal] = lSignal
             
-        elif(self.mOptions.mMissingDataOptions.mSignalMissingDataImputation == "Mean"):
+        elif(lMethod == "Mean"):
             lMean = iInputDS[iSignal].mean()
             lSignal = iInputDS[iSignal].fillna(lMean, method=None)
             iInputDS[iSignal] = lSignal
             
-        elif(self.mOptions.mMissingDataOptions.mSignalMissingDataImputation == "Median"):
+        elif(lMethod == "Median"):
             lMedian = iInputDS[iSignal].median()
             lSignal = iInputDS[iSignal].fillna(lMedian, method=None)
             iInputDS[iSignal] = lSignal
             
-        elif(self.mOptions.mMissingDataOptions.mSignalMissingDataImputation == "PreviousValue"):
+        elif(lMethod == "PreviousValue"):
             lSignal = iInputDS[iSignal].fillna(method='ffill')
             # replace the first empty values with the first known value
             lSignal = lSignal.fillna(method='bfill')
             iInputDS[iSignal] = lSignal
             
         return iInputDS
 
     def interpolate_time_if_needed(self, iInputDS , iTime):
         
         type1 = iInputDS[iTime].dtype
         if(type1.kind == 'M'):
             lMin = iInputDS[iTime].min()
             lDiffs = iInputDS[iTime] - lMin
             lDiffs = lDiffs.apply(lambda x : x.total_seconds())
-            # print("TIME_MIN" , lMin)
-            # print("TIME" , iInputDS[iTime].describe())
-            # print("TIME_DIFFS" , lDiffs.describe())
+            # tsutil.print_pyaf_detailed_info("TIME_MIN" , lMin)
+            # tsutil.print_pyaf_detailed_info("TIME" , iInputDS[iTime].describe())
+            # tsutil.print_pyaf_detailed_info("TIME_DIFFS" , lDiffs.describe())
             lTime = lDiffs.interpolate(method='linear', limit_direction='both', axis=0)
             lTime = lTime.apply(lambda x : lMin + datetime.timedelta(seconds=x))
-            # print("TIME2" , lTime.describe())
+            # tsutil.print_pyaf_detailed_info("TIME2" , lTime.describe())
             lTime = lTime.astype(type1)
             return lTime
         else:
             lTime = iInputDS[iTime].interpolate(method='linear', limit_direction='both', axis=0)
             lTime = lTime.astype(type1)
             return lTime
```

## pyaf/TS/ModelSelection_Legacy.py

```diff
@@ -25,45 +25,49 @@
         import json
         lPerfDump = json.dumps(lDict, default = lambda o: o.__dict__, indent=4, sort_keys=True);
         logger.info("PERF_DUMP_START")
         logger.info(lPerfDump)
         logger.info("PERF_DUMP_END")
         
 
-    def collectPerformanceIndices_ModelSelection(self, iSignal, iSigDecs) :
+    def collectPerformanceIndices_ModelSelection(self, iSignal, iPerfsByModel) :
         logger = tsutil.get_pyaf_logger();
-        lTimer = tsutil.cTimer(("MODEL_SELECTION", {"Signal" : iSignal, "Transformations" : sorted(list(iSigDecs.keys()))}))
+        lTimer = tsutil.cTimer(("LEGACY_MODEL_SELECTION", {"Signal" : iSignal}))
+        lCriterion = self.mOptions.mModelSelection_Criterion
+
         rows_list = []
-        lPerfsByModel = {}
-        for (lName, sigdec) in iSigDecs.items():
-            for (model , value) in sorted(sigdec.mPerfsByModel.items()):
-                lPerfsByModel[model] = value
-                lTranformName = sigdec.mSignal;
-                lDecompType = model[1];
-                lModelFormula = model
-                lModelCategory = value[0][2].get_model_category()
-                lSplit = value[0][2].mTimeInfo.mOptions.mCustomSplit
-                #  value format : self.mPerfsByModel[lModel.mOutName] = [lModel, lComplexity, lFitPerf , lForecastPerf, lTestPerf];
-                lComplexity = value[1];
-                lFitPerf = value[2];
-                lForecastPerf = value[3];
-                lTestPerf = value[4];
-                row = [lSplit, lTranformName, lDecompType, lModelFormula[3], lModelFormula, lModelCategory, lComplexity,
-                       lFitPerf,
-                       lForecastPerf,
-                       lTestPerf]
-                rows_list.append(row);
+        for (model , value) in sorted(iPerfsByModel.items()):
+            lTranformName = value["Signal"]
+            lDecompType = value["DecompositionType"];
+            lModelFormula = model
+            modelname = value["ModelName"]
+            lModelCategory = value["ModelCategory"]
+            lSplit = value["Split"]
+            #  value format : self.mPerfsByModel[lModel.mOutName] = [lModel, lComplexity, lFitPerf , lForecastPerf, lTestPerf];
+            lComplexity = value["Complexity"];
+            lOriginalSignal = value["OriginalSignal"]
+            lForecastColumn = str(lOriginalSignal) + "_Forecast";
+            lFitPerf = value["FitPerf"];
+            lForecastPerf = value["ForecastPerf"]
+            lTestPerf = value["TestPerf"]
+            H = value["Horizon"]
+            
+            row = [lSplit, lTranformName, lDecompType, lModelFormula[3], lModelFormula, lModelCategory, lComplexity,
+                   lFitPerf[lForecastColumn + "_" + str(1)].get(lCriterion),
+                   lForecastPerf[lForecastColumn + "_" + str(1)].get(lCriterion),
+                   lTestPerf[lForecastColumn + "_" + str(1)].get(lCriterion)]
+            rows_list.append(row);
 
         self.mTrPerfDetails =  pd.DataFrame(rows_list, columns=
                                             ('Split', 'Transformation', 'DecompositionType',
                                              'Model', 'DetailedFormula', 'Category', 'Complexity',
                                              'Fit' + self.mOptions.mModelSelection_Criterion,
                                              'Forecast' + self.mOptions.mModelSelection_Criterion,
                                              'Test' + self.mOptions.mModelSelection_Criterion)) 
-        # print(self.mTrPerfDetails.head(self.mTrPerfDetails.shape[0]));
+        # tsutil.print_pyaf_detailed_info(self.mTrPerfDetails.head(self.mTrPerfDetails.shape[0]));
         lIndicator = 'Forecast' + self.mOptions.mModelSelection_Criterion;
         lBestPerf = self.mTrPerfDetails[ lIndicator ].min();
         lHigherIsBetter = tsperf.cPerf.higher_values_are_better(self.mOptions.mModelSelection_Criterion)
         if(lHigherIsBetter):
             lBestPerf = self.mTrPerfDetails[ lIndicator ].max();
         # allow a loss of one point (0.01 of MAPE) if complexity is reduced.
         assert(not np.isnan(lBestPerf))
@@ -75,63 +79,59 @@
             self.dump_all_model_perfs_as_json()
         if(lHigherIsBetter):
             lInterestingModels = self.mTrPerfDetails[self.mTrPerfDetails[lIndicator] >= (lBestPerf - 0.01)].reset_index(drop=True);
         else:
             lInterestingModels = self.mTrPerfDetails[self.mTrPerfDetails[lIndicator] <= (lBestPerf + 0.01)].reset_index(drop=True);
             
         lInterestingModels.sort_values(by=['Complexity'] , ascending=False, inplace=True)
-        # print(self.mTransformList);
-        # print(lInterestingModels.head());
-        # print(self.mPerfsByModel);
-        lBestName = lInterestingModels['DetailedFormula'].iloc[0]
-        lBestModel = lPerfsByModel[lBestName][0][2];
-        # print("BEST_MODEL", lBestName, lBestModel)
-        self.mBestModel = lBestModel
-        self.mPerfsByModel = lPerfsByModel
+        # tsutil.print_pyaf_detailed_info(self.mTransformList);
+        # tsutil.print_pyaf_detailed_info(lInterestingModels.head());
+        # tsutil.print_pyaf_detailed_info(self.mPerfsByModel);
+        self.mBestModelName = lInterestingModels['DetailedFormula'].iloc[0]
         self.mModelShortList = lInterestingModels[['Transformation', 'DecompositionType', 'Model', lIndicator, 'Complexity']] 
-        return (iSignal, lPerfsByModel, lBestModel, self.mModelShortList)
+        return (iSignal, self.mBestModelName, self.mModelShortList)
 
 
     def perform_model_selection_cross_validation(self):
         lTimer = None
         if(self.mOptions.mDebugProfile):
             lTimer = tsutil.cTimer(("MODEL_SELECTION_FOR_CROSS_VALIDATION"))
         # self.mTrPerfDetails.to_csv("perf_time_series_cross_val.csv")
         lIndicator = 'Forecast' + self.mOptions.mModelSelection_Criterion;
         lColumns = ['Category', 'Complexity', lIndicator]
         lPerfByCategory = self.mTrPerfDetails[lColumns].groupby(by=['Category'] , sort=False)[lIndicator].mean()
         lPerfByCategory_df = pd.DataFrame(lPerfByCategory).reset_index()
         lPerfByCategory_df.columns = ['Category' , lIndicator]
-        print("CROSS_VAL_PERF", lPerfByCategory_df)
         # lPerfByCategory_df.to_csv("perf_time_series_cross_val_by_category.csv")
         lBestPerf = lPerfByCategory_df[ lIndicator ].min();
         lHigherIsBetter = tsperf.cPerf.higher_values_are_better(self.mOptions.mModelSelection_Criterion)
         if(lHigherIsBetter):
             lBestPerf = lPerfByCategory_df[ lIndicator ].max();
         lPerfByCategory_df.sort_values(by=[lIndicator, 'Category'] ,
                                 ascending=[not lHigherIsBetter, True],
                                 inplace=True);
         lPerfByCategory_df = lPerfByCategory_df.reset_index(drop=True);
+        tsutil.print_pyaf_detailed_info("CROSS_VAL_PERF", [row for row in lPerfByCategory_df.itertuples(name='CV')][:5])
                 
         if(lHigherIsBetter):
             lInterestingCategories_df = lPerfByCategory_df[lPerfByCategory_df[lIndicator] >= (lBestPerf - 0.01)].reset_index(drop=True);
         else:
             lInterestingCategories_df = lPerfByCategory_df[lPerfByCategory_df[lIndicator] <= (lBestPerf + 0.01)].reset_index(drop=True);
             
-        # print(lPerfByCategory_df.head());
-        # print(lInterestingCategories_df.head());
-        # print(self.mPerfsByModel);
+        # tsutil.print_pyaf_detailed_info(lPerfByCategory_df.head());
+        # tsutil.print_pyaf_detailed_info(lInterestingCategories_df.head());
+        # tsutil.print_pyaf_detailed_info(self.mPerfsByModel);
         lInterestingCategories = list(lInterestingCategories_df['Category'].unique())
         self.mTrPerfDetails['IC'] = self.mTrPerfDetails['Category'].apply(lambda x :1 if x in lInterestingCategories else 0) 
         lInterestingModels = self.mTrPerfDetails[self.mTrPerfDetails['IC'] == 1].copy()
         lInterestingModels.sort_values(by=['Complexity'] , ascending=False, inplace=True)
-        # print(self.mTransformList);
-        # print(lInterestingModels.head());
+        # tsutil.print_pyaf_detailed_info(self.mTransformList);
+        # tsutil.print_pyaf_detailed_info(lInterestingModels.head());
         lBestName = lInterestingModels['DetailedFormula'].iloc[0];
         lBestSplit = lInterestingModels['Split'].iloc[0];
         self.mBestModel = self.mPerfsByModel[lBestName][0][2];
         self.mModelShortList = lInterestingModels[['Model', 'Category', 'Split', lIndicator, 'IC']]
-        # print("BEST_MODEL", lBestName, self.mBestModel)
+        # tsutil.print_pyaf_detailed_info("BEST_MODEL", lBestName, self.mBestModel)
 
 
 def create_model_selector():
     return cModelSelector_OneSignal()
```

## pyaf/TS/ModelSelection_Voting.py

```diff
@@ -31,139 +31,132 @@
         import json
         lPerfDump = json.dumps(lDict, default = lambda o: o.__dict__, indent=4, sort_keys=True);
         logger.info("PERF_DUMP_START")
         logger.info(lPerfDump)
         logger.info("PERF_DUMP_END")
 
 
-    def collectPerformanceIndices_ModelSelection(self, iSignal, iSigDecs) :
+    def collectPerformanceIndices_ModelSelection(self, iSignal, iPerfsByModel) :
         logger = tsutil.get_pyaf_logger();
-        lTimer = tsutil.cTimer(("MODEL_SELECTION", {"Signal" : iSignal, "Transformations" : sorted(list(iSigDecs.keys()))}))
-        lVotingScores = self.compute_voting_scores(iSigDecs)
+        lTimer = tsutil.cTimer(("VOTING_MODEL_SELECTION", {"Signal" : iSignal}))
+        lVotingScores = self.compute_voting_scores(iPerfsByModel)
         lCriterion = self.mOptions.mModelSelection_Criterion
         rows_list = []
-        lPerfsByModel = {}
-        for (lName, sigdec) in iSigDecs.items():
-            for (model , value) in sorted(sigdec.mPerfsByModel.items()):
-                lPerfsByModel[model] = value
-                lTranformName = sigdec.mSignal;
-                lDecompType = model[1];
-                lModelFormula = model
-                tsmodel = value[0][2]
-                lModelCategory = tsmodel.get_model_category()
-                lSplit = value[0][2].mTimeInfo.mOptions.mCustomSplit
-                #  value format : self.mPerfsByModel[lModel.mOutName] = [lModel, lComplexity, lFitPerf , lForecastPerf, lTestPerf];
-                lComplexity = value[1];
-                model_perfs = tsmodel.get_perfs_summary()
-                lFitPerf = model_perfs["Fit"];
-                lForecastPerf = model_perfs["Forecast"]
-                lTestPerf = model_perfs["Test"]
-                H = tsmodel.mTimeInfo.mHorizon
-
-                lVoting = lVotingScores[ lModelFormula[3] ]
-                row = [lSplit, lTranformName, lDecompType, lModelFormula[3], lModelFormula, lModelCategory, lComplexity,
-                       lFitPerf[1].get(lCriterion),
-                       lFitPerf[H].get(lCriterion), 
-                       lForecastPerf[1].get(lCriterion),
-                       lForecastPerf[H].get(lCriterion),
-                       lTestPerf[1].get(lCriterion),
-                       lTestPerf[H].get(lCriterion),
-                       lVoting]
-                rows_list.append(row);
-
-        self.mTrPerfDetails =  pd.DataFrame(rows_list, columns=
-                                            ('Split', 'Transformation', 'DecompositionType',
-                                             'Model', 'DetailedFormula', 'Category', 'Complexity',
-                                             'Fit_' + self.mOptions.mModelSelection_Criterion + "_1",
-                                             'Fit_' + self.mOptions.mModelSelection_Criterion + "_H",
-                                             'Forecast_' + self.mOptions.mModelSelection_Criterion + "_1",
-                                             'Forecast_' + self.mOptions.mModelSelection_Criterion + "_H",
-                                             'Test_' + self.mOptions.mModelSelection_Criterion + "_1",
-                                             'Test_' + self.mOptions.mModelSelection_Criterion + "_H",
-                                             "Voting")) 
-        # print(self.mTrPerfDetails.head(self.mTrPerfDetails.shape[0]));
+        for (model , value) in sorted(iPerfsByModel.items()):
+            lTranformName = value["Signal"]
+            lDecompType = value["DecompositionType"];
+            lModelFormula = model
+            modelname = value["ModelName"]
+            lModelCategory = value["ModelCategory"]
+            lSplit = value["Split"]
+            #  value format : self.mPerfsByModel[lModel.mOutName] = [lModel, lComplexity, lFitPerf , lForecastPerf, lTestPerf];
+            lComplexity = value["Complexity"];
+            lOriginalSignal = value["OriginalSignal"]
+            lForecastColumn = str(lOriginalSignal) + "_Forecast";
+            lFitPerf = value["FitPerf"];
+            lForecastPerf = value["ForecastPerf"]
+            lTestPerf = value["TestPerf"]
+            H = value["Horizon"]
+
+            lVoting = lVotingScores[ modelname ]
+            row = [lSplit, lTranformName, lDecompType, lModelFormula[3], lModelFormula, lModelCategory, lComplexity]
+            for h in range(1, H+1):
+                row = row + [lFitPerf[lForecastColumn + "_" + str(h)].get(lCriterion),
+                             lForecastPerf[lForecastColumn + "_" + str(h)].get(lCriterion),
+                             lTestPerf[lForecastColumn + "_" + str(h)].get(lCriterion)]
+            row = row + [ lVoting ]
+            rows_list.append(row);
+
+        Cols = ['Split', 'Transformation', 'DecompositionType',
+                'Model', 'DetailedFormula', 'Category', 'Complexity']
+        for h in range(1, H+1):
+            Cols = Cols + ['Fit_' + self.mOptions.mModelSelection_Criterion + "_" + str(h),
+                           'Forecast_' + self.mOptions.mModelSelection_Criterion + "_" + str(h),
+                           'Test_' + self.mOptions.mModelSelection_Criterion + "_" + str(h)]
+            
+        Cols = Cols + ["Voting"]
+        self.mTrPerfDetails =  pd.DataFrame(rows_list, columns= Cols)
+        # tsutil.print_pyaf_detailed_info(self.mTrPerfDetails.head(self.mTrPerfDetails.shape[0]));
         lIndicator = 'Voting';
         lBestPerf = self.mTrPerfDetails[ lIndicator ].max();
         # allow a loss of one point (0.01 of MAPE) if complexity is reduced.
         assert(not np.isnan(lBestPerf))
         self.mTrPerfDetails.sort_values(by=[lIndicator, 'Complexity', 'Model'] ,
                                         ascending=[False, False, True],
                                         inplace=True);
         self.mTrPerfDetails = self.mTrPerfDetails.reset_index(drop=True);
         if(self.mOptions.mDebugPerformance):
             self.dump_all_model_perfs_as_json()
         lTol = 0.99
         lInterestingModels = self.mTrPerfDetails[self.mTrPerfDetails[lIndicator] >= (lBestPerf * lTol)].reset_index(drop=True);
         lInterestingModels.sort_values(by=['Complexity'] , ascending=[False], inplace=True)
-        # print(self.mTransformList);
-        # print(self.mPerfsByModel);
-        lBestName = lInterestingModels['DetailedFormula'].iloc[0]
-        lBestModel = lPerfsByModel[lBestName][0][2];
-        # print("BEST_MODEL", lBestName, lBestModel)
-        self.mBestModel = lBestModel
-        self.mPerfsByModel = lPerfsByModel
-        self.mModelShortList = lInterestingModels[['Transformation', 'DecompositionType', 'Model', lIndicator, 'Complexity', 'Forecast_' + self.mOptions.mModelSelection_Criterion + "_1",  'Forecast_' + self.mOptions.mModelSelection_Criterion + "_H"]] 
-        # print(self.mModelShortList.head());
-        return (iSignal, lPerfsByModel, lBestModel, self.mModelShortList)
+        # tsutil.print_pyaf_detailed_info(self.mTransformList);
+        # tsutil.print_pyaf_detailed_info(self.mPerfsByModel);
+        self.mBestModelName = lInterestingModels['DetailedFormula'].iloc[0]
+        # tsutil.print_pyaf_detailed_info("BEST_MODEL", lBestName, lBestModel)
+        self.mModelShortList = lInterestingModels[['Transformation', 'DecompositionType', 'Model', lIndicator, 'Complexity'] + ['Forecast_' + self.mOptions.mModelSelection_Criterion + "_" + str(h) for h in range(1, H+1)]] 
+        # tsutil.print_pyaf_detailed_info(self.mModelShortList.head());
+        return (iSignal, self.mBestModelName, self.mModelShortList)
 
 
     def perform_model_selection_cross_validation(self):
         lTimer = None
         if(self.mOptions.mDebugProfile):
             lTimer = tsutil.cTimer(("MODEL_SELECTION_FOR_CROSS_VALIDATION"))
         # self.mTrPerfDetails.to_csv("perf_time_series_cross_val.csv")
         lIndicator = [x for x in self.mTrPerfDetails.columns if x.startswith('Forecast_')][-1]
         lColumns = ['Category', 'Complexity', lIndicator]
         lPerfByCategory = self.mTrPerfDetails[lColumns].groupby(by=['Category'] , sort=False)[lIndicator].mean()
         lPerfByCategory_df = pd.DataFrame(lPerfByCategory).reset_index()
         lPerfByCategory_df.columns = ['Category' , lIndicator]
-        print("CROSS_VAL_PERF", lPerfByCategory_df)
         # lPerfByCategory_df.to_csv("perf_time_series_cross_val_by_category.csv")
         lBestPerf = lPerfByCategory_df[ lIndicator ].min();
         lHigherIsBetter = tsperf.cPerf.higher_values_are_better(self.mOptions.mModelSelection_Criterion)
         if(lHigherIsBetter):
             lBestPerf = lPerfByCategory_df[ lIndicator ].max();
         lPerfByCategory_df.sort_values(by=[lIndicator, 'Category'] ,
                                 ascending=[not lHigherIsBetter, True],
                                 inplace=True);
         lPerfByCategory_df = lPerfByCategory_df.reset_index(drop=True);
+        tsutil.print_pyaf_detailed_info("CROSS_VAL_PERF", [row for row in lPerfByCategory_df.itertuples(name='CV')][:5])
                 
         if(lHigherIsBetter):
             lInterestingCategories_df = lPerfByCategory_df[lPerfByCategory_df[lIndicator] >= (lBestPerf - 0.01)].reset_index(drop=True);
         else:
             lInterestingCategories_df = lPerfByCategory_df[lPerfByCategory_df[lIndicator] <= (lBestPerf + 0.01)].reset_index(drop=True);
             
-        # print(lPerfByCategory_df.head());
-        # print(lInterestingCategories_df.head());
-        # print(self.mPerfsByModel);
+        # tsutil.print_pyaf_detailed_info(lPerfByCategory_df.head());
+        # tsutil.print_pyaf_detailed_info(lInterestingCategories_df.head());
+        # tsutil.print_pyaf_detailed_info(self.mPerfsByModel);
         lInterestingCategories = list(lInterestingCategories_df['Category'].unique())
         self.mTrPerfDetails['IC'] = self.mTrPerfDetails['Category'].apply(lambda x :1 if x in lInterestingCategories else 0) 
         lInterestingModels = self.mTrPerfDetails[self.mTrPerfDetails['IC'] == 1].copy()
         lInterestingModels.sort_values(by=['Complexity'] , ascending=True, inplace=True)
-        # print(self.mTransformList);
-        # print(lInterestingModels.head());
+        # tsutil.print_pyaf_detailed_info(self.mTransformList);
+        # tsutil.print_pyaf_detailed_info(lInterestingModels.head());
         lBestName = lInterestingModels['DetailedFormula'].iloc[0];
         lBestSplit = lInterestingModels['Split'].iloc[0];
-        self.mBestModel = self.mPerfsByModel[lBestName][0][2];
+        self.mBestModelName = lBestName
         self.mModelShortList = lInterestingModels[['Model', 'Category', 'Split', lIndicator, 'IC']]
-        # print("BEST_MODEL", lBestName, self.mBestModel)
+        # tsutil.print_pyaf_detailed_info("BEST_MODEL", lBestName, self.mBestModel)
 
 
 class cModelSelector_Condorcet(cModelSelector_Voting):
     
     def __init__(self):
         cModelSelector_Voting.__init__(self);
         self.mCondorcetScores = None
         self.mCriteriaValues = None
+        self.mMaxCandidates = 128
 
-    def get_criterion_values(self, iModel):
+    def get_criterion_values(self, value):
         lCriterion = self.mOptions.mModelSelection_Criterion
-        lPerfs1 = iModel.mForecastPerfs
-        self.mHorizon = iModel.mTimeInfo.mHorizon
-        lForecastColumn = str(iModel.mOriginalSignal) + "_Forecast";
+        lPerfs1 = value["ForecastPerf"]
+        self.mHorizon = value["Horizon"]
+        lForecastColumn = value["OriginalSignal"] + "_Forecast";
         lCriterionValues = {}
         for h in range(self.mHorizon):
             lHorizonName = lForecastColumn + "_" + str(h + 1);
             lCriterionValues[h + 1] = lPerfs1[lHorizonName].get(lCriterion)
         return lCriterionValues
         
         
@@ -180,18 +173,18 @@
 
     def filter_worst_criteria_values(self):
         # Condorecet method will give the same result and run faster if we remove the worst models.
         lBestModels = []
         for h in range(self.mHorizon):
             lValues = [(k, v[h + 1]) for (k,v) in self.mCriteriaValues.items()]
             lValues = sorted(lValues, key = lambda x : x[1])
-            lBestModels = lBestModels + [k[0] for k in lValues[:32]] # 32 best for each horizon
+            lBestModels = lBestModels + [k[0] for k in lValues[:self.mMaxCandidates]] # self.mMaxCandidates best for each horizon
         lBestModels = set(lBestModels)
         lDiscrededModels = [x for x in self.mCriteriaValues.keys() if x not in lBestModels]
-        print("KEPT_DISCARDED_MODELS", len(self.mCriteriaValues.keys()) , len(lBestModels), len(lDiscrededModels))
+        tsutil.print_pyaf_detailed_info("KEPT_DISCARDED_MODELS", len(self.mCriteriaValues.keys()) , len(lBestModels), len(lDiscrededModels))
         for model_name in lDiscrededModels:
             self.mCriteriaValues.pop(model_name)
         
         
     def compute_condorcet_score(self, model_name):
         lCrit1 = self.mCriteriaValues.get(model_name)            
         if(lCrit1 is None):
@@ -201,25 +194,25 @@
             lCoeff = (h + 1) / self.mHorizon
             for (model_name_2, lCrit2) in self.mCriteriaValues.items():
                 if(model_name_2 != model_name):
                     lScore = lScore + self.isBetter(lCrit1[h + 1], lCrit2[h + 1]) * lCoeff
         lScore = round(lScore , 4)
         return lScore
         
-    def compute_voting_scores(self, iSigDecs):
+    def compute_voting_scores(self, iPerfsByModel):
+        lTimer = tsutil.cTimer(("MODEL_SELECTION_COMPUTE_VOTING_SCORES", len(iPerfsByModel)))
         self.mCondorcetScores = {}
         self.mCriteriaValues = {}
         lModels = {}
-        for (lName, sigdec) in iSigDecs.items():
-            for (model , value) in sorted(sigdec.mPerfsByModel.items()):
-                ts_model = value[0][2]
-                model_name = ts_model.mOutName
-                lModels[model_name] = ts_model
-                self.mCriteriaValues[model_name] = self.get_criterion_values(ts_model)
-        # self.filter_worst_criteria_values()
+        for (model , value) in sorted(iPerfsByModel.items()):
+            model_name = value["ModelName"]
+            lModels[model_name] = value
+            self.mCriteriaValues[model_name] = self.get_criterion_values(value)
+        if(len(self.mCriteriaValues) > self.mMaxCandidates):
+            self.filter_worst_criteria_values()
         for (model_name, ts_model) in lModels.items():
             self.mCondorcetScores[model_name] = self.compute_condorcet_score(model_name)
         return self.mCondorcetScores
 
 
 def create_model_selector(iMethod):
     return cModelSelector_Condorcet()
```

## pyaf/TS/Options.py

```diff
@@ -53,99 +53,96 @@
         self.mActiveTransformations = {};
         self.mActivePeriodics = {};
         self.mActiveTrends = {};
         self.mActiveAutoRegressions = {};
         #  Add Multiplicative Models/Seasonals #178 
         self.mActiveDecompositionTypes = {}
 
+    def set_active_models_for_fast_mode(self):
         # now , set he default models
         self.set_active_transformations(cModelControl.gKnownTransformations[0:4]);
         self.set_active_trends(cModelControl.gKnownTrends[0:4]);
         self.set_active_periodics(cModelControl.gKnownPeriodics);
         self.set_active_autoregressions(cModelControl.gKnownAutoRegressions[0:3]);
         # Add Multiplicative Models/Seasonals #178.
         # Only additive models are activated by default        
         self.set_active_decomposition_types(['T+S+R']);
 
+    def set_active_models_for_slow_mode(self):
+        self.set_active_transformations(cModelControl.gKnownTransformations);
+        self.set_active_trends(cModelControl.gKnownTrends);
+        self.set_active_periodics(cModelControl.gKnownPeriodics);
+        self.set_active_autoregressions(cModelControl.gKnownAutoRegressions);
+        self.set_active_decomposition_types(cModelControl.gKnownDecompositionTypes);
+
+
     def check_model_type_validity(self, category, allowed_values, value):
         from . import Utils as tsutil
         
         if(value not in allowed_values):
             raise tsutil.PyAF_Error("INVALID_MODEL_TYPE Invalid '" + category + "' Type '" + value + "'. Allowed '" + category + "' Values : " + str(allowed_values));
-        
+
+    def generic_model_activation(self, iTypes, iToBeActivated, default_model):
+        lActivatedModels = {}
+        for model_type in iTypes:
+            if(model_type in iToBeActivated):
+                lActivatedModels[model_type] = True;
+            else:
+                lActivatedModels[model_type] = False;
+        if(True not in lActivatedModels.values()):
+            # default
+            lActivatedModels[default_model] = True;
+        return lActivatedModels
         
     def set_active_decomposition_types(self, iDecompTypes):
         for dec_type in iDecompTypes:
             self.check_model_type_validity('DecompositionType', cModelControl.gKnownDecompositionTypes, dec_type)
             
-        self.mActiveDecompositionTypes = {};
-        for decomp_type in cModelControl.gKnownDecompositionTypes:
-            if(decomp_type in iDecompTypes):
-                self.mActiveDecompositionTypes[decomp_type] = True;
-            else:
-                self.mActiveDecompositionTypes[decomp_type] = False;
-        if(True not in self.mActiveDecompositionTypes.values()):
-            # default
-            self.mActiveTransformations['T+S+R'] = True;
+        self.mActiveDecompositionTypes = self.generic_model_activation(
+            cModelControl.gKnownDecompositionTypes,
+            iDecompTypes,
+            'T+S+R'
+        )
             
     def set_active_transformations(self, transformations):
         for transformation in transformations:
             self.check_model_type_validity('Transformation', cModelControl.gKnownTransformations, transformation)
             
-        self.mActiveTransformations = {};
-        for transformation in cModelControl.gKnownTransformations:
-            if(transformation in transformations):
-                self.mActiveTransformations[transformation] = True;
-            else:
-                self.mActiveTransformations[transformation] = False;
-        if(True not in self.mActiveTransformations.values()):
-            # default
-            self.mActiveTransformations['None'] = True;
+        self.mActiveTransformations = self.generic_model_activation(
+            cModelControl.gKnownTransformations,
+            transformations,
+            'None')
+        
     
     def set_active_trends(self, trends):
         for trend in trends:
             self.check_model_type_validity('Trend', cModelControl.gKnownTrends, trend)
             
-        self.mActiveTrends = {};
-        for trend in cModelControl.gKnownTrends:
-            if(trend in trends):
-                self.mActiveTrends[trend] = True;
-            else:
-                self.mActiveTrends[trend] = False;
-        if(True not in self.mActiveTrends.values()):
-            # default
-            self.mActiveTrends['ConstantTrend'] = True;                
+        self.mActiveTrends = self.generic_model_activation(
+            cModelControl.gKnownTrends,
+            trends,
+            'ConstantTrend')
     
     def set_active_periodics(self, periodics):
         for period in periodics:
             self.check_model_type_validity('Periodic', cModelControl.gKnownPeriodics, period)
             
-        self.mActivePeriodics = {};
-        for period in cModelControl.gKnownPeriodics:
-            if(period in periodics):
-                self.mActivePeriodics[period] = True;
-            else:
-                self.mActivePeriodics[period] = False;
-        if(True not in self.mActivePeriodics.values()):
-            # default
-            self.mActivePeriodics['NoCycle'] = True;
+        self.mActivePeriodics = self.generic_model_activation(
+            cModelControl.gKnownPeriodics,
+            periodics,
+            'NoCycle')
                     
     def set_active_autoregressions(self, autoregs):
         for autoreg in autoregs:
             self.check_model_type_validity('AutoRegression', cModelControl.gKnownAutoRegressions, autoreg)
             
-        self.mActiveAutoRegressions = {};
-        for autoreg in cModelControl.gKnownAutoRegressions:
-            if(autoreg in autoregs):
-                self.mActiveAutoRegressions[autoreg] = True;
-            else:
-                self.mActiveAutoRegressions[autoreg] = False;                
-        if(True not in self.mActiveAutoRegressions.values()):
-            # default
-            self.mActiveAutoRegressions['NoAR'] = True;
+        self.mActiveAutoRegressions = self.generic_model_activation(
+            cModelControl.gKnownAutoRegressions,
+            autoregs,
+            'NoAR')
 
     def disable_all_transformations(self):
         self.set_active_transformations([]);
     
     def disable_all_trends(self):
         self.set_active_trends([]);
     
@@ -210,57 +207,52 @@
         self.mCrossValidationOptions = cCrossValidationOptions()
         self.mCrostonOptions = cCrostonOptions()
         self.mMissingDataOptions = cMissingDataOptions()
         self.mDL_Backends = ("PyTorch", ) # Pytorch is the only supported backend for now
         self.mPytorch_Options = None
         self.mKeras_Options = None
         self.mVotingMethod = "Condorcet" # Or None for Legacy Method (backward compatibility with PyAF 4.0). 
+        self.mMovingWindowLengths = None # [5, 7, 12, 24 , 30, 60];
         self.disableDebuggingOptions();
 
     def disableDebuggingOptions(self):
         self.mDebug = False;
         self.mDebugCycles = False;
         self.mDebugAR = False;
         self.mDebugProfile = False;
         self.mDebugPerformance = False;
         
         
     def enable_slow_mode(self):
-        self.mQuantiles = [5, 10, 20]; # quintiles, deciles, and vingtiles;)
-        self.mMovingAverageLengths = [5, 7, 12, 24 , 30, 60];
-        self.mMovingMedianLengths = [5, 7, 12, 24 , 30, 60];
+        self.set_active_models_for_slow_mode()
+        self.mQuantiles = [ 20 ]; # vingtiles + use optimal rule
+        
         # PyAF does not detect complex seasonal patterns #73.
         # use unlimited cycle lengths in slow mode
         self.mCycleLengths = None;
 
-        self.set_active_transformations(cModelControl.gKnownTransformations);
-        self.set_active_trends(cModelControl.gKnownTrends);
-        self.set_active_periodics(cModelControl.gKnownPeriodics);
-        self.set_active_autoregressions(cModelControl.gKnownAutoRegressions);
-        self.set_active_decomposition_types(cModelControl.gKnownDecompositionTypes);
         
         self.mMaxAROrder = 64;
         self.mFilterSeasonals = False
         # disable cross validation
         # self.mCrossValidationOptions.mMethod = "TSCV";
         self.mActivateSampling = False
 
     def enable_fast_mode(self):
-        self.mQuantiles = [5, 10, 20]; # quintiles, deciles, and vingtiles;)
-        self.mMovingAverageLengths = [5, 7, 12, 24 , 30, 60];
-        self.mMovingMedianLengths = [5, 7, 12, 24 , 30, 60];
-        
+        self.set_active_models_for_fast_mode()
+        self.mQuantiles = [ 20 ]; # vingtiles + use diaconis rule
         self.mCycleLengths = [5, 7, 12, 24 , 30, 60];
 
         self.mMaxAROrder = 64;
         self.mFilterSeasonals = True
 
 
     # Add a low-memory mode for Heroku #25
     def enable_low_memory_mode(self):
+        self.set_active_models_for_fast_mode()
         self.mMaxAROrder = 7;
         self.set_active_transformations(['None']);
         self.mParallelMode = False;
         self.mFilterSeasonals = True
         
     def has_module_installed(self, module_name):
         import importlib
```

## pyaf/TS/Perf.py

```diff
@@ -56,15 +56,15 @@
                  'MASE' : self.mMASE, 'RMSSE' : self.mRMSSE,
                  "ErrorMean" : self.mErrorMean, "ErrorStdDev" : self.mErrorStdDev, 
                  "R2" : self.mR2, "Pearson" : self.mPearsonR, "MedAE": self.mMedAE, "LnQ" : self.mLnQ,
                  "KS" : self.mKS, "KendallTau" : self.mKendallTau, "MannWhitneyU" : self.mMWU, "AUC" : self.mAUC}
         return lDict
     
     def check_not_nan(self, sig , name):
-        #print("check_not_nan");
+        # tsutil.print_pyaf_detailed_info("check_not_nan");
         if(np.isnan(sig).any()):
             logger = tsutil.get_pyaf_logger();
             logger.error("PERF_WITH_NAN_IN_SIGNAL" + str(sig));
             raise tsutil.Internal_PyAF_Error("INVALID_COLUMN _FOR_PERF ['" + self.mName + "'] '" + name + "'");
         pass
 
     def pre_compute_abs_error_if_needed(self, signal , estimator):
@@ -233,24 +233,24 @@
         pass
 
 
     def compute_pearson_r(self, signal , estimator):
         from scipy.stats import pearsonr
         signal_std = np.std(signal);
         estimator_std = np.std(estimator);
-        # print("PEARSONR_DETAIL2" , signal)
-        # print("PEARSONR_DETAIL3" , estimator)
+        # tsutil.print_pyaf_detailed_info("PEARSONR_DETAIL2" , signal)
+        # tsutil.print_pyaf_detailed_info("PEARSONR_DETAIL3" , estimator)
         lEps = 1e-4
         r = 0.0;
         if(signal_std < lEps):
             return r
         if(estimator_std < lEps):
             return r
         (r , pval) = pearsonr(signal , estimator)
-        #  print("PEARSONR_DETAIL1" , signal_std, estimator_std, r)
+        # tsutil.print_pyaf_detailed_info("PEARSONR_DETAIL1" , signal_std, estimator_std, r)
         self.mPearsonR = round(r, 4)
         return self.mPearsonR;
 
     def compute_ErrorMean_ErrorStd(self, signal , estimator):
         myerror = estimator - signal 
         self.mErrorMean = np.mean(myerror)
         self.mErrorMean = round(self.mErrorMean, 4)
@@ -291,18 +291,18 @@
 
     def compute_signal_quantiles(self, signal , estimator):
         myerror = (estimator.values - signal.values);
         NQ = int(min(20, np.sqrt(signal.shape[0]))) # optimal quantiles number heuristics : sqrt(N)
         Q = int(100 // NQ)
         lPercentiles = [50 - q for q in range(Q, 50, Q)] + [50] + [50 + q for q in range(Q, 50, Q)]
         lPercentiles = sorted(lPercentiles)
-        # print(lPercentiles)
+        # tsutil.print_pyaf_detailed_info(lPercentiles)
         lSignalQuantiles = np.percentile(signal, lPercentiles)
         lSignalQuantiles = dict(zip(lPercentiles, list(lSignalQuantiles)))
-        # print("SIGNAL_QUANTILES" , (self.mName , lSignalQuantiles))
+        # tsutil.print_pyaf_detailed_info("SIGNAL_QUANTILES" , (self.mName , lSignalQuantiles))
         lPercentiles2 = [50 - q for q in range(Q, 50, Q)] + [50] + [50 + q for q in range(Q, 50, Q)]
         lErrorQuantiles = np.percentile(myerror, lPercentiles2)
         self.mErrorQuantiles = dict(zip(lPercentiles2, list(lErrorQuantiles)))
         return lSignalQuantiles
     
     def compute_CRPS(self, signal , estimator):
         lLossValues = []
@@ -311,15 +311,15 @@
         for (a, q) in self.mSignalQuantiles.items():
             lDiff_q = q - estimator.values
             lPinballLoss_a = (1.0 - a / 100) * np.maximum(lDiff_q, 0.0) +  a / 100 * np.maximum(-lDiff_q, 0)
             lLossValue_a = lPinballLoss_a.mean()
             lLossValues.append(lLossValue_a)
         lCRPS = np.mean(lLossValues)
         self.mCRPS = round( lCRPS , 4 )
-        # print("CRPS" , (self.mName , lCRPS))
+        # tsutil.print_pyaf_detailed_info("CRPS" , (self.mName , lCRPS))
         return self.mCRPS
 
     def compute_L1(self, signal , estimator):
         abs_error = self.pre_compute_abs_error_if_needed(signal , estimator);
         self.mL1 = np.mean(abs_error)
         self.mL1 = round(self.mL1, 4)
         return self.mL1
```

## pyaf/TS/Plots.py

```diff
@@ -18,22 +18,36 @@
 RESIDUE_COLOR='red'
 COMPONENT_COLOR='navy'
 SHADED_COLOR='turquoise'
 UPPER_COLOR='grey'
 LOWER_COLOR='black'
 
 
+def add_watermark(fig):
+    import matplotlib, pyaf, os
+    import matplotlib.pyplot as plt
+    lDict = {}
+    lDict["URI"] = "https://pypi.org/project/pyaf/"
+    lDict["Version"] =  pyaf.__version__
+    from datetime import datetime
+    lDict["Date"] = datetime.today().strftime('%Y-%m-%d')
+    lDict["PID"] = os.getpid()
+    lWaterMark = "Generated with PyAF. " + str(lDict)
+    fig.tight_layout()
+    plt.figtext(0.002, 0.002, lWaterMark, rotation = 'vertical', alpha = 0.2, fontsize = 6)
+    return 
+
 def add_patched_legend(ax , names):
     # matplotlib does not like labels starting with '_'
     patched_names = []
     for name in names:
         # remove leading '_' => here, this is almost OK: no signal transformation
         patched_name = name.lstrip('_')
         patched_names = patched_names + [ patched_name ]
-    # print("add_patched_legend" , names, patched_names)
+    # tsutil.print_pyaf_detailed_info("add_patched_legend" , names, patched_names)
     ax.legend(patched_names)
 
 def fig_to_png_base64(fig):
     figfile = BytesIO()
     fig.savefig(figfile, format='png')
     figfile.seek(0)  # rewind to beginning of file
     figdata_png = base64.b64encode(figfile.getvalue())
@@ -50,20 +64,21 @@
     assert(signal in df.columns)
     assert(estimator in df.columns)
     assert(residue in df.columns)
 
 
     import matplotlib
     import matplotlib.pyplot as plt
-    # print("MATPLOTLIB_BACKEND",  matplotlib.get_backend())
+    # tsutil.print_pyaf_detailed_info("MATPLOTLIB_BACKEND",  matplotlib.get_backend())
     # matplotlib.use('Agg')
     df1 = df.tail(max(max_length , 4 * horizon));
     if(name is not None):
         plt.switch_backend('Agg')
-    fig, axs = plt.subplots(ncols=2, figsize=(32, 16))
+    fig, axs = plt.subplots(ncols=2, figsize=(12, 8),
+                            gridspec_kw={'width_ratios': [4, 1]})
 
     lColor = COMPONENT_COLOR;
     if(name is not None and name.endswith("Forecast")):
         lColor = FORECAST_COLOR;
     df1.plot.line(time, [signal, estimator, residue],
                   color=[SIGNAL_COLOR, lColor, RESIDUE_COLOR],
                   ax=axs[0] , grid = True, legend=False)
@@ -74,14 +89,15 @@
         axs[0].set_title(estimator + "\n")
     residues =  df1[residue].values
 
     import scipy.stats as scistats
     resid = residues[~np.isnan(residues)]
     scistats.probplot(resid, dist="norm", plot=axs[1])
 
+    add_watermark(fig)
     return fig
 
 def decomp_plot(df, time, signal, estimator, residue, name = None, format='png', max_length = 1000, horizon = 1, title = None) :
     fig = decomp_plot_internal(df, time, signal, estimator, residue, name, format, max_length, horizon, title)
     if(name is not None):
         import matplotlib
         import matplotlib.pyplot as plt
@@ -106,45 +122,48 @@
     assert(df.shape[1] > 0)
     assert(time in df.columns)
     assert(signal in df.columns)
     assert(estimator in df.columns)
     assert(lower in df.columns)
     assert(upper in df.columns)
 
-
     df1 = df.tail(max(max_length, 4 * horizon)).copy();
     lMin = np.mean(df1[signal]) -  np.std(df1[signal]) * 10;
     lMax = np.mean(df1[signal]) +  np.std(df1[signal]) * 10;
     df1[lower] = df1[lower].apply(lambda x : x if (np.isnan(x) or x >= lMin) else np.nan);
     df1[upper] = df1[upper].apply(lambda x : x if (np.isnan(x) or x <= lMax) else np.nan);
 
     # last value of the signal
     lLastSignalPos = df1[signal].dropna().tail(1).index[0];
     lEstimtorValue = df1[estimator][lLastSignalPos];
     df1.loc[lLastSignalPos , lower] = lEstimtorValue;
     df1.loc[lLastSignalPos , upper] = lEstimtorValue;
-
+    
     import matplotlib
     # matplotlib.use('Agg')
     import matplotlib.pyplot as plt
+    
     if(name is not None):
         plt.switch_backend('Agg')
     fig, axs = plt.subplots(ncols=1, figsize=(16, 8))
+    
     if(title is not None):
         axs.set_title(title + "\n")
     else:
         axs.set_title("Prediction Intervals\n")
-        
+
     df1.plot.line(time, [signal, estimator, lower, upper],
                   color=[SIGNAL_COLOR, FORECAST_COLOR, LOWER_COLOR, UPPER_COLOR],
                   ax=axs, grid = True, legend=False)
     add_patched_legend(axs , [signal, estimator, lower, upper])
 
     axs.fill_between(df1[time].values, df1[lower], df1[upper], color=SHADED_COLOR, alpha=.2)
-
+    
+    add_watermark(fig)
+    
     return fig
 
 def prediction_interval_plot(df, time, signal, estimator, lower, upper, name = None, format='png', max_length = 1000, horizon = 1, title = None) :
     fig = prediction_interval_plot_internal(df, time, signal, estimator, lower, upper, name, format, max_length, horizon, title)
     if(name is not None):
         import matplotlib
         import matplotlib.pyplot as plt
@@ -192,27 +211,27 @@
     cm_turbo = matplotlib.colormaps.get('turbo')
     # quantize the colors (keep only 16)
     cm = matplotlib.colors.ListedColormap(cm_turbo.colors[0:256:16])
     #  Forecast Quantiles Plots can be improved #225
     # Better separate histograms (original issue solution). Assign a fixed height (1 cm) to each histogram.
     fig, axs = plt.subplots(horizon, 1, figsize=(12, horizon / 2.54), squeeze = True)
     # plt.subplots_adjust(hspace=1)
-    # print(axs)
+    # tsutil.print_pyaf_detailed_info(axs)
     if (horizon == 1):
         axs = [axs]
     for h in range(horizon):
         lIdx = df1.index[h]
         lTime = df1.loc[lIdx, time]
         q_values = df1.loc[lIdx, lQuantileNames].tolist()
         q_values = [max(x , -1e10) for x in q_values]
         q_values = [min(x , +1e10) for x in q_values]
         if((max(q_values) - min(q_values)) < lEps):
             # Avoid a warning from matplotlib for a constant signal.
             q_values = [min(q_values) - lEps] + [max(q_values) + lEps]
-        # print(h, horizon, lIdx, lTime, q_values)
+        # tsutil.print_pyaf_detailed_info(h, horizon, lIdx, lTime, q_values)
         _, bins1, patches = axs[h].hist(q_values, bins = q_values, weights=[1]*len(q_values), density = True)
         for i, p in enumerate(patches):
             j = (bins1[i] - lMin) / (lMax - lMin)
             plt.setp(p, 'facecolor', cm(j))
         if(h == 0):
             if(title is not None):
                 axs[h].set_title(title)
@@ -229,14 +248,15 @@
         axs[h].set_ylabel('H=' + str(h + 1), rotation=0, horizontalalignment='left')
         axs[h].set_yticks([])
         axs[h].set_yticklabels([])
         if(h < (horizon - 1)):
             axs[h].set_xlabel('')
             axs[h].set_xticklabels([])
 
+    add_watermark(fig)
     return fig
 
 def quantiles_plot(df, time, signal, estimator, iQuantiles, name = None, format='png', horizon = 1, title = None) :
     fig = quantiles_plot_internal(df, time, signal, estimator, iQuantiles, name, format, horizon, title)
     import matplotlib
     import matplotlib.pyplot as plt
     if(name is not None):
@@ -289,21 +309,22 @@
                                        fillcolor=color1, fontsize="12.0")
                 graph.add_node(node_col1);
                 lEdgeLabel = "";
                 if iAnnotations is not None:
                     lEdgeLabel = iAnnotations[col + "_" + col1];
                 lEdge = pydot.Edge(node_col, node_col1, color="red", label=lEdgeLabel, fontsize="12.0")
                 graph.add_edge(lEdge)
-    # print(graph.obj_dict)
+    # tsutil.print_pyaf_detailed_info(graph.obj_dict)
     return graph
     
 def plot_hierarchy(structure , iAnnotations, name):
     graph = plot_hierarchy_internal(structure , iAnnotations, name)
     if(name is not None):
-        graph.write_png(name);
+        log_saving_plot_message("Hierarchical_Structure", name + '.png')
+        graph.write_png(name + ".png");
     else:
         from IPython.display import Image, display
         plot1 = Image(graph.create_png())
         display(plot1)
 
 
 def plot_hierarchy_as_png_base64(structure , iAnnotations, name):
```

## pyaf/TS/PredictionIntervals.py

```diff
@@ -7,82 +7,149 @@
 import pandas as pd
 import numpy as np
 
 from . import SignalDecomposition as sigdec
 
 from . import Perf as tsperf
 from . import Utils as tsutil
+from . import TimeSeries_Cutting as tscut
+
 
 class cPredictionIntervalsEstimator:
     
     def __init__(self):
         self.mModel = None;
         self.mSignalFrame = None
         self.mHorizon = -1;
-        self.mFitPerformances = {}
-        self.mForecastPerformances = {}
-        self.mTestPerformances = {}
+        self.mPerformances = {"whole" : {}, "detrended" : {}, "deseasonalized" : {}, "transformed" : {}}
+        for lType in self.mPerformances.keys():
+            self.mPerformances[lType] = {tscut.eDatasetType.Fit : {}, tscut.eDatasetType.Forecast : {},  tscut.eDatasetType.Test : {}}
         self.mComputeAllPerfs = True
 
     def compute_one_perf(self, signal, estimator, iHorizonName):
         # Investigate Large Horizon Models #213 : generate all prediction intervals for all models.
         # Don't compute all the perf indicators for the model selection (AUC is not relevant here, speed issues).
         # Compute all the perf indicators for the selected model at the end of training.
         lPerf = tsperf.cPerf();
         if(self.mComputeAllPerfs):
             lPerf.compute(signal, estimator, iHorizonName);
         else:
             lCriterions = [ self.mModel.mTimeInfo.mOptions.mModelSelection_Criterion ]
             lDict = lPerf.computeCriterionValues(signal, estimator, lCriterions, iHorizonName);
             return lDict
         return lPerf
+
+    def compute_detrended_perfs(self, original_cut_dfs, forecast_cut_dfs, h):
+        lTransformedSignalColumn = self.mModel.mSignal;
+        lTrendColumn = self.mModel.mTrend.mOutName;
+        lSeasonalColumn = self.mModel.mCycle.mOutName;
+        lARColumn = self.mModel.mAR.mOutName;
+        lForecastColumn = str(self.mOriginalSignal) + "_Forecast";
+        lHorizonName = lForecastColumn + "_detrended_" + str(h + 1);
+        for (lDataset, lDF) in forecast_cut_dfs.items():
+            lOriginalDF = original_cut_dfs[lDataset]
+            if(lDF.shape[0] > 0):
+                lDetrendedForecast = lDF[lSeasonalColumn] + lDF[lARColumn]
+                lTarget = lOriginalDF[lTransformedSignalColumn] - lDF[lTrendColumn]
+                if(self.mModel.mDecompositionType == 'TSR'):
+                    lDetrendedForecast = lDF[lSeasonalColumn] * lDF[lARColumn]
+                lTarget = lOriginalDF[lTransformedSignalColumn] / lDF[lTrendColumn]
+                if(self.mModel.mDecompositionType == 'TS+R'):
+                    lDetrendedForecast = lDF[lARColumn]
+                    lTarget = lOriginalDF[lTransformedSignalColumn] / lDF[lTrendColumn]
+                self.mPerformances["detrended"][lDataset][lHorizonName] = self.compute_one_perf(lTarget, lDetrendedForecast, lHorizonName)
+
+
+    def compute_transformed_perfs(self, original_cut_dfs, forecast_cut_dfs, h):
+        lTransformedSignalColumn = self.mModel.mSignal;
+        lTrendColumn = self.mModel.mTrend.mOutName;
+        lSeasonalColumn = self.mModel.mCycle.mOutName;
+        lARColumn = self.mModel.mAR.mOutName;
+        lForecastColumn = str(self.mOriginalSignal) + "_Forecast";
+        lHorizonName = lForecastColumn + "_transformed_" + str(h + 1);
+
+        for (lDataset, lDF) in forecast_cut_dfs.items():
+            lOriginalDF = original_cut_dfs[lDataset]
+            if(lDF.shape[0] > 0):
+                self.mPerformances["transformed"][lDataset][lHorizonName] = self.compute_one_perf(lOriginalDF[lTransformedSignalColumn] , lDF[lTrendColumn] + lDF[lSeasonalColumn] + lDF[lARColumn], lHorizonName);
+
+
+    def compute_deseasonalized_perfs(self, original_cut_dfs, forecast_cut_dfs, h):
+        lTransformedSignalColumn = self.mModel.mSignal;
+        lTrendColumn = self.mModel.mTrend.mOutName;
+        lSeasonalColumn = self.mModel.mCycle.mOutName;
+        lARColumn = self.mModel.mAR.mOutName;
+        lForecastColumn = str(self.mOriginalSignal) + "_Forecast";
+        lHorizonName = lForecastColumn + "_deseasonalized_" + str(h + 1);
+        
+        for (lDataset, lDF) in forecast_cut_dfs.items():
+            lOriginalDF = original_cut_dfs[lDataset]
+            if(lDF.shape[0] > 0):
+                lDeseasonalizedForecast = lDF[lTrendColumn] + lDF[lARColumn]
+                lTarget = lOriginalDF[lTransformedSignalColumn] - lDF[lSeasonalColumn]
+                if(self.mModel.mDecompositionType == 'TSR'):
+                    lDeseasonalizedForecast = lDF[lTrendColumn] * lDF[lARColumn]
+                    lTarget = lOriginalDF[lTransformedSignalColumn] / lDF[lSeasonalColumn]
+                if(self.mModel.mDecompositionType == 'TS+R'):
+                    lDeseasonalizedForecast = lDF[lARColumn]
+                    lTarget = lOriginalDF[lTransformedSignalColumn] / lDF[lSeasonalColumn]
+                self.mPerformances["deseasonalized"][lDataset][lHorizonName] = self.compute_one_perf(lTarget, lDeseasonalizedForecast, lHorizonName);
+
+    def compute_whole_perfs(self, original_cut_dfs, forecast_cut_dfs, h):
+        lOriginalSignalColumn = self.mOriginalSignal;
+        lForecastColumn = str(self.mOriginalSignal) + "_Forecast";
+        lHorizonName = lForecastColumn + "_" + str(h + 1);
+        
+        for (lDataset, lDF) in forecast_cut_dfs.items():
+            lOriginalDF = original_cut_dfs[lDataset]
+            if(lDF.shape[0] > 0):
+                self.mPerformances["whole"][lDataset][lHorizonName] = self.compute_one_perf(lOriginalDF[lOriginalSignalColumn], lDF[lForecastColumn], lHorizonName);
+
         
     def computePerformances(self):
         # lTimer = tsutil.cTimer(("cPredictionIntervalsEstimator::computePerformances",
         #                        {"Model" : self.mModel.mOutName, "Horizon" : self.mModel.mTimeInfo.mHorizon}))
         self.mTime = self.mModel.mTime;
-        self.mSignal = self.mModel.mOriginalSignal;
+        self.mOriginalSignal = self.mModel.mOriginalSignal;
         self.mHorizon = self.mModel.mTimeInfo.mHorizon;
         lTimeColumn = self.mTime;
-        lSignalColumn = self.mSignal;
-        lForecastColumn = str(self.mSignal) + "_Forecast";
+        lOriginalSignalColumn = self.mOriginalSignal;
+        lForecastColumn = str(self.mOriginalSignal) + "_Forecast";
         df = self.mModel.mTrend.mSignalFrame.reset_index();
         N = df.shape[0];
-        (lOriginalFit, lOriginalForecast, lOriginalTest) = self.mModel.mTimeInfo.mSplit.cutFrame(df);
-        df1 = df;
+        original_cut_dfs = self.mModel.mTimeInfo.mSplit.cutFrame(df);
+        df1 = df[ [lTimeColumn , lOriginalSignalColumn] ];
         for h in range(0 , self.mHorizon):
-            df2 = None;
             df2 = self.mModel.forecastOneStepAhead(df1, horizon_index = h+1, perf_mode = True);
             df2 = df2.head(N);
-            lHorizonName = lForecastColumn + "_" + str(h + 1);
-            (lFrameFit, lFrameForecast, lFrameTest) = self.mModel.mTimeInfo.mSplit.cutFrame(df2);
-            self.mFitPerformances[lHorizonName] = self.compute_one_perf(lOriginalFit[lSignalColumn], lFrameFit[lForecastColumn], lHorizonName);
+            forecast_cut_dfs = self.mModel.mTimeInfo.mSplit.cutFrame(df2);
+            self.compute_whole_perfs(original_cut_dfs, forecast_cut_dfs, h)
+            # self.compute_detrended_perfs(original_cut_dfs, forecast_cut_dfs, h)
+            #self.compute_deseasonalized_perfs(original_cut_dfs, forecast_cut_dfs, h)
+            # self.compute_transformed_perfs(original_cut_dfs, forecast_cut_dfs, h)
             
-            self.mForecastPerformances[lHorizonName] = self.compute_one_perf(lOriginalForecast[lSignalColumn], lFrameForecast[lForecastColumn], lHorizonName);
-            if(lOriginalTest.shape[0] > 0):
-                self.mTestPerformances[lHorizonName] = self.compute_one_perf(lOriginalTest[lSignalColumn], lFrameTest[lForecastColumn], lHorizonName);
             df1 = df2[[lTimeColumn , lForecastColumn,
                        self.mModel.mTimeInfo.mRowNumberColumn,
                        self.mModel.mTimeInfo.mNormalizedTimeColumn]];
-            df1.columns = [lTimeColumn , lSignalColumn, self.mModel.mTimeInfo.mRowNumberColumn,
+            df1.columns = [lTimeColumn , lOriginalSignalColumn, self.mModel.mTimeInfo.mRowNumberColumn,
                            self.mModel.mTimeInfo.mNormalizedTimeColumn]
         # self.dump_detailed();
 
     def dump_detailed(self):
         logger = tsutil.get_pyaf_logger();
-        lForecastColumn = str(self.mSignal) + "_Forecast";
+        lForecastColumn = str(self.mOriginalSignal) + "_Forecast";
         for h in range(0 , self.mHorizon):
             lHorizonName = lForecastColumn + "_" + str(h + 1);
             hn = lHorizonName;
             logger.info("CONFIDENCE_INTERVAL_DUMP_FIT " +str(hn) + " " + str(self.mFitPerformances[hn].mL2) + " " + str(self.mFitPerformances[hn].mMAPE));
             logger.info("CONFIDENCE_INTERVAL_DUMP_FORECAST " +str(hn) + " " + str(self.mForecastPerformances[hn].mL2) + " " + str(self.mForecastPerformances[hn].mMAPE));
             logger.info("CONFIDENCE_INTERVAL_DUMP_TEST " +str(hn) + " " + str(self.mTestPerformances[hn].mL2) + " " + str(self.mTestPerformances[hn].mMAPE));
 
 
     def dump(self):
         logger = tsutil.get_pyaf_logger();
-        lForecastColumn = str(self.mSignal) + "_Forecast";
+        lForecastColumn = str(self.mOriginalSignal) + "_Forecast";
         for h in range(0 , self.mHorizon):
             lHorizonName = lForecastColumn + "_" + str(h + 1);
             hn = lHorizonName;
             logger.info("CONFIDENCE_INTERVAL_DUMP_FORECAST " + str(hn) + " " + str(self.mForecastPerformances[hn].mL2));
```

## pyaf/TS/Scikit_Models.py

```diff
@@ -11,38 +11,45 @@
         self.mNbExogenousLags = P;
         self.mScikitModel = None;
         self.mFeatureSelector = None
         self.mComplexity = tscomplex.eModelComplexity.High;
         self.set_name();
 
     def dumpCoefficients(self, iMax=10):
-        # print(self.mScikitModel.__dict__);
+        # tsutil.print_pyaf_detailed_info(self.mScikitModel.__dict__);
         pass
 
     def build_Scikit_Model(self):
         assert(0);
 
     def set_name(self):
         assert(0);
 
+    def get_used_variables(self):
+        lUsed = []
+        for (series, lList_p) in self.mLagsForSeries.items():
+            used = [p for p in lList_p if (series+'_Lag' + str(p) in self.mInputNamesAfterSelection)]
+            if(len(used) > 0):
+                lUsed = lUsed + [series]
+        return lUsed
 
     def fit(self):
-        #  print("ESTIMATE_SCIKIT_MODEL_START" , self.mCycleResidueName);
+        # tsutil.print_pyaf_detailed_info("ESTIMATE_SCIKIT_MODEL_START" , self.mCycleResidueName);
 
         self.build_Scikit_Model();
         
         series = self.mCycleResidueName; 
         self.mTime = self.mTimeInfo.mTime;
         self.mSignal = self.mTimeInfo.mSignal;
         lAREstimFrame = self.mSplit.getEstimPart(self.mARFrame)
 
         lARInputs = lAREstimFrame[self.mInputNames].values
 
         lARTarget = lAREstimFrame[series].values
-        # print(len(self.mInputNames), lARInputs.shape , lARTarget.shape)
+        # tsutil.print_pyaf_detailed_info(len(self.mInputNames), lARInputs.shape , lARTarget.shape)
         assert(lARInputs.shape[1] > 0);
         assert(lARTarget.shape[0] > 0);
         assert(lARInputs.shape[1] == len(self.mInputNames))
 
         from sklearn.feature_selection import SelectKBest
         from sklearn.feature_selection import f_regression
         lMaxFeatures = self.mOptions.mMaxFeatureForAutoreg;
@@ -50,15 +57,15 @@
             lMaxFeatures = lARInputs.shape[1];
         if(lMaxFeatures >= (lARInputs.shape[0] // 4)):
             lMaxFeatures = lARInputs.shape[0] // 4;
         self.mFeatureSelector =  SelectKBest(f_regression, k= lMaxFeatures);
         try:
             self.mFeatureSelector.fit(lARInputs, lARTarget);
         except Exception as e:
-            print("SCIKIT_MODEL_FEATURE_SELECTION_FAILURE" , self.mOutName, lARInputs.shape, e);
+            tsutil.print_pyaf_detailed_info("SCIKIT_MODEL_FEATURE_SELECTION_FAILURE" , self.mOutName, lARInputs.shape, e);
             if(self.mOptions.mDebug):
                 df1 = pd.DataFrame(lARInputs);
                 df1.columns = self.mInputNames
                 df1['TGT'] = lARTarget;
                 # df1.to_csv("SCIKIT_MODEL_FEATURE_SELECTION_FAILURE.csv.gz" , compression='gzip');
             # issue  #72 : ignore feature selection in case of failure.
             self.mFeatureSelector = None
@@ -69,21 +76,21 @@
             self.mInputNamesAfterSelection = [self.mInputNames[k] for k in lSupport];
                 
         else:
             lARInputsAfterSelection = lARInputs;
             self.mInputNamesAfterSelection = self.mInputNames;
 
         assert(len(self.mInputNamesAfterSelection) == lARInputsAfterSelection.shape[1]);
-        # print("FEATURE_SELECTION" , self.mOutName, lARInputs.shape[1] , lARInputsAfterSelection.shape[1]);
+        # tsutil.print_pyaf_detailed_info("FEATURE_SELECTION" , self.mOutName, lARInputs.shape[1] , lARInputsAfterSelection.shape[1]);
         del lARInputs;
 
         try:
             self.mScikitModel.fit(lARInputsAfterSelection, lARTarget)
         except Exception as e:
-            print("SCIKIT_MODEL_FIT_FAILURE" , self.mOutName, lARInputsAfterSelection.shape, e);
+            tsutil.print_pyaf_detailed_info("SCIKIT_MODEL_FIT_FAILURE" , self.mOutName, lARInputsAfterSelection.shape, e);
             if(self.mOptions.mDebug):
                 df1 = pd.DataFrame(lARInputsAfterSelection);
                 df1.columns = self.mInputNamesAfterSelection
                 df1['TGT'] = lARTarget;
                 # df1.to_csv("SCIKIT_MODEL_FIT_FAILURE.csv.gz" , compression='gzip');
             del self.mScikitModel
             self.mScikitModel = None;
@@ -102,22 +109,22 @@
             self.mARFrame[self.mOutName] = 0.0
             if(self.mDecompositionType in ['TSR']):
                 self.mARFrame[self.mOutName] = 1.0
                 
 
         self.compute_ar_residue(self.mARFrame)
 
-        # print("ESTIMATE_SCIKIT_MODEL_END" , self.mOutName);
+        # tsutil.print_pyaf_detailed_info("ESTIMATE_SCIKIT_MODEL_END" , self.mOutName);
 
 
     def transformDataset(self, df, horizon_index = 1):
         series = self.mCycleResidueName; 
         if(self.mExogenousInfo is not None):
             df = self.mExogenousInfo.transformDataset(df);
-        lag_df = self.generateLagsForForecast(df);
+        lag_df = self.generateLagsForForecast(df, selection = self.mInputNamesAfterSelection);
         inputs_after_feat_selection = lag_df[self.mInputNamesAfterSelection].values
         # inputs_after_feat_selection = self.mFeatureSelector.transform(inputs) if self.mFeatureSelector else inputs;
         if(self.mScikitModel is not None):
             pred = self.mScikitModel.predict(inputs_after_feat_selection)
             df[self.mOutName] = pred;
         else:
             df[self.mOutName] = 0.0
```

## pyaf/TS/SignalDecomposition.py

```diff
@@ -22,19 +22,19 @@
             raise tsutil.PyAF_Error("PYAF_ERROR_NEGATIVE_OR_NULL_HORIZON " + str(iHorizon));
         if(iTime not in iInputDS.columns):
             raise tsutil.PyAF_Error("PYAF_ERROR_TIME_COLUMN_NOT_FOUND " + str(iTime));
         for lSignal in [iSignal]:
             if(lSignal not in iInputDS.columns):
                 raise tsutil.PyAF_Error("PYAF_ERROR_SIGNAL_COLUMN_NOT_FOUND " + str(lSignal));
             type2 = iInputDS[lSignal].dtype
-            # print(type2)
+            # tsutil.print_pyaf_detailed_info(type2)
             if(type2.kind != 'i' and type2.kind != 'u' and type2.kind != 'f'):
                 raise tsutil.PyAF_Error("PYAF_ERROR_SIGNAL_COLUMN_TYPE_NOT_ALLOWED '" + str(lSignal) + "' '" + str(type2) + "'");
         type1 = iInputDS[iTime].dtype
-        # print(type1)
+        # tsutil.print_pyaf_detailed_info(type1)
         if(type1.kind != 'M' and type1.kind != 'i' and type1.kind != 'u' and type1.kind != 'f'):
             raise tsutil.PyAF_Error("PYAF_ERROR_TIME_COLUMN_TYPE_NOT_ALLOWED '" + str(iTime) + "' '" + str(type1) + "'");
         # time in exogenous data should be the strictly same type as time in training dataset (join needed)
         if(iExogenousData is not None):
             lExogenousDataFrame = iExogenousData[0];
             lExogenousVariables = iExogenousData[1];
             if(iTime not in lExogenousDataFrame.columns):
@@ -69,18 +69,20 @@
             if(dict == type(iExogenousData)):
                 self.mExogenousData[sig] = iExogenousData[sig]
             else:
                 self.mExogenousData[sig] = iExogenousData
         
             
     def train(self , iInputDS, iTimes, iSignals, iHorizons, iExogenousData = None):
+        logger = tsutil.get_pyaf_logger();
         from . import SignalDecomposition_Trainer as tstrainer
 
         self.reinterpret_by_signal_args(iTimes, iSignals, iHorizons, iExogenousData)
-        # print(iInputDS.shape, iInputDS.columns, self.mSignals, self.mDateColumns, self.mHorizons)
+        # tsutil.print_pyaf_detailed_info(iInputDS.shape, iInputDS.columns, self.mSignals, self.mDateColumns, self.mHorizons)
+        logger.info("TRAINING_ENGINE_START " + str({"Signals" : self.mSignals, "Horizons" : self.mHorizons}));
         lTimer = tsutil.cTimer(("TRAINING", {"Signals" : self.mSignals, "Horizons" : self.mHorizons}))
 
         for sig in self.mSignals:
             self.checkData(iInputDS, self.mDateColumns[sig], sig, self.mHorizons[sig], self.mExogenousData[sig]);
 
         self.mTrainingDataset = iInputDS; 
 
@@ -96,49 +98,50 @@
         # some backward compatibility
         lFirstSignal = self.mSignals[0] 
         self.mBestModel = self.mBestModels[lFirstSignal]
         self.mTrainingTime = lTimer.get_elapsed_time()
         for (lSignal, lBestModel) in self.mBestModels.items():
             lBestModel.clean_dataframes()
         del lTrainer
+        logger.info("TRAINING_ENGINE_END " + str(self.mTrainingTime));
         
 
 
     def forecast(self , iInputDS, iHorizon):
+        logger = tsutil.get_pyaf_logger();
+        logger.info("FORECASTING_ENGINE_START " + str({"Signals" : self.mSignals, "Horizons" : self.mHorizons}));
         from . import SignalDecomposition_Forecaster as tsforec
         lTimer = tsutil.cTimer(("FORECASTING", {"Signals" : self.mSignals, "Horizon" : iHorizon}))
         lForecaster = tsforec.cSignalDecompositionForecaster()
         lForecastFrame = lForecaster.forecast(self, iInputDS, iHorizon)
         del lForecaster
-        
+        logger.info("FORECASTING_ENGINE_END " + str(lTimer.get_elapsed_time()));
         return lForecastFrame;
 
 
     def getModelFormula(self):
         lFormula = {}
         for lSignal in self.mSignals:
             lFormula[lSignal] = self.mBestModel.getFormula();
         return lFormula;
 
     def get_competition_details(self):
         logger = tsutil.get_pyaf_logger();
         for lSignal in self.mSignals:
             logger.info("COMPETITION_DETAIL_START '" + lSignal + "'");
             lShortList_Dict = self.mModelShortListBySignal[lSignal].to_dict(orient = 'index')
-            # print(lShortList_Dict)
+            # tsutil.print_pyaf_detailed_info(lShortList_Dict)
             for k in sorted(lShortList_Dict.keys()):
                 v = lShortList_Dict[k]
                 logger.info("COMPETITION_DETAIL_SHORT_LIST '" + lSignal + "' " + str(k) + " " + str(v));
             logger.info("COMPETITION_DETAIL_END '" + lSignal + "'");
 
     def getModelInfo(self):
         for lSignal in self.mSignals:
             self.mBestModels[lSignal].getInfo()
-        logger = tsutil.get_pyaf_logger();
-        logger.info("TRAINING_TIME_IN_SECONDS " + str(self.mTrainingTime));
         self.get_competition_details()
         
 
     def to_dict(self, iWithOptions = False):
         dict1 = {}
         dict1["Training_Time"] = self.mTrainingTime
         for lSignal in self.mSignals:
```

## pyaf/TS/SignalDecomposition_AR.py

```diff
@@ -38,74 +38,75 @@
         if(self.mDecompositionType in ['T+S+R']):
             df[self.mOutName + '_residue'] = lSignal - lTrend - lCycle - lAR
         if(self.mDecompositionType in ['TS+R']):
             df[self.mOutName + '_residue'] = lSignal - lTrend * lCycle - lAR
         else:
             df[self.mOutName + '_residue'] = lSignal - (lTrend * lCycle * lAR)
         # df_detail = df[[self.mSignal, self.mTrend.mOutName, self.mCycle.mOutName, self.mOutName, self.mOutName + '_residue']]
-        # print("compute_ar_residue_detail ", (self.mOutName, self.mDecompositionType, df_detail.describe(include='all').to_dict()))
+        # tsutil.print_pyaf_detailed_info("compute_ar_residue_detail ", (self.mOutName, self.mDecompositionType, df_detail.describe(include='all').to_dict()))
         
     def plot(self):
         tsplot.decomp_plot(self.mARFrame, self.mTimeInfo.mNormalizedTimeColumn,
                            self.mCycleResidueName, self.mOutName , self.mOutName + '_residue', horizon = self.mTimeInfo.mHorizon);
 
 
     def register_lag(self, series, p):
         name = series+'_Lag' + str(p);
-        # print("register_lag", (series , p , name))
+        # tsutil.print_pyaf_detailed_info("register_lag", (series , p , name))
         assert(name not in self.mInputNames)
         self.mInputNames.append(name);
         self.mLagsForSeries[series] = self.mLagsForSeries.get(series , [])
         self.mLagsForSeries[series].append(p)
+
+    def get_used_variables(self):
+        return [x for x in self.mLagsForSeries.keys()]
         
     def dumpCoefficients(self):
         pass
     
     def computePerf(self):
-        self.mARFitPerf= tsperf.cPerf();
-        self.mARForecastPerf= tsperf.cPerf();
-        (lFrameFit, lFrameForecast, lFrameTest) = self.mSplit.cutFrame(self.mARFrame);
-        self.mARFitPerf.computeCriterionValues(
-            lFrameFit[self.mCycleResidueName],
-            lFrameFit[self.mOutName],
-            [self.mTimeInfo.mOptions.mModelSelection_Criterion],
-            self.mOutName)
-        self.mARForecastPerf.computeCriterionValues(
-            lFrameForecast[self.mCycleResidueName],
-            lFrameForecast[self.mOutName],
-            [self.mTimeInfo.mOptions.mModelSelection_Criterion],
-            self.mOutName)
+        self.mARPerfs = {}
+        lCutting = self.mSplit.cutFrame(self.mARFrame);
+        for(lDataset , lDF) in lCutting.items():
+            lPerf = tsperf.cPerf();
+            lPerf.computeCriterionValues(lDF[self.mCycleResidueName],
+                                         lDF[self.mOutName],
+                                         [self.mTimeInfo.mOptions.mModelSelection_Criterion],
+                                         self.mOutName + "_" + str(lDataset))
+            self.mARPerfs[lDataset] = lPerf
 
     def shift_series(self, series, p, idefault):
         N = series.shape[0];
         new_values = np.append([ idefault ]*p, series[0:N-p])
         return new_values
     
     def getDefaultValue(self, series):
         return self.mDefaultValues[series];
 
-    def generateLagsForForecast(self, df):
+    def generateLagsForForecast(self, df, selection = None):
         lDict = {}
         # lDict[self.mCycleResidueName] = df[self.mCycleResidueName]
         series = self.mCycleResidueName
         lSeries = df[self.mCycleResidueName]
         #  Investigate Large Horizon Models #213 : The model can produce overflows in its inputs when iterated. 
         lSeries = lSeries.values.clip(-1e+10, +1e10)
         for p in self.mLagsForSeries[self.mCycleResidueName]:
             name = series +'_Lag' + str(p);
-            lShiftedSeries = self.shift_series(lSeries, p , self.mDefaultValues[series]); 
-            lDict[name] = lShiftedSeries
+            if(selection is None or name in selection):
+                lShiftedSeries = self.shift_series(lSeries, p , self.mDefaultValues[series]);
+                lDict[name] = lShiftedSeries
         # Exogenous variables lags
         if(self.mExogenousInfo is not None):
             for ex in self.mExogenousInfo.mEncodedExogenous:
                 if(self.mLagsForSeries.get(ex)):
                     for p in self.mLagsForSeries[ex]:
                         name = ex +'_Lag' + str(p);
-                        lShiftedSeries = self.shift_series(df[ex], p , self.mDefaultValues[ex]); 
-                        lDict[name] = lShiftedSeries
+                        if(selection is None or name in selection):
+                            lShiftedSeries = self.shift_series(df[ex], p , self.mDefaultValues[ex]); 
+                            lDict[name] = lShiftedSeries
         cols = lDict.keys()
         lArray = np.concatenate([lDict[k].reshape(-1, 1) for k in lDict.keys()], axis = 1, dtype = lSeries.dtype)
         lag_df = pd.DataFrame(data = lArray, columns= cols, index = df.index, dtype = lSeries.dtype)
         return lag_df;
 
 
 class cZeroAR(cAbstractAR):
@@ -125,16 +126,14 @@
         if(self.mDecompositionType in ['TSR']):
             # multiplicative models
             self.mConstantValue = 1.0
         
         # self.mTimeInfo.addVars(self.mARFrame);
         # self.mARFrame[series] = self.mCycleFrame[series]
         self.mARFrame[self.mOutName] = self.mConstantValue;
-        self.mARFrame[self.mCycle.mOutName] = self.mConstantValue;
-        self.mARFrame[self.mTrend.mOutName] = self.mConstantValue;
         self.compute_ar_residue(self.mARFrame)
         assert(self.mARFrame.shape[0] > 0)
                 
 
     def transformDataset(self, df, horizon_index = 1):
         df[self.mOutName] = self.mConstantValue;
         self.compute_ar_residue(df)
@@ -229,30 +228,31 @@
                 for autoreg in self.mARList[cycle_residue]:
                     if(autoreg.mExogenousInfo is not None): # ARX,XGBX, ... only
                         for lag in lags_ex:
                             (name , p) = lag
                             autoreg.register_lag(name, p)
 
         self.mARFrame = pd.concat([self.mARFrame] + lag_dfs, axis = 1)
-
+        self.mARFrame = self.mARFrame.copy() # Avoid "PerformanceWarning: DataFrame is highly fragmented"
 
     # @profile
     def estimate_ar_models_for_cycle(self, cycle_residue):
         logger = tsutil.get_pyaf_logger();
         self.mARFrame = pd.DataFrame(index = self.mCycleFrame.index);
         self.mTimeInfo.addVars(self.mARFrame);
         self.mCycleFrame[cycle_residue] = self.mCycleFrame[cycle_residue]            
         self.mARFrame[cycle_residue] = self.mCycleFrame[cycle_residue]            
+        self.mARFrame[self.mTimeInfo.mSignal] = self.mCycleFrame[self.mTimeInfo.mSignal]
 
         self.mDefaultValues = {};
 
         self.addLagsForTraining(self.mCycleFrame, cycle_residue);
 
 
-        # print(self.mARFrame.info());
+        # tsutil.print_pyaf_detailed_info(self.mARFrame.info());
 
         lCleanListOfArModels = [];
         for autoreg in self.mARList[cycle_residue]:
             self.mARFrame[autoreg.mTrend.mOutName] = autoreg.mCycle.mTrendFrame[autoreg.mTrend.mOutName]            
             self.mARFrame[autoreg.mCycle.mOutName] = self.mCycleFrame[autoreg.mCycle.mOutName]            
             if((autoreg.mFormula == "NoAR") or (len(autoreg.mInputNames) > 0)):
                 lCleanListOfArModels.append(autoreg);
@@ -273,23 +273,24 @@
             autoreg.mOptions = self.mOptions;
             autoreg.mCycleFrame = self.mCycleFrame;
             autoreg.mARFrame = self.mARFrame
             autoreg.mTimeInfo = self.mTimeInfo;
             autoreg.mSplit = self.mSplit;
             autoreg.mDefaultValues = self.mDefaultValues;
             autoreg.mDecompositionType = self.mDecompositionType
+            autoreg.mInputNamesAfterSelection = autoreg.mInputNames
             lTimer = None
             if(self.mOptions.mDebugAR):
                 lTimer = tsutil.cTimer(("TRAINING_AR_MODEL", autoreg.mFormula, autoreg.mCycleResidueName))
             autoreg.fit();
             if(self.mOptions.mDebugAR):
                 autoreg.computePerf();
 
     def check_not_nan(self, sig , name):
-        #print("check_not_nan");
+        # tsutil.print_pyaf_detailed_info("check_not_nan");
         if(np.isnan(sig[:-1]).any()):
             logger = tsutil.get_pyaf_logger();
             logger.error("CYCLE_RESIDUE_WITH_NAN_IN_SIGNAL" + str(sig));
             raise tsutil.Internal_PyAF_Error("INVALID_COLUMN _FOR_CYCLE_RESIDUE ['"  + name + "'");
         pass
```

## pyaf/TS/SignalDecomposition_Cycle.py

```diff
@@ -9,14 +9,15 @@
 
 from . import Time as tsti
 from . import DateTime_Functions as dtfunc
 from . import Perf as tsperf
 from . import Plots as tsplot
 from . import Utils as tsutil
 from . import Complexity as tscomplex
+from . import TimeSeries_Cutting as tscut
 
 class cAbstractCycle:
     def __init__(self , trend):
         self.mTimeInfo = tsti.cTimeInfo()
         self.mTrendFrame = None
         self.mCycleFrame = None
         self.mTrend = trend;
@@ -31,20 +32,20 @@
 
     def plot(self):
         tsplot.decomp_plot(self.mCycleFrame, self.mTimeInfo.mNormalizedTimeColumn,
                            self.mTrend_residue_name, self.getCycleName() , self.getCycleResidueName(), horizon = self.mTimeInfo.mHorizon);
 
 
     def check_not_nan(self, sig , name):
-        #print("check_not_nan");
+        # tsutil.print_pyaf_detailed_info("check_not_nan");
         if(np.isnan(sig[:-1]).any() or np.isinf(sig[:-1]).any() ):
             logger = tsutil.get_pyaf_logger();
             logger.error("CYCLE_RESIDUE_WITH_NAN_IN_SIGNAL" + str(sig));
             raise tsutil.Internal_PyAF_Error("CYCLE_COLUMN _FOR_TREND_RESIDUE ['"  + name + "'");
-        # print("check_cycle_residue ", (name, self.mDecompositionType, sig[:-1].min(), sig[:-1].max(), sig[:-1].mean(), sig[:-1].std()))
+        # tsutil.print_pyaf_detailed_info("check_cycle_residue ", (name, self.mDecompositionType, sig[:-1].min(), sig[:-1].max(), sig[:-1].mean(), sig[:-1].std()))
         if(sig[:-1].max() > 1e5):
             self.dump_values()
             raise tsutil.Internal_PyAF_Error("Invalid cycle_residue_too_large '" + str(name) + "'");
         pass
         pass
 
     def compute_cycle_residue(self, df):
@@ -58,15 +59,15 @@
             df[self.getCycleResidueName()] = lSignal - lTrend * lCycle 
         else:
             lTrendCycle = lTrend * lCycle
             # This is questionable. But if only a few values are zero, it is the safest.
             lTrendCycle = lTrendCycle.apply(lambda x : x if(abs(x) > 1e-2) else 1e-2)
             df[self.getCycleResidueName()] = lSignal / lTrendCycle
         # df_detail = df[[self.mSignal, self.mTrend.mOutName, self.getCycleName(), self.getCycleResidueName()]]
-        # print("compute_cycle_residue_detail ", (lOutName, self.mDecompositionType, df_detail.describe(include='all').to_dict()))
+        # tsutil.print_pyaf_detailed_info("compute_cycle_residue_detail ", (lOutName, self.mDecompositionType, df_detail.describe(include='all').to_dict()))
         
 
     def compute_target_means_by_cycle_value(self , iCycleFrame, iCycleName):
         # we encode only using estimation
         lCycleFrameEstim = self.mSplit.getEstimPart(iCycleFrame);
         lGroupBy = lCycleFrameEstim.groupby(by=[iCycleName] , sort=False)[self.mTrend_residue_name]
         lEncodedValueDict = None
@@ -85,35 +86,30 @@
             return np.float64(lCycleFrameEstim[self.mTrend_residue_name].mean());
         return np.float64(lCycleFrameEstim[self.mTrend_residue_name].median());
 
     def computePerf(self):
         if(self.mOptions.mDebug):
             self.check_not_nan(self.mCycleFrame[self.getCycleResidueName()], self.getCycleResidueName())
         # self.mCycleFrame.to_csv(self.getCycleResidueName() + ".csv");
-        self.mCycleFitPerf = tsperf.cPerf();
-        self.mCycleForecastPerf = tsperf.cPerf();
+        self.mCyclePerfs = {}
         # self.mCycleFrame[[self.mTrend_residue_name, self.getCycleName()]].to_csv(self.getCycleName() + ".csv");
-        (lFrameFit, lFrameForecast, lFrameTest) = self.mSplit.cutFrame(self.mCycleFrame);
-        
-        self.mCycleFitPerf.computeCriterionValues(
-            lFrameFit[self.mTrend_residue_name], lFrameFit[self.getCycleName()],
-            [self.mOptions.mCycle_Criterion], self.getCycleName())
-        self.mCycleForecastPerf.computeCriterionValues(
-            lFrameForecast[self.mTrend_residue_name], lFrameForecast[self.getCycleName()],
-            [self.mOptions.mCycle_Criterion], self.getCycleName())
+        lCutting = self.mSplit.cutFrame(self.mCycleFrame);
+        for(lDataset , lDF) in lCutting.items():
+            lPerf = tsperf.cPerf();
+            lPerf.computeCriterionValues(
+                lDF[self.mTrend_residue_name], lDF[self.getCycleName()],
+                [self.mOptions.mCycle_Criterion], self.getCycleName() + "_" + str(lDataset))
+            self.mCyclePerfs[lDataset] = lPerf
         self.dumpCyclePerf()
 
     
     def dumpCyclePerf(self):
         if(self.mOptions.mDebugCycles):
             logger = tsutil.get_pyaf_logger();
-            lDict = {
-                "Fit" : self.mCycleFitPerf.getCriterionValue(self.mOptions.mCycle_Criterion),
-                "Forecast" : self.mCycleForecastPerf.getCriterionValue(self.mOptions.mCycle_Criterion),
-            }
+            lDict = self.mCyclePerfs
             logger.info("CYCLE_PERF_DETAIL " + self.mOptions.mCycle_Criterion  + " " + self.mOutName +  " " + str(lDict))
 
 
 class cZeroCycle(cAbstractCycle):
 
     def __init__(self , trend):
         super().__init__(trend);
@@ -134,14 +130,15 @@
         self.mSignal = self.mTimeInfo.mSignal;
         self.mTimeInfo.addVars(self.mCycleFrame);
         self.mConstantValue = 0.0        
         if(self.mDecompositionType in ['TS+R', 'TSR']):
             # multiplicative models
             self.mConstantValue = 1.0
 
+        self.mCycleFrame[self.mSignal] = self.mTrendFrame[self.mSignal]
         self.mCycleFrame[self.mTrend.mOutName] = self.mTrendFrame[self.mTrend.mOutName]
         self.mCycleFrame[self.mTrend_residue_name] = self.mTrendFrame[self.mTrend_residue_name]
         self.mCycleFrame[self.getCycleName()] = self.mConstantValue
         self.mOutName = self.getCycleName()
         self.compute_cycle_residue(self.mCycleFrame)
         
     def transformDataset(self, df):
@@ -211,27 +208,28 @@
     def fit(self):
         assert(self.mTimeInfo.isPhysicalTime());
         lHor = self.mTimeInfo.mHorizon;
         self.mTime = self.mTimeInfo.mTime;
         self.mSignal = self.mTimeInfo.mSignal;
         self.mTimeInfo.addVars(self.mCycleFrame);
         lName = self.getCycleName();
+        self.mCycleFrame[self.mSignal] = self.mTrendFrame[self.mSignal]
         self.mCycleFrame[self.mTrend_residue_name] = self.mTrendFrame[self.mTrend_residue_name]
         self.mCycleFrame[self.mTrend.mOutName] = self.mTrendFrame[self.mTrend.mOutName]
         self.mCycleFrame[lName] = self.compute_date_parts(self.mTrendFrame[self.mTime])
         self.mDefaultValue = self.compute_target_means_default_value()
         self.mEncodedValueDict = self.compute_target_means_by_cycle_value(self.mCycleFrame, self.getCycleName())
 
         self.mCycleFrame[lName + '_enc'] = self.mCycleFrame[lName].map(self.mEncodedValueDict).fillna(self.mDefaultValue)
         self.mCycleFrame[lName + '_enc'].fillna(self.mDefaultValue, inplace=True);
         self.mCycleFrame[lName + '_NotEncoded'] = self.mCycleFrame[lName];
         self.mCycleFrame[lName] = self.mCycleFrame[lName + '_enc'];
         
         self.mOutName = self.getCycleName()
-        #print("encoding '" + lName + "' " + str(self.mEncodedValueDict));
+        # tsutil.print_pyaf_detailed_info("encoding '" + lName + "' " + str(self.mEncodedValueDict));
         # The longer the seasonal, the more complex it is.
         self.mComplexity = tscomplex.eModelComplexity.Low;
         if(len(self.mEncodedValueDict.keys()) > 31):
             self.mComplexity = tscomplex.eModelComplexity.High;
         self.compute_cycle_residue(self.mCycleFrame)
 
     def transformDataset(self, df):
@@ -293,14 +291,15 @@
             lCycleLengths3 = lCycleLengths0 + lCycleLengths1 + lCycleLengths2
             lCycleLengths4 = list(set(lCycleLengths3))
             return [x for x in lCycleLengths4 if (x < signal_length // 6)]
         return [x for x in self.mOptions.mCycleLengths if (x < signal_length // 6)]
 
     def generate_cycles(self):
         self.mTimeInfo.addVars(self.mCycleFrame);
+        self.mCycleFrame[self.mSignal] = self.mTrendFrame[self.mSignal]
         self.mCycleFrame[self.mTrend_residue_name] = self.mTrendFrame[self.mTrend_residue_name]
         self.mCycleFrame[self.mTrend.mOutName] = self.mTrendFrame[self.mTrend.mOutName]
         self.mDefaultValue = self.compute_target_means_default_value();
         self.mCyclePerfByLength = {}
         lEstimResidue = self.mSplit.getEstimPart(self.mTrendFrame[self.mTrend_residue_name])
         lCycleLengths = self.get_tested_cycles(lEstimResidue.shape[0])
         lTimer = None
@@ -322,25 +321,25 @@
                 lValidFrame = self.mSplit.getValidPart(lCycleFrame);
                 lCritValues = lPerf.computeCriterionValues(lValidFrame[self.mTrend_residue_name],
                                                     lValidFrame[name_length + "_enc"],
                                                     [self.mCriterion],
                                                     "Validation")
                 lCritValue = lCritValues[self.mCriterion]
                 if(lCritValue is None):
-                    print("CYCFLE_CRITERION_VALUES", lCritValues)
+                    tsutil.print_pyaf_detailed_info("CYCFLE_CRITERION_VALUES", lCritValues)
                 if(lPerf.is_acceptable_criterion_value(self.mOptions.mCycle_Criterion, iRefValue = lCritValue)):
                     self.mCyclePerfByLength[lLength] = (round(lCritValue, 3) , len(lEncodedValueDict))
                     if(self.mOptions.mDebugCycles):
                         logger = tsutil.get_pyaf_logger();
                         logger.debug("CYCLE_INTERNAL_CRITERION " + name_length + " " + str(lLength) + \
                                      " " + self.mCriterion +" " + str(lCritValue))
         pass
 
     def fit(self):
-        # print("cycle_fit" , self.mTrend_residue_name);
+        # tsutil.print_pyaf_detailed_info("cycle_fit" , self.mTrend_residue_name);
         self.mTime = self.mTimeInfo.mTime;
         self.mSignal = self.mTimeInfo.mSignal;
         self.generate_cycles();
         self.computeBestCycle();
         self.mOutName = self.getCycleName()
         self.mFormula = "Cycle_None"
         if(self.mBestCycleLength is not None):
@@ -353,16 +352,16 @@
             if(len(lDict.keys()) > 31):
                 self.mComplexity = tscomplex.eModelComplexity.High;
 
     def transformDataset(self, df):
         if(self.mBestCycleLength is not None):
             lValueCol = df[self.mTimeInfo.mRowNumberColumn].mod(self.mBestCycleLength);
             df['cycle_internal'] = lValueCol;
-            # print("BEST_CYCLE" , self.mBestCycleLength)
-            # print(self.mBestCycleValueDict);
+            # tsutil.print_pyaf_detailed_info("BEST_CYCLE" , self.mBestCycleLength)
+            # tsutil.print_pyaf_detailed_info(self.mBestCycleValueDict);
             lDict = self.mBestCycleValueDict[self.mBestCycleLength];
             df[self.getCycleName()] = lValueCol.map(lDict).fillna(self.mDefaultValue)
         else:
             df[self.getCycleName()] = np.zeros_like(df[self.mTimeInfo.mRowNumberColumn]);
             if(self.mDecompositionType in ['TS+R', 'TSR']):
                 # multiplicative models
                 df[self.getCycleName()] = 1.0
@@ -452,14 +451,15 @@
 
 
     def estimateCycles(self):
         self.mTime = self.mTimeInfo.mTime;
         self.mSignal = self.mTimeInfo.mSignal;
         self.mCycleFrame = pd.DataFrame(index = self.mTrendFrame.index);
         self.mTimeInfo.addVars(self.mCycleFrame);
+        self.mCycleFrame[self.mSignal] = self.mTrendFrame[self.mSignal]
         for trend in self.mTrendList:
             lTrend_residue_name = trend.mOutName + '_residue'
             self.mCycleFrame[lTrend_residue_name] = self.mTrendFrame[lTrend_residue_name]
             for cycle in self.mCycleList[trend]:
                 cycle.fit();
                 cycle.computePerf();
                 self.mCycleFrame[cycle.getCycleName()] = cycle.mCycleFrame[cycle.getCycleName()]
@@ -471,38 +471,39 @@
             self.mCycleFrame = self.mCycleFrame.copy()
         pass
 
 
     def filterSeasonals(self):
         logger = tsutil.get_pyaf_logger();
         logger.debug("CYCLE_TRAINING_FILTER_SEASONALS_START")
+        lForecastDataset = tscut.eDatasetType.Forecast
         for trend in self.mTrendList:
             lPerfs = {}
             lTrend_residue_name = trend.mOutName + '_residue'
             lCycleList = []
             lSeasonals = {}
             for cycle in self.mCycleList[trend]:
                 if(isinstance(cycle , cSeasonalPeriodic)):
                     # check that the MAPE is not above 1.0
-                    if(cycle.mCycleForecastPerf.is_acceptable_criterion_value(self.mOptions.mCycle_Criterion)):
-                        lCritValue = cycle.mCycleForecastPerf.getCriterionValue(self.mOptions.mCycle_Criterion)
+                    if(cycle.mCyclePerfs[lForecastDataset].is_acceptable_criterion_value(self.mOptions.mCycle_Criterion)):
+                        lCritValue = cycle.mCyclePerfs[lForecastDataset].getCriterionValue(self.mOptions.mCycle_Criterion)
                         lCategories = len(cycle.mEncodedValueDict.keys())
                         lPerfs[cycle.mOutName] = (round(lCritValue, 3), lCategories)
                         lSeasonals[cycle.mOutName] = cycle
                 else:
                     lCycleList = lCycleList + [cycle]
             
             if(len(lSeasonals) == 0):
                 return
             lData = lPerfs.items()
             # less MAPE is better, less categories is better, the last is the name of the seasonal to have a total order.
             lSortingMethod_By_MAPE = lambda x : (x[1][0], x[0]) 
             lData = sorted(lData, key = lSortingMethod_By_MAPE) # MAPE => MASE
             assert(len(lData) > 0)
-            lBestPerf = lSeasonals[ lData[0][0] ].mCycleForecastPerf
+            lBestPerf = lSeasonals[ lData[0][0] ].mCyclePerfs[lForecastDataset]
             lBestCriterion = lData[0][1]
             lData_smallest = [x for x in lData if lBestPerf.is_close_criterion_value(self.mOptions.mCycle_Criterion,
                                                                                      x[1][0],
                                                                                      iTolerance = 0.05)]
             lSortingMethod_By_Length = lambda x : (x[1][1], x[0])
             lData_smallest = sorted(lData_smallest, key = lSortingMethod_By_Length)
             assert(len(lData_smallest) > 0)
```

## pyaf/TS/SignalDecomposition_Trainer.py

```diff
@@ -50,17 +50,17 @@
     def setParams(self , iInputDS, iTime, iSignal, iHorizon, iTransformation,
                   iDecomspositionType, iExogenousData = None):
         assert(iInputDS.shape[0] > 0)
         assert(iInputDS.shape[1] > 0)
         assert(iTime in iInputDS.columns)
         assert(iSignal in iInputDS.columns)
 
-        # print("setParams , head", iInputDS.head());
-        # print("setParams , tail", iInputDS.tail());
-        # print("setParams , columns", iInputDS.columns);
+        # tsutil.print_pyaf_detailed_info("setParams , head", iInputDS.head());
+        # tsutil.print_pyaf_detailed_info("setParams , tail", iInputDS.tail());
+        # tsutil.print_pyaf_detailed_info("setParams , columns", iInputDS.columns);
         
         self.mTime = iTime
         self.mOriginalSignal = iSignal;
 
         self.mDecompositionType = iDecomspositionType
         
         self.mTransformation = iTransformation;
@@ -101,20 +101,31 @@
         # lTimer = tsutil.cTimer(("UPDATE_PERFS_FOR_ALL_MODELS", {"Signal" : self.mOriginalSignal, "Transformation" : self.mSignal, "DecompositionType" : self.mDecompositionType}, len(iModels)))
         self.mPerfsByModel = {}
         for model in iModels.keys():
             # lTimer2 = tsutil.cTimer(("UPDATE_PERFS_FOR_MODEL", model))
             iModels[model].updatePerfs();
             
         for (name, model) in iModels.items():
-            # print(name, model.__dict__);
+            # tsutil.print_pyaf_detailed_info(name, model.__dict__);
             lComplexity = model.getComplexity_as_ordering_string();
-            (lFitPerf, lForecastPerf, lTestPerf) = model.get_aggregated_criterion_values_for_model_selection();
             lSplit = model.mTimeInfo.mOptions.mCustomSplit
-            
-            self.mPerfsByModel[(self.mSignal, self.mDecompositionType, lSplit, model.mOutName)] = [(self.mSignal, self.mDecompositionType, model), lComplexity, lFitPerf , lForecastPerf, lTestPerf];
+            model_perfs = model.get_perfs_summary()
+            self.mPerfsByModel[name] = {
+                "OriginalSignal" : self.mOriginalSignal,
+                "Signal" : self.mSignal,
+                "DecompositionType" : self.mDecompositionType,
+                "ModelName" : name,
+                "Complexity" : lComplexity,
+                "FitPerf" : model.mFitPerfs,
+                "ForecastPerf" : model.mForecastPerfs,
+                "TestPerf" : model.mTestPerfs,
+                "ModelCategory" : model.get_model_category(),
+                "Horizon" : model.mTimeInfo.mHorizon,
+                "Split" : lSplit
+            }
             
         return iModels;
 
 
     def train(self , iInputDS, iSplit, iTime, iSignal,
               iHorizon, iTransformation, iDecomspositionType):
         lTimer = tsutil.cTimer(("TRAINING", {"Signal" : iSignal,
@@ -137,17 +148,15 @@
         self.mSplit.estimate();
         self.mTimeInfo.mSignalFrame = self.mSignalFrame;
         self.mTimeInfo.estimate();
         self.mSignalFrame['row_number'] = np.arange(0, self.mSignalFrame.shape[0]);
 
         lSignal = self.mSignalFrame[self.mOriginalSignal]
         self.mTransformation.fit(lSignal);
-
-        self.mSignalFrame[self.mSignal] = self.mTransformation.apply(lSignal);
-        # self.mSignalFrame[self.mSignal] = self.mSignalFrame[self.mSignal].astype(np.float32);
+        self.mSignalFrame = self.mTransformation.transformDataset(self.mSignalFrame)
         
         if(self.mExogenousInfo is not None):
             lTimer2 = None
             if(self.mOptions.mDebugProfile):
                 lTimer2 = tsutil.cTimer(("TRAINING_EXOGENOUS_DATA", {"Signal" : iSignal}))
             self.mExogenousInfo.fit();
 
@@ -195,27 +204,29 @@
         lAREstimator.mDecompositionType = iDecomspositionType
         lAREstimator.mExogenousInfo = self.mExogenousInfo;
         lAREstimator.mOptions = self.mOptions;
         lAREstimator.estimate();
 
 
         # forecast perfs
-        lModels = {};
+        self.mModelsByName = {};
         for trend in lAREstimator.mTrendList:
             for cycle in lAREstimator.mCycleList[trend]:
                 cycle_residue = cycle.getCycleResidueName();
                 for autoreg in lAREstimator.mARList[cycle_residue]:
                     lModel = tsmodel.cTimeSeriesModel(self.mTransformation, self.mDecompositionType,
                                                       trend, cycle, autoreg);
-                    lModels[lModel.mOutName] = lModel;
+                    lSplit = lModel.mTimeInfo.mOptions.mCustomSplit
+                    lName = (self.mSignal, self.mDecompositionType, lSplit, lModel.mOutName)
+                    self.mModelsByName[lName] = lModel;
 
         del lAREstimator;
         
 
-        self.updatePerfsForAllModels(lModels);
+        self.updatePerfsForAllModels(self.mModelsByName);
         
         
 
 class cTraining_Arg:
     def __init__(self , name):
         self.mName = name;
         self.mInputDS = None;
@@ -229,31 +240,37 @@
 
 
 
 def run_transform_thread(arg):
     arg.mSigDec.train(arg.mInputDS, arg.mSplit, arg.mTime, arg.mSignal, arg.mHorizon, arg.mTransformation, arg.mDecompositionType);
     return arg;
 
-def run_finalize_training(arg):
-    (lSignal , sigdecs, lOptions) = arg
+def run_model_selection_one_signal(arg):
+    (lSignal , lPerfsByModel, lOptions) = arg
     lModelSelector = None
     if(lOptions.mVotingMethod is None):
         lModelSelector = tsleg.create_model_selector()
     else:
         lModelSelector = tsvote.create_model_selector(lOptions.mVotingMethod)
         
     lModelSelector.mOptions = lOptions
-    lModelSelector.collectPerformanceIndices_ModelSelection(lSignal, sigdecs)
+    lModelSelector.collectPerformanceIndices_ModelSelection(lSignal, lPerfsByModel)
     if(lOptions.mCrossValidationOptions.mMethod is not None):
         lModelSelector.perform_model_selection_cross_validation()
         
+    return (lSignal, lModelSelector.mBestModelName, lModelSelector.mTrPerfDetails, lModelSelector.mModelShortList)
+
+def run_finalize_training_one_signal(arg):
+    (lSignal , lBestModel) = arg
+
     # Prediction Intervals
-    lModelSelector.mBestModel.updateAllPerfs();
-    lModelSelector.mBestModel.computePredictionIntervals();
-    return (lSignal, lModelSelector.mPerfsByModel, lModelSelector.mBestModel, lModelSelector.mTrPerfDetails, lModelSelector.mModelShortList)
+    lBestModel.updateAllPerfs();
+    lBestModel.computePredictionIntervals();
+
+    return (lSignal, lBestModel)
 
 class cSignalDecompositionTrainer:
         
     def __init__(self):
         self.mSigDecBySplitAndTransform = {};
         self.mOptions = tsopts.cSignalDecomposition_Options();
         self.mExogenousData = None;
@@ -269,69 +286,102 @@
         return lSplits
 
 
     def train(self, iInputDS, iSplits, iTime, iSignals, iHorizon):
         
         self.train_all_transformations(iInputDS, iSplits, iTime, iSignals, iHorizon);
         
+        self.run_model_selection()
+        
         self.finalize_training()
         
         # self.cleanup_after_model_selection()
     
 
-    def finalize_training(self):
+    def run_model_selection(self):
 
         args = [];
+        lModelsByName = {}
         for (lSignal , sigdecs) in self.mSigDecBySplitAndTransform.items():
-            args = args + [(lSignal, sigdecs, self.mOptions)]
+            lPerfsByModel = {}
+            for (lName, sigdec) in sigdecs.items():
+                lModelsByName.update(sigdec.mModelsByName)
+                for (model , value) in sorted(sigdec.mPerfsByModel.items()):
+                    lPerfsByModel[model] = value
+            args = args + [(lSignal, lPerfsByModel, self.mOptions)]
 
         self.mPerfsByModel = {}
         self.mTrPerfDetails = {}
         self.mModelShortList = {}
         self.mBestModels = {}
         NCores = min(len(args) , self.mOptions.mNbCores) 
-        lTimer = tsutil.cTimer(("FINALIZE_TRAINING",
+        lTimer = tsutil.cTimer(("MODEL_SELECTION",
                                 {"Signals" : [lSignal for (lSignal , sigdecs) in self.mSigDecBySplitAndTransform.items()],
-                                 "Transformations" : [(lSignal, sorted(list(lSigDecs.keys()))) for (lSignal , lSigDecs) in self.mSigDecBySplitAndTransform.items()],
                                  "Cores" : NCores}))
         if(self.mOptions.mParallelMode and NCores > 1):
             from multiprocessing import Pool
             pool = Pool(NCores)
         
-            for res in pool.imap(run_finalize_training, args):
-                (lSignal, lPerfsByModel, lBestModel, lPerfDetails, lModelShortList) = res
+            for res in pool.imap(run_model_selection_one_signal, args):
+                (lSignal, lBestModelName, lPerfDetails, lModelShortList) = res
                 assert(self.mPerfsByModel.get(lSignal) is None)
                 self.mPerfsByModel[lSignal] = lPerfsByModel;
-                self.mBestModels[lSignal] = lBestModel
+                self.mBestModels[lSignal] = lModelsByName[lBestModelName]
                 self.mTrPerfDetails[lSignal] = lPerfDetails
                 self.mModelShortList[lSignal] = lModelShortList
             pool.close()
             pool.join()
+            del pool
         else:
             for arg in args:
-                res = run_finalize_training(arg)
-                (lSignal, lPerfsByModel, lBestModel, lPerfDetails, lModelShortList) = res
+                res = run_model_selection_one_signal(arg)
+                (lSignal, lBestModelName, lPerfDetails, lModelShortList) = res
                 assert(self.mPerfsByModel.get(lSignal) is None)
                 self.mPerfsByModel[lSignal] = lPerfsByModel;
-                self.mBestModels[lSignal] = lBestModel
+                self.mBestModels[lSignal] = lModelsByName[lBestModelName]
                 self.mTrPerfDetails[lSignal] = lPerfDetails
                 self.mModelShortList[lSignal] = lModelShortList
                 
         
+    def finalize_training(self):
+
+        args = [];
+        args = [(lSignal, lBestModel) for (lSignal, lBestModel) in self.mBestModels.items()]
+
+        NCores = min(len(args) , self.mOptions.mNbCores) 
+        lTimer = tsutil.cTimer(("FINALIZE_TRAINING",
+                                {"BestModels" : [(lSignal, lBestModel.mOutName) for (lSignal, lBestModel) in self.mBestModels.items()],
+                                 "Cores" : NCores}))
+        if(self.mOptions.mParallelMode and NCores > 1):
+            from multiprocessing import Pool
+            pool = Pool(NCores)
+        
+            for res in pool.imap(run_finalize_training_one_signal, args):
+                (lSignal, lBestModel) = res
+                self.mBestModels[lSignal] = lBestModel
+            pool.close()
+            pool.join()
+            del pool
+        else:
+            for arg in args:
+                res = run_finalize_training_one_signal(arg)
+                (lSignal, lBestModel) = res
+                self.mBestModels[lSignal] = lBestModel
+                
             
 
     def defineTransformations(self, iInputDS, iSplit, iTime, iSignal):
         lTransformationEstimator = tstransf.cTransformationEstimator()
         lTransformationEstimator.mOptions = self.mOptions
         lTransformationEstimator.defineTransformations(iInputDS, iTime, iSignal)
         self.mTransformList[(iSignal, iSplit)] = lTransformationEstimator.mTransformList
             
         
     def train_all_transformations(self , iInputDS, iSplits, iTimes, iSignals, iHorizons):
-        # print([transform1.mFormula for transform1 in self.mTransformList]);
+        # tsutil.print_pyaf_detailed_info([transform1.mFormula for transform1 in self.mTransformList]);
         args = [];
         for lSignal in iSignals:
             self.mSigDecBySplitAndTransform[lSignal] = {}
         lActiveDecompositionTypes = [decomp_type for (decomp_type, active_status) in self.mOptions.mActiveDecompositionTypes.items() if (active_status is True)]
         for lSplit in iSplits:
             for lSignal in iSignals:
                 self.defineTransformations(iInputDS, lSplit, iTimes[lSignal], lSignal);
@@ -364,14 +414,15 @@
             from multiprocessing import Pool
             pool = Pool(NCores)
             for res in pool.imap(run_transform_thread, args):
                 lSignal = res.mName[0]
                 self.mSigDecBySplitAndTransform[lSignal][res.mName] = res.mSigDec;
             pool.close()
             pool.join()
+            del pool
         else:
             for arg in args:
                 res = run_transform_thread(arg)
                 lSignal = res.mName[0]
                 self.mSigDecBySplitAndTransform[lSignal][res.mName] = res.mSigDec;
             
     def cleanup_after_model_selection(self):
```

## pyaf/TS/SignalDecomposition_Trend.py

```diff
@@ -24,39 +24,37 @@
         self.mTrendFrame = None
         self.mTrendPerf = tsperf.cPerf();
         self.mOutName = None
         self.mFormula = None;
         self.mComplexity = tscomplex.eModelComplexity.High;
 
     def check_not_nan(self, sig , name):
-        #print("check_not_nan");
+        # tsutil.print_pyaf_detailed_info("check_not_nan");
         if(np.isnan(sig[:-1]).any() or np.isinf(sig[:-1]).any() ):
             logger = tsutil.get_pyaf_logger();
             logger.error("TREND_RESIDUE_WITH_NAN_IN_SIGNAL" + str(sig));
             raise tsutil.Internal_PyAF_Error("INVALID_COLUMN _FOR_TREND_RESIDUE ['"  + name + "'");
         pass
 
 
     def computePerf(self):
         if(self.mOptions.mDebug):
             self.check_not_nan(self.mTrendFrame[self.mOutName + '_residue'], self.mOutName + '_residue')
         # self.mTrendFrame.to_csv(self.mOutName + '_residue' + ".csv");
 
-        self.mTrendFitPerf = tsperf.cPerf();
-        self.mTrendForecastPerf = tsperf.cPerf();
-        (lFrameFit, lFrameForecast, lFrameTest) = self.mSplit.cutFrame(self.mTrendFrame);
-        self.mTrendFitPerf.computeCriterionValues(lFrameFit[self.mSignal] ,
-                                                  lFrameFit[self.mOutName],
-                                                  [self.mTimeInfo.mOptions.mModelSelection_Criterion],
-                                                  self.mOutName)
-        self.mTrendForecastPerf.computeCriterionValues(lFrameForecast[self.mSignal] ,
-                                                       lFrameForecast[self.mOutName],
-                                                       [self.mTimeInfo.mOptions.mModelSelection_Criterion],
-                                                       self.mOutName)
-
+        self.mTrendPerfs = {}
+        lCutting = self.mSplit.cutFrame(self.mTrendFrame);
+        for(lDataset , lDF) in lCutting.items():
+            lPerf = tsperf.cPerf();
+            lPerf.computeCriterionValues(lDF[self.mSignal] ,
+                                         lDF[self.mOutName],
+                                         [self.mTimeInfo.mOptions.mModelSelection_Criterion],
+                                         self.mOutName + "_" + str(lDataset))
+            self.mTrendPerfs[lDataset] = lPerf
+            
 
     def compute_trend_residue(self, df):
         target = df[self.mSignal]
         lTrend = df[self.mOutName]
         if(self.mDecompositionType in ['T+S+R']):
             df[self.mOutName + '_residue'] = target - lTrend
         else:
@@ -66,15 +64,16 @@
 
     def addTrendInputVariables(self):
         self.mTime = self.mTimeInfo.mTime;
         self.mSignal = self.mTimeInfo.mSignal;
         self.mOutName = self.mSignal + "_" + self.mOutName;
         self.mTrendFrame = pd.DataFrame(index = self.mTimeInfo.mSignalFrame.index)
         self.mTimeInfo.addVars(self.mTrendFrame);
-
+        self.mTrendFrame[self.mSignal] = self.mSignalFrame[self.mSignal]
+        
     def fit(self):
         self.fit_specific()
         self.mTrendFrame[self.mOutName] = self.compute(self.mTrendFrame)
         self.compute_trend_residue(self.mTrendFrame)
 
     def transformDataset(self, df):
         df[self.mOutName] = self.compute(df)
@@ -109,18 +108,18 @@
         cAbstractTrend.__init__(self);
         self.mDefaultValue = None
         self.mOutName = "Lag1Trend"
         self.mFormula = self.mOutName;
         self.mComplexity = tscomplex.eModelComplexity.Low;
         
     def replaceFirstMissingValue(self, df, series):
-        # print(self.mDefaultValue, type(self.mDefaultValue));
+        # tsutil.print_pyaf_detailed_info(self.mDefaultValue, type(self.mDefaultValue));
         # Be explicit here .... some integer index does not work.
         df.loc[df.index[0] , series] = self.mDefaultValue;
-        # print(df.head());
+        # tsutil.print_pyaf_detailed_info(df.head());
         
     def fit_specific(self):
         lEstim = self.mSplit.getEstimPart(self.mTrendFrame);
         self.mDefaultValue = lEstim[self.mSignal ].iloc[0]        
 
     def compute(self, df):
         Y_pred = df[self.mSignal].shift(1)
@@ -134,18 +133,18 @@
 class cMovingAverageTrend(cAbstractTrend):
     def __init__(self, iWindow):
         cAbstractTrend.__init__(self);
         self.mOutName = "MovingAverage";
         self.mWindow = iWindow;
         self.mFormula = self.mOutName;
         self.mComplexity = tscomplex.eModelComplexity.Medium;
-        
-    def fit_specific(self):
         self.mOutName = self.mOutName + "(" + str(self.mWindow) + ")";
         self.mFormula = self.mOutName;
+        
+    def fit_specific(self):
         self.mMean = self.mSplit.getEstimPart(self.mTrendFrame)[self.mSignal].mean()
 
 
     def compute(self, df):
         Y_pred = df[self.mSignal].shift(1).rolling(self.mWindow).mean().fillna(method='bfill');
         Y_pred.fillna(self.mMean , inplace=True)
         return Y_pred
@@ -157,18 +156,18 @@
 class cMovingMedianTrend(cAbstractTrend):
     def __init__(self, iWindow):
         cAbstractTrend.__init__(self);
         self.mOutName = "MovingMedian";
         self.mWindow = iWindow;
         self.mFormula = self.mOutName;
         self.mComplexity = tscomplex.eModelComplexity.High;
-        
-    def fit_specific(self):
         self.mOutName = self.mOutName + "(" + str(self.mWindow) + ")";
         self.mFormula = self.mOutName;
+        
+    def fit_specific(self):
         self.mMean = self.mSplit.getEstimPart(self.mTrendFrame)[self.mSignal].mean()
 
 
     def compute(self, df):
         Y_pred = df[self.mSignal].shift(1).rolling(self.mWindow).median().fillna(method='bfill');
         Y_pred.fillna(self.mMean , inplace=True)
         return Y_pred
@@ -260,45 +259,40 @@
         N = self.mSignalFrame.shape[0];
         
         if(N > 1 and self.mOptions.mActiveTrends['LinearTrend']):
             self.mTrendList = self.mTrendList + [cLinearTrend()]
 
         if(N > 2 and self.mOptions.mActiveTrends['PolyTrend']):
             self.mTrendList = self.mTrendList + [cPolyTrend()]
-                
+
+        lWindows = self.mTimeInfo.get_moving_window_lengths_for_time_resolution()
         if(N > 2 and self.mOptions.mActiveTrends['MovingAverage']):
-            for i in self.mOptions.mMovingAverageLengths:
-                if(self.needMovingTrend(self.mSignalFrame , i)):
-                    self.mTrendList = self.mTrendList + [cMovingAverageTrend(i)]
+            for lLength in lWindows:
+                if(self.needMovingTrend(self.mSignalFrame , lLength)):
+                    self.mTrendList = self.mTrendList + [cMovingAverageTrend(lLength)]
 
         if(N > 2 and self.mOptions.mActiveTrends['MovingMedian']):
-            for i in self.mOptions.mMovingMedianLengths:
-                if(self.needMovingTrend(self.mSignalFrame , i)):
-                    self.mTrendList = self.mTrendList + [cMovingMedianTrend(i)]
+            for lLength in lWindows:
+                if(self.needMovingTrend(self.mSignalFrame , lLength)):
+                    self.mTrendList = self.mTrendList + [cMovingMedianTrend(lLength)]
         if(len(self.mTrendList) == 0):
             self.mTrendList = [cConstantTrend()];
             
-        # logger = tsutil.get_pyaf_logger();
-        # logger.info("ACTIVE_TRENDS" + str(self.mOptions.mActiveTrends));
-        # logger.info("TRENDS" + str([tr.mOutName for tr in self.mTrendList]));
+        # tsutil.print_pyaf_detailed_info("ACTIVE_TRENDS" + str(self.mOptions.mActiveTrends));
+        # tsutil.print_pyaf_detailed_info("TRENDS" + str([tr.mOutName for tr in self.mTrendList]));
 
 
         
     def plotTrend(self):
         for trend in self.mTrendList:
             tsplot.decomp_plot(self.mTrendFrame, self.mTimeInfo.mNormalizedTimeColumn, self.mSignal, trend.mOutName , trend.mOutName + '_residue', horizon = self.mTimeInfo.mHorizon);
             
 
-    def addTrendInputVariables(self):
-        for trend in self.mTrendList:
-            trend.addTrendInputVariables()
-        pass
-
     def check_residue(self , trend, sig, name):
-        # print("check_trend_residue ", (name, trend.mDecompositionType, sig.min(), sig.max(), sig.mean(), sig .std()))
+        # tsutil.print_pyaf_detailed_info("check_trend_residue ", (name, trend.mDecompositionType, sig.min(), sig.max(), sig.mean(), sig .std()))
         if(np.isnan(sig).any()):
             raise tsutil.Internal_PyAF_Error("Invalid residue_is_nan '" +
                                              str((name, trend.mDecompositionType, sig.min(), sig.max(), sig.mean(), sig .std())) + "'");
         if(sig.max() > 1.e5):
             raise tsutil.Internal_PyAF_Error("Invalid residue_too_large '" +
                                              str((name, trend.mDecompositionType, sig.min(), sig.max(), sig.mean(), sig .std())) + "'");
         pass
@@ -307,18 +301,20 @@
         lTimer = None
         if(self.mOptions.mDebugProfile):
             lTimer = tsutil.cTimer(("TRAINING_TRENDS", {"Signal" : self.mTimeInfo.mSignal}))
         self.mTime = self.mTimeInfo.mTime;
         self.mSignal = self.mTimeInfo.mSignal;
         self.mTrendFrame = pd.DataFrame(index = self.mSignalFrame.index)
         self.mTimeInfo.addVars(self.mTrendFrame);
+        self.mTrendFrame[self.mSignal] = self.mSignalFrame[self.mSignal]
         for trend in self.mTrendList:
             trend.mOptions = self.mOptions
             trend.mDecompositionType = self.mDecompositionType
             trend.mTrendFrame = self.mTrendFrame.copy()
+            trend.addTrendInputVariables();
             trend.fit();
             if(trend.mOptions.mDebugPerformance):
                 trend.computePerf();
             self.mTrendFrame[trend.mOutName] = trend.mTrendFrame[trend.mOutName]
             self.mTrendFrame[trend.mOutName + "_residue"] = trend.mTrendFrame[trend.mOutName + "_residue"]
             if(self.mOptions.mDebug):
                 self.check_residue(trend, self.mTrendFrame[trend.mOutName + "_residue"].values[:-1],
@@ -327,11 +323,10 @@
 
     def estimateTrend(self):
         self.defineTrends();
         for trend in self.mTrendList:
             trend.mSignalFrame = self.mSignalFrame;
             trend.mTimeInfo = self.mTimeInfo;            
             trend.mSplit = self.mSplit
-        self.addTrendInputVariables();
         self.estimateTrends()
         for trend in self.mTrendList:
             del trend.mTrendFrame
```

## pyaf/TS/SignalHierarchy.py

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 
 from .. import ForecastEngine as autof
 from . import Options as tsopts
 from . import Perf as tsperf
 from . import Utils as tsutil
 from . import Plots as tsplot
+from . import TimeSeries_Cutting as tscut
 
 import copy
 
 class cSignalHierarchy:
 
     def __init__(self):
         self.mHierarchy = None;
@@ -58,14 +59,16 @@
         lDict["Training_Time"] = self.mTrainingTime
         return lDict;
 
     def discard_nans_in_aggregate_signals(self):
         return False
     
     def create_HierarchicalStructure(self):
+        logger = tsutil.get_pyaf_hierarchical_logger();
+        logger.info("CREATE_HIERARCHICAL_STRUCTURE_START");
         self.mLevels = self.mHierarchy['Levels'];
         self.mStructure = {};
         df = self.mHierarchy['Data'];
         lLevelCount = len(self.mLevels);
         for level in range(lLevelCount):
             self.mStructure[level] = {};
         for row in range(df.shape[0]):
@@ -77,15 +80,16 @@
                     col1 = df[df.columns[level - 1]][row];
                     self.mStructure[level][col].add(col1);
         # Stabilize the order of nodes
         for level in  sorted(self.mStructure.keys()):
             for col in sorted(self.mStructure[level].keys()):
                 self.mStructure[level][col] = sorted(self.mStructure[level][col])
                     
-        # print(self.mStructure);
+        # tsutil.print_pyaf_detailed_info(self.mStructure);
+        logger.info("CREATE_HIERARCHICAL_STRUCTURE_END");
         pass
     
     def create_SummingMatrix(self):
         lNbNodes = sum([len(self.mStructure[level]) for level in self.mStructure.keys()]);
         lBaseLevelCount = len(self.mStructure[0]);
         lIndices = {};
         self.mSummingMatrix = np.zeros((lNbNodes, lBaseLevelCount));
@@ -99,64 +103,67 @@
                         for j in range(lBaseLevelCount):
                             self.mSummingMatrix[ i ][j] = self.mSummingMatrix[ ii ][j]  + self.mSummingMatrix[ i ][j];
             else:
                 for col in sorted(self.mStructure[level].keys()):
                     lNew_index = len(lIndices);
                     lIndices[ col ] = lNew_index;
                     self.mSummingMatrix[ lNew_index ] [ lNew_index ] = 1;
-        # print(self.mSummingMatrix);
+        # tsutil.print_pyaf_detailed_info(self.mSummingMatrix);
         self.mSummingMatrixInverse = np.linalg.pinv(self.mSummingMatrix);
-        # print(self.mSummingMatrixInverse);
+        # tsutil.print_pyaf_detailed_info(self.mSummingMatrixInverse);
 
     def checkData(self , df):
         if(self.mHorizon != int(self.mHorizon)):
             raise tsutil.PyAF_Error("PYAF_ERROR_NON_INTEGER_HORIZON " + str(self.mHorizon));
         if(self.mHorizon < 1):
             raise tsutil.PyAF_Error("PYAF_ERROR_NEGATIVE_OR_NULL_HORIZON " + str(self.mHorizon));
         if(self.mDateColumn not in df.columns):
             raise tsutil.PyAF_Error("PYAF_ERROR_HIERARCHY_TIME_COLUMN_NOT_FOUND " + str(self.mDateColumn));
         type1 = df[self.mDateColumn].dtype
-        # print(type1)
+        # tsutil.print_pyaf_detailed_info(type1)
         if(type1.kind != 'M' and type1.kind != 'i' and type1.kind != 'u' and type1.kind != 'f'):
             raise tsutil.PyAF_Error("PYAF_ERROR_TIME_COLUMN_TYPE_NOT_ALLOWED '" + str(self.mDateColumn) + "' '" + str(type1) + "'");
         # level 0 is the original/physical columns
         for k in self.mStructure[0]:
             if(k not in df.columns) :
                 raise tsutil.PyAF_Error("PYAF_ERROR_HIERARCHY_BASE_COLUMN_NOT_FOUND " + str(k));
-            # print(type2)
+            # tsutil.print_pyaf_detailed_info(type2)
             type2 = df[k].dtype
             if(type2.kind != 'i' and type2.kind != 'u' and type2.kind != 'f'):
                 raise tsutil.PyAF_Error("PYAF_ERROR_HIERARCHY_BASE_SIGNAL_COLUMN_TYPE_NOT_ALLOWED '" + str(k) + "' '" + str(type2) + "'");
 
 
     def create_all_levels_dataset(self, df):
+        logger = tsutil.get_pyaf_hierarchical_logger();
+        logger.info("CREATE_ALL_LEVELS_DATASET_START");
         self.checkData(df);
         lAllLevelsDataset = df.copy();
         lMapped = True;
         # level 0 is the original/physical columns
         for k in self.mStructure[0]:
             if(k not in df.columns) :
                 lMapped = False;
         if(not lMapped):
             i = 0;
             for k in self.mStructure[0]:
-                print("MAPPING_ORIGINAL_COLUMN" , df.columns[i + 1], "=>" , k)
+                tsutil.print_pyaf_detailed_info("MAPPING_ORIGINAL_COLUMN" , df.columns[i + 1], "=>" , k)
                 lAllLevelsDataset[k] = df[df.columns[i + 1]];
                 i = i + 1;
                 
         for level in  sorted(self.mStructure.keys()):
             if(level > 0):
                 for col in sorted(self.mStructure[level].keys()):
                     new_col = None;
                     for col1 in sorted(self.mStructure[level][col]):
                         if(new_col is None):
                             new_col = lAllLevelsDataset[col1];
                         else:
                             new_col = new_col + lAllLevelsDataset[col1];
                     lAllLevelsDataset[col] = new_col;
+        logger.info("CREATE_ALL_LEVELS_DATASET_END");
         return lAllLevelsDataset;
 
 
     def addVars(self, df):
         lAllLevelsDataset = self.create_all_levels_dataset(df);
         return lAllLevelsDataset;
 
@@ -170,14 +177,15 @@
 
     def get_horizon(self, level, signal):
         # only for temporal hierarchies
         return self.mHorizon
 
     def create_all_levels_models_with_one_engine(self, iAllLevelsDataset, H, iDateColumn):
         logger = tsutil.get_pyaf_hierarchical_logger();
+        logger.info("CREATE_ALL_LEVELS_MODELS_WITH_ONE_ENGINE_START");
         lSignals = []
         lDateColumns = {}
         lExogenousData = {}
         lHorizons = {}
         lDiscardNulls = {}
         for level in sorted(self.mStructure.keys()):
             for signal in sorted(self.mStructure[level].keys()):
@@ -193,28 +201,33 @@
             lEngine.mOptions.mMissingDataOptions.mTimeMissingDataImputation = "DiscardRow"
             lEngine.mOptions.mMissingDataOptions.mSignalMissingDataImputation = "DiscardRow"
             # Sampling is not compatible with Temporal Hierarchies (#163)
             lEngine.mOptions.mActivateSampling = False
         assert(iAllLevelsDataset.shape[0] > 0)
         lEngine.train(iAllLevelsDataset, lDateColumns , lSignals, lHorizons, iExogenousData = lExogenousData);
         self.mModels = lEngine
-        # print("CREATED_MODELS", self.mLevels, self.mModels)
+        # tsutil.print_pyaf_detailed_info("CREATED_MODELS", self.mLevels, self.mModels)
+        logger.info("CREATE_ALL_LEVELS_MODELS_WITH_ONE_ENGINE_END");
 
 
     def fit(self):
+        logger = tsutil.get_pyaf_hierarchical_logger();
+        logger.info("TRAINING_HIERARCHICAL_MODEL_START");
         lTimer = tsutil.cTimer(("HIERARCHICAL_TRAINING"))
+        self.check_combination_methods()
         self.create_HierarchicalStructure();
         # self.plot();
         self.create_SummingMatrix();
         lAllLevelsDataset = self.create_all_levels_dataset(self.mTrainingDataset);
         self.create_all_levels_models_with_one_engine(lAllLevelsDataset, self.mHorizon, self.mDateColumn);
         self.computeTopDownHistoricalProportions(lAllLevelsDataset);
         lForecast_DF = self.internal_forecast(self.mTrainingDataset , self.mHorizon)
         self.computePerfOnCombinedForecasts(lForecast_DF.head(lForecast_DF.shape[0] - self.mHorizon));
         self.mTrainingTime = lTimer.get_elapsed_time()
+        logger.info("TRAINING_HIERARCHICAL_MODEL_END " + str(self.mTrainingTime));
 
 
     def getModelInfo(self):
         lEngine = self.mModels
         lEngine.getModelInfo();
 
 
@@ -223,18 +236,19 @@
         lHasModels = (self.mModels is not None)
         if(lHasModels):
             lPrefixes = self.get_reconciled_forecast_prefixes()
             lAnnotations = {};
             for level in sorted(self.mStructure.keys()):
                 for signal in sorted(self.mStructure[level].keys()):
                     lEngine = self.mModels
-                    lMAPE = 'MAPE = %.4f' % self.mValidPerfs[str(signal) + "_Forecast"].mMAPE
+                    lValidPerfs = self.mPerformances[signal][tscut.eDatasetType.Forecast]
+                    lMAPE = 'MAPE = %.4f' % lValidPerfs[str(signal) + "_Forecast"].mMAPE
                     lReconciledMAPEs = [ ]
                     for lPrefix in lPrefixes:
-                        lMAPE_Rec = self.mValidPerfs[str(signal) + "_" + lPrefix + "_Forecast"].mMAPE
+                        lMAPE_Rec = lValidPerfs[str(signal) + "_" + lPrefix + "_Forecast"].mMAPE
                         lReconciledMAPEs.append('MAPE_' + lPrefix + ' = %.4f' % lMAPE_Rec);
                     lAnnotations[signal] = [signal , lMAPE ] + lReconciledMAPEs;
                     for col1 in sorted(self.mStructure[level][signal]):
                         lProp = self.mAvgHistProp[signal][col1] * 100;
                         lAnnotations[str(signal) +"_" + col1] = ('%2.2f %%' % lProp)
         return lAnnotations
 
@@ -248,15 +262,15 @@
         lAnnotations = self.get_plot_annotations()
         lBase64 = tsplot.plot_hierarchy_as_png_base64(self.mStructure, lAnnotations, name)
         return lBase64
     
     def standardPlots(self , name = None):
         lEngine = self.mModels
         lEngine.standardPlots(name + "_Hierarchy_Level_Signal_");
-        self.plot(name + "_Hierarchical_Structure.png")
+        self.plot(name + "_Hierarchical_Structure")
 
     def getPlotsAsDict(self):
         lDict = {}
         lDict["Models"] = self.mModels.getPlotsAsDict()
         lDict["Hierarchical_Structure"] = self.plot_as_png_base64()
         return lDict
     
@@ -304,27 +318,27 @@
             if(level > 0):
                 for col in sorted(self.mStructure[level].keys()):
                     self.mAvgHistProp[col] = {};
                     self.mPropHistAvg[col] = {};
                     for col1 in sorted(self.mStructure[level][col]):
                         self.mAvgHistProp[col][col1] = (lEstim[col1] / lEstim[col]).mean();
                         self.mPropHistAvg[col][col1] = lEstim[col1].mean() / lEstim[col].mean();
-        # print("AvgHitProp\n", self.mAvgHistProp);
-        # print("PropHistAvg\n", self.mPropHistAvg);
+        # tsutil.print_pyaf_detailed_info("AvgHitProp\n", self.mAvgHistProp);
+        # tsutil.print_pyaf_detailed_info("PropHistAvg\n", self.mPropHistAvg);
         pass
         
     def computeTopDownForecastedProportions(self, iForecast_DF):
         self.mForecastedProp = {};
         for level in  sorted(self.mStructure.keys()):
             if(level > 0):
                 for col in sorted(self.mStructure[level].keys()):
                     self.mForecastedProp[col] = {};
                     for col1 in sorted(self.mStructure[level][col]):
                         self.mForecastedProp[col][col1] = (iForecast_DF[col1] / iForecast_DF[col]).mean();
-        # print("ForecastedProp\n", self.mForecastedProp);
+        # tsutil.print_pyaf_detailed_info("ForecastedProp\n", self.mForecastedProp);
         pass
 
     def computeBottomUpForecast(self, iForecast_DF, level, signal, iPrefix = "BU"):
         new_BU_forecast = None;
         for col1 in sorted(self.mStructure[level][signal]):
             if(new_BU_forecast is None):
                 new_BU_forecast = iForecast_DF[col1 + "_Forecast"];
@@ -334,116 +348,126 @@
             new_BU_forecast = iForecast_DF[str(signal) + "_Forecast"];
         return new_BU_forecast;
 
     def computeBottomUpForecasts(self, iForecast_DF):
         logger = tsutil.get_pyaf_hierarchical_logger();
         logger.info("FORECASTING_HIERARCHICAL_MODEL_BOTTOM_UP_METHOD " + "BU");
         lForecast_DF_BU = iForecast_DF.copy()
-        # print("STRUCTURE " , self.mStructure.keys());
+        # tsutil.print_pyaf_detailed_info("STRUCTURE " , self.mStructure.keys());
         for level in sorted(self.mStructure.keys()):
             for signal in sorted(self.mStructure[level].keys()):
                 new_BU_forecast = self.computeBottomUpForecast(lForecast_DF_BU, level, signal);
                 lForecast_DF_BU[str(signal) + "_BU_Forecast"] = new_BU_forecast;
             
-        # print(lForecast_DF_BU.head());
-        # print(lForecast_DF_BU.tail());
+        # tsutil.print_pyaf_detailed_info(lForecast_DF_BU.head());
+        # tsutil.print_pyaf_detailed_info(lForecast_DF_BU.tail());
 
         return lForecast_DF_BU;
 
     def get_clean_signal_and_forecasts(self, iForecast_DF, signal, iPrefixes):
         lEngine = self.mModels
         lForecasts = [str(signal) + "_Forecast"]
         lForecasts = lForecasts + [str(signal) + "_" + lPrefix + "_Forecast" for lPrefix in iPrefixes]
         lColumns = [lEngine.mSignalDecomposition.mDateColumns[signal] , signal ] + lForecasts
         lForecast_DF = iForecast_DF[lColumns]
         return lForecast_DF
 
+    def check_combination_methods(self):
+        lCombinationMethods = self.mOptions.mHierarchicalCombinationMethod;
+        if type(lCombinationMethods) is not list:
+            lCombinationMethods = [lCombinationMethods];
+        for lMethod in lCombinationMethods:
+            if(not lMethod in ["BU" , 'TD' , 'MO' , 'OC']):
+                raise tsutil.PyAF_Error("PYAF_ERROR_HIERARCHY_UNKNOWN_RECONCILIATION_METHOD '" + str(lMethod) + "'");
+
+
+    
     def get_reconciled_forecast_prefixes(self):
         lCombinationMethods = self.mOptions.mHierarchicalCombinationMethod;
         if type(lCombinationMethods) is not list:
             lCombinationMethods = [lCombinationMethods];
         lPrefixes = [lPrefix for lPrefix in lCombinationMethods if (lPrefix != 'TD')];
         if('TD' in lCombinationMethods):
             lPrefixes = lPrefixes + ['AHP_TD', 'PHA_TD'];
         return lPrefixes
 
+    def computePerfOnCombinedForecasts_one_node(self, iForecast_DF, iPrefixes, signal):
+        logger = tsutil.get_pyaf_hierarchical_logger();
+        lForecast_DF = self.get_clean_signal_and_forecasts(iForecast_DF, signal, iPrefixes)
+        lColumns = [signal , str(signal) + "_Forecast"] + [str(signal) + "_" + lPrefix + "_Forecast" for lPrefix in iPrefixes]
+        lEngine = self.mModels
+        self.mPerformances[signal] = {}
+        lSplit = lEngine.mSignalDecomposition.mBestModel.mTimeInfo.mSplit
+        forecast_cut_dfs = lSplit.cutFrame(lForecast_DF);
+        for (lDataset, lDF) in forecast_cut_dfs.items():
+            self.mPerformances[signal][lDataset] = {}
+            lDF1 = lDF[lColumns]
+            if(self.discard_nans_in_aggregate_signals()):
+                lDF1 = lDF1.dropna()
+            lPerf = lEngine.computePerf(lDF1[signal], lDF1[str(signal) + "_Forecast"], signal)
+            self.mPerformances[signal][lDataset][str(signal) + "_Forecast"] = lPerf
+            for lPrefix in iPrefixes:
+                lName = str(signal) + "_" + lPrefix + "_Forecast"
+                lPerf_Combined = lEngine.computePerf(lDF1[signal], lDF1[lName], lName)
+                self.mPerformances[signal][lDataset][lName] = lPerf_Combined
+            for (sig , perf) in sorted(self.mPerformances[signal][lDataset].items()):
+                logger.info("REPORT_COMBINED_FORECASTS_PERF "  + str((lDataset.name, sig)) + " " + str(perf.to_dict()))
+        
     def computePerfOnCombinedForecasts(self, iForecast_DF):
         logger = tsutil.get_pyaf_hierarchical_logger();
         logger.info("FORECASTING_HIERARCHICAL_MODEL_OPTIMAL_COMBINATION_METHOD");
         lEngine = self.mModels
         lPrefixes = self.get_reconciled_forecast_prefixes()
         
-        self.mEstimPerfs = {}
-        self.mValidPerfs = {}
-        lPerfs = {};
+        self.mPerformances = {}
+        for lDataset in self.mPerformances.keys():
+            self.mPerformances[lDataset]["local"] = {} 
+            for lPrefix in lPrefixes:
+                self.mPerformances[lPrefix] = {}
         logger.info("STRUCTURE " + str(sorted(list(self.mStructure.keys()))));
         logger.info("DATASET_COLUMNS "  + str(iForecast_DF.columns));
         for level in sorted(self.mStructure.keys()):
             logger.info("STRUCTURE_LEVEL " + str((level, sorted(list(self.mStructure[level].keys())))));
             for signal in sorted(self.mStructure[level].keys()):
-                lForecast_DF = self.get_clean_signal_and_forecasts(iForecast_DF, signal, lPrefixes)                
-                lFrameFit = self.getEstimPart(lForecast_DF);
-                lFrameValid = self.getValidPart(lForecast_DF);
-                lColumns = [signal , str(signal) + "_Forecast"] + [str(signal) + "_" + lPrefix + "_Forecast" for lPrefix in lPrefixes]
-                lFrameFit = lFrameFit[lColumns]
-                lFrameValid = lFrameValid[lColumns]
-                if(self.discard_nans_in_aggregate_signals()):
-                    lFrameFit = lFrameFit.dropna()
-                    lFrameValid = lFrameValid.dropna()
-                lPerfFit = lEngine.computePerf(lFrameFit[signal], lFrameFit[str(signal) + "_Forecast"], signal)
-                lPerfValid = lEngine.computePerf(lFrameValid[signal], lFrameValid[str(signal) + "_Forecast"], signal)
-                self.mEstimPerfs[str(signal) + "_Forecast"] = lPerfFit
-                self.mValidPerfs[str(signal) + "_Forecast"] = lPerfValid
-                for iPrefix in lPrefixes:
-                    lName = str(signal) + "_" + iPrefix + "_Forecast"
-                    lPerfFit_Combined = lEngine.computePerf(lFrameFit[signal], lFrameFit[lName], lName)
-                    lPerfValid_Combined = lEngine.computePerf(lFrameValid[signal], lFrameValid[lName], lName)
-                    lPerfs[str(signal) + "_" + iPrefix] = (lPerfFit , lPerfValid, lPerfFit_Combined, lPerfValid_Combined);
-                    self.mEstimPerfs[lName] = lPerfFit_Combined
-                    self.mValidPerfs[lName] = lPerfValid_Combined
+                self.computePerfOnCombinedForecasts_one_node(iForecast_DF, lPrefixes, signal)
                                 
-        for (sig , perf) in sorted(lPerfs.items()):
-            logger.info("REPORT_COMBINED_FORECASTS_FIT_PERF "  + str(perf[2].to_dict()))
-            logger.info("REPORT_COMBINED_FORECASTS_VALID_PERF " + str(perf[3].to_dict()))
-        return lPerfs;
-
 
     def computeTopDownForecasts(self, iForecast_DF , iProp , iPrefix):
         logger = tsutil.get_pyaf_hierarchical_logger();
         logger.info("FORECASTING_HIERARCHICAL_MODEL_TOP_DOWN_METHOD " + iPrefix);
         lForecast_DF_TD = iForecast_DF.copy()
         lLevelsReversed = sorted(self.mStructure.keys(), reverse=True);
-        # print("TOPDOWN_STRUCTURE", self.mStructure)
-        # print("TOPDOWN_LEVELS", lLevelsReversed)
+        # tsutil.print_pyaf_detailed_info("TOPDOWN_STRUCTURE", self.mStructure)
+        # tsutil.print_pyaf_detailed_info("TOPDOWN_LEVELS", lLevelsReversed)
         # highest levels (fully aggregated)
         lHighestLevel = lLevelsReversed[0];
         for signal in sorted(self.mStructure[lHighestLevel].keys()):
             lForecast_DF_TD[str(signal) +"_" + iPrefix + "_Forecast"] =  iForecast_DF[str(signal) + "_Forecast"];
         for level in lLevelsReversed:
             for signal in sorted(self.mStructure[level].keys()):
                 for col in sorted(self.mStructure[level][signal]):
                     new_TD_forecast = lForecast_DF_TD[str(signal) + "_" + iPrefix + "_Forecast"] * iProp[signal][col];
                     lForecast_DF_TD[str(col) +"_" + iPrefix + "_Forecast"] = new_TD_forecast;
         
-        # print(lForecast_DF_TD.head());
-        # print(lForecast_DF_TD.tail());
+        # tsutil.print_pyaf_detailed_info(lForecast_DF_TD.head());
+        # tsutil.print_pyaf_detailed_info(lForecast_DF_TD.tail());
 
         return lForecast_DF_TD;
 
     def computeMiddleOutForecasts(self, iForecast_DF , iProp, iPrefix):
         logger = tsutil.get_pyaf_hierarchical_logger();
         logger.info("FORECASTING_HIERARCHICAL_MODEL_MIDDLE_OUT_METHOD " + iPrefix);
         lLevels = self.mStructure.keys();
         lMidLevel = len(lLevels) // 2;
         lForecast_DF_MO = iForecast_DF.copy()
         # lower levels .... top-down starting from the middle.
         levels_below = sorted([level for level in self.mStructure.keys()  if (level <= lMidLevel) ],
                               reverse=True);
-        # print("MIDDLE_OUT_STRUCTURE", self.mStructure)
-        # print("MIDDLE_OUT_LEVELS", levels_below)
+        # tsutil.print_pyaf_detailed_info("MIDDLE_OUT_STRUCTURE", self.mStructure)
+        # tsutil.print_pyaf_detailed_info("MIDDLE_OUT_LEVELS", levels_below)
         # mid-lewvel : do nothing ????
         for signal in sorted(self.mStructure[lMidLevel].keys()):
             lForecast_DF_MO[str(signal) +"_" + iPrefix + "_Forecast"] = iForecast_DF[str(signal) + "_Forecast"];
         # 
         for level in levels_below:
             for signal in sorted(self.mStructure[level].keys()):
                 for col in sorted(self.mStructure[level][signal]):
@@ -451,16 +475,16 @@
                     lForecast_DF_MO[str(col) +"_" + iPrefix + "_Forecast"] = new_MO_forecast;
         # higher levels .... bottom-up starting from the middle
         for level in range(lMidLevel + 1 , len(self.mStructure.keys())):
             for signal in sorted(self.mStructure[level].keys()):
                 new_MO_forecast = self.computeBottomUpForecast(lForecast_DF_MO, level, signal, iPrefix);
                 lForecast_DF_MO[str(signal) + "_" + iPrefix + "_Forecast"] = new_MO_forecast;
 
-        # print(lForecast_DF_MO.head());
-        # print(lForecast_DF_MO.tail());
+        # tsutil.print_pyaf_detailed_info(lForecast_DF_MO.head());
+        # tsutil.print_pyaf_detailed_info(lForecast_DF_MO.tail());
 
         return lForecast_DF_MO;
 
 
     def computeOptimalCombination(self, iForecast_DF):
         logger = tsutil.get_pyaf_hierarchical_logger();
         logger.info("FORECASTING_HIERARCHICAL_MODEL_OPTIMAL_COMBINATION_METHOD " + "OC");
@@ -468,37 +492,38 @@
         for level in  sorted(self.mStructure.keys()):
             for col in sorted(self.mStructure[level].keys()):
                 lBaseNames.append(col);
         lBaseForecastNames = [str(col) + "_Forecast" for col in lBaseNames]
         lBaseForecasts = iForecast_DF[lBaseForecastNames];
         # TODO : use linalg.solve here
         S = self.mSummingMatrix;
-        # print(S.shape);
+        # tsutil.print_pyaf_detailed_info(S.shape);
         lInv = np.linalg.inv(S.T.dot(S))
         lOptimalForecasts = S.dot(lInv).dot(S.T).dot(lBaseForecasts.values.T)
-        # print(lBaseForecasts.shape);
-        # print(lOptimalForecasts.shape);
+        # tsutil.print_pyaf_detailed_info(lBaseForecasts.shape);
+        # tsutil.print_pyaf_detailed_info(lOptimalForecasts.shape);
         lOptimalNames = [(str(col) + "_OC_Forecast") for col in lBaseNames];
         df = pd.DataFrame(lOptimalForecasts.T);
         df.columns = lOptimalNames;
         lForecast_DF_OC = pd.concat([iForecast_DF , df] , axis = 1);
         
-        # print(lForecast_DF_OC.head());
-        # print(lForecast_DF_OC.tail());
+        # tsutil.print_pyaf_detailed_info(lForecast_DF_OC.head());
+        # tsutil.print_pyaf_detailed_info(lForecast_DF_OC.tail());
         return lForecast_DF_OC;
 
     def internal_forecast(self , iInputDS, iHorizon):
 
         lAllLevelsDataset = self.create_all_levels_dataset(iInputDS);
         lForecast_DF = self.forecastAllModels_with_one_engine(lAllLevelsDataset, iHorizon, self.mDateColumn);
         lCombinationMethods = self.mOptions.mHierarchicalCombinationMethod;
         if type(lCombinationMethods) is not list:
             lCombinationMethods = [lCombinationMethods];
         logger = tsutil.get_pyaf_hierarchical_logger();
         logger.info("FORECASTING_HIERARCHICAL_MODEL_COMBINATION_METHODS " + str(lCombinationMethods));
+        self.check_combination_methods()
 
         for lMethod in lCombinationMethods:
             if(lMethod == "BU"):            
                 lForecast_DF_BU = self.computeBottomUpForecasts(lForecast_DF);
                 lForecast_DF = lForecast_DF_BU;
         
             if(lMethod == "TD"):
```

## pyaf/TS/Signal_Grouping.py

```diff
@@ -15,15 +15,15 @@
 
     def __init__(self):
         sighier.cSignalHierarchy.__init__(self)
         self.mLabels2Tuples = {};
         
     def tuple_to_string(self, k):
         str1 = "_".join(list(k));
-        # print(k , "=>" , str1);
+        # tsutil.print_pyaf_detailed_info(k , "=>" , str1);
         return str1;
     
     def add_level(self, previous_level):
         level = previous_level + 1;
         self.mStructure[level] = {};
         for group in self.mStructure[previous_level]:
             lGroupLabel = group; # self.tuple_to_string(group);
@@ -34,46 +34,46 @@
                     new_group[k] = "";
                     new_group = tuple(new_group);
                     lNewGroupLabel = self.tuple_to_string(new_group);
                     self.mLabels2Tuples[lNewGroupLabel] = new_group;
                     if(lNewGroupLabel not in self.mStructure[level]):
                         self.mStructure[level][lNewGroupLabel] = set();
                     self.mStructure[level][lNewGroupLabel].add(lGroupLabel)
-        # print("STRUCTURE_LEVEL" , level, self.mStructure[level]);
+        # tsutil.print_pyaf_detailed_info("STRUCTURE_LEVEL" , level, self.mStructure[level]);
 
     def create_HierarchicalStructure(self):
         
         # lGroups = {};
         # lGroups["State"] = ["NSW","VIC","QLD","SA","WA","NT","ACT","TAS"];
         # lGroups["Gender"] = ["female","male"];
         # lHierarchy['GroupOrder']= ["State" , "Gender"];
         
         lGroups = self.mHierarchy['Groups']
         self.mLevels = list(lGroups.keys());
         self.mLabels2Tuples = {};
         self.mStructure = {};
         array1 = [ sorted(lGroups[k]) for k in self.mHierarchy['GroupOrder'] ];
         prod = itertools.product( *array1 );
-        # print(prod);
+        # tsutil.print_pyaf_detailed_info(prod);
         # prod = itertools.product(['a' , 'b'] , ['1' , '2'] , ['cc' , 'dd']);
         level = 0;
         self.mStructure[level] = {}
         for k in prod:
-            # print("PRODUCT_DETAIL", k);
+            # tsutil.print_pyaf_detailed_info("PRODUCT_DETAIL", k);
             lGroupLabel = self.tuple_to_string(k);
             # Grouping genrates all possible group combinations.
             # Not all columns are mandatory. 
             if(lGroupLabel in self.mTrainingDataset.columns):
                 self.mLabels2Tuples[lGroupLabel] = k;
                 self.mStructure[level][lGroupLabel] = set();
-        # print("STRUCTURE_LEVEL" , level, self.mStructure[level]);
+        # tsutil.print_pyaf_detailed_info("STRUCTURE_LEVEL" , level, self.mStructure[level]);
         while(len(self.mStructure[level]) > 1):
             self.add_level(level);
             level = level + 1;
         
         # Stabilize the order of nodes
         for level in  sorted(self.mStructure.keys()):
             for col in sorted(self.mStructure[level].keys()):
                 self.mStructure[level][col] = sorted(self.mStructure[level][col])
                 
-        # print("STRUCTURE", self.mStructure);
+        # tsutil.print_pyaf_detailed_info("STRUCTURE", self.mStructure);
         pass
```

## pyaf/TS/Signal_Transformation.py

```diff
@@ -24,27 +24,24 @@
     tr1.mOriginalSignal = "selfTestSignal";
     tr1.fit(sig)
     sig_scaled = tr1.scale_signal(sig.values)
     sig1 = tr1.apply(sig);
     df['A_scaled'] = sig_scaled
     df['A_transformed'] = sig1
     sig2 = tr1.invert(df['A_transformed'])
-    # print(sig)
-    # print(sig1)
-    # print(sig2)
     n = np.linalg.norm(sig2 - sig)
     lName = tr1.get_name("Test")
     lEps = 1e-6
     lNotOK = (not lName.startswith('Quantized_')) and (n > lEps)
     if (lNotOK):
-        print("'" + lName + "'" , " : ", n)
-        print("A = " , sig.values.tolist())
-        print("A_SCALED = " , sig_scaled.tolist())
-        print("A_TRANSFORMED = " , sig1.tolist())
-        print("A_TRANSFORMED_TR = " , sig2.tolist())    
+        tsutil.print_pyaf_detailed_info("'" + lName + "'" , " : ", n)
+        tsutil.print_pyaf_detailed_info("A = " , sig.values.tolist())
+        tsutil.print_pyaf_detailed_info("A_SCALED = " , sig_scaled.tolist())
+        tsutil.print_pyaf_detailed_info("A_TRANSFORMED = " , sig1.tolist())
+        tsutil.print_pyaf_detailed_info("A_TRANSFORMED_TR = " , sig2.tolist())    
 
         assert(n <= lEps)    
 
 
 def testTransform(tr1):
     for seed_value in range(0,10,100):
         testTransform_one_seed(tr1, seed_value)
@@ -58,75 +55,74 @@
         pass
 
     def is_applicable(self, sig):
         return True;
 
 
     def checkSignalType(self, sig):
-        # print(df.info());
+        # tsutil.print_pyaf_detailed_info(df.info());
         type2 = sig.dtype
         if(type2.kind == 'O'):
             raise tsutil.PyAF_Error('Invalid Signal Column Type ' + sig.dtype);
 
     def fit_scaling_params(self, sig):
         self.mScaler.fit(sig.reshape(-1, 1))
 
     def scale_signal(self, sig):
         return self.mScaler.transform(sig.reshape(-1, 1)).ravel()
 
     def rescale_signal(self, sig1):
         return self.mScaler.inverse_transform(sig1.reshape(-1, 1)).ravel()
         
     def fit(self , sig):
-        # print("FIT_START", self.mOriginalSignal, sig.values[1:5]);
+        # tsutil.print_pyaf_detailed_info("FIT_START", self.mOriginalSignal, sig.values[1:5]);
         self.checkSignalType(sig)
         self.fit_scaling_params(sig.values);
         sig1 = self.scale_signal(sig.values);
         self.specific_fit(sig1);
-        # print("FIT_END", self.mOriginalSignal, sig1.values[1:5]);
+        # tsutil.print_pyaf_detailed_info("FIT_END", self.mOriginalSignal, sig1.values[1:5]);
         pass
 
     def apply(self, sig):
-        # print("APPLY_START", self.mOriginalSignal, sig.values[1:5]);
+        # tsutil.print_pyaf_detailed_info("APPLY_START", self.mOriginalSignal, sig.values[1:5]);
         self.checkSignalType(sig)
-        sig1 = self.scale_signal(sig.values);
-        sig2 = self.specific_apply(sig1);
-        # print("APPLY_END", self.mOriginalSignal, sig2.values[1:5]);
+        scaled_sig = self.scale_signal(sig.values);
+        applied_sig = self.specific_apply(scaled_sig);
+        # tsutil.print_pyaf_detailed_info("APPLY_END", self.mOriginalSignal, sig2.values[1:5]);
         if(self.mDebug):
             self.check_not_nan(sig2 , "transform_apply");
-        return sig2;
+        return {"scaled" : scaled_sig, "applied" : applied_sig}
 
     def invert(self, sig1):
-        # print("INVERT_START", self.mOriginalSignal, sig1.values[1:5]);
-        sig2 = self.specific_invert(sig1.values);
-        rescaled_sig = self.rescale_signal(sig2);
-        # print("INVERT_END", self.mOriginalSignal, rescaled_sig.values[1:5]);
-        return rescaled_sig;
+        # tsutil.print_pyaf_detailed_info("INVERT_START", self.mOriginalSignal, sig1.values[1:5]);
+        inverted_sig = self.specific_invert(sig1.values);
+        rescaled_sig = self.rescale_signal(inverted_sig);
+        # tsutil.print_pyaf_detailed_info("INVERT_END", self.mOriginalSignal, rescaled_sig.values[1:5]);
+        return {"inverted" : inverted_sig, "rescaled" : rescaled_sig}
 
     def transformDataset(self, df):
-        df["scaled_" + self.mOriginalSignal] = self.scale_signal(df[self.mOriginalSignal].values)
-        df[self.get_name(self.mOriginalSignal)] = self.apply(df[self.mOriginalSignal])
+        apply_result = self.apply(df[self.mOriginalSignal])
+        df[self.mOriginalSignal + "_scaled"] = apply_result["scaled"]
+        df[self.get_name(self.mOriginalSignal)] = apply_result["applied"]
         return df;
 
     def test(self):
         import copy;
         tr1 = copy.deepcopy(self);
         testTransform(tr1);
         pass
 
     def dump_apply_invert(self, sig_before_apply, sig_after_apply):
         sig = pd.Series(index = None);
         sig['before_apply'] = sig_before_apply;
         sig['after_apply'] = sig_after_apply;
-        print("dump_apply_invert_head", sig.head());
-        print("dump_apply_invert_tail", sig.tail());
         
     def check_not_nan(self, sig , name):
         if(np.isnan(sig).any()):
-            print("TRANSFORMATION_RESULT_WITH_NAN_IN_SIGNAL" , sig);
+            tsutil.print_pyaf_detailed_info("TRANSFORMATION_RESULT_WITH_NAN_IN_SIGNAL" , sig);
             raise tsutil.Internal_PyAF_Error("Invalid transformation for column '" + name + "'");
         pass
 
 
 class cSignalTransform_None(cAbstractSignalTransform):
 
     def __init__(self):
@@ -188,22 +184,31 @@
         self.mFormula = "Quantization";
         self.mComplexity = tscomplex.eModelComplexity.High;
         pass
 
     def get_name(self, iSig):
         return "Quantized_" + str(self.mQuantiles) + "_" + str(iSig);
 
-    def is_applicable(self, sig):
-        N = sig.shape[0];
-        if(N < (5 * self.mQuantiles)) :
-            return False;
-        return True;
+    def get_optimal_bin_number(self, sig):
+        # https://en.wikipedia.org/wiki/Histogram#Variable_bin_widths
+        # This choice of bins is motivated by maximizing the power of a Pearson chi-squared
+        # test testing whether the bins do contain equal numbers of samples.
+        # Q = 2*n^(2/5)
+        N = sig.shape[0]
+        Q = 2.0 * np.power(N , 2.0/5.0)
+        Q = max(1, int(Q))
+        return Q
     
     def specific_fit(self , sig):
+        Q_optimal = self.get_optimal_bin_number(sig)
         Q = self.mQuantiles;
+        Q = min(Q, Q_optimal)
+        # tsutil.print_pyaf_detailed_info(
+        #    "TRANSFORMATION_QUANTIZATION_OPTIMAL_RULE" ,
+        #    sig.shape[0], self.mQuantiles, Q_optimal, Q);
         q = pd.Series(range(0,Q)).apply(lambda x : np.quantile(sig, x/Q))
         self.mCurve = q.to_dict()
         (self.mMin, self.mMax) = (min(self.mCurve.keys()), max(self.mCurve.keys()))
         pass
 
     def signal2quant(self, x):
         curve = self.mCurve;
@@ -290,15 +295,15 @@
         self.mComplexity = tscomplex.eModelComplexity.Medium;
         pass
 
     def get_name(self, iSig):
         return "Diff_" + str(iSig);
 
     def specific_fit(self, sig):
-        # print(sig.head());
+        # tsutil.print_pyaf_detailed_info(sig.head());
         self.mFirstValue = sig[0];
         pass
     
 
     def specific_apply(self, sig):
         sig_diff = np.diff(sig)
         lResult = np.append([ sig[0] - self.mFirstValue ], sig_diff);
@@ -328,27 +333,29 @@
         return "RelDiff_" + str(iSig);
     
     def specific_fit(self, sig):
         self.mFirstValue = sig[0];
         pass
 
     def specific_apply(self, sig):
-        # print("RelDiff_apply_DEBUG_START" , self.mFirstValue, sig.values[0:10]);
+        # tsutil.print_pyaf_detailed_info("RelDiff_apply_DEBUG_START" , self.mFirstValue, sig[0:10]);
         sig_diff = np.diff(sig);
         sig_shifted = sig[:-1]
         rate = np.divide(sig_diff, sig_shifted, out=np.zeros_like(sig_diff), where=sig_shifted!=0)
         rate = np.append([0.0], rate)
+        # tsutil.print_pyaf_detailed_info("RelDiff_apply_DEBUG_END", rate[0:10]);
         return rate;
 
 
     def specific_invert(self, sig):
-        # print("RelDiff_invert_DEBUG_START" , self.mFirstValue, sig.values[0:10]);
+        # tsutil.print_pyaf_detailed_info("RelDiff_invert_DEBUG_START" , self.mFirstValue, sig[0:10]);
         rate = sig + 1;
         rate_cum = np.cumprod(rate).clip(-1e7, 1e7);
         sig_orig = self.mFirstValue * rate_cum;
+        # tsutil.print_pyaf_detailed_info("RelDiff_invert_DEBUG_END", sig_orig[:10]);
         return sig_orig;
 
     def dump_values(self):
         logger = tsutil.get_pyaf_logger();
         logger.info("REALTIVE_DIFFERENCING_TRANSFORMATION " + self.mFormula + " " + str(self.mFirstValue));
 
 class cSignalTransform_Logit(cAbstractSignalTransform):
@@ -499,15 +506,15 @@
         self.mSignalFrame = None
         self.mTransformList = {}
 
     def validateTransformation(self , transf , df, iTime, iSignal):
         lName = transf.get_name("");
         lIsApplicable = transf.is_applicable(df[iSignal]);
         if(lIsApplicable):
-            # print("Adding Transformation " , lName);
+            # tsutil.print_pyaf_detailed_info("Adding Transformation " , lName);
             # transf.test()
             self.mTransformList = self.mTransformList + [transf];
 
 
     
     def defineTransformations(self , df, iTime, iSignal):
         self.mTransformList = [];
```

## pyaf/TS/Temporal_Hierarchy.py

```diff
@@ -72,15 +72,15 @@
             df_resampled[lPeriod][lName] = df_resampled[lPeriod][lName] - lShift
             
         for lPeriod in self.mPeriods:
             lName = lPrefix + "_" + lPeriod + "_start"
             WData = df_resampled[lPeriod]
             # df[[self.mDateColumn , self.mSignal]].info()
             # WData.info()
-            # print("DATE_PERIOD", list(WData[lName])[:30])
+            # tsutil.print_pyaf_detailed_info("DATE_PERIOD", list(WData[lName])[:30])
             df_merge = df[[self.mDateColumn , self.mSignal]].merge(WData, left_on=self.mDateColumn,right_on=lName, how='left', suffixes=('_x', '_Period'), sort=True)
             df[self.mSignal + '_' + lPeriod] = df_merge[self.mSignal + '_Period']
             df[lName] = df_merge[lName]
             logger.info("FORECASTING_HIERARCHICAL_TEMPORAL_LEVEL " + str((lPeriod, lName, list(df.columns), WData.shape)))
             
 
         return df
@@ -101,19 +101,19 @@
             lName = lPrefix + "_" + lPeriod + "_start"
             df_resampled[lPeriod] = df1[self.mSignal].resample(lPeriod).sum().reset_index()
             df_resampled[lPeriod].columns = [lName , self.mSignal]
             # synchronize
             lShift = df_resampled[lPeriod][lName].iloc[0] - df[self.mDateColumn].iloc[0] 
             df_resampled[lPeriod][lName] = df_resampled[lPeriod][lName] - lShift
             lDate_Period = df_resampled[lPeriod][lName]
-            # print("AS_FREQ" , lPeriod , lDate_Period.head())
+            # tsutil.print_pyaf_detailed_info("AS_FREQ" , lPeriod , lDate_Period.head())
             lNewFreq = lHelper.computeTimeFrequency_in_seconds(lDate_Period)
             lHorizon = int(self.mHorizon * lBaseFreq / lNewFreq)
             lHorizon = max(1, lHorizon)
-            # print("AS_FREQ_2" , lPeriod , lBaseFreq , lNewFreq , lHorizon)
+            # tsutil.print_pyaf_detailed_info("AS_FREQ_2" , lPeriod , lBaseFreq , lNewFreq , lHorizon)
             self.mHorizons[lPeriod] = lHorizon
             logger.info("FORECASTING_HIERARCHICAL_TEMPORAL_HORIZONS_FIRST_RESAMPLED_DATA " + str(lPeriod) + " " + str(df_resampled[lPeriod].head(5).to_dict()) )
 
         logger.info("FORECASTING_HIERARCHICAL_TEMPORAL_HORIZONS " + str(self.mHorizons));
 
     def checkPhysicalTime(self):
         logger = tsutil.get_pyaf_hierarchical_logger();
@@ -153,9 +153,9 @@
             self.mStructure[lLevel] = {}
             
         for (lLevel, lPeriod) in enumerate(self.mPeriods):
             self.mStructure[lLevel][self.mSignal + '_' + lPeriod] = set()
             if(lLevel > 0):
                 self.mStructure[lLevel][self.mSignal + '_' + lPeriod] = set([self.mSignal + '_' + self.mPeriods[lLevel - 1]])
                 
-        # print(self.mStructure);
+        # tsutil.print_pyaf_detailed_info(self.mStructure);
         pass
```

## pyaf/TS/Time.py

```diff
@@ -43,19 +43,17 @@
         dict1["Horizon"] =  self.mHorizon;
         return dict1;
 
     def addVars(self, df):
         df[self.mRowNumberColumn] = self.mSignalFrame[self.mRowNumberColumn]
         df[self.mTime] = self.mSignalFrame[self.mTime]
         df[self.mNormalizedTimeColumn] = self.mSignalFrame[self.mNormalizedTimeColumn]
-        df[self.mSignal] = self.mSignalFrame[self.mSignal]
-        df[self.mOriginalSignal] = self.mSignalFrame[self.mOriginalSignal]
 
     def get_time_dtype(self):
-        # print(self.mTimeMax, type(self.mTimeMax))
+        # tsutil.print_pyaf_detailed_info(self.mTimeMax, type(self.mTimeMax))
         lType = self.mSignalFrame[self.mTime].dtype;
         return lType;
 
     def checkDateTypesForNewDataset(self, df):
         if(self.mTimeMax is not None):
             lType1 = self.get_time_dtype();
             lType2 = df[self.mTime].dtype
@@ -63,78 +61,94 @@
                 raise tsutil.PyAF_Error('Incompatible Time Column Type expected=' + str(lType1) + ' got: ' + str(lType2) + "'");
                 pass
         
 
     def transformDataset(self, df):
         self.checkDateTypesForNewDataset(df);
         # new row
-        lLastRow = df.tail(1).copy();
         lNextTime = self.nextTime(df, 1)
-        lLastRow[self.mTime] = lNextTime
-        lLastRow[self.mSignal] = np.nan
-        if(self.mNormalizedTimeColumn in df.columns):
-            lLastRow[self.mNormalizedTimeColumn] = self.normalizeTime(lNextTime)
-            lLastRow[self.mRowNumberColumn] = lLastRow[self.mRowNumberColumn].max() + 1
-        # print(lLastRow.columns ,  df.columns)
-        # assert(str(lLastRow.columns) == str(df.columns))
-
-        df = pd.concat([df, lLastRow], ignore_index=True, verify_integrity = True, sort=False); 
-        
+        lNextRowNumber = df.index.max() + 1
+        lNextValues = {
+            self.mRowNumberColumn : df.shape[0] + 1,
+            self.mTime : lNextTime,
+            self.mSignal : np.nan,
+            self.mNormalizedTimeColumn : self.normalizeTime(lNextTime)
+        }
+        lNewColumns = {}
+        # keep column order.
+        for col in df.columns:
+            # append an empty new value by default
+            lNewValue = np.nan
+            if col in lNextValues.keys():
+                lNewValue = lNextValues[col]
+            lNewColumns[col] = np.append(df[col].values, [ lNewValue ])
         if(self.mNormalizedTimeColumn not in df.columns):
-            df[self.mRowNumberColumn] = np.arange(0, df.shape[0]);
-            df[self.mNormalizedTimeColumn] = self.compute_normalized_date_column(df[self.mTime])
-            
-        # print(df.tail());
-        return df;
+            # Avoid unnecessary column order changes.
+            lNewTimeColumn = np.append(df[self.mTime].values, [lNextTime])
+            lNewColumns[self.mRowNumberColumn] = np.arange(0, df.shape[0] + 1);
+            lNewColumns[self.mNormalizedTimeColumn] = self.compute_normalized_date_column(lNewTimeColumn)
+                
+        df1 = pd.DataFrame(lNewColumns)
+        # Goal here : profiling/perf. Avoid reindexing. Keep this as the last op.
+        df1.index = df.index.tolist() + [lNextRowNumber]
+        return df1;
 
 
     def isPhysicalTime(self):
         lHelper = dtfunc.cDateTime_Helper()
         return lHelper.isPhysicalTime(self.mSignalFrame[self.mTime])
 
+    def get_moving_window_lengths_for_time_resolution(self):
+        if(not self.isPhysicalTime()):
+            return self.mOptions.mMovingWindowLengths or [];
+        if(self.mOptions.mMovingWindowLengths is not None):
+            return self.mOptions.mMovingWindowLengths            
+        lHelper = dtfunc.cDateTime_Helper()
+        return lHelper.get_moving_window_lengths_for_time_resolution(self.mResolution)
+
     
     def analyzeSeasonals(self):
         if(not self.isPhysicalTime()):
             return;
         lEstim = self.mSplit.getEstimPart(self.mSignalFrame);
         lEstimTime = lEstim[self.mTime]
         lHelper = dtfunc.cDateTime_Helper()
         self.mResolution = lHelper.guess_time_resolution(lEstimTime);
 
 
     def checkDateTypes(self):
-        # print(self.mSignalFrame.info());
+        # tsutil.print_pyaf_detailed_info(self.mSignalFrame.info());
         type1 = self.mSignalFrame[self.mTime].dtype
         if(type1.kind == 'O'):
             raise tsutil.PyAF_Error('Invalid Time Column Type ' + self.mTime + '[' + str(type1) + ']');
         
 
 
     def adaptTimeDeltaToTimeResolution(self):
         if(not self.isPhysicalTime()):
             return;
         lHelper = dtfunc.cDateTime_Helper()
         self.mTimeDelta = lHelper.adaptTimeDeltaToTimeResolution(self.mResolution , self.mTimeDelta);    
     
     def computeTimeDelta(self):
-        #print(self.mSignalFrame.columns);
-        # print(self.mSignalFrame[self.mTime].head());
+        # tsutil.print_pyaf_detailed_info(self.mSignalFrame.columns);
+        # tsutil.print_pyaf_detailed_info(self.mSignalFrame[self.mTime].head());
         lEstim = self.mSplit.getEstimPart(self.mSignalFrame)
         lTimeBefore = lEstim[self.mTime].shift(1);
         # lTimeBefore.fillna(self.mTimeMin, inplace=True)
         N = lEstim.shape[0];
         if(N == 1):
             if(self.isPhysicalTime()):
                 self.mTimeDelta = np.timedelta64(1,'D');
             else:
                 self.mTimeDelta = 1
             return
-        #print(self.mSignal, self.mTime, N);
-        #print(lEstim[self.mTime].head());
-        #print(lTimeBefore.head());
+        # tsutil.print_pyaf_detailed_info(self.mSignal, self.mTime, N);
+        # tsutil.print_pyaf_detailed_info(lEstim[self.mTime].head());
+        # tsutil.print_pyaf_detailed_info(lTimeBefore.head());
         lDiffs = lEstim[self.mTime][1:N] - lTimeBefore[1:N]
         
         if(self.mOptions.mTimeDeltaComputationMethod == "USER"):
             self.mTimeDelta = self.mOptions.mUserTimeDelta;
         if(self.mOptions.mTimeDeltaComputationMethod == "AVG"):
             self.mTimeDelta = np.mean(lDiffs);
             type1 = self.mSignalFrame[self.mTime].dtype
@@ -142,16 +156,16 @@
                 self.mTimeDelta = int(self.mTimeDelta)
         if(self.mOptions.mTimeDeltaComputationMethod == "MODE"):
             delta_counts = pd.DataFrame(lDiffs.value_counts());
             self.mTimeDelta = delta_counts[self.mTime].argmax();
         self.adaptTimeDeltaToTimeResolution();
 
     def estimate(self):
-        #print(self.mSignalFrame.columns);
-        #print(self.mSignalFrame[self.mTime].head());
+        # tsutil.print_pyaf_detailed_info(self.mSignalFrame.columns);
+        # tsutil.print_pyaf_detailed_info(self.mSignalFrame[self.mTime].head());
         self.checkDateTypes();
         
         self.mRowNumberColumn = "row_number"
         self.mNormalizedTimeColumn = self.mTime + "_Normalized";
 
         self.analyzeSeasonals();
 
@@ -159,15 +173,15 @@
         self.mTimeMin = lEstim[self.mTime].min();
         self.mTimeMax = lEstim[self.mTime].max();
         if(self.isPhysicalTime()):
             self.mTimeMin = np.datetime64(self.mTimeMin.to_pydatetime());
             self.mTimeMax = np.datetime64(self.mTimeMax.to_pydatetime());
         self.mTimeMinMaxDiff = self.mTimeMax - self.mTimeMin;
         self.mEstimCount = lEstim.shape[0]
-        # print(self.mTimeMin, self.mTimeMax , self.mTimeMinMaxDiff , (self.mTimeMax - self.mTimeMin)/self.mTimeMinMaxDiff)
+        # tsutil.print_pyaf_detailed_info(self.mTimeMin, self.mTimeMax , self.mTimeMinMaxDiff , (self.mTimeMax - self.mTimeMin)/self.mTimeMinMaxDiff)
         self.computeTimeDelta();
         self.mSignalFrame[self.mNormalizedTimeColumn] = self.compute_normalized_date_column(self.mSignalFrame[self.mTime])
         self.dump();
 
     def dump(self):
         time_info = self.info(); 
         
@@ -186,19 +200,19 @@
 
     def cast_to_time_dtype(self, iTimeValue):
         lType1 = self.get_time_dtype();
         lTimeValue = np.array([iTimeValue]).astype(lType1)[0];
         return lTimeValue;
     
     def nextTime(self, df, iSteps):
-        #print(df.tail(1)[self.mTime]);
+        # tsutil.print_pyaf_detailed_info(df.tail(1)[self.mTime]);
         lLastTime = df[self.mTime].values[-1]
         if(self.isPhysicalTime()):
             lLastTime = pd.Timestamp(lLastTime)
-            # print("NEXT_TIME" , lLastTime, iSteps, self.mTimeDelta);
+            # tsutil.print_pyaf_detailed_info("NEXT_TIME" , lLastTime, iSteps, self.mTimeDelta);
             lNextTime = lLastTime + iSteps * self.mTimeDelta;
             lNextTime = self.cast_to_time_dtype(lNextTime.to_datetime64())
         else:
             lNextTime = lLastTime + iSteps * self.mTimeDelta;
             lNextTime = self.cast_to_time_dtype(lNextTime)
```

## pyaf/TS/TimeSeriesModel.py

```diff
@@ -9,30 +9,28 @@
 
 from . import PredictionIntervals as predint
 
 from . import Plots as tsplot
 from . import Perf as tsperf
 from . import Utils as tsutil
 from . import Complexity as tscomplex
+from . import TimeSeries_Cutting as tscut
 
 
 def to_str(x):
     return str(np.round(x, 6))
 
 class cTimeSeriesModel:
     
     def __init__(self, transf, iDecompType, trend, cycle, autoreg):
         self.mTransformation = transf;
         self.mDecompositionType = iDecompType;
         self.mTrend = trend;
         self.mCycle = cycle;
         self.mAR = autoreg;
-        self.mFitPerformances = {}
-        self.mForecastPerformances = {}
-        self.mTestPerformances = {}
         self.mOutName = self.mAR.mOutName;
         self.mOriginalSignal = self.mTransformation.mOriginalSignal;
         self.mTimeInfo = self.mTrend.mTimeInfo;
         self.mTime = self.mTimeInfo.mTime;
         self.mSignal = self.mTimeInfo.mSignal;
         self.mTrainingVersionInfo = self.getVersions();
 
@@ -80,17 +78,17 @@
         # lTimer = tsutil.cTimer(("UPDATE_MODEL_PERFS", {"Signal" : self.mOriginalSignal, "Model" : self.mOutName}))
         lPredictionIntervalsEstimator = predint.cPredictionIntervalsEstimator();
         lPredictionIntervalsEstimator.mModel = self;
         lPredictionIntervalsEstimator.mComputeAllPerfs = compute_all_indicators
         lPredictionIntervalsEstimator.computePerformances();
         lForecastColumn = str(self.mOriginalSignal) + "_Forecast";
                     
-        self.mFitPerfs = lPredictionIntervalsEstimator.mFitPerformances
-        self.mForecastPerfs = lPredictionIntervalsEstimator.mForecastPerformances
-        self.mTestPerfs = lPredictionIntervalsEstimator.mTestPerformances
+        self.mFitPerfs = lPredictionIntervalsEstimator.mPerformances["whole"][tscut.eDatasetType.Fit]
+        self.mForecastPerfs = lPredictionIntervalsEstimator.mPerformances["whole"][tscut.eDatasetType.Forecast]
+        self.mTestPerfs = lPredictionIntervalsEstimator.mPerformances["whole"][tscut.eDatasetType.Test]
 
     def get_perfs_summary(self):
         output = {"Fit" : {}, "Forecast" : {}, "Test" : {}}
         lForecastColumn = str(self.mOriginalSignal) + "_Forecast";
         lCriterion = self.mTimeInfo.mOptions.mModelSelection_Criterion
         for h in [1, self.mTimeInfo.mHorizon]:
             lHorizonName = lForecastColumn + "_" + str(h);
@@ -186,61 +184,82 @@
         logger.info("TREND_DETAIL_END");
         logger.info("CYCLE_MODEL_DETAIL_START");
         self.mCycle.dump_values();
         logger.info("CYCLE_MODEL_DETAIL_END");
         logger.info("AR_MODEL_DETAIL_START");
         self.mAR.dumpCoefficients();
         logger.info("AR_MODEL_DETAIL_END");
-        
+        if(self.mAR.mExogenousInfo):
+            self.mAR.mExogenousInfo.info(used = self.mAR.get_used_variables())
     
     def getInfo(self):
         logger = tsutil.get_pyaf_logger();
         logger.info("TIME_DETAIL " + self.mTrend.mTimeInfo.info());
         self.signal_info()
         self.decomposition_info()
         self.perf_info()
         self.decomposition_detail_info()
 
-    def compute_model_forecast(self, iTrendValue, iCycleValue, iARValue):
+    def compute_transformed_forecast(self, iTrendValue, iCycleValue, iARValue):
         if(self.mDecompositionType in ['TS+R']):
             return iTrendValue * iCycleValue + iARValue
         if(self.mDecompositionType in ['TSR']):
             lTrendValue = iTrendValue.clip(-100, 100)
             lCycleValue = iCycleValue.clip(-100, 100)
             lARValue = iARValue.clip(-100, 100)
             return lTrendValue * lCycleValue * lARValue
         return iTrendValue + iCycleValue + iARValue
+    
+    def compute_detrended_signal(self, iTrendValue, iCycleValue, iARValue):
+        if(self.mDecompositionType in ['TS+R']):
+            # T and S are not easily separable. remove T*S ("TrendCycle component"). Can do better ?
+            return iARValue
+        if(self.mDecompositionType in ['TSR']):
+            lCycleValue = iCycleValue.clip(-100, 100)
+            lARValue = iARValue.clip(-100, 100)
+            return lCycleValue * lARValue
+        return iCycleValue + iARValue
+
+    def compute_deseasonalized_signal(self, iTrendValue, iCycleValue, iARValue):
+        if(self.mDecompositionType in ['TS+R']):
+            # T and S are not easily separable. remove T*S ("TrendCycle component"). Can do better ?
+            return iARValue
+        if(self.mDecompositionType in ['TSR']):
+            lTrendValue = iTrendValue.clip(-100, 100)
+            lARValue = iARValue.clip(-100, 100)
+            return lTrendValue * lARValue
+        return iTrendValue + iARValue
 
     def forecastOneStepAhead(self , df , horizon_index = 1, perf_mode = False):
         assert(self.mTime in df.columns)
         assert(self.mOriginalSignal in df.columns)
         lPrefix = self.mSignal + "_";
-        df1 = df;
+        df1 = df[ [self.mTime, self.mOriginalSignal] ].copy();
         # df1.to_csv("before.csv");
         # add new line with new time value, row_number and nromalized time
         # add signal tranformed column
         df1 = self.mTransformation.transformDataset(df1);
         # df1.to_csv("after_transformation.csv");
-        #print("Transformation update : " , df1.columns);
+        # tsutil.print_pyaf_detailed_info("Transformation update : " , df1.columns);
 
         df1 = self.mTimeInfo.transformDataset(df1);
         # df1.to_csv("after_time.csv");
-        # print("TimeInfo update : " , df1.columns);
+        # tsutil.print_pyaf_detailed_info("TimeInfo update : " , df1.columns);
         # compute the trend based on the transformed column and compute trend residue
         df1 = self.mTrend.transformDataset(df1);
-        #print("Trend update : " , df1.columns);
+        # tsutil.print_pyaf_detailed_info("Trend update : " , df1.columns);
         # df1.to_csv("after_trend.csv");
         # compute the cycle and its residue based on the trend residue
         df1 = self.mCycle.transformDataset(df1);
         # df1.to_csv("after_cycle.csv");
-        #print("Cycle update : " , df1.columns);
+        # tsutil.print_pyaf_detailed_info("Cycle update : " , df1.columns);
         # compute the AR componnet and its residue based on the cycle residue
         df1 = self.mAR.transformDataset(df1, horizon_index);
         # df1.to_csv("after_ar.csv");
-        #print("AR update : " , df1.columns);
+        # tsutil.print_pyaf_detailed_info("AR update : " , df1.columns);
         # compute the forecast and its residue (forecast = trend  + cycle + AR)
         df2 = df1;
         lTrendColumn = df2[self.mTrend.mOutName]
         lCycleColumn = df2[self.mCycle.mOutName]
         lARColumn = df2[self.mAR.mOutName]
         lSignal = df2[self.mSignal]
         if(not perf_mode):
@@ -249,56 +268,62 @@
             df2[lPrefix + 'Trend_residue'] = df2[self.mCycle.mTrend_residue_name]
             df2[lPrefix + 'Cycle'] =  lCycleColumn;
             df2[lPrefix + 'Cycle_residue'] = df2[self.mCycle.getCycleResidueName()];
             df2[lPrefix + 'AR'] =  lARColumn ;
             df2[lPrefix + 'AR_residue'] = df2[self.mAR.mOutName + '_residue'];
 
         lPrefix2 = str(self.mOriginalSignal) + "_";
-        # print("TimeSeriesModel_forecast_invert");
-        df2[lPrefix + 'TransformedForecast'] = self.compute_model_forecast(lTrendColumn, lCycleColumn, lARColumn)
-        df2[lPrefix2 + 'Forecast'] = self.mTransformation.invert(df2[lPrefix + 'TransformedForecast']);
+        # tsutil.print_pyaf_detailed_info("TimeSeriesModel_forecast_invert");
+        df2[lPrefix + 'TransformedForecast'] = self.compute_transformed_forecast(lTrendColumn, lCycleColumn, lARColumn)
+        df2[lPrefix + 'Detrended'] = self.compute_detrended_signal(lTrendColumn, lCycleColumn, lARColumn)
+        df2[lPrefix + 'Deseasonalized'] = self.compute_deseasonalized_signal(lTrendColumn, lCycleColumn, lARColumn)
+        invert_result = self.mTransformation.invert(df2[lPrefix + 'TransformedForecast'])
+        df2[lPrefix2 + 'TransformedForecast_inverted'] = invert_result["inverted"]
+        df2[lPrefix2 + 'Forecast'] = invert_result["rescaled"]
 
         if(not perf_mode):
             df2[lPrefix + 'TransformedResidue'] =  lSignal - df2[lPrefix + 'TransformedForecast']
             lOriginalSignal = df2[self.mOriginalSignal]
             df2[lPrefix2 + 'Residue'] =  lOriginalSignal - df2[lPrefix2 + 'Forecast']
         df2.reset_index(drop=True, inplace=True);
         return df2;
 
 
     def forecast_all_horizons(self , df , iHorizon):
         N0 = df.shape[0];
         df1 = self.forecastOneStepAhead(df, 1)
         lForecastColumnName = str(self.mOriginalSignal) + "_Forecast";
         for h in range(0 , iHorizon - 1):
-            # print(df1.info());
+            # tsutil.print_pyaf_detailed_info(df1.info());
             N = df1.shape[0];
             # replace the signal with the forecast in the last line  of the dataset
             lPos = df1.index[N - 1];
             lSignal = df1.loc[lPos , lForecastColumnName];
             df1.loc[lPos , self.mOriginalSignal] = lSignal;
             df1 = df1[[self.mTime , self.mOriginalSignal, self.mTimeInfo.mRowNumberColumn, self.mTimeInfo.mNormalizedTimeColumn]];
             df1 = self.forecastOneStepAhead(df1 , h+2)
 
         assert((N0 + iHorizon) == df1.shape[0])
         N1 = df1.shape[0];
         lPrefix = self.mSignal + "_";
-        lFieldsToErase = [ self.mOriginalSignal, self.mSignal, self.mOriginalSignal + "_Transformed", 
+        lFieldsToErase = [ self.mOriginalSignal, self.mSignal,
+                           self.mOriginalSignal + "_scaled", 
+                           self.mOriginalSignal + "_Transformed", 
                            self.mTrend.mOutName + '_residue', lPrefix + 'Trend_residue',
                            self.mCycle.mOutName + '_residue', lPrefix + 'Cycle_residue',
                            self.mAR.mOutName + '_residue',  lPrefix + 'AR_residue',
                            lPrefix + 'TransformedResidue', str(self.mOriginalSignal) + '_Residue']
         df1.loc[N1 -iHorizon : N1, lFieldsToErase] = np.nan
         return df1
 
     
     def forecast(self , df , iHorizon):
         df1 = self.forecast_all_horizons(df, iHorizon)
-        # print(df.head())
-        # print(df1.head())
+        # tsutil.print_pyaf_detailed_info(df.head())
+        # tsutil.print_pyaf_detailed_info(df1.head())
         if(self.mTimeInfo.mOptions.mAddPredictionIntervals):
             df1 = self.addPredictionIntervals(df, df1, iHorizon);
             self.addForecastQuantiles(df, df1, iHorizon);
         if(self.mTimeInfo.mOptions.mForecastRectifier is not None):
             df1 = self.applyForecastRectifier(df1)
         return df1
 
@@ -318,39 +343,39 @@
         lUpperBoundName = lForecastColumn + '_Upper_Bound';
         iForecastFrame[lLowerBoundName] = np.nan; 
         iForecastFrame[lUpperBoundName] = np.nan; 
 
         lConfidence = 1.96 ; # 0.95
         # the prediction intervals are only computed for the training horizon
         lHorizon = min(iHorizon , self.mTimeInfo.mHorizon);
-        lWidths = [lConfidence * self.mPredictionIntervalsEstimator.mForecastPerformances[lForecastColumn + "_" + str(h + 1)].mL2
+        lWidths = [lConfidence * self.mPredictionIntervalsEstimator.mPerformances["whole"][tscut.eDatasetType.Forecast][lForecastColumn + "_" + str(h + 1)].mL2
                    for h in range(0 , self.mTimeInfo.mHorizon)]
         lWidths = (lWidths + [np.nan]*iHorizon)[:iHorizon]
         lForcastValues = iForecastFrame.loc[N:N+iHorizon, lForecastColumn]
-        # print(lForcastValues.head(lHorizon))
-        # print(iHorizon, self.mTimeInfo.mHorizon, lHorizon, lForcastValues.shape)
-        # print(lWidths)
+        # tsutil.print_pyaf_detailed_info(lForcastValues.head(lHorizon))
+        # tsutil.print_pyaf_detailed_info(iHorizon, self.mTimeInfo.mHorizon, lHorizon, lForcastValues.shape)
+        # tsutil.print_pyaf_detailed_info(lWidths)
         iForecastFrame.loc[N:N+iHorizon, lLowerBoundName] = lForcastValues - lWidths
         iForecastFrame.loc[N:N+iHorizon, lUpperBoundName] = lForcastValues + lWidths
         return iForecastFrame;
 
     def addForecastQuantiles(self, iInputDS, iForecastFrame, iHorizon):
         lSignalColumn = self.mOriginalSignal;
 
         N = iInputDS.shape[0] ;
         lForecastColumn = str(lSignalColumn) + "_Forecast";
         lQuantileName = lForecastColumn + "_Quantile_"
 
         # the prediction intervals are only computed for the training horizon
         lHorizon = min(iHorizon , self.mTimeInfo.mHorizon);
-        lPerfs = [self.mPredictionIntervalsEstimator.mForecastPerformances[lForecastColumn + "_" + str(h + 1)]
+        lPerfs = [self.mPredictionIntervalsEstimator.mPerformances["whole"][tscut.eDatasetType.Forecast][lForecastColumn + "_" + str(h + 1)]
                    for h in range(0 , self.mTimeInfo.mHorizon)]
         lForcastValues = iForecastFrame.loc[N:N+iHorizon, lForecastColumn]
         
-        lQuantiles = self.mPredictionIntervalsEstimator.mForecastPerformances[lForecastColumn + "_1"].mErrorQuantiles.keys()
+        lQuantiles = self.mPredictionIntervalsEstimator.mPerformances["whole"][tscut.eDatasetType.Forecast][lForecastColumn + "_1"].mErrorQuantiles.keys()
         lQuantiles = sorted(lQuantiles)
         for q in lQuantiles:
             iForecastFrame[lQuantileName + str(q)] = np.nan
             lQuants = [lPerf.mErrorQuantiles[q] for lPerf in lPerfs]
             lQuants = (lQuants + [np.nan]*iHorizon)[:iHorizon]
             iForecastFrame.loc[N:N+iHorizon, lQuantileName + str(q)] =  lForcastValues.values + np.array(lQuants)
         return iForecastFrame;
@@ -361,17 +386,24 @@
         lTime = self.mTimeInfo.mNormalizedTimeColumn;            
         tsplot.decomp_plot(df,
                            lTime, lPrefix + 'Signal',
                            lPrefix + 'Forecast' , lPrefix + 'Residue', horizon = self.mTimeInfo.mHorizon, title = self.mOriginalSignal + " Forecasts");
 
     def to_dict(self, iWithOptions = False):
         dict1 = {};
+        lExogData = None
+        if(self.mAR is not None and self.mAR.mExogenousInfo is not None):
+            lExogData = self.mAR.mExogenousInfo.to_dict(used = self.mAR.get_used_variables())
         d1 = { "Time" : self.mTimeInfo.to_dict(),
                "Signal" : self.mOriginalSignal,
-               "Training_Signal_Length" : self.mTimeInfo.mSignalFrame.shape[0]};
+               "Training_Signal_Length" : self.mTimeInfo.mSignalFrame.shape[0],
+              }
+        if(lExogData is not None):
+            d1["Exogenous_Data"] = lExogData
+            
         dict1["Dataset"] = d1;
         lTransformation = self.mTransformation.mFormula;
         d2 = { "Best_Decomposition" : self.mOutName,
                "Signal_Decomposition_Type" : self.mDecompositionType,
                "Signal_Transoformation" : lTransformation,
                "Trend" : self.mTrend.mFormula,
                "Cycle" : self.mCycle.mFormula,
@@ -424,38 +456,40 @@
         for h in [1, self.mTimeInfo.mHorizon]:
             lHorizonName = lForecastColumn + "_" + str(h);
             lPerf = self.mForecastPerfs[lHorizonName]
             lTitle = lTitle + "MAPE_" + str(h) + " = " + str(lPerf.mMAPE) + " "
             if(lCriterion != "MAPE"):
                 lTitle = lTitle + lCriterion + "_" + str(h) + " = " + str(lPerf.getCriterionValue(lCriterion)) + " "
         return lTitle
-            
+
     def standardPlots(self, name = None, format = 'png'):
         lOutput =  self.getForecastDatasetForPlots();
         self.plotResidues(name = name, format=format, iOutputDF = lOutput);
-        # print(lOutput.columns)
+        # tsutil.print_pyaf_detailed_info(lOutput.columns)
         lPrefix = str(self.mOriginalSignal) + "_";
         lForecastColumn = lPrefix + 'Forecast';
         lTime = self.mTimeInfo.mTime;            
+        self.mTimeInfo.mSplit.add_dataset_indicators(lOutput)
         lOutput.set_index(lTime, inplace=True, drop=False);
-        # print(lOutput[lTime].dtype);
+        # tsutil.print_pyaf_detailed_info(lOutput[lTime].dtype);
 
         # Add more informative title for this plot.  Investigate Model Esthetics for PyAF #212 
         lTitle = self.get_title_details_for_plots("Prediction Intervals")
-        tsplot.prediction_interval_plot(lOutput,
-                                        lTime, self.mOriginalSignal,
-                                        lForecastColumn,
-                                        lForecastColumn + '_Lower_Bound',
-                                        lForecastColumn + '_Upper_Bound',
-                                        name = name,
-                                        format= format, horizon = self.mTimeInfo.mHorizon,
-                                        title = lTitle);
+        if(self.mTimeInfo.mOptions.mAddPredictionIntervals):
+            tsplot.prediction_interval_plot(lOutput,
+                                            lTime, self.mOriginalSignal,
+                                            lForecastColumn,
+                                            lForecastColumn + '_Lower_Bound',
+                                            lForecastColumn + '_Upper_Bound',
+                                            name = name,
+                                            format= format, horizon = self.mTimeInfo.mHorizon,
+                                            title = lTitle);
         
         if(self.mTimeInfo.mOptions.mAddPredictionIntervals):
-            lQuantiles = self.mPredictionIntervalsEstimator.mForecastPerformances[lForecastColumn + "_1"].mErrorQuantiles.keys()
+            lQuantiles = self.mPredictionIntervalsEstimator.mPerformances["whole"][tscut.eDatasetType.Forecast][lForecastColumn + "_1"].mErrorQuantiles.keys()
             lQuantiles = sorted(lQuantiles)
             tsplot.quantiles_plot(lOutput,
                                   lTime, self.mOriginalSignal,
                                   lForecastColumn  ,
                                   lQuantiles,
                                   name = name,
                                   format= format,
@@ -482,18 +516,19 @@
         lDict["Prediction_Intervals"] = self.getPredictionIntervalPlot(df)
         if(self.mTimeInfo.mOptions.mAddPredictionIntervals):            
             lDict["Forecast_Quantiles"] = self.getForecastQuantilesPlot(df)
         return lDict;
 
     def getPredictionIntervalPlot(self, df = None):        
         lOutput = df if df is not None else self.getForecastDatasetForPlots();
-        # print(lOutput.columns)
+        # tsutil.print_pyaf_detailed_info(lOutput.columns)
         lPrefix = str(self.mOriginalSignal) + "_";
         lForecastColumn = lPrefix + 'Forecast';
         lTime = self.mTimeInfo.mTime;
+        self.mTimeInfo.mSplit.add_dataset_indicators(lOutput)
         lOutput.set_index(lTime, inplace=True, drop=False);
         # Add more informative title for this plot.  Investigate Model Esthetics for PyAF #212 
         lTitle = self.get_title_details_for_plots("Prediction Intervals")
         return tsplot.prediction_interval_plot_as_png_base64(lOutput,
                                                              lTime, self.mOriginalSignal,
                                                              lForecastColumn  ,
                                                              lForecastColumn + '_Lower_Bound',
@@ -503,15 +538,15 @@
                                                              title = lTitle);
     
     def getForecastQuantilesPlot(self, df = None):
         lOutput = df if df is not None else self.getForecastDatasetForPlots();
         lPrefix = self.mOriginalSignal + "_";
         lTime = self.mTime;
         lForecastColumn = lPrefix + 'Forecast';
-        lQuantiles = self.mPredictionIntervalsEstimator.mForecastPerformances[lForecastColumn + "_1"].mErrorQuantiles.keys()
+        lQuantiles = self.mPredictionIntervalsEstimator.mPerformances["whole"][tscut.eDatasetType.Forecast][lForecastColumn + "_1"].mErrorQuantiles.keys()
         lQuantiles = sorted(lQuantiles)
         return tsplot.quantiles_plot_as_png_base64(lOutput,
                                                    lTime, self.mOriginalSignal,
                                                    lForecastColumn  ,
                                                    lQuantiles,
                                                    name = "Forecast_Quantiles [" + self.mOutName + "]",
                                                    format= format,
@@ -520,9 +555,9 @@
 
     def getVersions(self):
         lVersionDict = tsutil.getVersions();
         return lVersionDict;
 
     def clean_dataframes(self):
         self.mTrend.mSignalFrame = self.mTrend.mSignalFrame[[self.mTime, self.mOriginalSignal, self.mSignal]].copy()
-        # print(self.mTrend.mSignalFrame.columns)
+        # tsutil.print_pyaf_detailed_info(self.mTrend.mSignalFrame.columns)
```

## pyaf/TS/TimeSeries_Cutting.py

```diff
@@ -2,17 +2,24 @@
 # All rights reserved.
 
 # This file is part of the Python Automatic Forecasting (PyAF) library and is made available under
 # the terms of the 3 Clause BSD license
 
 import pandas as pd
 import numpy as np
+from enum import IntEnum
 
 from . import Utils as tsutil
 
+class eDatasetType(IntEnum):
+    Fit = 1
+    Forecast = 2
+    Test = 3
+
+
 class cCuttingInfo:
     def __init__(self):
         pass
 
 
     def estimate(self):
         self.defineCuttingParameters();
@@ -69,42 +76,51 @@
         self.mValidStart = self.mEstimEnd;
         self.mValidEnd = self.mValidStart + lValSize;
         self.mTestStart = self.mValidEnd;
         self.mTestEnd = self.mTestStart + lTestSize;
         
     def defineCuttingParameters(self):
         lStr = "CUTTING_START SignalVariable='" + self.mSignal +"'";
-        # print(lStr);
-        #print(self.mSignalFrame.head())
+        # tsutil.print_pyaf_detailed_info(lStr);
+        # tsutil.print_pyaf_detailed_info(self.mSignalFrame.head())
         if(self.mOptions.mCustomSplit is not None):
             self.set_split(self.mOptions.mCustomSplit)
         else:
             self.set_default_split()
 
         lStr = "CUTTING_PARAMETERS " + str(self.mTrainSize) + " Estimation = (" + str(self.mEstimStart) + " , " + str(self.mEstimEnd) + ")";
         lStr += " Validation = (" + str(self.mValidStart) + " , " + str(self.mValidEnd) + ")";
         lStr += " Test = (" + str(self.mTestStart) + " , " + str(self.mTestEnd) + ")";
-        #print(lStr);
+        # tsutil.print_pyaf_detailed_info(lStr);
         
         pass
 
     def cutFrame(self, df):
-        lFrameFit = df[self.mEstimStart : self.mEstimEnd];
-        lFrameForecast = df[self.mValidStart : self.mValidEnd];
-        lFrameTest = df[self.mTestStart : self.mTestEnd];
-        return (lFrameFit, lFrameForecast, lFrameTest)
+        lDict = {
+            eDatasetType.Fit : df[self.mEstimStart : self.mEstimEnd],
+            eDatasetType.Forecast : df[self.mValidStart : self.mValidEnd],
+            eDatasetType.Test : df[self.mTestStart : self.mTestEnd]
+        }
+        return lDict
 
     def getEstimPart(self, df):
         lFrameFit = df[self.mEstimStart : self.mEstimEnd];
         return lFrameFit;
 
     def getValidPart(self, df):
         lFrameValid = df[self.mValidStart : self.mValidEnd];
         return lFrameValid;
 
+    def add_dataset_indicators(self, df):
+        lCutting = self.cutFrame(df)
+        for (lDataset, lFrame) in lCutting.items():
+            lColumnName = "dataset_indicator_" + lDataset.name
+            df[lColumnName] = np.nan
+            df.loc[lFrame.index, lColumnName] = 1.0
+        return df
 
     def info(self):
         lStr2 += " Estimation = (" + str(self.mEstimStart) + " , " + str(self.mEstimEnd) + ")";
         lStr2 += " Validation = (" + str(self.mValidStart) + " , " + str(self.mValidEnd) + ")";
         lStr2 += " Test = (" + str(self.mTestStart) + " , " + str(self.mTestEnd) + ")";
         lStr2 += " Horizon=" + str(self.mHorizon) +"";
         return lStr2;
```

## pyaf/TS/Utils.py

```diff
@@ -18,15 +18,15 @@
 
 
 class cMemoize:
     def __init__(self, f):
         self.mFunction = f
         self.mCache = {}
     def __call__(self, *args):
-        # print("MEMOIZING" , self.mFunction , args)
+        # tsutil.print_pyaf_detailed_info("MEMOIZING" , self.mFunction , args)
         if not args in self.mCache:
             self.mCache[args] = self.mFunction(*args)
         return self.mCache[args]
     
     def __get__(self, obj, objtype):
         # Support instance methods.
         return partial(self.__call__, obj)
@@ -57,45 +57,54 @@
     import logging;
     logger = logging.getLogger('pyaf.std');
     if(logger.handlers == []):
         import logging.config
         logging.basicConfig(level=logging.INFO)        
     return logger;
 
+def print_pyaf_detailed_info(*args, **kwargs):
+    import logging;
+    logger = logging.getLogger('pyaf.detailed');
+    logger.setLevel(logging.DEBUG) # LOG EVERYTHING
+    logger.log(logging.DEBUG, "DETAIL_MESSAGE" + str(args))
+
 def get_pyaf_timing_logger():
     import logging;
     logger = logging.getLogger('pyaf.timing');
     if(logger.handlers == []):
         import logging.config
         logging.basicConfig(level=logging.INFO)        
     return logger;
 
 def get_pyaf_hierarchical_logger():
     import logging;
     logger = logging.getLogger('pyaf.hierarchical');
     return logger;
 
-
+def activate_timer_logging():
+    import logging;
+    logger = logging.getLogger('pyaf.timing');
+    logger.setLevel(logging.DEBUG)
 
 class cTimer:
     def __init__(self, iMess = "PYAF_UNKNOWN_OP", iDebug = False):
         self.mMessage = iMess
         self.mStart = datetime.now();
         self.logger = get_pyaf_timing_logger();
-        self.logger.info(("OPERATION_START", self.mMessage))
+        self.logger.debug(("OPERATION_START", self.mMessage))
 
     def get_elapsed_time(self):
         lDelta = datetime.now() - self.mStart
         lDelta = round(lDelta.total_seconds(), 3)
         return lDelta
 
     def __del__(self):
         self.mEnd = datetime.now();
         lDelta = self.get_elapsed_time()
-        self.logger.info(("OPERATION_END_ELAPSED" , lDelta, self.mMessage))
+        self.logger.debug(("OPERATION_END_ELAPSED" , lDelta, self.mMessage))
 
 def get_module_version_when_available(module_name):
     try:
         import sys # importlib
         # mod = importlib.import_module(module_name)
         mod = sys.modules[module_name]
         return mod.__version__
@@ -119,9 +128,9 @@
     import sys
     # Limit this list to the already imported/used modules only.
     lModules = [x for x in lModules if x in sys.modules.keys()]
 
     for module_name in lModules:
         lVersionDict[module_name + "_version"] = get_module_version_when_available(module_name)
     
-    # print([(k, lVersionDict[k]) for k in sorted(lVersionDict)]);
+    # tsutil.print_pyaf_detailed_info([(k, lVersionDict[k]) for k in sorted(lVersionDict)]);
     return lVersionDict;
```

## Comparing `pyaf-5.0rc2.dist-info/LICENSE` & `pyaf-5.0rc3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyaf-5.0rc2.dist-info/METADATA` & `pyaf-5.0rc3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaf
-Version: 5.0rc2
+Version: 5.0rc3
 Summary: Python Automatic Forecasting
 Home-page: https://github.com/antoinecarme/pyaf
 Author: Antoine CARME
 Author-email: antoine.carme@outlook.com
 License: BSD 3-clause
 Keywords: arx automatic-forecasting autoregressive benchmark cycle decomposition exogenous forecasting heroku hierarchical-forecasting horizon jupyter pandas python scikit-learn seasonal time-series transformation trend web-service
 Classifier: Development Status :: 5 - Production/Stable
@@ -175,15 +175,15 @@
 
 It can be installed from PyPI for the latest official release:
    
 	pip install pyaf
    
 The development version is also available by executing:
 
-	pip install scipy pandas scikit-learn matplotlib pydot dill sqlalchemy xgboost statsmodels
+	pip install scipy pandas scikit-learn matplotlib pydot xgboost statsmodels
 	pip install --upgrade git+git://github.com/antoinecarme/pyaf.git
 
 
 Development
 -----------
 
 Code contributions are welcome. Bug reports, request for new features and
```

## Comparing `pyaf-5.0rc2.dist-info/RECORD` & `pyaf-5.0rc3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,51 @@
-pyaf/ForecastEngine.py,sha256=TvO8h1oP9ZyJeuXjSPX5LW6N1SwkPgqLN0Xa3nw5_W0,2601
-pyaf/HierarchicalForecastEngine.py,sha256=9VEmE2I8807Ak4zn89rTe9XVHswgg8gJY6erEQ0cl6M,4288
-pyaf/__init__.py,sha256=pLiwBIC6IxscUiS3qrXJllHn2DBdI-CewYgJ4DM6RnQ,475
+pyaf/ForecastEngine.py,sha256=8qQOjRzvdiXoIvV_2LYjRNd8dUpUc95vHRMhElar59U,2286
+pyaf/HierarchicalForecastEngine.py,sha256=rBq-h5FBvBukQEeZAqGXLl1dNxaoGaH5XjGl1fouAKU,3972
+pyaf/__init__.py,sha256=ZjEi8FSiYDRnRz3QKj11eq2nu3Dl_rahA4SQPsSakCQ,576
 pyaf/Bench/Artificial.py,sha256=c4kAAr09Bimv7RGV-L7cRs2vYIU-mwE8pongi2Z2dsU,559
-pyaf/Bench/GenericBenchmark.py,sha256=ozhh2FdsIQKmXGJx-FqCxiTGKu03f0Vcg5k7dkR6gvw,19020
+pyaf/Bench/GenericBenchmark.py,sha256=jsSz214TIZFY_ozZAOt6HPEqT0g7dic7Fa9G5wfezCE,18471
 pyaf/Bench/MComp.py,sha256=CTesgD9jiN6QtOAQj6yNUqGWneItJj-mk4cJ24Dhxbs,773
 pyaf/Bench/NN3.py,sha256=Jz4BAQlNGq1bJs3l4juhWCoeenfcyR8iNdcP22Opnsg,693
-pyaf/Bench/TS_datasets.py,sha256=E6sIa1jrHdCeyFY7eiF_81esjDb1-bAk1AiTeFb3IHM,38915
+pyaf/Bench/TS_datasets.py,sha256=hxD8mLcWGQtQXVGQ64XnhF5iT4cRVh0tHb1ns12JdVA,39004
 pyaf/Bench/YahooStocks.py,sha256=JabK1b2-Z1YCMND0y4VCRe021mhtt3_FCUN9QImZLQs,516
 pyaf/Bench/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyaf/Bench/download_all_stock_prices.py,sha256=kxJoVHh85b1X9OgimYsArjCTuldPxhkm7U0IuCvrl14,341
 pyaf/Bench/stocks_symbol_list.py,sha256=9bjDLUJBFViBbHc0QXqbuU7l3Xe78fADGUCSo9ZscHM,69054
-pyaf/CodeGen/TS_CodeGen_Objects.py,sha256=0ptb0TfBp2ygWNUZIKPLXD3aB6QaJEQn7SYCm-Kd5TI,47821
-pyaf/CodeGen/TS_CodeGenerator.py,sha256=R8Uc4XTFmJ-ilD19iRwMVk-EazbSftAsmDfC6CWUVj8,1877
-pyaf/CodeGen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyaf/TS/Complexity.py,sha256=goc2F7KwdP9gX-DrjKqqcc4jsl--yQ4uJFQxYFbk59M,510
-pyaf/TS/DateTime_Functions.py,sha256=9cHnFJFq25nRAyYa81o85Z2PnP38UUw6WW-ABFStNvY,6748
-pyaf/TS/Exogenous.py,sha256=2wG3UCP1GFg8KQJHvRs1MLXpT1vbJLT5QYgBfI9RR8o,6232
-pyaf/TS/Intermittent_Models.py,sha256=PmCFyLA2AvXdqbYJ3P9GXdqeUoC92ZK0EC04G8kHpI0,6430
+pyaf/TS/DateTime_Functions.py,sha256=W6X5AN1A3kj9cEHb1sxjBwtDDONwUXOIrOaHeHWS3D0,7339
+pyaf/TS/Exogenous.py,sha256=IeOHcQtipTwB0VWtjMp5e-HZ9h-ho-p_FYeVzxkZ7-Y,9827
+pyaf/TS/Intermittent_Models.py,sha256=JY5wl9dYA29MyX77272zZJ5fiCmsC9mRjYJJuGGNu18,6715
 pyaf/TS/Keras_Models.py,sha256=7OIStpfBy8rcYuaDb983lfE89ztn39Oi41P6CnyZdHc,6757
-pyaf/TS/MissingData.py,sha256=zRgjbOqIO9hV37xvQXzPXkore5hmfOq5Ln2eLYcJIgI,4387
-pyaf/TS/ModelSelection_Legacy.py,sha256=ZNrccmgxexVuJKKlTa5Ki17twaGvTXBJwDvb6Lc2I1Y,7378
-pyaf/TS/ModelSelection_Voting.py,sha256=XVO4JOkAeJqZkYeHHBKOtqVqd8ZrTSq-753Z51bIVnI,11568
-pyaf/TS/Options.py,sha256=S0pyPjPqckqP4Ptm3aO4qFjhLlVTzXMTyik0A82BQHE,12893
-pyaf/TS/Perf.py,sha256=W0JLGh-NWZd8Li5a3CypM0Bo-WGi5r0PVxiiQSu9Xds,16910
-pyaf/TS/Plots.py,sha256=X070poNVvoQeQodvxU5wUogw3RXJu1vsTzIBXun6kSw,12670
-pyaf/TS/PredictionIntervals.py,sha256=dsdpZmds6wNgLR4zYAlUBOj1jFOJptQRLTaI0B3mpJc,4542
+pyaf/TS/MissingData.py,sha256=bAzgplX1YSUeTqQIoj0m9_52WEct5KAYjnMHlTd_rww,4876
+pyaf/TS/ModelSelection_Legacy.py,sha256=vq0_eMFaF0i-9PNK04a1VMVs4JKaCZG5_GqurDaLdzQ,7727
+pyaf/TS/ModelSelection_Voting.py,sha256=2agHo0IG1xPsbfRAYGQmNSE9MrnprxOMuRlNL3i8ZmI,11293
+pyaf/TS/Options.py,sha256=-wgmaXs_m5MiFaektNBm-UAdSPS2MV3akrjVkyM3TXc,12097
+pyaf/TS/Perf.py,sha256=j8wb6HJfiYuMREV_SDLTNRBNnISzTOBogA_FLpt6kgw,17092
+pyaf/TS/Plots.py,sha256=VTh3Oq0mgsmqFDYPdrib5-lmQc6SR8UO17WooPM_ZyA,13535
+pyaf/TS/PredictionIntervals.py,sha256=hERgEcxQwHHth-_yjpED_NWcBU8xj6a1Fmp0Y2lDq0g,8552
 pyaf/TS/Pytorch_Models.py,sha256=TeIs_-ch77O6QHCk7fS6mY6bNBGWm9JDcn_-0wYgl8s,8405
-pyaf/TS/Scikit_Models.py,sha256=z8nzXynmE0N0wEIiAlUCQDU1Hr72zYjaUXqV1X_vOgg,10020
-pyaf/TS/SignalDecomposition.py,sha256=TW5U7BWo252-CoP1BASRY_JfIbgfQW5RZWIZkaZiZYA,7280
-pyaf/TS/SignalDecomposition_AR.py,sha256=l6YZ6_bBwrTNUCoV5vMQhlqVC1sKCWk-nqaG1A4hTtY,18240
-pyaf/TS/SignalDecomposition_Cycle.py,sha256=uF3AY2A-AmfnW_4qPfhgT7TVQaClZaPMoH2QzB98y6k,27054
+pyaf/TS/Scikit_Models.py,sha256=yESkHo9boCY-j4rbgEycA1yFbpNYQvgp6fZu-brQJiI,10555
+pyaf/TS/SignalDecomposition.py,sha256=4AXIL4p_-kDbSPLhdFrRDBO4mN7KLzQo56vMvXje1lA,7719
+pyaf/TS/SignalDecomposition_AR.py,sha256=2xf_c-OMVZlOyqtOaAGd-aQv7DIf1nN_iHm88U9gEMM,18596
+pyaf/TS/SignalDecomposition_Cycle.py,sha256=jPDZuGljbt3_OhPOUsaJmIEw4CoipUhzEfCV1a9bg-I,27307
 pyaf/TS/SignalDecomposition_Forecaster.py,sha256=dNBe9DPlZfXxC3oTtvidW8b4xut_aMLEBZae2MvMyFo,3383
-pyaf/TS/SignalDecomposition_Quant.py,sha256=YC6Iy0NITJuB3emLJUauhgooJrcOh3ZwqJD43SQ20aM,886
-pyaf/TS/SignalDecomposition_Trainer.py,sha256=ge5vNIhg1z7M439Jo3Gx7aGRTw6VYS9Ee5fqjwLYzJs,16395
-pyaf/TS/SignalDecomposition_Trend.py,sha256=5kletewd0LTO7evBDvC7_dOFBSa4_XupYE7kyDIM76g,13987
-pyaf/TS/SignalHierarchy.py,sha256=8tXTyUHZ_4CJVBMhqNBEz9GVv5_FctmLJl4775AJySs,25147
-pyaf/TS/Signal_Grouping.py,sha256=BKQZB7bTscadGjLw_uBmk9MX21Yp3fTC0MeJQD00oiQ,3158
-pyaf/TS/Signal_Transformation.py,sha256=hmeQiYnzBXuKTIAFL4uHMGmQgrOFcADfMfjK6yLmWG4,16930
-pyaf/TS/Temporal_Hierarchy.py,sha256=sFtiPVXJVxUDocwXGRAlweDKQuX63AIUOXZsISZLvIc,7269
-pyaf/TS/Time.py,sha256=KW-mzCYK7_PkDDEewiWWyHKDU3DNqyqXtG_W3E2wDHs,7913
-pyaf/TS/TimeSeriesModel.py,sha256=aztErxapzXzFGTSFCT_79MqvI4T4UAEUHTbQYtSvpgA,29365
-pyaf/TS/TimeSeries_Cutting.py,sha256=vJ-9oX9KAYRWz3uwrIqvukfWjherdStpoyqq5PoAv54,4279
-pyaf/TS/Utils.py,sha256=uAvZpR9oIqll6Z3JBdlJaRg39EoT3R96n9G55WCzA3s,3677
+pyaf/TS/SignalDecomposition_Trainer.py,sha256=myoZ4X-uL1FGCFXUmRSe6nwC08kNyWYe_0NxRvo66wo,18323
+pyaf/TS/SignalDecomposition_Trend.py,sha256=D9b4T_8Jm92ntuYMRl-URwRW6OA_lXPefg1VzNJPd4I,13834
+pyaf/TS/SignalHierarchy.py,sha256=t7YEs7JJbSnRp1hgWNJsLZGzSzB91-3LfZOPK5thb7c,27008
+pyaf/TS/Signal_Grouping.py,sha256=5Cg27O5Hwrs1PvRxecGXzQIVi_yFlJTTTRN3vi-hYbs,3314
+pyaf/TS/Signal_Transformation.py,sha256=AawbLWjWZVsVtQBOH0sklCKoaiAh708fm_RUeEvI79o,18016
+pyaf/TS/Temporal_Hierarchy.py,sha256=wiYmaVcqDNMXndSl_w5mvvG-mNQjEYHiw8Ss1hSajqg,7373
+pyaf/TS/Time.py,sha256=KdekJ3ZjO9eDIozqCRF6KCxFsNEU_CYzBkr7Wbt63_M,8867
+pyaf/TS/TimeSeriesModel.py,sha256=tW861RZcGJ5MXE3-PD1aD9QcgdYlUZPRpzeR7e6kBSc,32048
+pyaf/TS/TimeSeries_Cutting.py,sha256=46-76pWYXSuuDe630XpQEAxBe5UVQ5udBqSbWwIS4d4,4784
+pyaf/TS/Utils.py,sha256=xvLf-VILSr4KYgBhYI5E_uk8bBfL3bSeFkU2ux2ktPA,4091
 pyaf/TS/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyaf/WS/WS_Backend.py,sha256=59iHHP9vy9FCn1ec3qInPGYS49bAL_QZlekFIFyEKgc,13735
 pyaf/WS/WS_REST_Flask.py,sha256=8iJogNOMSSUoQ7tbHwDmRB4MUle8WcR-zGVAezktPfE,3518
 pyaf/WS/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyaf/WS/test_heroku_web_service.py,sha256=c4-8peJHvnh7T5KPvJjsJa2027eIjZPLEVq1OAuFPXM,926
-pyaf-5.0rc2.dist-info/AUTHORS.rst,sha256=Xhzh4ffCpVhEqA3n_8I6JvdiLY0AOyep3NVpw_DXRnM,320
-pyaf-5.0rc2.dist-info/LICENSE,sha256=sJTYEQF0ukhsLrmMOePls1_XnT9IPADEwLX95sf56oM,1541
-pyaf-5.0rc2.dist-info/METADATA,sha256=-NK9EDVEx2qYZYfFUcJwW6843dnnvg3RBla8j_WV8nU,13869
-pyaf-5.0rc2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-pyaf-5.0rc2.dist-info/top_level.txt,sha256=iUrQRoSaZLm46bz5I1Ib6dk0Ih-Dsa5dbVce7bum1Os,5
-pyaf-5.0rc2.dist-info/RECORD,,
+pyaf-5.0rc3.dist-info/AUTHORS.rst,sha256=Xhzh4ffCpVhEqA3n_8I6JvdiLY0AOyep3NVpw_DXRnM,320
+pyaf-5.0rc3.dist-info/LICENSE,sha256=sJTYEQF0ukhsLrmMOePls1_XnT9IPADEwLX95sf56oM,1541
+pyaf-5.0rc3.dist-info/METADATA,sha256=eEb5VuPaC9gBw5HV05yTNB9pav1l5G9N0Ot1i75mH7I,13853
+pyaf-5.0rc3.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+pyaf-5.0rc3.dist-info/top_level.txt,sha256=iUrQRoSaZLm46bz5I1Ib6dk0Ih-Dsa5dbVce7bum1Os,5
+pyaf-5.0rc3.dist-info/RECORD,,
```

