# Comparing `tmp/misura-1.1.0.tar.gz` & `tmp/misura-1.2.0.tar.gz`

## Comparing `misura-1.1.0.tar` & `misura-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.1.0/.gitattributes
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 misura-1.1.0/Makefile
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 misura-1.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 misura-1.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 misura-1.1.0/.github/SECURITY.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 misura-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 misura-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     6623 2020-02-02 00:00:00.000000 misura-1.1.0/docs/docs.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.1.0/src/misura/__init__.py
--rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 misura-1.1.0/src/misura/conversion.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 misura-1.1.0/src/misura/globals.py
--rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 misura-1.1.0/src/misura/units.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.1.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.1.0/LICENSE
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 misura-1.1.0/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 misura-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.2.0/.gitattributes
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.2.0/Makefile
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 misura-1.2.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 misura-1.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 misura-1.2.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 misura-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 misura-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 misura-1.2.0/docs/docs.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 misura-1.2.0/src/misura/__init__.py
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 misura-1.2.0/src/misura/conversion.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 misura-1.2.0/src/misura/globals.py
+-rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 misura-1.2.0/src/misura/units.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 misura-1.2.0/tests/tests.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 misura-1.2.0/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 misura-1.2.0/PKG-INFO
```

### Comparing `misura-1.1.0/.github/CODE_OF_CONDUCT.md` & `misura-1.2.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `misura-1.1.0/.github/CONTRIBUTING.md` & `misura-1.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `misura-1.1.0/.github/SECURITY.md` & `misura-1.2.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `misura-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `misura-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `misura-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.1.0/.github/workflows/python-publish.yml` & `misura-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.1.0/docs/docs.md` & `misura-1.2.0/docs/docs.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 
 ## Table of Contents
 
 0. [Projects built with misura](#projects-built-with-misura)
 1. [Introduction](#introduction)
 	1. [Globals](#globals)
 2. [Units of measure](#units-of-measure)
-	1. [Creation of numbers with units of measure](#creation-of-numbers-with-units-of-measure)
-3. [Conversions](#conversions)
+	1. [Creation of quantities with units of measure](#creation-of-quantities-with-units-of-measure)
+3. [Unit conversions](#unit-conversions)
 	1. [Available units](#available-units)
-	2. [Manually convert a number](#manually-convert-a-number)
-	3. [Partially convert a number](#partially-convert-a-number)
+	2. [Manually convert a quantity](#manually-convert-a-quantity)
+	3. [Partially convert a quantity](#partially-convert-a-quantity)
 	4. [Automatic conversion](#automatic-conversion)
+4. [Unit unpacking](#unit-unpacking)
+	1. [Manually unpacking a quantity](#manually-unpacking-a-quantity)
 
 ## Introduction
 
 Python library for easy unit handling and conversion for scientific & engineering applications.  
 
 **misura** is a Python library designed to simplify the *handling of units of measure* for scientific and engineering applications. It provides a unified interface for *dealing with different units and their conversions*, allowing for quick and accurate calculations without the need for complex manual conversions.  
 
@@ -32,21 +34,21 @@
 
 * `misura.style.unitHighlighting`, bool: Enables units of measure highlighting. Dafault: `True`.
 
 ## Units of measure
 
 [Go back to ToC](#table-of-contents)
 
-### Creation of numbers with units of measure
+### Creation of quantities with units of measure
 
 ``` python
 misura.units.unit
 	__init__(self, value: any, symbol: str)
 ```
-**value** must be an object which implements the following methods, which are the available operations between *misura.unit* objects[^1]:
+`value` must be an object which implements the following methods, which are the available operations between *misura.unit* objects[^1]:
 
 [^1]: Not all of them are needed but only the ones used.
 
 ``` python
 def __str__(self) -> str
 def __format__(self, string) -> str
 
