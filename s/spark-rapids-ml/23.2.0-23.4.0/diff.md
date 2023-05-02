# Comparing `tmp/spark_rapids_ml-23.2.0-11_ab575bc-py3-none-any.whl.zip` & `tmp/spark_rapids_ml-23.4.0-38_b251734-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 48340 bytes, number of entries: 16
--rw-r--r--  2.0 unx      615 b- defN 23-Mar-31 03:18 spark_rapids_ml/__init__.py
--rw-r--r--  2.0 unx     7537 b- defN 23-Mar-31 03:18 spark_rapids_ml/classification.py
--rw-r--r--  2.0 unx    13898 b- defN 23-Mar-31 03:18 spark_rapids_ml/clustering.py
--rw-r--r--  2.0 unx    29087 b- defN 23-Mar-31 03:18 spark_rapids_ml/core.py
--rw-r--r--  2.0 unx    13614 b- defN 23-Mar-31 03:18 spark_rapids_ml/feature.py
--rw-r--r--  2.0 unx    21944 b- defN 23-Mar-31 03:18 spark_rapids_ml/knn.py
--rw-r--r--  2.0 unx    14846 b- defN 23-Mar-31 03:18 spark_rapids_ml/params.py
--rw-r--r--  2.0 unx    20878 b- defN 23-Mar-31 03:18 spark_rapids_ml/regression.py
--rw-r--r--  2.0 unx    12675 b- defN 23-Mar-31 03:18 spark_rapids_ml/tree.py
--rw-r--r--  2.0 unx     6529 b- defN 23-Mar-31 03:18 spark_rapids_ml/utils.py
--rw-r--r--  2.0 unx      592 b- defN 23-Mar-31 03:18 spark_rapids_ml/common/__init__.py
--rw-r--r--  2.0 unx     5992 b- defN 23-Mar-31 03:18 spark_rapids_ml/common/cuml_context.py
--rw-r--r--  2.0 unx     8539 b- defN 23-Mar-31 04:39 spark_rapids_ml-23.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-31 04:39 spark_rapids_ml-23.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-31 04:39 spark_rapids_ml-23.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1356 b- defN 23-Mar-31 04:39 spark_rapids_ml-23.2.0.dist-info/RECORD
-16 files, 158210 bytes uncompressed, 46108 bytes compressed:  70.9%
+Zip file size: 52237 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      615 b- defN 23-Apr-28 03:47 spark_rapids_ml/__init__.py
+-rw-r--r--  2.0 unx     9944 b- defN 23-Apr-28 03:47 spark_rapids_ml/classification.py
+-rw-r--r--  2.0 unx    13967 b- defN 23-Apr-28 03:47 spark_rapids_ml/clustering.py
+-rw-r--r--  2.0 unx    29140 b- defN 23-Apr-28 03:47 spark_rapids_ml/core.py
+-rw-r--r--  2.0 unx    13432 b- defN 23-Apr-28 03:47 spark_rapids_ml/feature.py
+-rw-r--r--  2.0 unx    24378 b- defN 23-Apr-28 03:47 spark_rapids_ml/knn.py
+-rw-r--r--  2.0 unx    14982 b- defN 23-Apr-28 03:47 spark_rapids_ml/params.py
+-rw-r--r--  2.0 unx    22364 b- defN 23-Apr-28 03:47 spark_rapids_ml/regression.py
+-rw-r--r--  2.0 unx    16334 b- defN 23-Apr-28 03:47 spark_rapids_ml/tree.py
+-rw-r--r--  2.0 unx    12469 b- defN 23-Apr-28 03:47 spark_rapids_ml/utils.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Apr-28 03:47 spark_rapids_ml/common/__init__.py
+-rw-r--r--  2.0 unx     6545 b- defN 23-Apr-28 03:47 spark_rapids_ml/common/cuml_context.py
+-rw-r--r--  2.0 unx     8766 b- defN 23-Apr-28 06:15 spark_rapids_ml-23.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 06:15 spark_rapids_ml-23.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-28 06:15 spark_rapids_ml-23.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1357 b- defN 23-Apr-28 06:15 spark_rapids_ml-23.4.0.dist-info/RECORD
+16 files, 174993 bytes uncompressed, 50005 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: spark_rapids_ml/common/__init__.py
 Comment: 
 
 Filename: spark_rapids_ml/common/cuml_context.py
 Comment: 
 
-Filename: spark_rapids_ml-23.2.0.dist-info/METADATA
+Filename: spark_rapids_ml-23.4.0.dist-info/METADATA
 Comment: 
 
-Filename: spark_rapids_ml-23.2.0.dist-info/WHEEL
+Filename: spark_rapids_ml-23.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: spark_rapids_ml-23.2.0.dist-info/top_level.txt
+Filename: spark_rapids_ml-23.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: spark_rapids_ml-23.2.0.dist-info/RECORD
+Filename: spark_rapids_ml-23.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_rapids_ml/__init__.py

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "23.2.0"
+__version__ = "23.4.0"
```

## spark_rapids_ml/classification.py

```diff
@@ -9,47 +9,68 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Any, Callable, Literal, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple, Type, Union
+
+if TYPE_CHECKING:
+    import cudf
 
-import cudf
 import numpy as np
 import pandas as pd
 from pyspark import Row
-from pyspark.ml.classification import _RandomForestClassifierParams
-from pyspark.ml.param.shared import HasProbabilityCol
+from pyspark.ml.classification import BinaryRandomForestClassificationSummary
+from pyspark.ml.classification import (
+    RandomForestClassificationModel as SparkRandomForestClassificationModel,
+)
+from pyspark.ml.classification import (
+    RandomForestClassificationSummary,
+    _RandomForestClassifierParams,
+)
+from pyspark.ml.linalg import Vector
+from pyspark.ml.param.shared import HasProbabilityCol, HasRawPredictionCol
 from pyspark.sql import Column, DataFrame
 from pyspark.sql.functions import col
 from pyspark.sql.types import DoubleType, FloatType, IntegerType, IntegralType
 
