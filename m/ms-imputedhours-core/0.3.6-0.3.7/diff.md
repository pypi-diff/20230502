# Comparing `tmp/ms_imputedhours_core-0.3.6.tar.gz` & `tmp/ms_imputedhours_core-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_imputedhours_core-0.3.6.tar", max compression
+gzip compressed data, was "ms_imputedhours_core-0.3.7.tar", max compression
```

## Comparing `ms_imputedhours_core-0.3.6.tar` & `ms_imputedhours_core-0.3.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/LICENSE
--rw-r--r--   0        0        0     2401 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/README.md
--rw-r--r--   0        0        0       22 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/__init__.py
--rw-r--r--   0        0        0     3238 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__tests__/__init__.py
--rw-r--r--   0        0        0     3228 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__tests__/test_agreements.py
--rw-r--r--   0        0        0     4113 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/__tests__/__init__.py
--rw-r--r--   0        0        0     6179 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/__tests__/test_employee.py
--rw-r--r--   0        0        0     6953 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__tests__/__init__.py
--rw-r--r--   0        0        0     9019 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__tests__/test_data.py
--rw-r--r--   0        0        0    10493 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/bigquery.py
--rw-r--r--   0        0        0      171 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/constants.py
--rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
--rw-r--r--   0        0        0     4491 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
--rw-r--r--   0        0        0     6206 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
--rw-r--r--   0        0        0      776 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
--rw-r--r--   0        0        0      654 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/alert.py
--rw-r--r--   0        0        0     3599 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/bigquery.py
--rw-r--r--   0        0        0      423 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/dates.py
--rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/transformers/__init__.py
--rw-r--r--   0        0        0     3828 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/transformers/hours.py
--rw-r--r--   0        0        0      203 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/office/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/office/__tests__/__init__.py
--rw-r--r--   0        0        0      678 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/office/__tests__/test_office.py
--rw-r--r--   0        0        0      950 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-02 11:35:11.139471 ms_imputedhours_core-0.3.7/LICENSE
+-rw-r--r--   0        0        0     2401 2023-05-02 11:35:11.139471 ms_imputedhours_core-0.3.7/README.md
+-rw-r--r--   0        0        0       22 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/__init__.py
+-rw-r--r--   0        0        0     3238 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__tests__/__init__.py
+-rw-r--r--   0        0        0     3228 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__tests__/test_agreements.py
+-rw-r--r--   0        0        0     2472 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/__tests__/__init__.py
+-rw-r--r--   0        0        0     9750 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/__tests__/test_employee.py
+-rw-r--r--   0        0        0     7081 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__tests__/__init__.py
+-rw-r--r--   0        0        0     9019 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__tests__/test_data.py
+-rw-r--r--   0        0        0    10493 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/bigquery.py
+-rw-r--r--   0        0        0      171 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/constants.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
+-rw-r--r--   0        0        0     4491 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
+-rw-r--r--   0        0        0     6206 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0      776 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
+-rw-r--r--   0        0        0      654 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/alert.py
+-rw-r--r--   0        0        0     3599 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/bigquery.py
+-rw-r--r--   0        0        0      423 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/dates.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/transformers/__init__.py
+-rw-r--r--   0        0        0     3828 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/transformers/hours.py
+-rw-r--r--   0        0        0      203 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/office/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/office/__tests__/__init__.py
+-rw-r--r--   0        0        0      678 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/office/__tests__/test_office.py
+-rw-r--r--   0        0        0      950 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.7/PKG-INFO
```

### Comparing `ms_imputedhours_core-0.3.6/LICENSE` & `ms_imputedhours_core-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/README.md` & `ms_imputedhours_core-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__init__.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__tests__/test_agreements.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__tests__/test_agreements.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/__tests__/test_employee.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/__tests__/test_employee.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,47 +2,48 @@
 from datetime import datetime
 from unittest.mock import Mock
 
 from freezegun import freeze_time
 
 from ms_imputedhours_core.employee import calculate_real_capacity, get_real_fte
 
