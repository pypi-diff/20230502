# Comparing `tmp/cuellartensorflow-1.0.2.tar.gz` & `tmp/cuellartensorflow-1.0.3.tar.gz`

## Comparing `cuellartensorflow-1.0.2.tar` & `cuellartensorflow-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.2/Readme.md
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.2/src/cuellartensorflow/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.2/LICENSE
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.2/README.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.3/Readme.md
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.3/src/cuellartensorflow/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.3/README.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 cuellartensorflow-1.0.3/PKG-INFO
```

### Comparing `cuellartensorflow-1.0.2/Readme.md` & `cuellartensorflow-1.0.3/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 ```python
 from cuellartensorflow import train_language_model
 
 modelo = train_language_model(
     language="es",
     num_articles=10,
-    num_epochs=10
+    num_epochs=10,
+    batch_size=64
 )
 ```
 cambia el parametro "es" de la funcion  languaje="es"  para entrenar el modelo con un idioma distinto consulta la documentacion de wikipedia para mayor informacion, "num_articles" para especificar el numero de articulos a usar para el entrenamiento, "num_epochs" para especificar el numero de epocas a usar para el entrenamiento del modelo
 
 Para generar texto usando nuestro modelo recien creado puedes usar el siguiente codigo:
 
 ```python
```

### Comparing `cuellartensorflow-1.0.2/src/cuellartensorflow/__init__.py` & `cuellartensorflow-1.0.3/src/cuellartensorflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import wikipedia
 import tensorflow as tf
 import numpy as np
 import pickle
 from tqdm import tqdm
 import random
 
-def train_language_model(language, num_articles, num_epochs):
+def train_language_model(language, num_articles, num_epochs, batch_size):
     # Establecer idioma de wikipedia
     wikipedia.set_lang(language)
 
     # Obtener una lista aleatoria de títulos de artículos
     titles = wikipedia.random(pages=num_articles)
 
     # Unir los contenidos de los artículos en una sola cadena de texto
@@ -31,15 +31,15 @@
     with open('tokenizer.pkl', 'wb') as f:
         pickle.dump(tokenizer, f)
 
     # Convertir el texto en una secuencia de tokens
     sequences = tokenizer.texts_to_sequences([text])[0]
 
     # Crear una lista de ventanas deslizantes con longitud de 100 tokens
-    window_size = 100
+    window_size = 10
     windows = []
     for i in range(len(sequences) - window_size):
         window = sequences[i:i + window_size]
         windows.append(window)
 
     # Convertir las ventanas a un array de numpy
     windows = np.array(windows)
@@ -59,27 +59,27 @@
 
     # Compilar modelo
     model.compile(loss='categorical_crossentropy', optimizer='adam', metrics=['accuracy'])
 
     # Entrenar modelo
     model.fit(x=train_data[:, :-1], y=tf.keras.utils.to_categorical(train_data[:, -1], num_classes=len(tokenizer.word_index) + 1), 
               validation_data=(val_data[:, :-1], tf.keras.utils.to_categorical(val_data[:, -1], num_classes=len(tokenizer.word_index) + 1)), 
-              epochs=num_epochs, batch_size=128)
+              epochs=num_epochs, batch_size=batch_size)
 
     # Guardar modelo entrenado
     model.save('tf_model.h5')
 
 def generate_text(seed_text, num_words, temperature):
     # Cargar el modelo entrenado y el tokenizador desde los archivos
     model = tf.keras.models.load_model("tf_model.h5")
     with open("tokenizer.pkl", 'rb') as f:
         tokenizer = pickle.load(f)
 
     # Definir la longitud de la secuencia de entrada y la temperatura
-    sequence_length = 100
+    sequence_length = 10
     temperature = temperature
 
     # Convertir la semilla inicial del texto en una secuencia de tokens
     seed_sequence = tokenizer.texts_to_sequences([seed_text])[0]
 
     # Generar texto
     generated_text = ""
```

### Comparing `cuellartensorflow-1.0.2/LICENSE` & `cuellartensorflow-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cuellartensorflow-1.0.2/README.md` & `cuellartensorflow-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 ```python
 from cuellartensorflow import train_language_model
 
 modelo = train_language_model(
     language="es",
     num_articles=10,
-    num_epochs=10
+    num_epochs=10,
+    batch_size=64
 )
 ```
 cambia el parametro "es" de la funcion  languaje="es"  para entrenar el modelo con un idioma distinto consulta la documentacion de wikipedia para mayor informacion, "num_articles" para especificar el numero de articulos a usar para el entrenamiento, "num_epochs" para especificar el numero de epocas a usar para el entrenamiento del modelo
 
 Para generar texto usando nuestro modelo recien creado puedes usar el siguiente codigo:
 
 ```python
```

### Comparing `cuellartensorflow-1.0.2/pyproject.toml` & `cuellartensorflow-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "cuellartensorflow"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Emiliano Cuellar", email="ec446162@gmail.com" },
 ]
 description = "Una libreria simple para crear modelos de lenguaje con tensorflow"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `cuellartensorflow-1.0.2/PKG-INFO` & `cuellartensorflow-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuellartensorflow
-Version: 1.0.2
+Version: 1.0.3
 Summary: Una libreria simple para crear modelos de lenguaje con tensorflow
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Emiliano Cuellar <ec446162@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,16 @@
 
 ```python
 from cuellartensorflow import train_language_model
 
 modelo = train_language_model(
     language="es",
     num_articles=10,
-    num_epochs=10
+    num_epochs=10,
+    batch_size=64
 )
 ```
 cambia el parametro "es" de la funcion  languaje="es"  para entrenar el modelo con un idioma distinto consulta la documentacion de wikipedia para mayor informacion, "num_articles" para especificar el numero de articulos a usar para el entrenamiento, "num_epochs" para especificar el numero de epocas a usar para el entrenamiento del modelo
 
 Para generar texto usando nuestro modelo recien creado puedes usar el siguiente codigo:
 
 ```python
```