@@ -76,26 +78,26 @@
 def __le__(self, other: any) -> any
 def __gt__(self, other: any) -> any
 def __ge__(self, other: any) -> any
 def __eq__(self, other: any) -> any
 def __ne__(self, other: any) -> any
 ```
 
-**symbol** must be the string of the units of measure, separated by a space and followed by their exponents.  
+`symbol` must be the string of the units of measure, separated by a space and followed by their exponents.  
 Some examples are:
 
 * Metres: `"m"`.
 * Metres squared: `"m2"`.
 * Metres per second: `"m s-1"`.
 * Metres per second squared: `"m s-2"`.
 * kilograms: `"kg"`.
 * Litres: `"L"`.
 * `"kg2 m-3 s4 K2.5"`
 
-## Conversions
+## Unit conversions
 
 [Go back to ToC](#table-of-contents)
 
 ### Available units
 
 Currently available units are:
 
@@ -163,15 +165,15 @@
 * from `"m2"` to `"mm2"`.
 * from `"g"` to `"kg"`.
 * from `"mW"` to `"MW"`.
 * from `"QJ"` to `"qJ"`.
 
 At the moment *it is not possible* to convert from base units to derived units and viceversa.
 
-### Manually convert a number
+### Manually convert a quantity
 
 ``` python
 misura.units.convert(first: unit, target: str, partial: bool = False) -> unit
 ```
 
 The function `convert` takes a misura.unit and a target symbol string and tries to convert it, raising a `ConversionError` should this fail.
 
@@ -185,23 +187,25 @@
 print(convert(num1, "cm2"))
 print(convert(num1, "kg"))
 ```
 
 The output is:
 
 	2000.0 cm(2)
+	
 	misura.conversion.ConversionError: cannot convert from 'm2' to 'kg'
+	raised by: '0.2 m(2)' -> 'kg'
 
-### Partially convert a number
+### Partially convert a quantity
 
 ``` python
 misura.units.convert(first: unit, target: str, partial: bool = False) -> unit
 ```
 
-A partial conversion takes place when only some of the units of measure of a number get converted.
+A partial conversion takes place when only some of the units of measure of a quantity get converted.
 
 An example is:
 
 ``` python
 from misura import unit, convert
 
 num1 = unit(200, "m s-1")
@@ -213,15 +217,15 @@
 
 	0.2 km / s
 
 The partial conversions works on the family of units that exists both in the unit and in the target passed to `convert`.
 
 ### Automatic conversion
 
-During operations between numbers with compatible but different units of measure, the second number gets converted, partially or totally, according to the first number's unit of measure.
+During operations between quantities with compatible but different units of measure, the second quantity gets converted, partially or totally, according to the first quantity's unit of measure.
 
 An example is:
 
 ``` python
 from misura import unit
 
 num1 = unit(2, "m s-1")
@@ -231,15 +235,17 @@
 print(num1 + num2)
 print(num1 + num3)
 ```
 
 The output is:
 
 	2.004 m / s
+	
 	misura.conversion.ConversionError: cannot convert from 'kg' to 'm s-1'
+	raised by: '5 kg' -> 'm s-1'
 
 Total conversion is used for operations such as addition and subraction, while partial conversion is used for multiplication and division.
 
 An example is:
 
 ``` python
 from misura import unit
@@ -248,8 +254,41 @@
 num2 = unit(4, "cm s")
 
 print(num1 * num2)
 ```
 
 The output is:
 
-	0.08 m(2) s
+	0.08 m(2) s
+
+## Unit unpacking
+
+[Go back to ToC](#table-of-contents)
+
+### Manually unpacking a quantity
+
+``` python
+def unpack(first: unit, targets: str = "") -> unit:
+```
+
+The function `unpack` takes a misura.unit and an optional target symbol string and tries to unpack the specified derived units, raising a `UnpackError` should this fail.  
+Leaving `targets` empty will unpack every derived unit.
+
+An example is:
+
+``` python
+from misura import unit, unpack
+
+num1 = unit(0.2, "C2 W")
+
+print(unpack(num1))
+print(unpack(num1, "C"))
+print(unpack(num1, "kg"))
+```
+
+The output is:
+
+	0.2 A(2) kg m(2) / s
+	0.2 A(2) W s(2)
+
+	misura.conversion.UnpackError: cannot unpack 'kg' from 'C2 W'
+	raised by: '0.2 C(2) W'
```

#### html2text {}

