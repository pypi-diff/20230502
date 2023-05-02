# Comparing `tmp/MKN_third_codes-0.6.0.4.tar.gz` & `tmp/MKN_third_codes-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.0.4.tar", last modified: Mon May  1 14:07:31 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.4.tar", last modified: Tue May  2 11:29:14 2023, max compression
```

## Comparing `MKN_third_codes-0.6.0.4.tar` & `MKN_third_codes-0.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 14:07:31.740379 MKN_third_codes-0.6.0.4/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.0.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-01 14:07:31.727414 MKN_third_codes-0.6.0.4/MKN_third_codes/
--rw-rw-rw-   0        0        0    31448 2023-05-01 13:56:42.000000 MKN_third_codes-0.6.0.4/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:07:31.738385 MKN_third_codes-0.6.0.4/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     5224 2023-05-01 14:07:31.000000 MKN_third_codes-0.6.0.4/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-01 14:07:31.000000 MKN_third_codes-0.6.0.4/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:07:31.000000 MKN_third_codes-0.6.0.4/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 14:07:31.000000 MKN_third_codes-0.6.0.4/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5224 2023-05-01 14:07:31.740379 MKN_third_codes-0.6.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3575 2023-05-01 14:07:24.000000 MKN_third_codes-0.6.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 14:07:31.741377 MKN_third_codes-0.6.0.4/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-05-01 14:07:29.000000 MKN_third_codes-0.6.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:29:14.027226 MKN_third_codes-0.6.4/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-02 11:29:14.011270 MKN_third_codes-0.6.4/MKN_third_codes/
+-rw-rw-rw-   0        0        0    38047 2023-05-02 11:26:33.000000 MKN_third_codes-0.6.4/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:29:14.026229 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     6630 2023-05-02 11:29:13.000000 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-02 11:29:13.000000 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 11:29:13.000000 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 11:29:13.000000 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6630 2023-05-02 11:29:14.027226 MKN_third_codes-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4186 2023-05-02 11:28:59.000000 MKN_third_codes-0.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 11:29:14.028224 MKN_third_codes-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      503 2023-05-02 11:16:11.000000 MKN_third_codes-0.6.4/setup.py
```

### Comparing `MKN_third_codes-0.6.0.4/LICENSE.txt` & `MKN_third_codes-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.0.4/MKN_third_codes/solutions.py` & `MKN_third_codes-0.6.4/MKN_third_codes/solutions.py`

 * *Files 8% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         else:
             self.waiting_time = 1
 
     def calculate_square(self, maxEnd:float, waiter_time):
         return ((min(self.end_time, maxEnd) - self.start_time - waiter_time)**2)/2
 
 regular_int = r'-?\d+'
-regular_float = r'-?\d+(?:\.\d+)?'
+regular_float = r'-?\d+(?:[\.\,]\d+)?'
 
 def combinations(k:float=0,n:float=0):
     """
     Функция, считающая число сочетаний из n по k
 
     Args:
         k (float): аргумент k - количество повторений
@@ -326,14 +326,16 @@
     WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
     """
     humans = int(input("Введите количество человек: "))
     result = things_complexity_solution(humans)
     print("Таблица:")
     for cell in result.cells:
         print(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.all_th})")
+    for cell in result.cells:
+        print(cell.good_th)
 
 def things_complexity_solution(humans:int = 0):
     """
     Решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
     WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
 
     Args:
@@ -341,17 +343,16 @@
 
     Returns:
         EttaTable: таблица ячеек таблицы
     """
     #следующей строчкой находим количество всех перестановок
     allPerestan = math.factorial(humans)
 
+    #определяем таблицу
     myTable = EttaTable(cells=[])
-
-    #для каждой "Этта" от 0 до humans вычисляем вероятность (Этта людей получили свои вещи)
     for j in range(0, humans+1):
         myTable.cells.append(EttaTableCell(j, 0, allPerestan))
 
     #Функция, проходящаяся по всем перестановкам, и записивыающая их в таблицу
     def goThrough(n, layer, used):
         if layer == humans:#раздали все предметы
             myTable.cells[n].good_th += 1
@@ -367,14 +368,49 @@
 
     #пересчёт вероятностей
     for j in range(0, humans+1):
         myTable.cells[j].reset_probability()
     
     return myTable
 
+def things_complexity_optimized_solution(humans:int = 0):
+    """
+    Оптимизированное решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
+    
+    Суть оптимизации:
+        На больших значениях n существует закономерность в значениях кол-ва перестановок для СВ равной от 2 до n-2, где СВ обозначает 'какое кол-во людей получили свои вещи'
+
+    Args:
+        humans (int): кол-во людей
+
+    Returns:
+        EttaTable: таблица ячеек таблицы
+    """
+    #следующей строчкой находим количество всех перестановок
+    allPerestan = math.factorial(humans)
+
+    #определяем таблицу
+    myTable = EttaTable(cells=[])
+    for j in range(0, humans+1):
+        myTable.cells.append(EttaTableCell(j, 0, allPerestan))
+
+    myTable.cells[0].good_th = int(round(math.factorial(humans)/math.e))
+    myTable.cells[1].good_th = myTable.cells[0].good_th + (-1)**(humans+1)
+    myTable.cells[-1].good_th = 1
+    myTable.cells[-2].good_th = 0
+
+    for id in range(2, humans-1):
+        myTable.cells[id].good_th = int(round(myTable.cells[id-1].good_th / id))
+
+    #пересчёт вероятностей
+    for j in range(0, humans+1):
+        myTable.cells[j].reset_probability()
+    
+    return myTable
+
 def things_complexity_request(text: str = None):
     """
     Решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
     WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
 
     Args:
         text (str): текст запроса, который может быть None или вводом пользователя
@@ -400,14 +436,57 @@
                     answer.append(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.all_th})")
                 return answer
             else:
                 return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
+def things_complexity_optimized_request(text, maximum_full:int = 11):
+    """
+    Оптимизированное решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
+    WARNING: т.к. для n > maximum_full используется приблизительный подсчёт кол-ва перестановок, значения могут быть весьма неточными, если поставить maximum_full слишком низким
+
+    Суть оптимизации:
+        На больших значениях n существует закономерность в значениях кол-ва перестановок для СВ равной от 2 до n-2, где СВ обозначает 'какое кол-во людей получили свои вещи'
+
+    Args:
+        text (str): текст запроса, который может быть None или вводом пользователя
+        maximum_full (int) = 11: максимальное количсетво людей, для которых значения СВ будут считаться полностью. для запросов, где пользователь указывает n>maximum_full, функция посчитает приблизительные значения
+    
+    Returns:
+        list: массив строчек ответа
+    """
+    if text == None:
+        return ["""Введите количество человек (число n)"""]
+    else:
+        try:
+            request = [int(parameter) for parameter in re.findall(regular_int, text)]
+            if len(request) == 1:
+                answer = []
+
+                humans_num = request[0]
+                if humans_num <= maximum_full:
+                    result = things_complexity_solution(humans_num)
+                else:
+                    result = things_complexity_optimized_solution(humans_num)
+
+                answer.append("Таблица:")
+                k=0
+                for cell in result.cells:
+                    if k <= 1 or k >= humans_num-2:
+                        answer.append(f"E = {cell.etta_value}; P = {cell.probability} ({cell.good_th}/{cell.all_th})")
+                    else:
+                        answer.append(f"E = {cell.etta_value}; P ≈ {cell.probability} ({cell.good_th}/{cell.all_th})")
+                    k += 1
+                return answer
+            else:
+                return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
+        except:
+            return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
+
 def geometric_meeting_terminal():
     """
     Общее решение задачи о встрече двух участников
     """
     ln = float(input("Введите отрезок меры: "))
     fM = Meetiner(float(input("Введите начальный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
     float(input("Введите конечный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
@@ -471,42 +550,50 @@
 
                 return answer
             else:
                 return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
-def find_math_prediction_solution(table: EttaTable = None, degree: float = 1):
+def find_math_prediction_solution(table: EttaTable = None, degree: float = 1, ignore_errors: bool = False):
     """
     Нахождение МО по таблице значений случайных величин
 
     Args:
         table (EttaTable): таблица значений случайных величин
     
     Returns:
-        float: Математическое ожидание
+        string: Математическое ожидание||'ошибка распределения'
     """
     if table == None:
         return "Wrong Table"
     else:
         matP = 0
+        total_probability = 0
         for cell in table.cells:
             matP += (cell.etta_value**degree)*cell.probability
-        return matP
+            total_probability += cell.probability
+        if total_probability != 1 and not ignore_errors:
+            return "Ошибка распределения (error code: 1)"
+        return str(matP)
 
 def find_math_prediction_terminal():
     """
     Нахождение МО по таблице значений случайных величин
     """
     n = int(input("Введите количество значений в таблице: "))
     table = EttaTable()
     for i in range(0, n):
-        v, p = map(int, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
+        v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
         table.cells.append(EttaTableCell(etta_value=v, probability=p))
-    print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {find_math_prediction_solution(table)}")
+    result = find_math_prediction_solution(table)
+    if "ошибка" not in result.lower():
+        print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result}")
+    else:
+        print(result)
 
 def find_math_prediction_request(text: str = None):
     """
     Нахождение МО по таблице значений случайных величин
 
     Args:
         text (str): текст запроса, который может быть None или вводом пользователя
@@ -525,47 +612,58 @@
             table = EttaTable()
 
             for i in range(0, n):
                 table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
 
             answer = []
 
-            answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {find_math_prediction_solution(table)}")
+            result = find_math_prediction_solution(table)
+            if "ошибка" not in result.lower():
+                answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {find_math_prediction_solution(table)}")
+            else:
+                answer.append(result)
 
             return answer
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
 def find_dispersion_solution(table: EttaTable):
     """
     Функция, считающая дисперсию для таблицы СВ
 
     Args:
         table (EttaTable): таблица СВ
 
     Returns:
-        float: дисперсия СВ
+        string: дисперсия СВ/ошибка
     """
     if table != None:
         summ = 0
         math_prediction = find_math_prediction_solution(table, 1)
-        for cell in table.cells:
-            summ += (cell.etta_value - math_prediction)**2 * cell.probability
-        return summ
+        if "ошибка" not in math_prediction.lower():
+            for cell in table.cells:
+                summ += (cell.etta_value - float(math_prediction))**2 * cell.probability
+            return str(summ)
+        else:
+            return "Ошибка при вычислении мат. ожидания. Проверьте коррекность введённых данных. (error code: 1)"
 
 def find_dispersion_terminal():
     """
     Функция, считающая дисперсию для таблицы СВ
     """
     n = int(input("Введите количество значений в таблице: "))
     table = EttaTable()
     for i in range(0, n):
-        v, p = map(int, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
+        v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
         table.cells.append(EttaTableCell(etta_value=v, probability=p))
-    print(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {find_dispersion_solution(table)}")
+    result = find_dispersion_solution(table)
+    if "ошибка" not in result.lower():
+        print(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result}")
+    else:
+        print(result)
 
 def find_dispersion_request(text: str = None):
     """
     Нахождение дисперси СВ по таблице значений СВ
 
     Args:
         text (str): текст запроса, который может быть None или вводом пользователя
@@ -584,15 +682,19 @@
             table = EttaTable()
 
             for i in range(0, n):
                 table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
 
             answer = []
 
-            answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {find_dispersion_solution(table)}")
+            result = find_dispersion_solution(table)
+            if "ошибка" not in result.lower():
+                answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result}")
+            else:
+                answer.append(result)
 
             return answer
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
 def table_analysis_solution(table: EttaTable):
     """
@@ -612,18 +714,26 @@
 def table_analysis_terminal():
     """
     Функция, считающая дисперсию и математическое ожидание для таблицы СВ
     """
     n = int(input("Введите количество значений в таблице: "))
     table = EttaTable()
     for i in range(0, n):
-        v, p = map(int, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
-        table.cells.append(EttaTableCell(etta_value=v, probability=p))
+        v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения: ").split())
+        table.cells.append(EttaTableCell(etta_value=v, probability=max(p,0)))
+        
     result = table_analysis_solution(table)
-    print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}\nDx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
+
+    if "ошибка" not in result[0].lower() and "ошибка" not in result[1].lower():
+        print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}\nDx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
+    else:
+        print("Возникла ошибка при вычислении. Проверьте коррекность введённых данных.")
+        print("Дополнительная информация об ошибке:")
+        print(result[0])
+        print(result[1])
 
 def table_analysis_request(text: str = None):
     """
     Нахождение дисперси и математического ожидания СВ по таблице значений СВ
 
     Args:
         text (str): текст запроса, который может быть None или вводом пользователя
@@ -633,22 +743,29 @@
     """
     if text == None:
         return ["""Введите количество значений таблицы (число n)
 В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
     else:
         try:
             request = [float(parameter) for parameter in re.findall(regular_float, text)]
-
+            print(request)
             n = int(request[0])
             table = EttaTable()
 
             for i in range(0, n):
-                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
+                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=max(request[2+i*2],0)))
+                print(table.cells[i].probability, table.cells[i].etta_value)
 
             answer = []
             result = table_analysis_solution(table)
-            answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}")
-            answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
-
+            
+            if "ошибка" not in result[0].lower() and "ошибка" not in result[1].lower():
+                answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}")
+                answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
+            else:
+                answer.append("Возникла ошибка при вычислении. Проверьте коррекность введённых данных.")
+                answer.append("Дополнительная информация об ошибке:")
+                answer.append(result[0])
+                answer.append(result[1])
             return answer
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
```

