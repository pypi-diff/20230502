# Comparing `tmp/MKN_third_codes-0.6.4.tar.gz` & `tmp/MKN_third_codes-0.6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.4.tar", last modified: Tue May  2 11:29:14 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.4.1.tar", last modified: Tue May  2 13:17:03 2023, max compression
```

## Comparing `MKN_third_codes-0.6.4.tar` & `MKN_third_codes-0.6.4.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 11:29:14.027226 MKN_third_codes-0.6.4/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-02 11:29:14.011270 MKN_third_codes-0.6.4/MKN_third_codes/
--rw-rw-rw-   0        0        0    38047 2023-05-02 11:26:33.000000 MKN_third_codes-0.6.4/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:29:14.026229 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     6630 2023-05-02 11:29:13.000000 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-02 11:29:13.000000 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 11:29:13.000000 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 11:29:13.000000 MKN_third_codes-0.6.4/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6630 2023-05-02 11:29:14.027226 MKN_third_codes-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     4186 2023-05-02 11:28:59.000000 MKN_third_codes-0.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-02 11:29:14.028224 MKN_third_codes-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0      503 2023-05-02 11:16:11.000000 MKN_third_codes-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:17:03.307134 MKN_third_codes-0.6.4.1/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.4.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-02 13:17:03.284197 MKN_third_codes-0.6.4.1/MKN_third_codes/
+-rw-rw-rw-   0        0        0       62 2023-05-02 13:02:12.000000 MKN_third_codes-0.6.4.1/MKN_third_codes/global_variables.py
+-rw-rw-rw-   0        0        0    28519 2023-05-02 13:02:50.000000 MKN_third_codes-0.6.4.1/MKN_third_codes/solutions.py
+-rw-rw-rw-   0        0        0     9634 2023-05-02 13:00:59.000000 MKN_third_codes-0.6.4.1/MKN_third_codes/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:17:03.305138 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     6987 2023-05-02 13:17:03.000000 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-02 13:17:03.000000 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:17:03.000000 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 13:17:03.000000 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6987 2023-05-02 13:17:03.306136 MKN_third_codes-0.6.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4362 2023-05-02 13:16:36.000000 MKN_third_codes-0.6.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 13:17:03.307134 MKN_third_codes-0.6.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-05-02 13:04:13.000000 MKN_third_codes-0.6.4.1/setup.py
```

### Comparing `MKN_third_codes-0.6.4/LICENSE.txt` & `MKN_third_codes-0.6.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.4/MKN_third_codes/solutions.py` & `MKN_third_codes-0.6.4.1/MKN_third_codes/solutions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,216 +1,11 @@
 import math
 import re