```diff
@@ -1,49 +1,51 @@
 # misura's documentation ## Projects built with misura Let_me_knowshould_you
 want_your_project_listed_here._##_Table_of_Contents_0._[Projects_built_with
 misura](#projects-built-with-misura)_1._[Introduction](#introduction)_1._
 [Globals](#globals)_2._[Units_of_measure](#units-of-measure)_1._[Creation_of
-numbers_with_units_of_measure](#creation-of-numbers-with-units-of-measure)_3._
-[Conversions](#conversions)_1._[Available_units](#available-units)_2._[Manually
-convert_a_number](#manually-convert-a-number)_3._[Partially_convert_a_number]
-(#partially-convert-a-number)_4._[Automatic_conversion](#automatic-conversion)
+quantities_with_units_of_measure](#creation-of-quantities-with-units-of-
+measure)_3._[Unit_conversions](#unit-conversions)_1._[Available_units]
+(#available-units)_2._[Manually_convert_a_quantity](#manually-convert-a-
+quantity)_3._[Partially_convert_a_quantity](#partially-convert-a-quantity)_4._
+[Automatic_conversion](#automatic-conversion)_4._[Unit_unpacking](#unit-
+unpacking)_1._[Manually_unpacking_a_quantity](#manually-unpacking-a-quantity)
 ##_Introduction_Python_library_for_easy_unit_handling_and_conversion_for
 scientific_&_engineering_applications._**misura**_is_a_Python_library_designed
 to_simplify_the_*handling_of_units_of_measure*_for_scientific_and_engineering
 applications._It_provides_a_unified_interface_for_*dealing_with_different_units
 and_their_conversions*,_allowing_for_quick_and_accurate_calculations_without
 the_need_for_complex_manual_conversions._**misura**_is_written_in_Python_and
 developed_by_[Andrea_Di_Antonio](https://github.com/diantonioandrea)._###
 Globals_misura_has_some_"global_options"_to_allow_personalization._Available
 options_are:_*_`misura.style.unitHighlighting`,_bool:_Enables_units_of_measure
 highlighting._Dafault:_`True`._##_Units_of_measure_[Go_back_to_ToC](#table-of-
-contents)_###_Creation_of_numbers_with_units_of_measure_```_python
-misura.units.unit___init__(self,_value:_any,_symbol:_str)_```_**value**_must_be
+contents)_###_Creation_of_quantities_with_units_of_measure_```_python
+misura.units.unit___init__(self,_value:_any,_symbol:_str)_```_`value`_must_be
 an_object_which_implements_the_following_methods,_which_are_the_available
 operations_between_*misura.unit*_objects[^1]:_[^1]:_Not_all_of_them_are_needed
 but_only_the_ones_used._```_python_def___str__(self)_->_str_def___format__
 (self,_string)_->_str_def___int__(self)_->_int_def___float__(self)_->_float_def
 __complex__(self)_->_complex_def___bool__(self)_->_bool_def___abs__(self)_-
 >_any_def___pos__(self)_->_any_def___neg__(self)_->_any_def___invert__(self)_-
 >_any_def___round__(self,_number:_int)_->_any_def___floor__(self,_number:_int)
 ->_any_def___ceil__(self,_number:_int)_->_any_def___trunc__(self,_number:_int)
 ->_any_def___add__(self,_other:_any)_->_any_def___sub__(self,_other:_any)_-
 >_any_def___mul__(self,_other:_any)_->_any_def___truediv__(self,_other:_any)_-
 >_any_def___floordiv__(self,_other:_any)_->_any_def___pow__(self,_other:_any)_-
 >_any_def___mod__(self,_other:_any)_->_any_def___lt__(self,_other:_any)_->_any
 def___le__(self,_other:_any)_->_any_def___gt__(self,_other:_any)_->_any_def
 __ge__(self,_other:_any)_->_any_def___eq__(self,_other:_any)_->_any_def___ne__
-(self,_other:_any)_->_any_```_**symbol**_must_be_the_string_of_the_units_of
+(self,_other:_any)_->_any_```_`symbol`_must_be_the_string_of_the_units_of
 measure,_separated_by_a_space_and_followed_by_their_exponents._Some_examples
 are:_*_Metres:_`"m"`._*_Metres_squared:_`"m2"`._*_Metres_per_second:_`"m_s-1"`.
 *_Metres_per_second_squared:_`"m_s-2"`._*_kilograms:_`"kg"`._*_Litres:_`"L"`._*
-`"kg2_m-3_s4_K2.5"`_##_Conversions_[Go_back_to_ToC](#table-of-contents)_###
-Available_units_Currently_available_units_are:_*_SI_base_units:_*_Time,_Second,
-**s**._*_Length,_Metre,_**m**._*_Mass,_Kilogram,_**kg**._*_Electric_current,
-Ampere,_**A**._*_Thermodynamic_temperature,_Kelvin,_**K**._*_Amount_of
+`"kg2_m-3_s4_K2.5"`_##_Unit_conversions_[Go_back_to_ToC](#table-of-contents)
+###_Available_units_Currently_available_units_are:_*_SI_base_units:_*_Time,
+Second,_**s**._*_Length,_Metre,_**m**._*_Mass,_Kilogram,_**kg**._*_Electric
+current,_Ampere,_**A**._*_Thermodynamic_temperature,_Kelvin,_**K**._*_Amount_of
 substance,_Mole,_**mol**._*_Luminous_intensity,_Candela,_**cd**._*_SI_derived
 units._*_Plane_angle,_Radian,_**rad**._*_Solid_angle,_Steradian,_**sr**._*
 Frequency,_Hertz,_**Hz**._*_Force,_Newton,_**N**._*_Pressure,_Pascal,_**Pa**._*
 Energy,_Joule,_**J**._*_Power,_Watt,_**W**._*_Electric_charge,_Coulomb,_**C**.
 *_Electric_potential,_Volt,_**V**._*_Capacitance,_Farad,_**F**._*_Resistance,
 Ohm,_**Î©**._*_Electrical_conductance,_Siemens,_**S**._*_Magnetic_flux,_Weber,
 **Wb**._*_Magentic_flux_density,_Tesla,_**T**._*_Inductance,_Henry,_**H**._*
