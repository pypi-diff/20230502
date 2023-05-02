# Comparing `tmp/quick_resto_API-1.1.7.tar.gz` & `tmp/quick_resto_API-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_resto_API-1.1.7.tar", last modified: Fri Apr 28 14:10:46 2023, max compression
+gzip compressed data, was "quick_resto_API-1.1.8.tar", last modified: Tue May  2 14:36:18 2023, max compression
```

## Comparing `quick_resto_API-1.1.7.tar` & `quick_resto_API-1.1.8.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.804617 quick_resto_API-1.1.7/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      145 2023-04-28 14:10:46.804617 quick_resto_API-1.1.7/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      226 2022-07-30 16:30:44.000000 quick_resto_API-1.1.7/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.781618 quick_resto_API-1.1.7/quick_resto_API/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5150 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.782618 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.791618 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4403 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/account_type_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4600 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4464 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4431 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4296 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/business_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4430 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/cancellation_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4393 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/company_info_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4512 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4455 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4388 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4716 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4512 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5626 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/dish_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4297 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/employee_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4356 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/encashment_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4546 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4464 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4168 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/hall_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4546 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4612 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5869 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4225 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/markup_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4411 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5832 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/modifier_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4658 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4328 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/order_info_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4546 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4411 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4412 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/payment_type_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5869 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4430 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7934 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/providers_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4605 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4353 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/sale_place_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4600 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5933 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/semi_product_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4188 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/shift_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6047 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/single_product_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4453 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4194 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/store_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4202 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/table_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4403 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4294 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4444 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4320 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/operations_with_objects.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       25 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/system_object.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2947 2022-08-29 08:42:46.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4045 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_interface.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.791618 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.780618 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.791618 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/alcohol/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1432 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1139 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.793618 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2082 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/business.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2043 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/company_info.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2335 2022-08-08 09:56:10.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1084 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1523 2022-07-25 09:16:26.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/payment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4413 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/payment_types.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      554 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.795618 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      922 2023-04-03 12:13:12.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1050 2023-04-03 12:13:17.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/account_type.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3641 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1109 2023-04-03 12:13:08.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3911 2023-04-03 12:35:57.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/customer.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1166 2023-04-03 12:13:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1974 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3104 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1091 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/group.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4490 2022-08-29 09:39:40.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/markup.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3599 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.798618 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3912 2022-08-29 07:33:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/cancellation.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      944 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/device_command.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/encashment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1150 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/hall.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1837 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8027 2023-04-28 14:05:39.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/order_info.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4908 2023-02-09 11:42:24.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/order_item.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3107 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2661 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2285 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7697 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/shift.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2502 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2060 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3783 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4101 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1851 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3121 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.798618 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/personnel/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1478 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/personnel/employee.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1353 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/personnel/user.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.802617 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1267 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2128 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2146 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2792 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1492 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4215 2022-10-23 12:12:25.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2810 2022-09-07 13:17:38.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1069 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      678 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2008 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2708 2022-12-15 17:43:37.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2223 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4389 2023-02-09 11:48:16.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2565 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1271 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1264 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3405 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2137 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      802 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4986 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3366 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1819 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3241 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1097 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/store.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1815 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.803617 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/platform/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      393 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/platform/right.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      557 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/platform/right_link.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1447 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/platform/role.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2090 2022-09-01 15:28:18.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/quick_resto_object.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      735 2022-07-15 09:27:22.000000 quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/styler.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-28 14:10:46.782618 quick_resto_API-1.1.7/quick_resto_API.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      145 2023-04-28 14:10:46.000000 quick_resto_API-1.1.7/quick_resto_API.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8520 2023-04-28 14:10:46.000000 quick_resto_API-1.1.7/quick_resto_API.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-28 14:10:46.000000 quick_resto_API-1.1.7/quick_resto_API.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       16 2023-04-28 14:10:46.000000 quick_resto_API-1.1.7/quick_resto_API.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2023-04-28 14:10:46.804617 quick_resto_API-1.1.7/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      806 2023-04-28 14:09:33.000000 quick_resto_API-1.1.7/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.615297 quick_resto_API-1.1.8/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-02 14:36:18.615297 quick_resto_API-1.1.8/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      219 2023-05-02 14:35:20.000000 quick_resto_API-1.1.8/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.591298 quick_resto_API-1.1.8/quick_resto_API/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5150 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.593298 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.601298 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4403 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/account_type_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4600 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4464 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4431 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4296 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/business_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4430 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cancellation_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4393 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/company_info_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4512 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4455 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4388 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4716 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4512 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5626 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/dish_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4297 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/employee_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4356 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/encashment_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4546 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4464 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4168 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/hall_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4546 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4612 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5869 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4225 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/markup_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4411 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5832 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/modifier_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4658 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4328 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/order_info_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4546 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4411 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4412 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/payment_type_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5869 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4430 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7934 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/providers_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4605 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4353 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/sale_place_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4600 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5933 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/semi_product_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4188 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/shift_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6047 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/single_product_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4453 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4194 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/store_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4202 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/table_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4403 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4294 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4444 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4320 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/operations_with_objects.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       25 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/system_object.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2947 2022-08-29 08:42:46.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4045 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_interface.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.601298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.590298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.602298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1432 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1139 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.603298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2082 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/business.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2043 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/company_info.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2335 2022-08-08 09:56:10.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1084 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1523 2022-07-25 09:16:26.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/payment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4413 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/payment_types.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      554 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.605298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      922 2023-04-03 12:13:12.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1050 2023-04-03 12:13:17.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/account_type.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3641 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1109 2023-04-03 12:13:08.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3911 2023-04-03 12:35:57.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1166 2023-04-03 12:13:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1974 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3104 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1091 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/group.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4490 2022-08-29 09:39:40.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/markup.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3599 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.608298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3912 2022-08-29 07:33:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/cancellation.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      944 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/device_command.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/encashment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1150 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/hall.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1837 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8027 2023-04-28 14:05:39.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/order_info.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4908 2023-02-09 11:42:24.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/order_item.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3107 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2661 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2285 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7697 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/shift.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2502 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2060 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3783 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4101 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1851 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3121 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.608298 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1478 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/employee.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1353 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/user.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.614297 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1267 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2128 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2146 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2792 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1492 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4215 2022-10-23 12:12:25.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2810 2022-09-07 13:17:38.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1069 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      678 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2008 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2708 2022-12-15 17:43:37.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2223 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4389 2023-02-09 11:48:16.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2565 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1271 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1264 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3405 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2137 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      802 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4986 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3366 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1819 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3241 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1097 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/store.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1815 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.615297 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      393 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/right.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      557 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/right_link.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1447 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/role.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2090 2022-09-01 15:28:18.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/quick_resto_object.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      735 2022-07-15 09:27:22.000000 quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/styler.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-02 14:36:18.592298 quick_resto_API-1.1.8/quick_resto_API.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-02 14:36:18.000000 quick_resto_API-1.1.8/quick_resto_API.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8520 2023-05-02 14:36:18.000000 quick_resto_API-1.1.8/quick_resto_API.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-02 14:36:18.000000 quick_resto_API-1.1.8/quick_resto_API.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       16 2023-05-02 14:36:18.000000 quick_resto_API-1.1.8/quick_resto_API.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2023-05-02 14:36:18.615297 quick_resto_API-1.1.8/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      950 2023-05-02 14:36:05.000000 quick_resto_API-1.1.8/setup.py
```

### Comparing `quick_resto_API-1.1.7/quick_resto_API/__init__.py` & `quick_resto_API-1.1.8/quick_resto_API/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/account_type_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/account_type_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/business_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/business_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/cancellation_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cancellation_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/company_info_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/company_info_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/dish_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/dish_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/employee_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/employee_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/encashment_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/encashment_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/hall_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/hall_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/markup_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/markup_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/modifier_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/modifier_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/order_info_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/order_info_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/payment_type_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/payment_type_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/providers_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/providers_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/sale_place_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/sale_place_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/semi_product_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/semi_product_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/shift_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/shift_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/single_product_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/single_product_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/store_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/store_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/table_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/table_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/terminal_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/terminal_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/operations_with_objects/operations_with_objects.py` & `quick_resto_API-1.1.8/quick_resto_API/operations_with_objects/operations_with_objects.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_api.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_api.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_interface.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_interface.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/business.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/business.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/company_info.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/company_info.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/payment.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/payment.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/payment_types.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/payment_types.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/account_type.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/account_type.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/customer.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/group.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/group.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/markup.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/markup.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/cancellation.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/cancellation.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/device_command.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/device_command.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/encashment.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/encashment.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/hall.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/hall.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/order_info.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/order_info.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/order_item.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/order_item.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/shift.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/shift.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/table.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/table.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/terminal.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/personnel/employee.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/employee.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/personnel/user.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/personnel/user.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/store.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/store.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/platform/right_link.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/right_link.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/platform/role.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/platform/role.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/quick_resto_object.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/quick_resto_object.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API/quick_resto_objects/styler.py` & `quick_resto_API-1.1.8/quick_resto_API/quick_resto_objects/styler.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.1.7/quick_resto_API.egg-info/SOURCES.txt` & `quick_resto_API-1.1.8/quick_resto_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