-
-class Box():
-    """
-    Класс урны (коробки) для задачи об урнах
-
-    Args:
-        white (int): кол-во белых шаров (не является параметром)
-        black (int): кол-во черных шаров (не является параметром)
-        grabbing (int): кол-во шаров, забираемых из коробки
-    
-    Parameters:
-        balls (list): массив длиной 2, хранящий информация о количестве Б и Ч шаров ([Б, Ч])
-
-    Methods:
-        None
-    """
-    def __init__(self, white:int=0, black:int=0, grabbing:int=0):
-        self.balls = [white, black]
-        self.grabbing = grabbing
-
-class Hypotes():
-    """
-    Класс гипотезы для задачи об урнах
-
-    Args:
-        balls (list): массив, длиной 2, обозначающий количество белых и чёрных шаров ([Б, Ч])
-        probability (float): вероятность наступления гипотезы
-        id (int): порядковый номер гипотезы
-    
-    Parameters:
-        depend_probability (float): вероятность достать Б шар из урны с шарами self.balls
-        hypo_text (str): строка формата 'H(id): nБ mЧ; P(H(id)) = p; P(A|H(id)) = p`'
-        summary_text (str): строка, использующаяся для составления строки для уравнения суммы вероятностей гипотез
-
-    Methods:
-        None
-    """
-    def __init__(self, balls=None, probability=0, id=0):
-        if balls == None:
-            balls = [0,0]
-        self.balls = balls
-        self.probability = probability
-        self.depend_probability = balls[0]/sum(balls)
-        self.id = id
-        self.hypo_text = f"H{self.id}: {self.balls[0]} Б, {self.balls[1]} Ч; P(H{self.id}) = {self.probability}; P(A|H{self.id}) = {self.depend_probability}"
-        self.summary_text = f"P(A|H{self.id})P(H{self.id})"
-
-class Hypoteses():
-    """
-    Класс, использующийся только для решения задачи об урнах. Бесполезен вне решения.
-
-    Methods:
-        check_correctly
-        get_whites_n_blacks_from_boxes
-        get_from_boxes
-        get_zn
-    """
-    def __init__(self, boxes):
-        self.U = boxes
-        self.P = 0
-        self.main_z = 1
-
-    def check_correctly(self, mnoz, whites, totalWhite):#проверяет, что все предоставленные слагаемые
-                                                        #содержат требуемое по условию количество шаров
-        new_mnoz = []
-        for i in range(0, len(mnoz)):
-            if whites[i] == totalWhite:
-                new_mnoz.append(mnoz[i])
-        return(new_mnoz)
-    
-    def get_whites_n_blacks_from_boxes(self, wGrab=0, id=0, whites=None, mnoz=None, totalW=0):#посчитать для взятия "wGrab" белых шаров из
-                                                                            #оставшихся урн, включая урну с индексом "id"
-        if whites == None:
-            whites = []
-        if mnoz == None:
-            mnoz = []
-        if id >= len(self.U):
-            return self.check_correctly(mnoz, whites, totalW)
-        
-        grabbing = self.U[id].grabbing#сколько всего берём шаров из урны
-
-        mx_kW = self.U[id].balls[0]#сколько всего Б шаров
-        mx_kB = self.U[id].balls[1]#сколько всего Ч шаров
-
-        mn_kW = grabbing - mx_kB#сколько минимум Б шаров потребуется
-        kW = max(mn_kW, 0)#старт Б шаров
-        kB = min(mx_kB, grabbing)#старт Ч шаров
-
-        mx_kW = max(min([mx_kW, grabbing]), 0)#максимум можно взять из этой урны Б шаров
-
-        if mnoz == []:#если множество слагаемых гипотезы пусто
-            while kW <= mx_kW:#перебираем все возможные варианты взятия шаров из этой урны
-                mnoz.append(1)
-                whites.append(kW)
-                mnoz[-1] *= combinations(kW, self.U[id].balls[0])*combinations(kB, self.U[id].balls[1])
-                kW += 1
-                kB -= 1
-        else:#если множество слагаемых гипотезы не пусто
-            new_mnoz = []
-            new_whites = []
-            while kW <= mx_kW:#перебираем все возможные варианты взятия шаров из этой урны
-                editor = combinations(kW, self.U[id].balls[0])*combinations(kB, self.U[id].balls[1])
-                for i in range(0, len(mnoz)):#каждое из существующих слагаемых умножаем на результат
-                                            #перемножения перестановок Kw из Nw и Kb из Nb шаров
-                    new_mnoz.append(mnoz[i]*editor)
-                    new_whites.append(whites[i] + kW)
-                kW += 1
-                kB -= 1
-            mnoz = new_mnoz
-            whites = new_whites
-        return self.get_whites_n_blacks_from_boxes(wGrab-kW, id+1, whites, mnoz, totalW)
-
-    def get_from_boxes(self):#решает задачу через теорему гипотез
-        grabGlob = 0#сколько всего берём шаров из урн
-        whiteGlob, blackGlob = 0, 0
-        for box in self.U:
-            grabGlob += box.grabbing
-            whiteGlob += box.balls[0]
-            blackGlob += box.balls[1]
-        
-        if grabGlob > whiteGlob+blackGlob:
-            return
-
-        revealing_after_B = max(grabGlob-blackGlob, 0)
-
-        gW = max(0, revealing_after_B)#от скольки белых шаров может находиться в n+1 урне (куда их все складывают)
-        gW_end = min(whiteGlob, grabGlob)#до скольки белых шаров может находиться в n+1 урне
-
-        hypoteses_P_array = []
-        while gW <= gW_end:#генерируем гипотезы для всех возможных количеств Белых и Черных шаров
-            hypoteses_P_array.append([sum(self.get_whites_n_blacks_from_boxes(gW, 0, [], [], gW))/self.get_zn(), gW, grabGlob-gW])
-            gW += 1
-        return hypoteses_P_array#массив вероятностей для всех гипотез
-
-    def get_zn(self):#получить общий знаменатель для формулы вероятности гипотезы
-        if self.main_z == 1:
-            for i in range(len(self.U)):
-                self.main_z *= combinations(self.U[i].grabbing, sum(self.U[i].balls))
-        return self.main_z
-
-class EttaTableCell():
-    """
-    Ячейка таблицы Етта, со значением и вероятностью
-
-    Args:
-        etta_value (int): значение СВ "Етта"
-        good_th (int): количество удачных исходов
-        all_th (int): количество всех исходов
-        probability (float): вероятность
-
-    Methods:
-        reset_probability
-    """
-    def __init__(self, etta_value:int=0, good_th:int=1, all_th:int=1, probability:float=None):
-        self.etta_value = etta_value
-        self.good_th = good_th
-        self.all_th = all_th
-        self.probability = probability
-        if self.probability == None:
-            self.reset_probability()
-
-    def reset_probability(self):
-        self.probability = self.good_th/self.all_th
-
-class EttaTable():
-    """
-    Таблица значений Етта
-
-    Args:
-        cells (): массив ячеек
-    """
-    def __init__(self, cells=None):
-        self.cells = cells
-        if self.cells == None:
-            self.cells=[]
-
-class Meetiner():
-    """
-    Класс, использующийся для решения задач типа встречи двух целей
-
-    Args:
-        start_time (float): начальный момент, относительно нулевой координаты, когда может появиться участник
-        end_time (float): конечный момент, относительно нулевой координаты, когда может появиться участник
-        waitind_time (float): кол-во меры, в течении которой участник ждёт
-    
-    Methods:
-        calculate_square
-    """
-    def __init__(self, start_time:float=0, end_time:float='inf', waiting_time:float=1):
-        if start_time >= 0:
-            self.start_time = start_time
-        else:
-            self.start_time = 0
-        if end_time >= 0:
-            self.end_time = end_time
-        else:
-            self.end_time = float('inf')
-        if waiting_time >= 0:
-            self.waiting_time = waiting_time
-        else:
-            self.waiting_time = 1
-
-    def calculate_square(self, maxEnd:float, waiter_time):
-        return ((min(self.end_time, maxEnd) - self.start_time - waiter_time)**2)/2
-
-regular_int = r'-?\d+'
-regular_float = r'-?\d+(?:[\.\,]\d+)?'
+from utils import Box, Hypotes, Hypoteses, EttaTable, EttaTableCell, Meetiner
+from global_variables import regular_int, regular_float
 
 def combinations(k:float=0,n:float=0):
     """
     Функция, считающая число сочетаний из n по k
 
     Args:
         k (float): аргумент k - количество повторений
```

### Comparing `MKN_third_codes-0.6.4/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
-Name: MKN-third-codes
-Version: 0.6.4
+Name: MKN_third_codes
+Version: 0.6.4.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.4
+# 📦 Версия: 0.6.4.1
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
 - Функции find_disperion => нахождение дисперсии для таблицы СВ
 - Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
 - Функция combinations => число сочетаний
-- Функция complexity_universal_formula => формула, находящая коэффициент,
+
+### `подробно изменения расписаны в Change Log`
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
+## Структура
+- модуль `solutions` - методы
+- модуль `utils` - классы
+- модуль `global_variables` - глобальные переменные библиотеки
 ## 🕹 Функции
-- 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
-- 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
-- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
-- 📊 Некоторые функции имеют метафикс '_optimized'. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
+- 📱 любая функция, решающая задачу имеет суффикс `_terminal`. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
+- 📲 любая функция, решающая задачу имеет суффикс `_solution`. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
+- 📨 любая функция, решающая задачу имеет суффикс `_request`. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
+- 📊 Некоторые функции имеют метафикс `_optimized`. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
 ### Консоль: `pip install --upgrade MKN_third_codes`
 ## Страница библиотеки: [MKN_lib][libaPage]
 
@@ -48,19 +53,25 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.4.1 (02/05/2023)
+```
+------------------
+━ структуризация проекта на модули utils, global_variables и solutions
+------------------
+```
 ## 0.6.4 (02/05/2023)
 ```
 ------------------
 ┏ добавлены 'optimized' типы функций для 'things_complexity_request' и 'things_complexity_solution'
-┣ исправлены типы для вводимых переменных в функциях. связанных с нахождением МО и D
+┣ исправлены типы для вводимых переменных в функциях, связанных с нахождением МО и D
 ┣ добавлен чекер на соблюдение распределения вероятностей для функций, связанных с таблицей
 ┃   ┗ error code 1: сумма вероятностей ячеек таблицы не равна 1
 ┗ изменено регулярное выражение для типа float (используется в 'request' функциях)
 ------------------
 ```
 # ------------------
 ## 0.6.0 (01/05/2023)
```

### Comparing `MKN_third_codes-0.6.4/PKG-INFO` & `MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
-Name: MKN_third_codes
-Version: 0.6.4
+Name: MKN-third-codes
+Version: 0.6.4.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.4
+# 📦 Версия: 0.6.4.1
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
 - Функции find_disperion => нахождение дисперсии для таблицы СВ
 - Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
 - Функция combinations => число сочетаний
-- Функция complexity_universal_formula => формула, находящая коэффициент,
+
+### `подробно изменения расписаны в Change Log`
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
+## Структура
+- модуль `solutions` - методы
+- модуль `utils` - классы
+- модуль `global_variables` - глобальные переменные библиотеки
 ## 🕹 Функции
-- 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
-- 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
-- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
-- 📊 Некоторые функции имеют метафикс '_optimized'. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
+- 📱 любая функция, решающая задачу имеет суффикс `_terminal`. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
+- 📲 любая функция, решающая задачу имеет суффикс `_solution`. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
+- 📨 любая функция, решающая задачу имеет суффикс `_request`. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
+- 📊 Некоторые функции имеют метафикс `_optimized`. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
 ### Консоль: `pip install --upgrade MKN_third_codes`
 ## Страница библиотеки: [MKN_lib][libaPage]
 
@@ -48,19 +53,25 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.4.1 (02/05/2023)
+```
+------------------
+━ структуризация проекта на модули utils, global_variables и solutions
+------------------
+```
 ## 0.6.4 (02/05/2023)
 ```
 ------------------
 ┏ добавлены 'optimized' типы функций для 'things_complexity_request' и 'things_complexity_solution'
-┣ исправлены типы для вводимых переменных в функциях. связанных с нахождением МО и D
+┣ исправлены типы для вводимых переменных в функциях, связанных с нахождением МО и D
 ┣ добавлен чекер на соблюдение распределения вероятностей для функций, связанных с таблицей
 ┃   ┗ error code 1: сумма вероятностей ячеек таблицы не равна 1
 ┗ изменено регулярное выражение для типа float (используется в 'request' функциях)
 ------------------
 ```
 # ------------------
 ## 0.6.0 (01/05/2023)
```

### Comparing `MKN_third_codes-0.6.4/README.md` & `MKN_third_codes-0.6.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.4
+# 📦 Версия: 0.6.4.1
 
 - Функции buckets_n_balls => задачи про урны
 - Функции things_complexity => задачи про путаницу вещей
 - Функции geometric_meeting => задачи про встречи
 - Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
 - Функции find_disperion => нахождение дисперсии для таблицы СВ
 - Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
 - Функция combinations => число сочетаний
-- Функция complexity_universal_formula => формула, находящая коэффициент,
+
+### `подробно изменения расписаны в Change Log`
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
+## Структура
+- модуль `solutions` - методы
+- модуль `utils` - классы
+- модуль `global_variables` - глобальные переменные библиотеки
 ## 🕹 Функции
-- 📱 любая функция, решающая задачу имеет суффикс '_terminal'. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
-- 📲 любая функция, решающая задачу имеет суффикс '_solution'. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
-- 📨 любая функция, решающая задачу имеет суффикс '_request'. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
-- 📊 Некоторые функции имеют метафикс '_optimized'. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
+- 📱 любая функция, решающая задачу имеет суффикс `_terminal`. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
+- 📲 любая функция, решающая задачу имеет суффикс `_solution`. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
+- 📨 любая функция, решающая задачу имеет суффикс `_request`. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
+- 📊 Некоторые функции имеют метафикс `_optimized`. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
 # ✅ Установка
 ### Консоль: `pip install --upgrade MKN_third_codes`
 ## Страница библиотеки: [MKN_lib][libaPage]
```