@@ -54,30 +56,40 @@
 magnitude:_q-_=_1e-30_r-_=_1e-27_y-_=_1e-24_z-_=_1e-21_a-_=_1e-18_f-_=_1e-15_p-
 =_1e-12_n-_=_1e-09_Âµ-_=_1e-06_m-_=_1e-03_c-_=_1e-02_d-_=_1e-01_-----------
 -_da-_=_1e+01_h-_=_1e+02_k-_=_1e+03_M-_=_1e+06_G-_=_1e+09_T-_=_1e+12_P-_=_1e+15
 E-_=_1e+18_Z-_=_1e+21_Y-_=_1e+24_R-_=_1e+27_Q-_=_1e+30_so_that_all_the
 following_example_conversions_are_possible:_*_from_`"m2"`_to_`"mm2"`._*_from
 `"g"`_to_`"kg"`._*_from_`"mW"`_to_`"MW"`._*_from_`"QJ"`_to_`"qJ"`._At_the
 moment_*it_is_not_possible*_to_convert_from_base_units_to_derived_units_and
-viceversa._###_Manually_convert_a_number_```_python_misura.units.convert(first:
-unit,_target:_str,_partial:_bool_=_False)_->_unit_```_The_function_`convert`
-takes_a_misura.unit_and_a_target_symbol_string_and_tries_to_convert_it,_raising
-a_`ConversionError`_should_this_fail._An_example_is:_```_python_from_misura
-import_unit,_convert_num1_=_unit(0.2,_"m2")_print(convert(num1,_"cm2"))_print
-(convert(num1,_"kg"))_```_The_output_is:_2000.0_cm(2)
-misura.conversion.ConversionError:_cannot_convert_from_'m2'_to_'kg'_###
-Partially_convert_a_number_```_python_misura.units.convert(first:_unit,_target:
-str,_partial:_bool_=_False)_->_unit_```_A_partial_conversion_takes_place_when
-only_some_of_the_units_of_measure_of_a_number_get_converted._An_example_is:_```
-python_from_misura_import_unit,_convert_num1_=_unit(200,_"m_s-1")_print(convert
-(num1,_"km"))_```_The_output_is:_0.2_km_/_s_The_partial_conversions_works_on
-the_family_of_units_that_exists_both_in_the_unit_and_in_the_target_passed_to
-`convert`._###_Automatic_conversion_During_operations_between_numbers_with
-compatible_but_different_units_of_measure,_the_second_number_gets_converted,
-partially_or_totally,_according_to_the_first_number's_unit_of_measure._An
-example_is:_```_python_from_misura_import_unit_num1_=_unit(2,_"m_s-1")_num2_=
-unit(4,_"cm_das-1")_num3_=_unit(5,_"kg")_print(num1_+_num2)_print(num1_+_num3)
-```_The_output_is:_2.004_m_/_s_misura.conversion.ConversionError:_cannot
-convert_from_'kg'_to_'m_s-1'_Total_conversion_is_used_for_operations_such_as
+viceversa._###_Manually_convert_a_quantity_```_python_misura.units.convert
+(first:_unit,_target:_str,_partial:_bool_=_False)_->_unit_```_The_function
+`convert`_takes_a_misura.unit_and_a_target_symbol_string_and_tries_to_convert
+it,_raising_a_`ConversionError`_should_this_fail._An_example_is:_```_python
+from_misura_import_unit,_convert_num1_=_unit(0.2,_"m2")_print(convert(num1,
+"cm2"))_print(convert(num1,_"kg"))_```_The_output_is:_2000.0_cm(2)
+misura.conversion.ConversionError:_cannot_convert_from_'m2'_to_'kg'_raised_by:
+'0.2_m(2)'_->_'kg'_###_Partially_convert_a_quantity_```_python
+misura.units.convert(first:_unit,_target:_str,_partial:_bool_=_False)_->_unit
+```_A_partial_conversion_takes_place_when_only_some_of_the_units_of_measure_of
+a_quantity_get_converted._An_example_is:_```_python_from_misura_import_unit,
+convert_num1_=_unit(200,_"m_s-1")_print(convert(num1,_"km"))_```_The_output_is:
+0.2_km_/_s_The_partial_conversions_works_on_the_family_of_units_that_exists
+both_in_the_unit_and_in_the_target_passed_to_`convert`._###_Automatic
+conversion_During_operations_between_quantities_with_compatible_but_different
+units_of_measure,_the_second_quantity_gets_converted,_partially_or_totally,
+according_to_the_first_quantity's_unit_of_measure._An_example_is:_```_python
+from_misura_import_unit_num1_=_unit(2,_"m_s-1")_num2_=_unit(4,_"cm_das-1")_num3
+=_unit(5,_"kg")_print(num1_+_num2)_print(num1_+_num3)_```_The_output_is:_2.004
+m_/_s_misura.conversion.ConversionError:_cannot_convert_from_'kg'_to_'m_s-1'
+raised_by:_'5_kg'_->_'m_s-1'_Total_conversion_is_used_for_operations_such_as
 addition_and_subraction,_while_partial_conversion_is_used_for_multiplication
 and_division._An_example_is:_```_python_from_misura_import_unit_num1_=_unit(2,
 "m")_num2_=_unit(4,_"cm_s")_print(num1_*_num2)_```_The_output_is:_0.08_m(2)_s
+##_Unit_unpacking_[Go_back_to_ToC](#table-of-contents)_###_Manually_unpacking_a
+quantity_```_python_def_unpack(first:_unit,_targets:_str_=_"")_->_unit:_```_The
+function_`unpack`_takes_a_misura.unit_and_an_optional_target_symbol_string_and
+tries_to_unpack_the_specified_derived_units,_raising_a_`UnpackError`_should
+this_fail._Leaving_`targets`_empty_will_unpack_every_derived_unit._An_example
+is:_```_python_from_misura_import_unit,_unpack_num1_=_unit(0.2,_"C2_W")_print
+(unpack(num1))_print(unpack(num1,_"C"))_print(unpack(num1,_"kg"))_```_The
+output_is:_0.2_A(2)_kg_m(2)_/_s_0.2_A(2)_W_s(2)_misura.conversion.UnpackError:
+cannot_unpack_'kg'_from_'C2_W'_raised_by:_'0.2_C(2)_W'
```