### Comparing `MKN_third_codes-0.6.0.4/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 Metadata-Version: 2.1
-Name: MKN-third-codes
-Version: 0.6.0.4
+Name: MKN_third_codes
+Version: 0.6.4
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.0
+# 📦 Версия: 0.6.4
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
 - Функции find_disperion => нахождение дисперсии для таблицы СВ
 - Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
 - Функция combinations => число сочетаний
+- Функция complexity_universal_formula => формула, находящая коэффициент,
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
 ## 🕹 Функции
 - 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
+- 📊 Некоторые функции имеют метафикс '_optimized'. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
 ### Консоль: `pip install --upgrade MKN_third_codes`
 ## Страница библиотеки: [MKN_lib][libaPage]
 
 # 🧀 Не хотите париться с библиотекой?
 ## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
 ### Автор бота: [Алексей Шумков][LehaVK]
 
 # ☎️ Контакты #
-## Я в ВК: <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VK_Compact_Logo_%282021-present%29.svg/2048px-VK_Compact_Logo_%282021-present%29.svg.png" alt="мл-icon" height="25rem">[Долгун Иван][vkCom]
-## Я в Discord: <img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/discord-square-color-icon.png" alt="discord-icon" height="25rem" style="vertical-align: middle;">ИVAN#2599
+## Я в ВК: <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VK_Compact_Logo_%282021-present%29.svg/2048px-VK_Compact_Logo_%282021-present%29.svg.png" alt="vk-icon" height="27rem">[Долгун Иван][vkCom]
+## Я в Discord: <img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/discord-square-color-icon.png" alt="discord-icon" height="27rem" style="vertical-align: middle;">ИVAN#2599
 
 [vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.4 (02/05/2023)
+```
+------------------
+┏ добавлены 'optimized' типы функций для 'things_complexity_request' и 'things_complexity_solution'
+┣ исправлены типы для вводимых переменных в функциях. связанных с нахождением МО и D
+┣ добавлен чекер на соблюдение распределения вероятностей для функций, связанных с таблицей
+┃   ┗ error code 1: сумма вероятностей ячеек таблицы не равна 1
+┗ изменено регулярное выражение для типа float (используется в 'request' функциях)
+------------------
+```
+# ------------------
 ## 0.6.0 (01/05/2023)
 ```
 ------------------
 ┏ добавлены 'find_dispersion' решения
 ┣ добавлены 'table_analysis' решения
 ┗ иправлена ошибка в вычислениях задачи о путанице вещей
 ------------------
```

### Comparing `MKN_third_codes-0.6.0.4/PKG-INFO` & `MKN_third_codes-0.6.4/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 Metadata-Version: 2.1
-Name: MKN_third_codes
-Version: 0.6.0.4
+Name: MKN-third-codes
+Version: 0.6.4
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.0
+# 📦 Версия: 0.6.4
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
 - Функции find_disperion => нахождение дисперсии для таблицы СВ
 - Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
 - Функция combinations => число сочетаний
+- Функция complexity_universal_formula => формула, находящая коэффициент,
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
 ## 🕹 Функции
 - 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
+- 📊 Некоторые функции имеют метафикс '_optimized'. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
 ### Консоль: `pip install --upgrade MKN_third_codes`
 ## Страница библиотеки: [MKN_lib][libaPage]
 
 # 🧀 Не хотите париться с библиотекой?
 ## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
 ### Автор бота: [Алексей Шумков][LehaVK]
 
 # ☎️ Контакты #
-## Я в ВК: <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VK_Compact_Logo_%282021-present%29.svg/2048px-VK_Compact_Logo_%282021-present%29.svg.png" alt="мл-icon" height="25rem">[Долгун Иван][vkCom]
-## Я в Discord: <img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/discord-square-color-icon.png" alt="discord-icon" height="25rem" style="vertical-align: middle;">ИVAN#2599
+## Я в ВК: <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VK_Compact_Logo_%282021-present%29.svg/2048px-VK_Compact_Logo_%282021-present%29.svg.png" alt="vk-icon" height="27rem">[Долгун Иван][vkCom]
+## Я в Discord: <img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/discord-square-color-icon.png" alt="discord-icon" height="27rem" style="vertical-align: middle;">ИVAN#2599
 
 [vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.4 (02/05/2023)
+```
+------------------
+┏ добавлены 'optimized' типы функций для 'things_complexity_request' и 'things_complexity_solution'
+┣ исправлены типы для вводимых переменных в функциях. связанных с нахождением МО и D
+┣ добавлен чекер на соблюдение распределения вероятностей для функций, связанных с таблицей
+┃   ┗ error code 1: сумма вероятностей ячеек таблицы не равна 1
+┗ изменено регулярное выражение для типа float (используется в 'request' функциях)
+------------------
+```
+# ------------------
 ## 0.6.0 (01/05/2023)
 ```
 ------------------
 ┏ добавлены 'find_dispersion' решения
 ┣ добавлены 'table_analysis' решения
 ┗ иправлена ошибка в вычислениях задачи о путанице вещей
 ------------------
```

### Comparing `MKN_third_codes-0.6.0.4/README.md` & `MKN_third_codes-0.6.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.0
+# 📦 Версия: 0.6.4
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
 - Функции find_disperion => нахождение дисперсии для таблицы СВ
 - Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
 - Функция combinations => число сочетаний
+- Функция complexity_universal_formula => формула, находящая коэффициент,
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
 ## 🕹 Функции
 - 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
+- 📊 Некоторые функции имеют метафикс '_optimized'. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
 ### Консоль: `pip install --upgrade MKN_third_codes`
 ## Страница библиотеки: [MKN_lib][libaPage]
 
 # 🧀 Не хотите париться с библиотекой?
 ## Бот [Lengendary Solver Bot][AlekseiBot] предоставляет возможность использования всех возможностей библиотеки в удобном интерфейсе телеграма.
 ### Автор бота: [Алексей Шумков][LehaVK]
 
 # ☎️ Контакты #
-## Я в ВК: <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VK_Compact_Logo_%282021-present%29.svg/2048px-VK_Compact_Logo_%282021-present%29.svg.png" alt="мл-icon" height="25rem">[Долгун Иван][vkCom]
-## Я в Discord: <img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/discord-square-color-icon.png" alt="discord-icon" height="25rem" style="vertical-align: middle;">ИVAN#2599
+## Я в ВК: <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VK_Compact_Logo_%282021-present%29.svg/2048px-VK_Compact_Logo_%282021-present%29.svg.png" alt="vk-icon" height="27rem">[Долгун Иван][vkCom]
+## Я в Discord: <img src="https://uxwing.com/wp-content/themes/uxwing/download/brands-and-social-media/discord-square-color-icon.png" alt="discord-icon" height="27rem" style="vertical-align: middle;">ИVAN#2599
 
 [vkCom]: https://vk.com/ivandolgun
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
```