-DEFAULT_AGREEMENT_HOURS = {
-    'totalHours': 150.0,
+DEFAULT_AGREEMENT_HOURS = {  # January 2022
+    'totalHours': 168.0,
     'days': {
-        1: '0',
-        2: '8',
-        3: '8',
-        4: '5.5',
-        5: '0',
-        6: '0',
-        7: '8',
-        8: '8',
-        9: '0',
-        10: '8',
-        11: '5.5',
-        12: '0',
-        13: '0',
-        14: '8',
-        15: '8',
-        16: '8',
-        17: '8',
-        18: '5.5',
-        19: '0',
-        20: '0',
-        21: '8',
-        22: '8',
-        23: '8',
-        24: '8',
-        25: '5.5',
-        26: '0',
-        27: '0',
-        28: '8',
-        29: '8',
-        30: '8',
+        '1-1': '0',
+        '2-1': '0',
+        '3-1': '8',
+        '4-1': '8',
+        '5-1': '8',
+        '6-1': '8',
+        '7-1': '8',
+        '8-1': '0',
+        '9-1': '0',
+        '10-1': '8',
+        '11-1': '8',
+        '12-1': '8',
+        '13-1': '8',
+        '14-1': '8',
+        '15-1': '0',
+        '16-1': '0',
+        '17-1': '8',
+        '18-1': '8',
+        '19-1': '8',
+        '20-1': '8',
+        '21-1': '8',
+        '22-1': '0',
+        '23-1': '0',
+        '24-1': '8',
+        '25-1': '8',
+        '26-1': '8',
+        '27-1': '8',
+        '28-1': '8',
+        '29-1': '0',
+        '30-1': '0',
+        '31-1': '8',
     },
 }
 
 
 class TestSuite(unittest.TestCase):
     @freeze_time("2022-11-11")
     def test_get_real_fte_returns_successfactor_fte_when_date_is_not_future_and_employee_has_not_fte(
@@ -95,21 +96,21 @@
     ):  # noqa: E501
         """
         A normal month is a definition for a month where the employee
         will work 100% of the hours of his agreement, and does not
         coincide with any special date as the end or start
         of the employment contract.
         """
-        expected_result = 150.0
+        expected_result = 168.0
         hiring_date = datetime.strptime('17/09/2021', '%d/%m/%Y')
         end_date = None
         date = datetime.strptime('01/01/2022', '%d/%m/%Y')
         to_date = datetime.strptime('31/01/2022', '%d/%m/%Y')
         fte = 1.0  # 100%
-        calculate_range = False
+        calculate_range = True
 
         result = calculate_real_capacity(
             DEFAULT_AGREEMENT_HOURS,
             hiring_date,
             end_date,
             date,
             to_date,
@@ -125,15 +126,15 @@
     ):  # noqa: E501
         """
         A normal month is a definition for a month where the employee
         will work 100% of the hours of his agreement, and does not
         coincide with any special date as the end or start
         of the employment contract.
         """
-        expected_result = 75.0
+        expected_result = 84.0
         hiring_date = datetime.strptime('17/09/2021', '%d/%m/%Y')
         end_date = None
         date = datetime.strptime('01/01/2022', '%d/%m/%Y')
         to_date = datetime.strptime('31/01/2022', '%d/%m/%Y')
         fte = 0.5  # 50%
         calculate_range = False
 
@@ -160,51 +161,153 @@
         of the employment contract.
         """
         expected_result = 0.0
         hiring_date = datetime.strptime('01/02/2022', '%d/%m/%Y')
         end_date = None
         date = datetime.strptime('01/01/2022', '%d/%m/%Y')
         to_date = datetime.strptime('31/01/2022', '%d/%m/%Y')
-        fte = 0.5  # 50%
+        fte = 1  # 100%
         calculate_range = False
 
         result = calculate_real_capacity(
             DEFAULT_AGREEMENT_HOURS,
             hiring_date,
             end_date,
             date,
             to_date,
             fte,
             calculate_range,
         )
 
         self.assertEqual(result, expected_result)
 
-    @freeze_time("2022-11-11")
-    def test_calculate_real_capacity_return_only_work_days_when_employee_has_end_date(
+    @freeze_time("2022-1-31")
+    def test_calculate_real_capacity_return_all_capacity_when_calculate_range_is_false(
         self,
     ):  # noqa: E501
         """
         A normal month is a definition for a month where the employee
         will work 100% of the hours of his agreement, and does not
         coincide with any special date as the end or start
         of the employment contract.
         """
-        expected_result = 33.5
+        expected_result = 168.0
         hiring_date = datetime.strptime('01/02/2021', '%d/%m/%Y')
         end_date = datetime.strptime('15/01/2022', '%d/%m/%Y')
-        date = datetime.strptime('01/01/2022', '%d/%m/%Y')
+        from_date = datetime.strptime('01/01/2022', '%d/%m/%Y')
         to_date = datetime.strptime('31/01/2022', '%d/%m/%Y')
-        fte = 0.5  # 50%
+        fte = 1  # 100%
         calculate_range = False
 
         result = calculate_real_capacity(
             DEFAULT_AGREEMENT_HOURS,
             hiring_date,
             end_date,
-            date,
+            from_date,
+            to_date,
+            fte,
+            calculate_range,
+        )
+
+        self.assertEqual(result, expected_result)
+
+    @freeze_time("2022-1-31")
+    def test_calculate_real_capacity_return_all_capacity_when_employee_end_or_hiring_date_months_are_not_equal_thant_calculation(
+        self,
+    ):  # noqa: E501
+        """
+        A normal month is a definition for a month where the employee
+        will work 100% of the hours of his agreement, and does not
+        coincide with any special date as the end or start
+        of the employment contract.
+        """
+        expected_result = 168.0
+        hiring_date = datetime.strptime('01/02/2021', '%d/%m/%Y')
+        end_date = datetime.strptime('15/02/2022', '%d/%m/%Y')
+        from_date = datetime.strptime('01/01/2022', '%d/%m/%Y')
+        to_date = datetime.strptime('31/01/2022', '%d/%m/%Y')
+        fte = 1  # 100%
+        calculate_range = True
+
+        result = calculate_real_capacity(
+            DEFAULT_AGREEMENT_HOURS,
+            hiring_date,
+            end_date,
+            from_date,
+            to_date,
+            fte,
+            calculate_range,
+        )
+
+        self.assertEqual(result, expected_result)
+
+    @freeze_time("2022-01-31")
+    def test_calculate_real_capacity_return_only_work_days_when_employee_has_end_date(
+        self,
+    ):  # noqa: E501
+        expected_result = 80.0
+        hiring_date = datetime.strptime('01/02/2021', '%d/%m/%Y')
+        end_date = datetime.strptime('15/01/2022', '%d/%m/%Y')
+        from_date = datetime.strptime('01/01/2022', '%d/%m/%Y')
+        to_date = datetime.strptime('31/01/2022', '%d/%m/%Y')
+        fte = 1  # 100%
+        calculate_range = True
+
+        result = calculate_real_capacity(
+            DEFAULT_AGREEMENT_HOURS,
+            hiring_date,
+            end_date,
+            from_date,
+            to_date,
+            fte,
+            calculate_range,
+        )
+
+        self.assertEqual(result, expected_result)
+
+    @freeze_time("2022-01-31")
+    def test_calculate_real_capacity_return_only_work_days_when_employee_hiring_date_is_same_month_than_calculation(  # noqa: E501
+        self,
+    ):
+        expected_result = 88.0
+        hiring_date = datetime.strptime('15/01/2022', '%d/%m/%Y')
+        end_date = None
+        from_date = datetime.strptime('01/01/2022', '%d/%m/%Y')
+        to_date = datetime.strptime('31/01/2022', '%d/%m/%Y')
+        fte = 1  # 100%
+        calculate_range = True
+
+        result = calculate_real_capacity(
+            DEFAULT_AGREEMENT_HOURS,
+            hiring_date,
+            end_date,
+            from_date,
+            to_date,
+            fte,
+            calculate_range,
+        )
+
+        self.assertEqual(result, expected_result)
+
+    @freeze_time("2022-01-31")
+    def test_calculate_real_capacity_return_only_work_days_when_employee_hiring_and_end_date_are_in_calculation_month(  # noqa: E501
+        self,
+    ):
+        expected_result = 80.0
+        hiring_date = datetime.strptime('15/01/2022', '%d/%m/%Y')
+        end_date = datetime.strptime('28/01/2022', '%d/%m/%Y')
+        from_date = datetime.strptime('01/01/2022', '%d/%m/%Y')
+        to_date = datetime.strptime('31/01/2022', '%d/%m/%Y')
+        fte = 1  # 100%
+        calculate_range = True
+
+        result = calculate_real_capacity(
+            DEFAULT_AGREEMENT_HOURS,
+            hiring_date,
+            end_date,
+            from_date,
             to_date,
             fte,
             calculate_range,
         )
 
         self.assertEqual(result, expected_result)
```

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__init__.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,15 @@
         )
         employee_current_capacity = (
             current_month_data.get(email, EMPTY_AGREEMENT_HOURS_DATA)[
                 'totalHours'
             ]
             / 3600
         )
+
         employee_real_capacity = calculate_real_capacity(
             agreement_hours,
             successfactor_data.get('hiring_date'),
             successfactor_data.get('enddate'),
             from_date,
             to_date,
             employee_fte,
@@ -167,14 +168,17 @@
             'real_capacity': employee_real_capacity,
             'current_capacity': employee_current_capacity,
             'current_percentage_hours_imputed': capacity_percentage,
             'supervisor': successfactor_data['supervisor'],
             'name': successfactor_data['name'],
         }
 
+        if email == 'daniel.guell@makingscience.com':
+            print(employees_data[email])
+            
     return employees_data
 
 
 def get_all_imputations_per_day(from_date, to_date):
     current_month_data = group_task_by_email(
         get_imputed_hours(from_date, to_date)
     )
@@ -208,9 +212,9 @@
             if supervisor_email not in employees_data.keys():
                 employees_data[supervisor_email] = {}
 
             employees_data[supervisor_email][email] = {
                 'data': current_data[email],
                 'name': successfactor_data['name'],
             }
-
+    # TODO:Fix this
     return employees_data
```

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__tests__/test_data.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__tests__/test_data.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/bigquery.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/alert.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/bigquery.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/transformers/hours.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/transformers/hours.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/ms_imputedhours_core/office/__tests__/test_office.py` & `ms_imputedhours_core-0.3.7/ms_imputedhours_core/office/__tests__/test_office.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.6/pyproject.toml` & `ms_imputedhours_core-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-imputedhours-core"
-version = "0.3.6"
+version = "0.3.7"
 description = "Python library to collect data about jira imputed hours and employee agreements"
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_imputedhours_core"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_imputedhours_core-0.3.6/PKG-INFO` & `ms_imputedhours_core-0.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-imputedhours-core
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python library to collect data about jira imputed hours and employee agreements
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