### Comparing `misura-1.1.0/src/misura/conversion.py` & `misura-1.2.0/src/misura/conversion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # Exceptions.
 
 class ConversionError(Exception):
-    def __init__(self, first, target) -> None:
-        super().__init__("cannot convert from \'{}\' to \'{}\'".format(first.symbol(), target))
+    def __init__(self, first, target: str) -> None:
+        super().__init__("cannot convert from \'{0}\' to \'{1}\'\nraised by: \'{2}\' -> \'{1}\'".format(first.symbol(), target, first))
+
+class UnpackError(Exception):
+    def __init__(self, first, target: str) -> None:
+        super().__init__("cannot unpack \'{1}\' from \'{0}\'\nraised by: \'{2}\'".format(first.symbol(), target, first))
 
 # Conversion table.
 
 # Base units - SI.
 SI_TABLE = {
     "time": {'qs': 1e-30, 'rs': 1e-27, 'ys': 1e-24, 'zs': 1e-21, 'as': 1e-18, 'fs': 1e-15, 'ps': 1e-12, 'ns': 1e-09, 'µs': 1e-06, 'ms': 0.001, 'cs': 0.01, 'ds': 0.1, 's': 1.0, 'das': 10.0, 'hs': 100.0, 'ks': 1000.0, 'Ms': 1000000.0, 'Gs': 1000000000.0, 'Ts': 1000000000000.0, 'Ps': 1000000000000000.0, 'Es': 1e+18, 'Zs': 1e+21, 'Ys': 1e+24, 'Rs': 1e+27, 'Qs': 1e+30},
     
     "length": {'qm': 1e-30, 'rm': 1e-27, 'ym': 1e-24, 'zm': 1e-21, 'am': 1e-18, 'fm': 1e-15, 'pm': 1e-12, 'nm': 1e-09, 'µm': 1e-06, 'mm': 0.001, 'cm': 0.01, 'dm': 0.1, 'm': 1.0, 'dam': 10.0, 'hm': 100.0, 'km': 1000.0, 'Mm': 1000000.0, 'Gm': 1000000000.0, 'Tm': 1000000000000.0, 'Pm': 1000000000000000.0, 'Em': 1e+18, 'Zm': 1e+21, 'Ym': 1e+24, 'Rm': 1e+27, 'Qm': 1e+30},
     
     "mass": {'qg': 1e-30, 'rg': 1e-27, 'yg': 1e-24, 'zg': 1e-21, 'ag': 1e-18, 'fg': 1e-15, 'pg': 1e-12, 'ng': 1e-09, 'µg': 1e-06, 'mg': 0.001, 'cg': 0.01, 'dg': 0.1, 'g': 1.0, 'dag': 10.0, 'hg': 100.0, 'kg': 1000.0, 'Mg': 1000000.0, 'Gg': 1000000000.0, 'Tg': 1000000000000.0, 'Pg': 1000000000000000.0, 'Eg': 1e+18, 'Zg': 1e+21, 'Yg': 1e+24, 'Rg': 1e+27, 'Qg': 1e+30},
     
     "electric current": {'qA': 1e-30, 'rA': 1e-27, 'yA': 1e-24, 'zA': 1e-21, 'aA': 1e-18, 'fA': 1e-15, 'pA': 1e-12, 'nA': 1e-09, 'µA': 1e-06, 'mA': 0.001, 'cA': 0.01, 'dA': 0.1, 'A': 1.0, 'daA': 10.0, 'hA': 100.0, 'kA': 1000.0, 'MA': 1000000.0, 'GA': 1000000000.0, 'TA': 1000000000000.0, 'PA': 1000000000000000.0, 'EA': 1e+18, 'ZA': 1e+21, 'YA': 1e+24, 'RA': 1e+27, 'QA': 1e+30},
     
-    "thermodynamic temperature": {'qT': 1e-30, 'rT': 1e-27, 'yT': 1e-24, 'zT': 1e-21, 'aT': 1e-18, 'fT': 1e-15, 'pT': 1e-12, 'nT': 1e-09, 'µT': 1e-06, 'mT': 0.001, 'cT': 0.01, 'dT': 0.1, 'T': 1.0, 'daT': 10.0, 'hT': 100.0, 'kT': 1000.0, 'MT': 1000000.0, 'GT': 1000000000.0, 'TT': 1000000000000.0, 'PT': 1000000000000000.0, 'ET': 1e+18, 'ZT': 1e+21, 'YT': 1e+24, 'RT': 1e+27, 'QT': 1e+30},
+    "thermodynamic temperature": {'qK': 1e-30, 'rK': 1e-27, 'yK': 1e-24, 'zK': 1e-21, 'aK': 1e-18, 'fK': 1e-15, 'pK': 1e-12, 'nK': 1e-09, 'µK': 1e-06, 'mK': 0.001, 'cK': 0.01, 'dK': 0.1, 'K': 1.0, 'daK': 10.0, 'hK': 100.0, 'kK': 1000.0, 'MK': 1000000.0, 'GK': 1000000000.0, 'TK': 1000000000000.0, 'PK': 1000000000000000.0, 'EK': 1e+18, 'ZK': 1e+21, 'YK': 1e+24, 'RK': 1e+27, 'QK': 1e+30},
     
     "amount of substance": {'qmol': 1e-30, 'rmol': 1e-27, 'ymol': 1e-24, 'zmol': 1e-21, 'amol': 1e-18, 'fmol': 1e-15, 'pmol': 1e-12, 'nmol': 1e-09, 'µmol': 1e-06, 'mmol': 0.001, 'cmol': 0.01, 'dmol': 0.1, 'mol': 1.0, 'damol': 10.0, 'hmol': 100.0, 'kmol': 1000.0, 'Mmol': 1000000.0, 'Gmol': 1000000000.0, 'Tmol': 1000000000000.0, 'Pmol': 1000000000000000.0, 'Emol': 1e+18, 'Zmol': 1e+21, 'Ymol': 1e+24, 'Rmol': 1e+27, 'Qmol': 1e+30},
     
     "luminous intensity": {'qcd': 1e-30, 'rcd': 1e-27, 'ycd': 1e-24, 'zcd': 1e-21, 'acd': 1e-18, 'fcd': 1e-15, 'pcd': 1e-12, 'ncd': 1e-09, 'µcd': 1e-06, 'mcd': 0.001, 'ccd': 0.01, 'dcd': 0.1, 'cd': 1.0, 'dacd': 10.0, 'hcd': 100.0, 'kcd': 1000.0, 'Mcd': 1000000.0, 'Gcd': 1000000000.0, 'Tcd': 1000000000000.0, 'Pcd': 1000000000000000.0, 'Ecd': 1e+18, 'Zcd': 1e+21, 'Ycd': 1e+24, 'Rcd': 1e+27, 'Qcd': 1e+30}
 }
 
 # Derived units - SI.