-from spark_rapids_ml.core import CumlT, alias, pred
-from spark_rapids_ml.tree import (
+from .core import CumlT, alias, pred
+from .tree import (
     _RandomForestClass,
     _RandomForestCumlParams,
     _RandomForestEstimator,
     _RandomForestModel,
 )
+from .utils import _get_spark_session
 
 
-class _RFClassifierParams(_RandomForestClassifierParams, HasProbabilityCol):
+class _RFClassifierParams(
+    _RandomForestClassifierParams, HasProbabilityCol, HasRawPredictionCol
+):
     def __init__(self, *args: Any):
         super().__init__(*args)
 
     def setProbabilityCol(
         self: "_RFClassifierParams", value: str
     ) -> "_RFClassifierParams":
         """
         Sets the value of :py:attr:`probabilityCol`.
         """
         return self._set(probabilityCol=value)
 
+    def setRawPredictionCol(
+        self: "_RFClassifierParams", value: str
+    ) -> "_RFClassifierParams":
+        """
+        Sets the value of :py:attr:`rawPredictionCol`.
+        """
+        return self._set(rawPredictionCol=value)
+
 
 class RandomForestClassifier(
     _RandomForestClass,
     _RandomForestEstimator,
     _RandomForestCumlParams,
     _RFClassifierParams,
 ):
@@ -160,33 +181,57 @@
     """
 
     def __init__(
         self,
         n_cols: int,
         dtype: str,
         treelite_model: str,
+        model_json: List[str],
         num_classes: int,
     ):
         super().__init__(
             dtype=dtype,
             n_cols=n_cols,
             treelite_model=treelite_model,
+            model_json=model_json,
             num_classes=num_classes,
         )
         self._num_classes = num_classes
+        self._model_json = model_json
+        self._rf_spark_model: Optional[SparkRandomForestClassificationModel] = None
+
+    def cpu(self) -> SparkRandomForestClassificationModel:
+        """Return the PySpark ML RandomForestClassificationModel"""
+
+        if self._rf_spark_model is None:
+            sc = _get_spark_session().sparkContext
+            assert sc._jvm is not None
+
+            uid, java_trees = self._convert_to_java_trees(self.getImpurity())
+
+            # Create the Spark RandomForestClassificationModel
+            java_rf_model = sc._jvm.org.apache.spark.ml.classification.RandomForestClassificationModel(
+                uid,
+                java_trees,
+                self.numFeatures,
+                self._num_classes,
+            )
+            self._rf_spark_model = SparkRandomForestClassificationModel(java_rf_model)
+            self._copyValues(self._rf_spark_model)
+        return self._rf_spark_model
 
     def _get_cuml_transform_func(
         self, dataset: DataFrame
     ) -> Tuple[
         Callable[..., CumlT],
-        Callable[[CumlT, Union[cudf.DataFrame, np.ndarray]], pd.DataFrame],
+        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
     ]:
         _construct_rf, _ = super()._get_cuml_transform_func(dataset)
 
-        def _predict(rf: CumlT, pdf: Union[cudf.DataFrame, np.ndarray]) -> pd.Series:
+        def _predict(rf: CumlT, pdf: Union["cudf.DataFrame", np.ndarray]) -> pd.Series:
             data = {}
             rf.update_labels = False
             data[pred.prediction] = rf.predict(pdf)
             probs = rf.predict_proba(pdf)
             if isinstance(probs, pd.DataFrame):
                 # For 2302, when input is multi-cols, the output will be DataFrame
                 data[pred.probability] = pd.Series(probs.values.tolist())
@@ -206,7 +251,34 @@
         """Indicates whether a training summary exists for this model instance."""
         return False
 
     @property
     def numClasses(self) -> int:
         """Number of classes (values which the label can take)."""
         return self._num_classes
+
+    def predictRaw(self, value: Vector) -> Vector:
+        """
+        Raw prediction for each possible label.
+        """
+        return self.cpu().predictRaw(value)
+
+    def predictProbability(self, value: Vector) -> Vector:
+        """
+        Predict the probability of each class given the features.
+        """
+        return self.cpu().predictProbability(value)
+
+    def evaluate(
+        self, dataset: DataFrame
+    ) -> Union[
+        BinaryRandomForestClassificationSummary, RandomForestClassificationSummary
+    ]:
+        """
+        Evaluates the model on a test dataset.
+
+        Parameters
+        ----------
+        dataset : :py:class:`pyspark.sql.DataFrame`
+            Test dataset to evaluate model on.
+        """
+        return self.cpu().evaluate(dataset)
```

## spark_rapids_ml/clustering.py

```diff
@@ -10,17 +10,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    cast,
+)
+
+if TYPE_CHECKING:
+    import cudf
 
-import cudf
 import numpy as np
 import pandas as pd
 from pyspark.ml.clustering import KMeansModel as SparkKMeansModel
 from pyspark.ml.clustering import _KMeansParams
 from pyspark.ml.linalg import Vector
 from pyspark.sql.dataframe import DataFrame
 from pyspark.sql.types import (
@@ -29,61 +41,57 @@
     IntegerType,
     Row,
     StringType,
     StructField,
     StructType,
 )
 
-from spark_rapids_ml.core import (
+from .core import (
     CumlInputType,
     CumlT,
     _CumlEstimator,
     _CumlModelSupervised,
     param_alias,
 )
-from spark_rapids_ml.params import HasFeaturesCols, P, _CumlClass, _CumlParams
-from spark_rapids_ml.utils import (
+from .params import HasFeaturesCols, P, _CumlClass, _CumlParams
+from .utils import (
     _ArrayOrder,
     _concat_and_free,
     _get_spark_session,
     get_logger,
     java_uid,
 )
 
 
 class KMeansClass(_CumlClass):
     @classmethod
-    def _cuml_cls(cls) -> List[type]:
-        from cuml import KMeans
-
-        return [KMeans]
-
-    @classmethod
     def _param_mapping(cls) -> Dict[str, Optional[str]]:
         return {
             "distanceMeasure": None,
             "initMode": "init",
             "k": "n_clusters",
             "initSteps": "",
             "maxIter": "max_iter",
             "seed": "random_state",
             "tol": "tol",
             "weightCol": None,
         }
 
-    @classmethod
-    def _param_excludes(cls) -> List[str]:
-        """
-        For some reason, spark-rapids-ml may not support all the parameters.
-        In that case, we need to explicitly exclude them.
-        """
-        return [
-            "handle",
-            "output_type",
-        ]
+    def _get_cuml_params_default(self) -> Dict[str, Any]:
+        return {
+            "n_clusters": 8,
+            "max_iter": 300,
+            "tol": 0.0001,
+            "verbose": False,
+            "random_state": 1,
+            "init": "scalable-k-means++",
+            "n_init": 1,
+            "oversampling_factor": 2.0,
+            "max_samples_per_batch": 32768,
+        }
 
 
 class _KMeansCumlParams(_CumlParams, _KMeansParams, HasFeaturesCols):
     """
     Shared Spark Params for KMeans and KMeansModel.
     """
 
@@ -192,26 +200,28 @@
     |[1.0, 1.0]|         0|
     |[9.0, 8.0]|         1|
     |[8.0, 9.0]|         1|
     +----------+----------+
     >>> gpu_kmeans.save("/tmp/kmeans")
     >>> gpu_model.save("/tmp/kmeans_model")
 
+    >>> # vector column input
     >>> from spark_rapids_ml.clustering import KMeans
     >>> from pyspark.ml.linalg import Vectors
     >>> data = [(Vectors.dense([0.0, 0.0]),),
     ...         (Vectors.dense([1.0, 1.0]),),
     ...         (Vectors.dense([9.0, 8.0]),),
     ...         (Vectors.dense([8.0, 9.0]),),]
     >>> df = spark.createDataFrame(data, ["features"])
     >>> gpu_kmeans = KMeans(k=2).setFeaturesCol("features")
     >>> gpu_kmeans.getFeaturesCol()
     'features'
     >>> gpu_model = gpu_kmeans.fit(df)
 
+    >>> # multi-column input
     >>> data = [(0.0, 0.0),
     ...         (1.0, 1.0),
     ...         (9.0, 8.0),
     ...         (8.0, 9.0),]
     >>> df = spark.createDataFrame(data, ["f1", "f2"])
     >>> gpu_kmeans = KMeans(k=2).setFeaturesCols(["f1", "f2"])
     >>> gpu_kmeans.getFeaturesCols()
@@ -384,15 +394,15 @@
     def _transform_array_order(self) -> _ArrayOrder:
         return "C"
 
     def _get_cuml_transform_func(
         self, dataset: DataFrame
     ) -> Tuple[
         Callable[..., CumlT],
-        Callable[[CumlT, Union[cudf.DataFrame, np.ndarray]], pd.DataFrame],
+        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
     ]:
         cuml_alg_params = self.cuml_params.copy()
 
         cluster_centers_ = self.cluster_centers_
         dtype = self.dtype
         n_cols = self.n_cols
         array_order = self._transform_array_order()
```

## spark_rapids_ml/core.py

```diff
@@ -27,22 +27,26 @@
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
-import cudf
 import numpy as np
 import pandas as pd
 from pyspark import RDD, TaskContext
 from pyspark.ml import Estimator, Model
 from pyspark.ml.functions import array_to_vector, vector_to_array
 from pyspark.ml.linalg import VectorUDT
-from pyspark.ml.param.shared import HasLabelCol, HasPredictionCol
+from pyspark.ml.param.shared import (
+    HasLabelCol,
+    HasOutputCol,
+    HasPredictionCol,
+    HasProbabilityCol,
+)
 from pyspark.ml.util import (
     DefaultParamsReader,
     DefaultParamsWriter,
     MLReadable,
     MLReader,
     MLWritable,
     MLWriter,
@@ -55,26 +59,27 @@
     DoubleType,
     FloatType,
     IntegralType,
     Row,
     StructType,
 )
 
-from spark_rapids_ml.common.cuml_context import CumlContext
-from spark_rapids_ml.params import _CumlParams
-from spark_rapids_ml.utils import (
+from .common.cuml_context import CumlContext
+from .params import _CumlParams
+from .utils import (
     _ArrayOrder,
     _get_gpu_id,
     _get_spark_session,
     _is_local,
     dtype_to_pyspark_type,
     get_logger,
 )
 
 if TYPE_CHECKING:
+    import cudf
     from cuml.cluster.kmeans_mg import KMeansMG
     from cuml.decomposition.pca_mg import PCAMG
 
     CumlT = TypeVar("CumlT", PCAMG, KMeansMG)
 else:
     CumlT = Any
 
@@ -604,15 +609,15 @@
         return cls(**attr_dict)
 
     @abstractmethod
     def _get_cuml_transform_func(
         self, dataset: DataFrame
     ) -> Tuple[
         Callable[..., CumlT],
-        Callable[[CumlT, Union[cudf.DataFrame, np.ndarray]], pd.DataFrame],
+        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
     ]:
         """
         Subclass must implement this function to return two functions,
         1. a function to construct cuml counterpart instance
         2. a function to transform the dataset
 
         Eg,
@@ -746,25 +751,25 @@
         elif isinstance(schema, StructType):
             return False if len(schema.names) > 1 else True
 
     def _has_probability_col(self) -> bool:
         """This API is needed and can be overwritten by subclass which
         hasn't implemented predict probability yet"""
 
-        return (
-            True
-            if self.hasParam("probabilityCol") and self.isDefined("probabilityCol")
-            else False
-        )
+        return True if isinstance(self, HasProbabilityCol) else False
 
-    @abstractmethod
     def _get_prediction_name(self) -> str:
         """Different algos have different prediction names,
         eg, PCA: value of outputCol param, RF/LR/Kmeans: value of predictionCol name"""
-        raise NotImplementedError()
+        if isinstance(self, HasPredictionCol):
+            return self.getPredictionCol()
+        elif isinstance(self, HasOutputCol):
+            return self.getOutputCol()
+        else:
+            raise ValueError("Please set predictionCol or outputCol")
 
     def _transform(self, dataset: DataFrame) -> DataFrame:
         """This version of transform is directly adding extra columns to the dataset"""
         dataset, select_cols, input_is_multi_cols = self._pre_process_data(dataset)
 
         is_local = _is_local(_get_spark_session().sparkContext)
 
@@ -843,10 +848,7 @@
     def numFeatures(self) -> int:
         """
         Returns the number of features the model was trained on. If unknown, returns -1
         """
 
         num_features = self.n_cols if self.n_cols else -1
         return num_features
-
-    def _get_prediction_name(self) -> str:
-        return self.getPredictionCol()
```

## spark_rapids_ml/feature.py

```diff
@@ -11,20 +11,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import itertools
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
+
+if TYPE_CHECKING:
+    import cudf
 
-import cudf
 import numpy as np
 import pandas as pd
-from pyspark.ml import Model
 from pyspark.ml.common import _py2java
 from pyspark.ml.feature import PCAModel as SparkPCAModel
 from pyspark.ml.feature import _PCAParams
 from pyspark.ml.linalg import DenseMatrix, DenseVector
 from pyspark.ml.param.shared import HasInputCols
 from pyspark.sql.dataframe import DataFrame
 from pyspark.sql.types import (
@@ -33,51 +34,42 @@
     IntegerType,
     Row,
     StringType,
     StructField,
     StructType,
 )
 
-from spark_rapids_ml.core import (
+from .core import (
     CumlInputType,
     CumlT,
     _CumlEstimator,
     _CumlModelWithColumns,
     param_alias,
 )
-from spark_rapids_ml.params import P, _CumlClass, _CumlParams
-from spark_rapids_ml.utils import (
+from .params import P, _CumlClass, _CumlParams
+from .utils import (
     PartitionDescriptor,
     _get_spark_session,
     dtype_to_pyspark_type,
     java_uid,
 )
 
 
 class PCAClass(_CumlClass):
     @classmethod
-    def _cuml_cls(cls) -> List[type]:
-        from cuml import PCA
-
-        return [PCA]
-
-    @classmethod
     def _param_mapping(cls) -> Dict[str, Optional[str]]:
         return {"k": "n_components"}
 
-    @classmethod
-    def _param_excludes(cls) -> List[str]:
-        return [
-            "copy",
-            "handle",
-            "iterated_power",
-            "output_type",
-            "random_state",
-            "tol",
-        ]
+    def _get_cuml_params_default(self) -> Dict[str, Any]:
+        return {
+            "n_components": None,
+            "svd_solver": "auto",
+            "verbose": False,
+            "whiten": False,
+        }
 
 
 class _PCACumlParams(_CumlParams, _PCAParams, HasInputCols):
     """
     Shared Spark Params for PCA and PCAModel.
     """
 
@@ -146,24 +138,26 @@
     >>> print(gpu_model.pc)
     DenseMatrix([[0.70710678],
                  [0.70710678]])
     >>> print(gpu_model.explainedVariance)
     [1.0]
     >>> gpu_pca.save("/tmp/pca")
 
+    >>> # vector column input
     >>> from pyspark.ml.linalg import Vectors
     >>> data = [(Vectors.dense([1.0, 1.0]),),
     ...         (Vectors.dense([2.0, 2.0]),),
     ...         (Vectors.dense([3.0, 3.0]),),]
     >>> df = spark.createDataFrame(data, ["features"])
     >>> gpu_pca = PCA(k=1).setInputCol("features")
     >>> gpu_pca.getInputCol()
     'features'
     >>> gpu_model = gpu_pca.fit(df)
 
+    >>> # multi-column input
     >>> data = [(1.0, 1.0),
     ...         (2.0, 2.0),
     ...         (3.0, 3.0),]
     >>> df = spark.createDataFrame(data, ["f1", "f2"])
     >>> gpu_pca = PCA(k=1).setInputCols(["f1", "f2"])
     >>> gpu_pca.getInputCols()
     ['f1', 'f2']
@@ -338,22 +332,19 @@
                 java_uid(sc, "pca"), java_pc, java_explainedVariance
             )
             self._pca_ml_model = SparkPCAModel(java_model)
             self._copyValues(self._pca_ml_model)
 
         return self._pca_ml_model
 
-    def _get_prediction_name(self) -> str:
-        return self.getOutputCol()
-
     def _get_cuml_transform_func(
         self, dataset: DataFrame
     ) -> Tuple[
         Callable[..., CumlT],
-        Callable[[CumlT, Union[cudf.DataFrame, np.ndarray]], pd.DataFrame],
+        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
     ]:
         cuml_alg_params = self.cuml_params.copy()
 
         n_cols = self.n_cols
         dype = self.dtype
         components = self.components_
         mean = self.mean_
```

## spark_rapids_ml/knn.py

```diff
@@ -11,80 +11,74 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import asyncio
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
+
+if TYPE_CHECKING:
+    import cudf
 
-import cudf
 import numpy as np
 import pandas as pd
 from pyspark.ml.functions import vector_to_array
 from pyspark.ml.linalg import VectorUDT
 from pyspark.ml.param.shared import (
     HasInputCol,
     HasInputCols,
     HasLabelCol,
     Param,
     Params,
     TypeConverters,
 )
+from pyspark.ml.util import MLReader, MLWriter
 from pyspark.sql import Column, DataFrame
-from pyspark.sql.functions import col, lit
+from pyspark.sql.functions import col, lit, monotonically_increasing_id
 from pyspark.sql.types import (
     ArrayType,
     DoubleType,
     FloatType,
     LongType,
     Row,
     StructField,
     StructType,
 )
 
-from spark_rapids_ml.core import (
+from .core import (
     CumlInputType,
     CumlT,
     _CumlCaller,
     _CumlEstimatorSupervised,
     _CumlModel,
     alias,
     param_alias,
 )
-from spark_rapids_ml.params import P, _CumlClass, _CumlParams
-from spark_rapids_ml.utils import _concat_and_free
+from .params import P, _CumlClass, _CumlParams
+from .utils import _concat_and_free
 
 
 class NearestNeighborsClass(_CumlClass):
     @classmethod
-    def _cuml_cls(cls) -> List[type]:
-        from cuml import NearestNeighbors as cumlNearestNeighbors
-        from cuml.neighbors.nearest_neighbors_mg import (
-            NearestNeighborsMG,  # to include the batch_size parameter that exists in the MG class
-        )
-
-        return [cumlNearestNeighbors, NearestNeighborsMG]
-
-    @classmethod
     def _param_mapping(cls) -> Dict[str, Optional[str]]:
         return {"k": "n_neighbors"}
 
-    @classmethod
-    def _param_excludes(cls) -> List[str]:
-        return [
-            "handle",
-            "algorithm",
-            "metric",
-            "p",
-            "algo_params",
-            "metric_expanded",
-            "metric_params",
-            "output_type",
-        ]
+    def _get_cuml_params_default(self) -> Dict[str, Any]:
+        return {"n_neighbors": 5, "verbose": False, "batch_size": 2000000}
 
 
 class _NearestNeighborsCumlParams(_CumlParams, HasInputCol, HasLabelCol, HasInputCols):
     """
     Shared Spark Params for NearestNeighbor and NearestNeighborModel.
     """
 
@@ -127,15 +121,15 @@
         """
         Sets the value of :py:attr:`inputCols`. Used when input vectors are stored as multiple feature columns.
         """
         return self.set_params(inputCols=value)
 
     def setIdCol(self: P, value: str) -> P:
         """
-        Sets the value of `id_col`. If not set, an id column will be added with column name `id`. The id column is used to specify nearest neighbor vectors by associated id value.
+        Sets the value of `id_col`. If not set, an id column will be added with column name `unique_id`. The id column is used to specify nearest neighbor vectors by associated id value.
         """
         self.set_params(id_col=value)
         return self
 
     def getIdCol(self) -> str:
         """
         Gets the value of `id_col`.
@@ -148,37 +142,53 @@
         """
         if not self.isSet("id_col") and self.getIdCol() in df.columns:
             raise ValueError(
                 f"Cannot create a default id column since a column with the default name '{self.getIdCol()}' already exists."
                 + "Please specify an id column"
             )
 
+        id_col_name = self.getIdCol()
         df_withid = (
-            df if self.isSet("id_col") else self._df_zip_with_index(df, self.getIdCol())
+            df
+            if self.isSet("id_col")
+            else df.select(monotonically_increasing_id().alias(id_col_name), "*")
         )
         return df_withid
 
-    @staticmethod
-    def _df_zip_with_index(df: DataFrame, id_col_name: str) -> DataFrame:
-        """
-        Add a row number column (or equivalently id column) to df using zipWithIndex. Used when id_col is not set.
-        TODO: May replace zipWithIndex with monotonically_increasing_id if row number does not have to consecutive.
-        """
-        out_schema = StructType(
-            [StructField(id_col_name, LongType(), False)] + df.schema.fields
-        )
-        zipped_rdd = df.rdd.zipWithIndex()
-        new_rdd = zipped_rdd.map(lambda row: [row[1]] + list(row[0]))
-        return new_rdd.toDF(schema=out_schema)
-
 
 class NearestNeighbors(
     NearestNeighborsClass, _CumlEstimatorSupervised, _NearestNeighborsCumlParams
 ):
     """
+    NearestNeighbors retrieves the exact k nearest neighbors in item vectors for each
+    query vector. The main methods accept distributed CPU dataframes as inputs,
+    leverage GPUs to accelerate computation, and take care of communication and
+    aggregation automatically. However, it should be noted that only the euclidean
+    distance (also known as L2 distance) is supported in the current implementations
+    and the feature data type must be of the float type. All other data types will
+    be converted into float during computation.
+
+    Parameters
+    ----------
+    k: int (default = 5)
+        the default number nearest neighbors to retrieve for each query.
+
+    inputCol: str
+        the name of the column that contains input vectors. inputCol should be set when feature vectors
+        are stored in a single column of a dataframe.
+
+    inputCols: List[str]
+        the names of feature columns that form input vectors. inputCols should be set when input vectors
+        are stored as multiple feature columns of a dataframe.
+
+    idCol: str
+        the name of the column in a dataframe that uniquely identifies each vector. idCol should be set
+        if such a column exists in the dataframe. If idCol is not set, a column with the name `unique_id`
+        will be automatically added to the dataframe and used as unique identifier for each vector.
+
     Examples
     --------
     >>> from spark_rapids_ml.knn import NearestNeighbors
     >>> data = [(0, [1.0, 1.0]),
     ...         (1, [2.0, 2.0]),
     ...         (2, [3.0, 3.0]),]
     >>> data_df = spark.createDataFrame(data, schema="id int, features array<float>")
@@ -217,14 +227,41 @@
     |        item_df|       query_df|EuclideanDistance|
     +---------------+---------------+-----------------+
     |{1, [2.0, 2.0]}|{3, [1.0, 1.0]}|        1.4142135|
     |{0, [1.0, 1.0]}|{3, [1.0, 1.0]}|              0.0|
     |{2, [3.0, 3.0]}|{4, [3.0, 3.0]}|              0.0|
     |{1, [2.0, 2.0]}|{4, [3.0, 3.0]}|        1.4142135|
     +---------------+---------------+-----------------+
+
+    >>> # vector column input
+    >>> from spark_rapids_ml.knn import NearestNeighbors
+    >>> from pyspark.ml.linalg import Vectors
+    >>> data = [(0, Vectors.dense([1.0, 1.0]),),
+    ...         (1, Vectors.dense([2.0, 2.0]),),
+    ...         (2, Vectors.dense([3.0, 3.0]),)]
+    >>> data_df = spark.createDataFrame(data, ["id", "features"])
+    >>> query = [(3, Vectors.dense([1.0, 1.0]),),
+    ...          (4, Vectors.dense([3.0, 3.0]),)]
+    >>> query_df = spark.createDataFrame(query, ["id", "features"])
+    >>> topk = 2
+    >>> gpu_knn = NearestNeighbors().setInputCol("features").setIdCol("id").setK(topk)
+    >>> gpu_model = gpu_knn.fit(data_df)
+
+    >>> # multi-column input
+    >>> from spark_rapids_ml.knn import NearestNeighbors
+    >>> data = [(0, 1.0, 1.0),
+    ...         (1, 2.0, 2.0),
+    ...         (2, 3.0, 3.0),]
+    >>> data_df = spark.createDataFrame(data, schema="id int, f1 float, f2 float")
+    >>> query = [(3, 1.0, 1.0),
+    ...          (4, 3.0, 3.0),]
+    >>> query_df = spark.createDataFrame(query, schema="id int, f1 float, f2 float")
+    >>> topk = 2
+    >>> gpu_knn = NearestNeighbors().setInputCols(["f1", "f2"]).setIdCol("id").setK(topk)
+    >>> gpu_model = gpu_knn.fit(data_df)
     """
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__()
         self.set_params(**kwargs)
         self._label_isdata = 0
         self._label_isquery = 1
@@ -264,14 +301,25 @@
         self, dataset: DataFrame
     ) -> Callable[[CumlInputType, Dict[str, Any]], Dict[str, Any],]:
         """
         This class overrides _fit and will not call _get_cuml_fit_func.
         """
         pass
 
+    def write(self) -> MLWriter:
+        raise NotImplementedError(
+            "NearestNeighbors does not support saving/loading, just re-create the estimator."
+        )
+
+    @classmethod
+    def read(cls) -> MLReader:
+        raise NotImplementedError(
+            "NearestNeighbors does not support saving/loading, just re-create the estimator."
+        )
+
 
 class NearestNeighborsModel(
     _CumlCaller, _CumlModel, NearestNeighborsClass, _NearestNeighborsCumlParams
 ):
     def __init__(
         self,
         item_df_withid: DataFrame,
@@ -519,15 +567,15 @@
             "NearestNeighborsModel does not provide a transform function. Use 'kneighbors' instead."
         )
 
     def _get_cuml_transform_func(
         self, dataset: DataFrame
     ) -> Tuple[
         Callable[..., CumlT],
-        Callable[[CumlT, Union[cudf.DataFrame, np.ndarray]], pd.DataFrame],
+        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
     ]:
         raise NotImplementedError(
             "'_CumlModel._get_cuml_transform_func' method is not implemented. Use 'kneighbors' instead."
         )
 
     def exactNearestNeighborsJoin(
         self,
@@ -594,7 +642,18 @@
             knnjoin_df = knnjoin_df.select(
                 knnjoin_df["item_df"].dropFields(id_col_name).alias("item_df"),
                 knnjoin_df["query_df"].dropFields(id_col_name).alias("query_df"),
                 distCol,
             )
 
         return knnjoin_df
+
+    def write(self) -> MLWriter:
+        raise NotImplementedError(
+            "NearestNeighborsModel does not support saving/loading, just re-fit the estimator to re-create a model."
+        )
+
+    @classmethod
+    def read(cls) -> MLReader:
+        raise NotImplementedError(
+            "NearestNeighborsModel does not support loading/loading, just re-fit the estimator to re-create a model."
+        )
```

## spark_rapids_ml/params.py

```diff
@@ -1,14 +1,30 @@
-from typing import Any, Dict, List, Optional, Tuple, TypeVar, Union
+#
+# Copyright (c) 2023, NVIDIA CORPORATION.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
+from abc import abstractmethod
+from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
-import cupy
 from pyspark.ml.param import Param, Params, TypeConverters
 from pyspark.sql import SparkSession
 
-from spark_rapids_ml.utils import _get_default_params_from_func, _is_local
+from .utils import _is_local
 
 P = TypeVar("P", bound="_CumlParams")
 
 
 class HasFeaturesCols(Params):
     """
     Mixin for param featuresCols: features column names for multi-column input.
@@ -35,41 +51,14 @@
     """
     Base class for all _CumlEstimator and _CumlModel implemenations.
 
     Defines helper methods for mapping Spark ML Params to cuML class parameters.
     """
 
     @classmethod
-    def _cuml_cls(cls) -> List[type]:
-        """
-        Return a list of cuML python counterpart class names, which will be used to
-        auto-generate Spark params.
-        """
-        raise NotImplementedError
-
-    @classmethod
-    def _param_excludes(cls) -> List[str]:
-        """
-        Return a list of cuML class parameters which should not be auto-populated into the
-        Spark class.
-
-        Example
-        -------
-
-        .. code-block::python
-
-            return [
-                "handle",
-                "output_type",
-            ]
-
-        """
-        return []
-
-    @classmethod
     def _param_mapping(cls) -> Dict[str, Optional[str]]:
         """
         Return a mapping of Spark ML Param names to cuML parameter names, which is used maintain
         associations from Spark params to cuML parameters.
 
         If the Spark Param has no equivalent cuML parameter, the cuML name can be set to:
         - empty string, if a defined Spark Param should just be silently ignored, or
@@ -93,55 +82,57 @@
                 "tol": "tol",
                 "weightCol": None,
             }
         """
         return {}
 
     @classmethod
-    def _param_value_mapping(cls) -> Dict[str, Dict[str, Union[str, None]]]:
+    def _param_value_mapping(
+        cls,
+    ) -> Dict[str, Callable[[str], Union[None, str, float, int]]]:
         """
-        Return a dictionary of cuML parameter names and their mapping of Spark ML Param string
-        values to cuML string values.
+        Return a dictionary of cuML parameter names and a function mapping their Spark ML Param string
+        values to cuML values of either str, float, or int type.
 
-        If the mapped value is None, then the Spark value is unsupported, and an error will be
-        raised.
+        The mapped function should accept all string inputs and return None for any unmapped input values.
+
+        If it is desired that a cuML string value be accepted as a valid input, it must be explicitly mapped to
+        itself in the function (see "squared_loss" and "eig" in example below).
 
         Example
         -------
 
         .. code-block:: python
 
             # For LinearRegression
             return {
-                "loss": {
+                "loss": lambda x: {
                     "squaredError": "squared_loss",
                     "huber": None,
-                },
-                "solver": {
+                    "squared_loss": "squared_loss",
+                }.get(x, None),
+                "solver": lambda x: {
                     "auto": "eig",
                     "normal": "eig",
                     "l-bfgs": None,
-                }
+                    "eig": "eig",
+                }.get(x, None),
             }
 
         """
         return {}
 
-    @classmethod
-    def _get_cuml_params_default(cls) -> Dict[str, Any]:
-        """
-        Inspect the __init__ function of associated _cuml_cls() to return a dictionary of
-        parameter names and their default values.
-        """
-        params = {}
-        for cls_type in cls._cuml_cls():
-            params.update(
-                _get_default_params_from_func(cls_type, cls._param_excludes())
-            )
-        return params
+    @abstractmethod
+    def _get_cuml_params_default(self) -> Dict[str, Any]:
+        """Return a dictionary of parameter names and their default values.
+
+        Note, please don't import cuml class and inspect the signatures to
+        get the parameters, since it may break the rule that spark-rapids-ml should
+        run on the driver side without rapids dependencies"""
+        raise NotImplementedError()
 
 
 class _CumlParams(_CumlClass, Params):
     """
     Mix-in to handle common parameters for all Spark Rapids ML algorithms, along with utilties
     for synchronizing between Spark ML Params and cuML class parameters.
     """
@@ -307,28 +298,31 @@
         num_workers = 1
         try:
             spark = SparkSession.getActiveSession()
             if spark:
                 sc = spark.sparkContext
                 if _is_local(sc):
                     # assume using all local GPUs for Spark local mode
+                    # TODO suggest using more CPUs (e.g. local[*]) if number of GPUs > number of CPUs
+                    import cupy
+
                     num_workers = cupy.cuda.runtime.getDeviceCount()
                 else:
                     num_executors = int(
-                        spark.conf.get("spark.executor.instances", "-1")
+                        spark.conf.get("spark.executor.instances", "-1")  # type: ignore
                     )
                     if num_executors == -1:
                         jsc = spark.sparkContext._jsc.sc()
                         num_executors = len(jsc.statusTracker().getExecutorInfos()) - 1
 
                     gpus_per_executor = float(
-                        spark.conf.get("spark.executor.resource.gpu.amount", "1")
+                        spark.conf.get("spark.executor.resource.gpu.amount", "1")  # type: ignore
                     )
                     gpus_per_task = float(
-                        spark.conf.get("spark.task.resource.gpu.amount", "1")
+                        spark.conf.get("spark.task.resource.gpu.amount", "1")  # type: ignore
                     )
 
                     if gpus_per_task != 1:
                         msg = (
                             "WARNING: cuML requires 1 GPU per task, "
                             "'spark.task.resource.gpu.amount' is currently set to {}"
                         )
@@ -402,20 +396,12 @@
         """
         value_map = self._param_value_mapping()
         if k not in value_map:
             # no value mapping required
             self._cuml_params[k] = v
         else:
             # value map exists
-            supported_values = set([x for x in value_map[k].values() if x is not None])
-            if v in supported_values:
-                # already a valid value
-                self._cuml_params[k] = v
+            mapped_v = value_map[k](v)
+            if mapped_v:
+                self._cuml_params[k] = mapped_v
             else:
-                # try to map to a valid value
-                mapped_v = value_map[k].get(v, None)
-                if mapped_v:
-                    self._cuml_params[k] = mapped_v
-                else:
-                    raise ValueError(
-                        f"Value '{v}' for '{k}' param is unsupported, expected: {supported_values}"
-                    )
+                raise ValueError(f"Value '{v}' for '{k}' param is unsupported")
```

## spark_rapids_ml/regression.py

```diff
@@ -8,74 +8,73 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
+
+if TYPE_CHECKING:
+    import cudf
 
-import cudf
 import numpy as np
 import pandas as pd
 from pyspark import Row
 from pyspark.ml.common import _py2java
 from pyspark.ml.linalg import Vector, Vectors, _convert_to_vector
 from pyspark.ml.regression import LinearRegressionModel as SparkLinearRegressionModel
+from pyspark.ml.regression import LinearRegressionSummary
 from pyspark.ml.regression import (
-    LinearRegressionSummary,
-    _LinearRegressionParams,
-    _RandomForestRegressorParams,
+    RandomForestRegressionModel as SparkRandomForestRegressionModel,
 )
+from pyspark.ml.regression import _LinearRegressionParams, _RandomForestRegressorParams
 from pyspark.sql import Column, DataFrame
 from pyspark.sql.types import (
     ArrayType,
     DoubleType,
     FloatType,
     IntegerType,
     StringType,
     StructField,
     StructType,
 )
 
-from spark_rapids_ml.core import (
+from .core import (
     CumlInputType,
     CumlT,
     _CumlEstimatorSupervised,
     _CumlModelSupervised,
     param_alias,
 )
-from spark_rapids_ml.params import HasFeaturesCols, P, _CumlClass, _CumlParams
-from spark_rapids_ml.tree import (
+from .params import HasFeaturesCols, P, _CumlClass, _CumlParams
+from .tree import (
     _RandomForestClass,
     _RandomForestCumlParams,
     _RandomForestEstimator,
     _RandomForestModel,
 )
-from spark_rapids_ml.utils import (
-    PartitionDescriptor,
-    _get_spark_session,
-    cudf_to_cuml_array,
-    java_uid,
-)
+from .utils import PartitionDescriptor, _get_spark_session, cudf_to_cuml_array, java_uid
 
 T = TypeVar("T")
 
 
 class LinearRegressionClass(_CumlClass):
     @classmethod
-    def _cuml_cls(cls) -> List[type]:
-        # from cuml.dask.linear_model import LinearRegression
-        from cuml.linear_model.linear_regression import LinearRegression
-        from cuml.linear_model.ridge import Ridge
-        from cuml.solvers import CD
-
-        return [LinearRegression, Ridge, CD]
-
-    @classmethod
     def _param_mapping(cls) -> Dict[str, Optional[str]]:
         return {
             "aggregationDepth": "",
             "elasticNetParam": "l1_ratio",
             "epsilon": "",
             "fitIntercept": "fit_intercept",
             "loss": "loss",
@@ -85,23 +84,45 @@
             "solver": "solver",
             "standardization": "normalize",
             "tol": "tol",
             "weightCol": None,
         }
 
     @classmethod
-    def _param_value_mapping(cls) -> Dict[str, Dict[str, Union[str, None]]]:
+    def _param_value_mapping(
+        cls,
+    ) -> Dict[str, Callable[[str], Union[None, str, float, int]]]:
         return {
-            "loss": {"squaredError": "squared_loss", "huber": None},
-            "solver": {"auto": "eig", "normal": "eig", "l-bfgs": None},
+            "loss": lambda x: {
+                "squaredError": "squared_loss",
+                "huber": None,
+                "squared_loss": "squared_loss",
+            }.get(x, None),
+            "solver": lambda x: {
+                "auto": "eig",
+                "normal": "eig",
+                "l-bfgs": None,
+                "eig": "eig",
+            }.get(x, None),
         }
 
-    @classmethod
-    def _param_excludes(cls) -> List[str]:
-        return ["handle", "output_type"]
+    def _get_cuml_params_default(self) -> Dict[str, Any]:
+        return {
+            "algorithm": "eig",
+            "fit_intercept": True,
+            "normalize": False,
+            "verbose": False,
+            "alpha": 0.0001,
+            "solver": "eig",
+            "loss": "squared_loss",
+            "l1_ratio": 0.15,
+            "max_iter": 1000,
+            "tol": 0.001,
+            "shuffle": True,
+        }
 
 
 class _LinearRegressionCumlParams(
     _CumlParams, _LinearRegressionParams, HasFeaturesCols
 ):
     """
     Shared Spark Params for LinearRegression and LinearRegressionModel.
@@ -483,15 +504,15 @@
         Fall back to PySpark ML LinearRegressionModel"""
         return self.cpu().evaluate(dataset)
 
     def _get_cuml_transform_func(
         self, dataset: DataFrame
     ) -> Tuple[
         Callable[..., CumlT],
-        Callable[[CumlT, Union[cudf.DataFrame, np.ndarray]], pd.DataFrame],
+        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
     ]:
         coef_ = self.coef_
         intercept_ = self.intercept_
         n_cols = self.n_cols
         dtype = self.dtype
 
         def _construct_lr() -> CumlT:
@@ -501,26 +522,30 @@
             lr.coef_ = cudf_to_cuml_array(np.array(coef_, order="F").astype(dtype))
             lr.intercept_ = intercept_
             lr.n_cols = n_cols
             lr.dtype = np.dtype(dtype)
 
             return lr
 
-        def _predict(lr: CumlT, pdf: Union[cudf.DataFrame, np.ndarray]) -> pd.Series:
+        def _predict(lr: CumlT, pdf: Union["cudf.DataFrame", np.ndarray]) -> pd.Series:
             ret = lr.predict(pdf)
             return pd.Series(ret)
 
         return _construct_lr, _predict
 
 
 class _RandomForestRegressorClass(_RandomForestClass):
     @classmethod
-    def _param_value_mapping(cls) -> Dict[str, Dict[str, Union[str, None]]]:
+    def _param_value_mapping(
+        cls,
+    ) -> Dict[str, Callable[[str], Union[None, str, float, int]]]:
         mapping = super()._param_value_mapping()
-        mapping["split_criterion"] = {"variance": "mse"}
+        mapping["split_criterion"] = lambda x: {"variance": "mse", "mse": "mse"}.get(
+            x, None
+        )
         return mapping
 
 
 class RandomForestRegressor(
     _RandomForestRegressorClass,
     _RandomForestEstimator,
     _RandomForestCumlParams,
@@ -607,12 +632,40 @@
     """
 
     def __init__(
         self,
         n_cols: int,
         dtype: str,
         treelite_model: str,
+        model_json: List[str],
     ):
-        super().__init__(dtype=dtype, n_cols=n_cols, treelite_model=treelite_model)
+        super().__init__(
+            dtype=dtype,
+            n_cols=n_cols,
+            treelite_model=treelite_model,
+            model_json=model_json,
+        )
+
+        self._rf_spark_model: Optional[SparkRandomForestRegressionModel] = None
+
+    def cpu(self) -> SparkRandomForestRegressionModel:
+        """Return the PySpark ML RandomForestRegressionModel"""
+
+        if self._rf_spark_model is None:
+            sc = _get_spark_session().sparkContext
+            assert sc._jvm is not None
+
+            uid, java_trees = self._convert_to_java_trees(self.getImpurity())
+            # Create the Spark RandomForestClassificationModel
+            java_rf_model = (
+                sc._jvm.org.apache.spark.ml.regression.RandomForestRegressionModel(
+                    uid,
+                    java_trees,
+                    self.numFeatures,
+                )
+            )
+            self._rf_spark_model = SparkRandomForestRegressionModel(java_rf_model)
+            self._copyValues(self._rf_spark_model)
+        return self._rf_spark_model
 
     def _is_classification(self) -> bool:
         return False
```

## spark_rapids_ml/tree.py

```diff
@@ -10,64 +10,73 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import base64
+import json
 import math
 import pickle
 from abc import abstractmethod
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    cast,
+)
+
+if TYPE_CHECKING:
+    import cudf
 
-import cudf
 import numpy as np
 import pandas as pd
+from pyspark.ml.classification import DecisionTreeClassificationModel
+from pyspark.ml.classification import (
+    RandomForestClassificationModel as SparkRandomForestClassificationModel,
+)
 from pyspark.ml.linalg import Vector
 from pyspark.ml.param.shared import HasFeaturesCol, HasLabelCol
-from pyspark.ml.tree import _DecisionTreeModel
+from pyspark.ml.regression import DecisionTreeRegressionModel
+from pyspark.ml.regression import (
+    RandomForestRegressionModel as SparkRandomForestRegressionModel,
+)
 from pyspark.sql import DataFrame
-from pyspark.sql.types import IntegerType, StringType, StructField, StructType
+from pyspark.sql.types import (
+    ArrayType,
+    IntegerType,
+    StringType,
+    StructField,
+    StructType,
+)
 
-from spark_rapids_ml.core import (
+from .core import (
     CumlInputType,
     CumlT,
     _CumlEstimatorSupervised,
     _CumlModelSupervised,
     param_alias,
 )
-from spark_rapids_ml.params import HasFeaturesCols, P, _CumlClass, _CumlParams
-from spark_rapids_ml.utils import _concat_and_free
+from .params import HasFeaturesCols, P, _CumlClass, _CumlParams
+from .utils import (
+    _concat_and_free,
+    _get_spark_session,
+    _str_or_numerical,
+    java_uid,
+    translate_trees,
+)
 
 
 class _RandomForestClass(_CumlClass):
     @classmethod
-    def _cuml_cls(cls) -> List[type]:
-        from cuml.ensemble.randomforest_common import BaseRandomForestModel
-
-        return [BaseRandomForestModel]
-
-    @classmethod
-    def _param_excludes(cls) -> List[str]:
-        return [
-            "handle",
-            "output_type",
-            "accuracy_metric",
-            "dtype",
-            "criterion",
-            "min_weight_fraction_leaf",
-            "max_leaf_nodes",
-            "min_impurity_split",
-            "oob_score",
-            "n_jobs",
-            "warm_start",
-            "class_weight",
-        ]
-
-    @classmethod
     def _param_mapping(cls) -> Dict[str, Optional[str]]:
         return {
             "maxBins": "n_bins",
             "maxDepth": "max_depth",
             "numTrees": "n_estimators",
             "impurity": "split_criterion",
             "featureSubsetStrategy": "max_features",
@@ -81,23 +90,53 @@
             "subsamplingRate": "",
             "minWeightFractionPerNode": "",
             "weightCol": None,
             "leafCol": None,
         }
 
     @classmethod
-    def _param_value_mapping(cls) -> Dict[str, Dict[str, Union[str, None]]]:
+    def _param_value_mapping(
+        cls,
+    ) -> Dict[str, Callable[[str], Union[None, str, float, int]]]:
+        def _tree_mapping(feature_subset: str) -> Union[None, str, float, int]:
+            _maybe_numerical = _str_or_numerical(feature_subset)
+            if isinstance(_maybe_numerical, int) or isinstance(_maybe_numerical, float):
+                _numerical = _maybe_numerical
+                return _numerical
+            else:
+                _str = _maybe_numerical
+                _tree_string_mapping: Dict[str, Union[None, str, float, int]] = {
+                    "onethird": 1 / 3.0,
+                    "all": 1.0,
+                    "auto": "auto",
+                    "sqrt": "sqrt",
+                    "log2": "log2",
+                }
+                return _tree_string_mapping.get(_str, None)
+
         return {
-            "max_features": {
-                "onethird": str(1 / 3.0),
-                "all": "1.0",
-                "auto": "auto",
-                "sqrt": "sqrt",
-                "log2": "log2",
-            },
+            "max_features": _tree_mapping,
+        }
+
+    def _get_cuml_params_default(self) -> Dict[str, Any]:
+        return {
+            "n_streams": 4,
+            "n_estimators": 100,
+            "max_depth": 16,
+            "max_features": "auto",
+            "n_bins": 128,
+            "bootstrap": True,
+            "verbose": False,
+            "min_samples_leaf": 1,
+            "min_samples_split": 2,
+            "max_samples": 1.0,
+            "max_leaves": -1,
+            "min_impurity_decrease": 0.0,
+            "random_state": None,
+            "max_batch_size": 4096,
         }
 
 
 class _RandomForestCumlParams(
     _CumlParams,
     HasFeaturesCol,
     HasFeaturesCols,
@@ -231,50 +270,63 @@
             # Fit a random forest model on the dataset (X, y)
             rf.fit(X, y, convert_dtype=False)
 
             # serialized_model is Dictionary type
             serialized_model = rf._get_serialized_model()
             pickled_model = pickle.dumps(serialized_model)
             msg = base64.b64encode(pickled_model).decode("utf-8")
-            messages = context.allGather(msg)
+            trees = rf.get_json()
+            data = {"model_bytes": msg, "model_json": trees}
+            messages = context.allGather(json.dumps(data))
 
             # concatenate the random forest in the worker0
             if part_id == 0:
-                mod_bytes = [pickle.loads(base64.b64decode(i)) for i in messages]
+                mod_bytes = []
+                mod_jsons = []
+                for msg in messages:
+                    data = json.loads(msg)
+                    mod_bytes.append(
+                        pickle.loads(base64.b64decode(data["model_bytes"]))
+                    )
+                    mod_jsons.append(data["model_json"])
+
                 all_tl_mod_handles = [rf._tl_handle_from_bytes(i) for i in mod_bytes]
                 rf._concatenate_treelite_handle(all_tl_mod_handles)
 
                 from cuml.fil.fil import TreeliteModel
 
                 for tl_handle in all_tl_mod_handles:
                     TreeliteModel.free_treelite_model(tl_handle)
 
                 final_model_bytes = pickle.dumps(rf._get_serialized_model())
                 final_model = base64.b64encode(final_model_bytes).decode("utf-8")
                 result = {
                     "treelite_model": [final_model],
                     "dtype": rf.dtype.name,
                     "n_cols": rf.n_cols,
+                    "model_json": [mod_jsons],
                 }
                 if is_classification:
                     result["num_classes"] = rf.num_classes
                 return result
             else:
                 return {}
 
         return _rf_fit
 
     def _out_schema(self) -> Union[StructType, str]:
         fields = [
             StructField("treelite_model", StringType(), False),
             StructField("n_cols", IntegerType(), False),
             StructField("dtype", StringType(), False),
+            StructField("model_json", ArrayType(StringType()), False),
         ]
         if self._is_classification():
             fields.append(StructField("num_classes", IntegerType(), False))
+
         return StructType(fields)
 
     def _require_nccl_ucx(self) -> Tuple[bool, bool]:
         return False, False
 
 
 class _RandomForestModel(
@@ -282,82 +334,143 @@
     _RandomForestCumlParams,
 ):
     def __init__(
         self,
         n_cols: int,
         dtype: str,
         treelite_model: str,
+        model_json: List[str] = [],
         num_classes: int = -1,  # only for classification
     ):
         if self._is_classification():
             super().__init__(
                 dtype=dtype,
                 n_cols=n_cols,
                 treelite_model=treelite_model,
                 num_classes=num_classes,
+                model_json=model_json,
             )
         else:
-            super().__init__(dtype=dtype, n_cols=n_cols, treelite_model=treelite_model)
+            super().__init__(
+                dtype=dtype,
+                n_cols=n_cols,
+                treelite_model=treelite_model,
+                model_json=model_json,
+            )
+        self._num_classes = num_classes
+        self._model_json = model_json
+        self._treelite_model = treelite_model
 
-        self.treelite_model = treelite_model
+    def cpu(
+        self,
+    ) -> Union[SparkRandomForestRegressionModel, SparkRandomForestClassificationModel]:
+        raise NotImplementedError()
 
     @property
     def featureImportances(self) -> Vector:
         """Estimate the importance of each feature."""
-        raise NotImplementedError
+        return self.cpu().featureImportances
 
     @property
     def getNumTrees(self) -> int:
         """Number of trees in ensemble."""
         return self.getOrDefault("numTrees")
 
     @property
     def toDebugString(self) -> str:
         """Full description of model."""
-        raise NotImplementedError
+        return self.cpu().toDebugString
 
     @property
     def totalNumNodes(self) -> int:
         """Total number of nodes, summed over all trees in the ensemble."""
-        raise NotImplementedError
+        return self.cpu().totalNumNodes
 
     @property
-    def trees(self) -> List[_DecisionTreeModel]:
+    def trees(
+        self,
+    ) -> Union[
+        List[DecisionTreeRegressionModel], List[DecisionTreeClassificationModel]
+    ]:
         """Trees in this ensemble. Warning: These have null parent Estimators."""
-        raise NotImplementedError
+        return self.cpu().trees
 
     @property
     def treeWeights(self) -> List[float]:
         """Return the weights for each tree."""
-        raise NotImplementedError
+        return self.cpu().treeWeights
 
     def predict(self, value: Vector) -> float:
         """
-        (Not supported) Predict label for the given features.
+        Predict label for the given features.
         """
-        raise NotImplementedError
+        return self.cpu().predict(value)
 
     def predictLeaf(self, value: Vector) -> float:
         """
-        (Not supported) Predict the indices of the leaves corresponding to the feature vector.
+        Predict the indices of the leaves corresponding to the feature vector.
         """
-        raise NotImplementedError
+        return self.cpu().predictLeaf(value)
 
     @abstractmethod
     def _is_classification(self) -> bool:
         """Indicate if it is regression or classification model"""
         raise NotImplementedError()
 
+    def _convert_to_java_trees(self, impurity: str) -> Tuple[Any, List[Any]]:
+        """Convert cuml trees to Java decision tree model"""
+        sc = _get_spark_session().sparkContext
+        assert sc._jvm is not None
+        assert sc._gateway is not None
+
+        # Convert cuml trees to Spark trees
+        trees = [
+            translate_trees(sc, impurity, trees)
+            for trees_json in self._model_json
+            for trees in json.loads(trees_json)
+        ]
+
+        if self._is_classification():
+            uid = java_uid(sc, "rfc")
+            java_decision_tree_model_class = (
+                sc._jvm.org.apache.spark.ml.classification.DecisionTreeClassificationModel
+            )
+            # Wrap the trees into Spark DecisionTreeClassificationModel
+            decision_trees = [
+                java_decision_tree_model_class(
+                    uid, tree, self.numFeatures, self._num_classes
+                )
+                for tree in trees
+            ]
+        else:
+            uid = java_uid(sc, "rfr")
+            java_decision_tree_model_class = (
+                sc._jvm.org.apache.spark.ml.regression.DecisionTreeRegressionModel
+            )
+            # Wrap the trees into Spark DecisionTreeClassificationModel
+            decision_trees = [
+                java_decision_tree_model_class(uid, tree, self.numFeatures)
+                for tree in trees
+            ]
+
+        java_trees = sc._gateway.new_array(
+            java_decision_tree_model_class, len(decision_trees)
+        )
+        for i in range(len(decision_trees)):
+            java_trees[i] = decision_trees[i]
+
+        return uid, java_trees
+
     def _get_cuml_transform_func(
         self, dataset: DataFrame
     ) -> Tuple[
         Callable[..., CumlT],
-        Callable[[CumlT, Union[cudf.DataFrame, np.ndarray]], pd.DataFrame],
+        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
     ]:
-        treelite_model = self.treelite_model
+        treelite_model = self._treelite_model
 
         is_classification = self._is_classification()
 
         def _construct_rf() -> CumlT:
             model = pickle.loads(base64.b64decode(treelite_model))
 
             if is_classification:
@@ -366,14 +479,14 @@
                 from cuml import RandomForestRegressor as cuRf
 
             rf = cuRf()
             rf._concatenate_treelite_handle([rf._tl_handle_from_bytes(model)])
 
             return rf
 
-        def _predict(rf: CumlT, pdf: Union[cudf.DataFrame, np.ndarray]) -> pd.Series:
+        def _predict(rf: CumlT, pdf: Union["cudf.DataFrame", np.ndarray]) -> pd.Series:
             rf.update_labels = False
             ret = rf.predict(pdf)
             return pd.Series(ret)
 
         # TBD: figure out why RF algo's warns regardless of what np array order is set
         return _construct_rf, _predict
```

## spark_rapids_ml/utils.py

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, NVIDIA CORPORATION.
+# Copyright (c) 2022-2023, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,27 +12,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import inspect
 import logging
 import sys
-from typing import Any, Callable, Dict, List, Literal, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Tuple, Union
 
-import cudf
-import numpy as np
-
-try:
-    # Compatible with older cuml version (before 23.02)
-    from cuml.common.array import CumlArray
-    from cuml.common.input_utils import input_to_cuml_array
-except ImportError:
-    from cuml.common import input_to_cuml_array
-    from cuml.internals.array import CumlArray
+if TYPE_CHECKING:
+    import cudf
 
+import numpy as np
 from pyspark import BarrierTaskContext, SparkContext, TaskContext
 from pyspark.sql import SparkSession
 
 _ArrayOrder = Literal["C", "F"]
 
 
 def _get_spark_session() -> SparkSession:
@@ -47,14 +40,29 @@
 
 
 def _is_local(sc: SparkContext) -> bool:
     """Whether it is Spark local mode"""
     return sc._jsc.sc().isLocal()  # type: ignore
 
 
+def _str_or_numerical(x: str) -> Union[str, float, int]:
+    """
+    Convert to int if x is str representation of integer,
+    otherwise float if x is representation of float, otherwise return input string.
+    """
+    try:
+        _x: Union[str, int, float] = int(x)
+    except:
+        try:
+            _x = float(x)
+        except:
+            _x = x
+    return _x
+
+
 def _get_gpu_id(task_context: TaskContext) -> int:
     """Get the gpu id from the task resources"""
     if task_context is None:
         # safety check.
         raise RuntimeError("_get_gpu_id should not be invoked from driver side.")
     resources = task_context.resources()
     if "gpu" not in resources:
@@ -148,17 +156,20 @@
     d_type = np_array_list[0].dtype
     concated = np.empty(shape=concat_shape, order=order, dtype=d_type)
     np.concatenate(np_array_list, out=concated)
     del np_array_list[:]
     return concated
 
 
-def cudf_to_cuml_array(
-    gdf: Union[cudf.DataFrame, cudf.Series], order: str = "F"
-) -> CumlArray:
+def cudf_to_cuml_array(gdf: Union["cudf.DataFrame", "cudf.Series"], order: str = "F"):  # type: ignore
+    try:
+        # Compatible with older cuml version (before 23.02)
+        from cuml.common.input_utils import input_to_cuml_array
+    except ImportError:
+        from cuml.common import input_to_cuml_array
     cumlarray, _, _, _ = input_to_cuml_array(gdf, order=order)
     return cumlarray
 
 
 def dtype_to_pyspark_type(dtype: Union[np.dtype, str]) -> str:
     """Convert np.dtype to the corresponding pyspark type"""
     dtype = np.dtype(dtype)
@@ -193,7 +204,180 @@
     return logger
 
 
 def java_uid(sc: SparkContext, prefix: str) -> str:
     """Returns a random UID that concatenates the given prefix, "_", and 12 random hex chars."""
     assert sc._jvm is not None
     return sc._jvm.org.apache.spark.ml.util.Identifiable.randomUID(prefix)
+
+
+def _fake_java_impurity_calc(sc: SparkContext, count: int = 3):  # type: ignore
+    """Fake a java ImpurityCalculator"""
+    assert sc._jvm is not None
+    assert sc._gateway is not None
+
+    object_class = sc._jvm.double
+    fake_python_impurity_calc = [0 for _ in range(count)]
+    fake_java_impurity_calc = sc._gateway.new_array(
+        object_class, len(fake_python_impurity_calc)
+    )
+    for i in range(len(fake_python_impurity_calc)):
+        fake_java_impurity_calc[i] = float(fake_java_impurity_calc[i])
+
+    return fake_java_impurity_calc
+
+
+def _create_internal_node(sc: SparkContext, impurity: str, model: Dict[str, Any], left, right):  # type: ignore
+    """Return a Java InternalNode"""
+
+    assert sc._jvm is not None
+    assert sc._gateway is not None
+
+    java_split = sc._jvm.org.apache.spark.ml.tree.ContinuousSplit(
+        int(model["split_feature"]), float(model["split_threshold"])
+    )
+
+    fake_java_impurity_calc = _fake_java_impurity_calc(sc)
+
+    if impurity == "gini":
+        java_impurity_cal = sc._jvm.org.apache.spark.mllib.tree.impurity.GiniCalculator(
+            fake_java_impurity_calc, int(model["instance_count"])
+        )
+    elif impurity == "entropy":
+        java_impurity_cal = (
+            sc._jvm.org.apache.spark.mllib.tree.impurity.EntropyCalculator(
+                fake_java_impurity_calc, int(model["instance_count"])
+            )
+        )
+    elif impurity == "variance":
+        java_impurity_cal = (
+            sc._jvm.org.apache.spark.mllib.tree.impurity.VarianceCalculator(
+                fake_java_impurity_calc, int(model["instance_count"])
+            )
+        )
+    else:
+        # never reach here
+        raise ValueError("Unsupported impurity! ", impurity)
+
+    java_internal_node = sc._jvm.org.apache.spark.ml.tree.InternalNode(
+        0.0,  # prediction value is nonsense for internal node, just fake it
+        0.0,  # impurity value is nonsense for internal node. just fake it
+        float(model["gain"]),
+        left,
+        right,
+        java_split,
+        java_impurity_cal,
+    )
+
+    return java_internal_node
+
+
+def _create_leaf_node(sc: SparkContext, impurity: str, model: Dict[str, Any]):  # type: ignore
+    """Return a Java LeaftNode
+    Please note that, cuml trees uses probs as the leaf values while spark uses
+    the stats (how many counts this node has for each label), but they are behave
+    the same purpose when doing prediction
+    """
+    assert sc._jvm is not None
+    assert sc._gateway is not None
+
+    leaf_values = model["leaf_value"]
+
+    if impurity == "gini" or impurity == "entropy":
+        object_class = sc._jvm.double
+        java_probs = sc._gateway.new_array(object_class, len(leaf_values))
+        for i in range(len(leaf_values)):
+            java_probs[i] = float(leaf_values[i])
+
+        java_impurity_cal = (
+            sc._jvm.org.apache.spark.mllib.tree.impurity.GiniCalculator(
+                java_probs, int(model["instance_count"])
+            )
+            if impurity == "gini"
+            else sc._jvm.org.apache.spark.mllib.tree.impurity.EntropyCalculator(
+                java_probs, int(model["instance_count"])
+            )
+        )
+        prediction = np.argmax(np.asarray(leaf_values))
+
+    elif impurity == "variance":
+        fake_java_impurity_calc = _fake_java_impurity_calc(sc, 3)
+        java_impurity_cal = (
+            sc._jvm.org.apache.spark.mllib.tree.impurity.VarianceCalculator(
+                fake_java_impurity_calc, int(model["instance_count"])
+            )
+        )
+        prediction = leaf_values[0]
+    else:
+        # never reach here
+        raise ValueError("Unsupported impurity! ", impurity)
+
+    java_leaf_node = sc._jvm.org.apache.spark.ml.tree.LeafNode(
+        float(prediction),
+        0.0,  # TODO calculate the impurity according to leaf value, prediction doesn't require it.
+        java_impurity_cal,
+    )
+    return java_leaf_node
+
+
+def translate_trees(sc: SparkContext, impurity: str, model: Dict[str, Any]):  # type: ignore
+    """Translate Cuml RandomForest trees to PySpark trees
+
+    Cuml trees
+    [
+      {
+        "nodeid": 0,
+        "split_feature": 3,
+        "split_threshold": 0.827687974732221,
+        "gain": 0.41999999999999998,
+        "instance_count": 10,
+        "yes": 1,
+        "no": 2,
+        "children": [
+          {
+            "nodeid": 1,
+            "leaf_value": [
+              1,
+              0
+            ],
+            "instance_count": 7
+          },
+          {
+            "nodeid": 2,
+            "leaf_value": [
+              0,
+              1
+            ],
+            "instance_count": 3
+          }
+        ]
+      }
+    ]
+
+    Spark trees,
+             InternalNode {split{featureIndex=3, threshold=0.827687974732221}, gain = 0.41999999999999998}
+             /         \
+           left        right
+           /             \
+    LeafNode           LeafNode
+    """
+    if "split_feature" in model:
+        left_child_id = model["yes"]
+        right_child_id = model["no"]
+
+        for child in model["children"]:
+            if child["nodeid"] == left_child_id:
+                left_child = child
+            elif child["nodeid"] == right_child_id:
+                right_child = child
+            else:
+                raise ValueError("Unexpected node id")
+
+        return _create_internal_node(
+            sc,
+            impurity,
+            model,
+            translate_trees(sc, impurity, left_child),
+            translate_trees(sc, impurity, right_child),
+        )
+    elif "leaf_value" in model:
+        return _create_leaf_node(sc, impurity, model)
```

## spark_rapids_ml/common/cuml_context.py

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, NVIDIA CORPORATION.
+# Copyright (c) 2022-2023, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,26 +14,26 @@
 # limitations under the License.
 #
 import asyncio
 import base64
 import json
 import os
 from asyncio import AbstractEventLoop
-from typing import Any, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, List, Optional, Tuple
 
 import psutil
-from pylibraft.common import Handle
+
+if TYPE_CHECKING:
+    # need this first to load shared ucx shared libraries from ucx-py instead of raft-dask
+    from ucp import Endpoint
+    from pylibraft.common import Handle  # isort: split
+    from raft_dask.common import UCX
+    from raft_dask.common.nccl import nccl
+
 from pyspark import BarrierTaskContext
-from raft_dask.common import UCX
-from raft_dask.common.comms_utils import (
-    inject_comms_on_handle,
-    inject_comms_on_handle_coll_only,
-)
-from raft_dask.common.nccl import nccl
-from ucp import Endpoint
 
 
 class CumlContext:
     def __init__(
         self,
         rank: int,
         nranks: int,
@@ -44,29 +44,35 @@
         """
         Initialize the nccl unique id for workers.
 
         1. get the nccl unique id for worker 0
         2. do all gather for all the workers to get the nccl unique uid.
         3. if require_ucx is true, initialize ucx and inject ucx together with nccl into a handle
         """
+        # need this first to load shared ucx shared libraries from ucx-py instead of raft-dask
+        from ucp import Endpoint
+        from pylibraft.common import Handle  # isort: split
+        from raft_dask.common import UCX
+        from raft_dask.common.nccl import nccl
+
         self.enable = enable
-        self._handle: Optional[Handle] = None
+        self._handle: Optional["Handle"] = None
         self._loop: Optional[AbstractEventLoop] = None
 
         if not enable:
             return
 
         self._rank = rank
         self._nranks = nranks
         self._require_ucx = require_ucx
 
         self._handle = Handle(n_streams=0)
-        self._nccl_comm: Optional[nccl] = None
+        self._nccl_comm: Optional["nccl"] = None
         self._nccl_unique_id = None
-        self._ucx: Optional[UCX] = None
+        self._ucx: Optional["UCX"] = None
         self._ucx_port = None
         self._ucx_eps = None
 
         nccl_uid = ""
         if context.partitionId() == 0:
             nccl_uid = base64.b64encode(nccl.get_unique_id()).decode("utf-8")
 
@@ -93,40 +99,46 @@
             self._ucx = UCX.get()
             self._ucx_port = self._ucx.listener_port()
             msgs = context.allGather(json.dumps((nccl_uid, self._ucx_port)))
             self._nccl_unique_id = base64.b64decode(json.loads(msgs[0])[0])
             self._ports = [json.loads(msg)[1] for msg in msgs]
 
     @property
-    def handle(self) -> Optional[Handle]:
+    def handle(self) -> Optional["Handle"]:
         return self._handle
 
     def __enter__(self) -> "CumlContext":
         if not self.enable:
             return self
 
+        from raft_dask.common.nccl import nccl
+
         # initialize nccl and inject it to the handle. A GPU must be assigned exclusively before init() is called
         self._nccl_comm = nccl()
         self._nccl_comm.init(self._nranks, self._nccl_unique_id, self._rank)
 
         if self._require_ucx is False:
+            from raft_dask.common.comms_utils import inject_comms_on_handle_coll_only
+
             inject_comms_on_handle_coll_only(
                 self._handle, self._nccl_comm, self._nranks, self._rank, True
             )
         else:
             self._loop = asyncio.new_event_loop()
             asyncio.set_event_loop(self._loop)
             self._ucx_eps = self._loop.run_until_complete(
                 asyncio.ensure_future(
                     CumlContext._ucp_create_endpoints(
                         self._ucx, list(zip(self._ips, self._ports))
                     )
                 )
             )
 
+            from raft_dask.common.comms_utils import inject_comms_on_handle
+
             inject_comms_on_handle(
                 self._handle,
                 self._nccl_comm,
                 self._ucx.get_worker(),  # type: ignore
                 self._ucx_eps,
                 self._nranks,
                 self._rank,
@@ -154,18 +166,18 @@
             ip = if_addrs_dict[ifname][0].address
             if ip == target_ip:
                 return ifname
         raise ValueError(f"target_ip ${target_ip} does not exist")
 
     @staticmethod
     async def _ucp_create_endpoints(
-        ucx_worker: UCX,
+        ucx_worker: "UCX",
         target_ip_ports: List[Tuple[str, int]],
         additional_timeout: float = 0.1,
-    ) -> Endpoint:
+    ) -> "Endpoint":
         """
         ucp initialization may require a larger additional_timeout a complex network environment
         """
         eps = [None] * len(target_ip_ports)
         for i in range(len(eps)):
             ip, port = target_ip_ports[i]
             ep = await ucx_worker.get_endpoint(ip, port)
```

## Comparing `spark_rapids_ml-23.2.0.dist-info/METADATA` & `spark_rapids_ml-23.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-rapids-ml
-Version: 23.2.0
+Version: 23.4.0
 Summary: Apache Spark integration with RAPIDS and cuML
 Author-email: Jinfeng Li <jinfeng@nvidia.com>, Bobby Wang <bobwang@nvidia.com>, Erik Ordentlich <eordentlich@nvidia.com>, Lee Yang <leey@nvidia.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,31 +20,36 @@
 
 ## Installation
 
 For simplicity, the following instructions just use Spark local mode, assuming a server with at least one GPU.
 
 First, install RAPIDS cuML per [these instructions](https://rapids.ai/start.html).
 ```bash
-conda create -n rapids-23.02 \
+conda create -n rapids-23.04 \
     -c rapidsai -c nvidia -c conda-forge \
-    cuml=23.02 python=3.8 cudatoolkit=11.5
+    cuml=23.04 python=3.8 cudatoolkit=11.5
 ```
 
 **Note**: while testing, we recommend using conda or docker to simplify installation and isolate your environment while experimenting.  Once you have a working environment, you can then try installing directly, if necessary.
 
 **Note**: you can select the latest version compatible with your environment from [rapids.ai](https://rapids.ai/start.html#get-rapids).
 
 Once you have the conda environment, activate it and install the required packages.
 ```bash
-conda activate rapids-23.02
+conda activate rapids-23.04
 
-git clone --branch spark-cuml https://github.com/NVIDIA/spark-rapids-ml.git
+# for development access to notebooks, tests, and benchmarks
+git clone --branch main https://github.com/NVIDIA/spark-rapids-ml.git
 cd spark-rapids-ml/python
 pip install -r requirements.txt
 pip install -e .
+
+# OPTIONAL: for package installation only
+pip install -r https://raw.githubusercontent.com/NVIDIA/spark-rapids-ml/main/python/requirements.txt
+pip install spark-rapids-ml
 ```
 
 ## Examples
 
 These examples demonstrate the API using toy datasets.  However, GPUs are more effective when using larger datasets that require extensive compute.  So once you are confident in your environment setup, use a more representative dataset for your specific use case to gauge how GPUs can improve performance.
 
 ### PySpark shell
```

## Comparing `spark_rapids_ml-23.2.0.dist-info/RECORD` & `spark_rapids_ml-23.4.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-spark_rapids_ml/__init__.py,sha256=u1v1efJkJLSHx2ssRHEqnXxT13QuOAA2nFN__T8yr6I,615
-spark_rapids_ml/classification.py,sha256=JDQrPmUWarZv8zmjdWuyE0Gd-YImZNLzRimeCAHkvv0,7537
-spark_rapids_ml/clustering.py,sha256=XMcWEhoF730Pe1bmLTQ2raRs1RfCLynrPST60KCVnNs,13898
-spark_rapids_ml/core.py,sha256=QzeaGhvU6Nh1eKWuOvt7zvK5cHSFqlYJrJV2t1yp7lE,29087
-spark_rapids_ml/feature.py,sha256=vwqbePGg5c6YcUZSHra27LR-2rPh6mTeJSobB8LlkmQ,13614
-spark_rapids_ml/knn.py,sha256=F_b5LipgZOEoWuEmZ8Ys_8Yo0LpsZxjKsMHpUsYyoao,21944
-spark_rapids_ml/params.py,sha256=txA-jrwqc208W2CgE1PwQ0HdCa9InMNGXIgWrstkSHE,14846
-spark_rapids_ml/regression.py,sha256=-k_xKK5NkLTL7tDL3fo6ntulRocsYwJjAO-nFTTEE2Y,20878
-spark_rapids_ml/tree.py,sha256=li9Z5gyGJfp6G9uryRNKJySADUGdy_rpMUNrvaFJuik,12675
-spark_rapids_ml/utils.py,sha256=xUhlX52mvb6TPCAuPScEkJFYTUXVb7N4QX8R2_ndNBY,6529
+spark_rapids_ml/__init__.py,sha256=oY9PRQNy7_o7_RTmZdOPCGSQULof69lJhQ_YYdeo6KQ,615
+spark_rapids_ml/classification.py,sha256=QQr846lH_1uV0JsSyweI3Sj-Yd_06zn_zr5Q4jTXgac,9944
+spark_rapids_ml/clustering.py,sha256=S2amR5SzrSi4XTcW4n8pWkFgJ1ra_GII8mHKFQdVwz4,13967
+spark_rapids_ml/core.py,sha256=LcglBygvbTER9GYF2o4QSXdqtmzP6TEj_DLoNVGUcQ0,29140
+spark_rapids_ml/feature.py,sha256=TebOT6NsvlxttxGJGA6kIEo2S_xWFeJADfkBMQUHlPQ,13432
+spark_rapids_ml/knn.py,sha256=C84bRRieGzr8QOTNri43vCjAUCem6Dwz1UEO_F0xTHc,24378
+spark_rapids_ml/params.py,sha256=z5LanyAZV1odr4VT8rl9RNnziNHDpv8xJ_7XQuu1aHQ,14982
+spark_rapids_ml/regression.py,sha256=vmWJgbjB6cLWhGOZ0Nc-39yz_uRenpaOhpaPIRFqeMI,22364
+spark_rapids_ml/tree.py,sha256=ArQGXc_hOLSJ309YlgmEdWEtfpMk7iwH5GZOp4dR2yI,16334
+spark_rapids_ml/utils.py,sha256=__THblBCEJmSkSCPMGpjpFrE9JqhNqQxGFS56efTWok,12469
 spark_rapids_ml/common/__init__.py,sha256=dbWdFUlhiiYjOXLG8mDgkN9ccO6VzvpdP5TZ4koaanM,592
-spark_rapids_ml/common/cuml_context.py,sha256=IquJSl66mdQ5XJ7yM6AyovzTUjV9enxnh1B5kbt8-QA,5992
-spark_rapids_ml-23.2.0.dist-info/METADATA,sha256=tXTDk5sp0EATLgWMFbcY5BrF_gf3hcuui_opq8RV3UI,8539
-spark_rapids_ml-23.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-spark_rapids_ml-23.2.0.dist-info/top_level.txt,sha256=ypWU-O052mYZy_QAptA2bkv4jYjExoi8Hcr0dmH3WZQ,16
-spark_rapids_ml-23.2.0.dist-info/RECORD,,
+spark_rapids_ml/common/cuml_context.py,sha256=GNVhKeiV1FsXAAaCLSHTtFU4YX5L61uK6BEdQ_RCBNE,6545
+spark_rapids_ml-23.4.0.dist-info/METADATA,sha256=DjRU1LtwKegr0ASqEvFrmMkkukga1wUau89Kzyqh6LE,8766
+spark_rapids_ml-23.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spark_rapids_ml-23.4.0.dist-info/top_level.txt,sha256=ypWU-O052mYZy_QAptA2bkv4jYjExoi8Hcr0dmH3WZQ,16
+spark_rapids_ml-23.4.0.dist-info/RECORD,,
```