@@ -63,8 +67,30 @@
     "radionuclide activity": {'qBq': 1e-30, 'rBq': 1e-27, 'yBq': 1e-24, 'zBq': 1e-21, 'aBq': 1e-18, 'fBq': 1e-15, 'pBq': 1e-12, 'nBq': 1e-09, 'µBq': 1e-06, 'mBq': 0.001, 'cBq': 0.01, 'dBq': 0.1, 'Bq': 1.0, 'daBq': 10.0, 'hBq': 100.0, 'kBq': 1000.0, 'MBq': 1000000.0, 'GBq': 1000000000.0, 'TBq': 1000000000000.0, 'PBq': 1000000000000000.0, 'EBq': 1e+18, 'ZBq': 1e+21, 'YBq': 1e+24, 'RBq': 1e+27, 'QBq': 1e+30},
 
     "absorbed dose": {'qGy': 1e-30, 'rGy': 1e-27, 'yGy': 1e-24, 'zGy': 1e-21, 'aGy': 1e-18, 'fGy': 1e-15, 'pGy': 1e-12, 'nGy': 1e-09, 'µGy': 1e-06, 'mGy': 0.001, 'cGy': 0.01, 'dGy': 0.1, 'Gy': 1.0, 'daGy': 10.0, 'hGy': 100.0, 'kGy': 1000.0, 'MGy': 1000000.0, 'GGy': 1000000000.0, 'TGy': 1000000000000.0, 'PGy': 1000000000000000.0, 'EGy': 1e+18, 'ZGy': 1e+21, 'YGy': 1e+24, 'RGy': 1e+27, 'QGy': 1e+30},
 
     "equivalent dose": {'qSv': 1e-30, 'rSv': 1e-27, 'ySv': 1e-24, 'zSv': 1e-21, 'aSv': 1e-18, 'fSv': 1e-15, 'pSv': 1e-12, 'nSv': 1e-09, 'µSv': 1e-06, 'mSv': 0.001, 'cSv': 0.01, 'dSv': 0.1, 'Sv': 1.0, 'daSv': 10.0, 'hSv': 100.0, 'kSv': 1000.0, 'MSv': 1000000.0, 'GSv': 1000000000.0, 'TSv': 1000000000000.0, 'PSv': 1000000000000000.0, 'ESv': 1e+18, 'ZSv': 1e+21, 'YSv': 1e+24, 'RSv': 1e+27, 'QSv': 1e+30},
 
     "catalyc activity": {'qkat': 1e-30, 'rkat': 1e-27, 'ykat': 1e-24, 'zkat': 1e-21, 'akat': 1e-18, 'fkat': 1e-15, 'pkat': 1e-12, 'nkat': 1e-09, 'µkat': 1e-06, 'mkat': 0.001, 'ckat': 0.01, 'dkat': 0.1, 'kat': 1.0, 'dakat': 10.0, 'hkat': 100.0, 'kkat': 1000.0, 'Mkat': 1000000.0, 'Gkat': 1000000000.0, 'Tkat': 1000000000000.0, 'Pkat': 1000000000000000.0, 'Ekat': 1e+18, 'Zkat': 1e+21, 'Ykat': 1e+24, 'Rkat': 1e+27, 'Qkat': 1e+30}
+}
+
+SI_DERIVED_UNPACKING_TABLE = {
+    "Hz": "s-1",
+    "N": "kg m s-2",
+    "Pa": "kg m-1 s-2",
+    "J": "kg m2 s-2",
+    "W": "kg m2 s-3",
+    "C": "A s",
+    "V": "kg m2 s-3 A-1",
+    "F": "kg-1 m-2 s4 A2",
+    "Ω": "kg m2 s-3 A-2",
+    "S": "kg-1 m-2 s3 A2",
+    "Wb": "kg m2 s-2 A-1",
+    "T": "kg s-2 A-1",
+    "H": "kg m2 s-2 A-2",
+    "lm": "cd sr",
+    "lx": "cd sr m-2",
+    "Bq": "s-1",
+    "Gy": "m2 s-2",
+    "Sv": "m2 s-2",
+    "kat": "mol s-1"
 }
```

### Comparing `misura-1.1.0/LICENSE` & `misura-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.1.0/README.md` & `misura-1.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 **misura** is a Python library designed to simplify the *handling of units of measure* for scientific and engineering applications. It provides a unified interface for *dealing with different units and their conversions*, allowing for quick and accurate calculations without the need for complex manual conversions.  
 
 Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/misura/blob/main/.github/CONTRIBUTING.md) and at the [examples](#examples).
 
 ### Features
 
-* Mathematical and logic perations between units: [Example](#mathematical-operations), [example](#comparisons).
+* Mathematical and logical operations between units: [Example](#mathematical-operations), [example](#comparisons).
 * Manual conversions: [Example](#manual-and-automatic-conversion).
 * Automatic conversions on operations: [Example](#manual-and-automatic-conversion).
+* Unpack derived units: [Example](#unpack-derived-units).
 * Large compatibility with other libraries: [Example](#working-with-other-libraries).
 * Custom exceptions: [Example](#comparisons).
 
 ## Installation
 
 ### Installing misura
 
@@ -115,14 +116,31 @@
 
 The output is:
 
 	20000.0 cm(2)
 	4.005 kg
 	0.4 km / s
 
+### Unpack derived units
+
+``` python
+from misura import unit, unpack
+
+num1 = unit(2, "J2")
+num2 = unit(4, "C H")
+
+print(unpack(num1))
+print(unpack(num2, "H"))
+```
+
+The output is:
+
+	2.0 kg(2) m(4) / s(4)
+	4.0 C kg m(2) / A(2) s(2)
+
 ### Comparisons
 
 ``` python
 from misura import unit
 
 num1 = unit(2, "m s-1")
 num2 = unit(4, "m s-1")
@@ -133,15 +151,17 @@
 print(num1 > num3)
 ```
 
 The output is:
 
 	False
 	True
-	misura.units.SymbolError: unsupported operand symbol(s) for >: 'm s-1.0' and 's'
+	
+	misura.conversion.ConversionError: cannot convert from 's' to 'm s-1'
+	raised by: '2 s' -> m 's-1'
 
 ### Unary operators and functions
 
 ``` python
 from misura import unit
 from misura import style
 from math import trunc
```

### Comparing `misura-1.1.0/pyproject.toml` & `misura-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["setuptools", "colorama"]
```

### Comparing `misura-1.1.0/PKG-INFO` & `misura-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
 Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -25,17 +25,18 @@
 
 **misura** is a Python library designed to simplify the *handling of units of measure* for scientific and engineering applications. It provides a unified interface for *dealing with different units and their conversions*, allowing for quick and accurate calculations without the need for complex manual conversions.  
 
 Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/misura/blob/main/.github/CONTRIBUTING.md) and at the [examples](#examples).
 
 ### Features
 
-* Mathematical and logic perations between units: [Example](#mathematical-operations), [example](#comparisons).
+* Mathematical and logical operations between units: [Example](#mathematical-operations), [example](#comparisons).
 * Manual conversions: [Example](#manual-and-automatic-conversion).
 * Automatic conversions on operations: [Example](#manual-and-automatic-conversion).
+* Unpack derived units: [Example](#unpack-derived-units).
 * Large compatibility with other libraries: [Example](#working-with-other-libraries).
 * Custom exceptions: [Example](#comparisons).
 
 ## Installation
 
 ### Installing misura
 
@@ -132,14 +133,31 @@
 
 The output is:
 
 	20000.0 cm(2)
 	4.005 kg
 	0.4 km / s
 
+### Unpack derived units
+
+``` python
+from misura import unit, unpack
+
+num1 = unit(2, "J2")
+num2 = unit(4, "C H")
+
+print(unpack(num1))
+print(unpack(num2, "H"))
+```
+
+The output is:
+
+	2.0 kg(2) m(4) / s(4)
+	4.0 C kg m(2) / A(2) s(2)
+
 ### Comparisons
 
 ``` python
 from misura import unit
 
 num1 = unit(2, "m s-1")
 num2 = unit(4, "m s-1")
@@ -150,15 +168,17 @@
 print(num1 > num3)
 ```
 
 The output is:
 
 	False
 	True
-	misura.units.SymbolError: unsupported operand symbol(s) for >: 'm s-1.0' and 's'
+	
+	misura.conversion.ConversionError: cannot convert from 's' to 'm s-1'
+	raised by: '2 s' -> m 's-1'
 
 ### Unary operators and functions
 
 ``` python
 from misura import unit
 from misura import style
 from math import trunc
```

