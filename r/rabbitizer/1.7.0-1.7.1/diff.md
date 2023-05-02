# Comparing `tmp/rabbitizer-1.7.0.tar.gz` & `tmp/rabbitizer-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitizer-1.7.0.tar", last modified: Sun Apr 30 17:01:47 2023, max compression
+gzip compressed data, was "rabbitizer-1.7.1.tar", last modified: Tue May  2 17:02:54 2023, max compression
```

## Comparing `rabbitizer-1.7.0.tar` & `rabbitizer-1.7.1.tar`

### file list

```diff
@@ -1,212 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.991098 rabbitizer-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-30 17:01:47.991098 rabbitizer-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.967098 rabbitizer-1.7.0/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.967098 rabbitizer-1.7.0/include/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/analysis/RabbitizerLoPairingInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/analysis/RabbitizerRegistersTracker.h
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/analysis/RabbitizerTrackedRegisterState.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.967098 rabbitizer-1.7.0/include/common/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/common/Abi.inc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/common/Abi_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/common/Abi_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/common/RabbitizerConfig.h
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/common/RabbitizerVersion.h
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/common/Utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.971098 rabbitizer-1.7.0/include/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/AccessType.inc
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/AccessType_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/AccessType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/InstrCategory.inc
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/InstrCategory_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/InstrCategory_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/InstrId_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/InstrId_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/InstrSuffix.inc
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/InstrSuffix_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/InstrSuffix_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/OperandType_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/OperandType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/OperandType_function_declarations.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/OperandType_function_declarations.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerAccessType.h
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerInstrCategory.h
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerInstrDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerInstrId.h
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerInstrSuffix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerInstruction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerInstructionR3000GTE.h
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerInstructionR5900.h
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerInstructionRsp.h
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerOperandType.h
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerRegister.h
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/RabbitizerRegisterDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/Registers_enums.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/Registers_enums.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.971098 rabbitizer-1.7.0/include/instructions/instr_id/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/RabbitizerInstrId_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/RabbitizerInstrId_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/RabbitizerInstrId_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/RabbitizerInstrId_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.975098 rabbitizer-1.7.0/include/instructions/instr_id/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1.inc
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.975098 rabbitizer-1.7.0/include/instructions/instr_id/r3000gte/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r3000gte/r3000gte_cop2_gte.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.975098 rabbitizer-1.7.0/include/instructions/instr_id/r5900/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop2_special1.inc
--rw-r--r--   0 runner    (1001) docker     (123)    15801 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop2_special2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_mmi.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_mmi_0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_mmi_1.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_mmi_2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_mmi_3.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.975098 rabbitizer-1.7.0/include/instructions/instr_id/rsp/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_cop2_vu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_normal_swc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.979098 rabbitizer-1.7.0/include/instructions/operands/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/operands/RabbitizerOperandType_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/operands/RabbitizerOperandType_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/operands/RabbitizerOperandType_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/operands/RabbitizerOperandType_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.979098 rabbitizer-1.7.0/include/instructions/registers/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop1Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop1N32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop1N64.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop1O32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_GprN32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_GprO32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_R5900VF.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_R5900VI.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspCop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspCop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspGpr.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspVector.inc
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/include/rabbitizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.983098 rabbitizer-1.7.0/rabbitizer/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/AccessType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/Config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/Enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/InstrCategory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/InstrId.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/LoPairingInfo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/OperandType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/RegCop1N32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/RegCop1N64.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/RegCop1O32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/RegGprN32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/RegGprO32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/RegistersTracker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/TrackedRegisterState.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/Utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.983098 rabbitizer-1.7.0/rabbitizer/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/enums_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/enums_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_enum_Abi.c
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_enum_AccessType.c
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_enum_InstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_enum_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_type_Enum.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.983098 rabbitizer-1.7.0/rabbitizer/enums/registers/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/rabbitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/rabbitizer_global_config.c
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/rabbitizer_module.c
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/rabbitizer_module.h
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/rabbitizer_submodule_Utils.c
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/rabbitizer_type_Instruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/rabbitizer_type_LoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/rabbitizer_type_RegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/rabbitizer/rabbitizer_type_TrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.983098 rabbitizer-1.7.0/rabbitizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-30 17:01:47.000000 rabbitizer-1.7.0/rabbitizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-30 17:01:47.000000 rabbitizer-1.7.0/rabbitizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:01:47.000000 rabbitizer-1.7.0/rabbitizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 17:01:47.000000 rabbitizer-1.7.0/rabbitizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 17:01:47.991098 rabbitizer-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.967098 rabbitizer-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.983098 rabbitizer-1.7.0/src/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/analysis/RabbitizerLoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/analysis/RabbitizerRegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/analysis/RabbitizerTrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.987098 rabbitizer-1.7.0/src/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/common/RabbitizerConfig.c
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/common/RabbitizerVersion.c
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/common/Utils.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.987098 rabbitizer-1.7.0/src/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/InstrCategory_Names_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/InstrCategory_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)   111098 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/InstrDescriptor_Descriptors_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/InstrDescriptor_Descriptors_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    32772 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/InstrId_Names_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/InstrId_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstrDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstrSuffix.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.987098 rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/
--rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
--rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.987098 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionCpu/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.987098 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR3000GTE/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.991098 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR5900/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
--rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:01:47.991098 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionRsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerRegister.c
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RabbitizerRegisterDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/Registers_Names_arrays.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-30 17:01:40.000000 rabbitizer-1.7.0/src/instructions/Registers_Names_arrays.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.599279 rabbitizer-1.7.1/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.599279 rabbitizer-1.7.1/include/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/analysis/RabbitizerLoPairingInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/analysis/RabbitizerRegistersTracker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/analysis/RabbitizerTrackedRegisterState.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.603278 rabbitizer-1.7.1/include/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/Abi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/Abi_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/Abi_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/RabbitizerConfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/RabbitizerVersion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/Utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.603278 rabbitizer-1.7.1/include/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/AccessType.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/AccessType_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/AccessType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrCategory.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrCategory_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrCategory_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    26768 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrId_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrId_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrIds.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrSuffix.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrSuffix_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrSuffix_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandType_enum.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandType_function_declarations.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandType_function_declarations.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandTypes.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerAccessType.h
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstrCategory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstrDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstrId.h
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstrSuffix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstruction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstructionR3000GTE.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstructionR5900.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstructionRsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerOperandType.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerRegister.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerRegisterDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/Registers_enums.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/Registers_enums.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.603278 rabbitizer-1.7.1/include/instructions/instr_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/instr_id/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/instr_id/r3000gte/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r3000gte/r3000gte_cop2_gte.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/instr_id/r5900/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_special1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_special2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_3.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/instr_id/rsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop2_vu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal_swc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/operands/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.611279 rabbitizer-1.7.1/include/instructions/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1N32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1N64.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1O32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_GprN32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_GprO32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_R5900VF.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_R5900VI.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspGpr.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspVector.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/rabbitizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.611279 rabbitizer-1.7.1/rabbitizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/Abi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/AccessType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/Config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/Enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/InstrCategory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/InstrId.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/LoPairingInfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/OperandType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegCop1N32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegCop1N64.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegCop1O32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegGprN32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegGprO32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegistersTracker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/TrackedRegisterState.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/Utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/rabbitizer/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/enums_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/enums_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_Abi.c
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_AccessType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_InstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_type_Enum.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/rabbitizer/enums/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_global_config.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_module.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_submodule_Utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_type_Instruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_type_LoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_type_RegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_type_TrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/rabbitizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-02 17:02:54.000000 rabbitizer-1.7.1/rabbitizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-02 17:02:54.000000 rabbitizer-1.7.1/rabbitizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:02:54.000000 rabbitizer-1.7.1/rabbitizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 17:02:54.000000 rabbitizer-1.7.1/rabbitizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.599279 rabbitizer-1.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/src/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/analysis/RabbitizerLoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/analysis/RabbitizerRegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/analysis/RabbitizerTrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/src/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/common/RabbitizerConfig.c
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/common/RabbitizerVersion.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/common/Utils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrCategory_Names_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrCategory_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)   113998 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrDescriptor_Descriptors_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrDescriptor_Descriptors_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    35672 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrId_Names_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrId_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstrDescriptor.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstrSuffix.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionCpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerRegister.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerRegisterDescriptor.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/Registers_Names_arrays.table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/Registers_Names_arrays.table.template
```

### Comparing `rabbitizer-1.7.0/LICENSE` & `rabbitizer-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/PKG-INFO` & `rabbitizer-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.7.0
+Version: 1.7.1
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.7.0/README.md` & `rabbitizer-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/analysis/RabbitizerLoPairingInfo.h` & `rabbitizer-1.7.1/include/analysis/RabbitizerLoPairingInfo.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/analysis/RabbitizerRegistersTracker.h` & `rabbitizer-1.7.1/include/analysis/RabbitizerRegistersTracker.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/analysis/RabbitizerTrackedRegisterState.h` & `rabbitizer-1.7.1/include/analysis/RabbitizerTrackedRegisterState.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/common/RabbitizerConfig.h` & `rabbitizer-1.7.1/include/common/RabbitizerConfig.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/common/RabbitizerVersion.h` & `rabbitizer-1.7.1/include/common/RabbitizerVersion.h`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 extern "C" {
 #endif
 
 
 // Header version
 #define RAB_VERSION_MAJOR 1
 #define RAB_VERSION_MINOR 7
-#define RAB_VERSION_PATCH 0
+#define RAB_VERSION_PATCH 1
 
 #define RAB_VERSION_STR RAB_STRINGIFY(RAB_VERSION_MAJOR) "." RAB_STRINGIFY(RAB_VERSION_MINOR) "." RAB_STRINGIFY(RAB_VERSION_PATCH)
 
 // Compiled library version
 extern const int RabVersion_Major;
 extern const int RabVersion_Minor;
 extern const int RabVersion_Patch;
```

### Comparing `rabbitizer-1.7.0/include/common/Utils.h` & `rabbitizer-1.7.1/include/common/Utils.h`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #endif
 
 
 #if !defined(__GNUC__) && !defined(__clang__)
 #define __attribute__(x)
 #endif
 
-#if __STDC_VERSION__ >= 202000L
+#if (defined(__STDC_VERSION__) && __STDC_VERSION__ >= 202000L) || (defined(__cplusplus) && __cplusplus >= 201103L)
 #define CONST [[gnu::const]]
 #define DEPRECATED(reason) [[deprecated (reason)]]
 #define FALLTHROUGH [[fallthrough]]
 #define NODISCARD [[nodiscard]]
 #define NORETURN [[noreturn]]
 #define NON_NULL(...) [[gnu::nonnull (__VA_ARGS__)]]
 #define PURE [[gnu::pure]]
@@ -69,18 +69,17 @@
  */
 #define SHIFTL(v, s, w) (MASK((v), (w)) << (s))
 #define SHIFTR(v, s, w) (MASK((v) >> (s), (w)))
 
 #define BITREPACK(fullword, v, s, w) ((SHIFTR((fullword), (s)+(w), 32-((s)+(w))) << ((s)+(w))) | SHIFTL((v), (s), (w)) | MASK((fullword), (s)))
 #define BITREPACK_RIGHT(fullword, v, s, w) (SHIFTL((v), (s), (w)) | MASK((fullword), (s)))
 
-
 #define RABUTILS_BUFFER_ADVANCE(buffer, totalSize, expression) \
     do {                                                       \
-        size_t __tempSize = expression;                        \
+        size_t __tempSize = (size_t)(expression);              \
         (buffer) += __tempSize;                                \
         (totalSize) += __tempSize;                             \
     } while (0)
 
 #define RABUTILS_BUFFER_WRITE_CHAR(buffer, totalSize, character) \
     do {                                                         \
         *(buffer) = (character);                                 \
```

### Comparing `rabbitizer-1.7.0/include/instructions/InstrId_enum.table.template` & `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_InstrId.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 /* SPDX-FileCopyrightText: © 2022 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-#define RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, ...) \
-    RABBITIZER_INSTR_ID_##prefix##_##name,
+#include "enums_utils.h"
+#include "instructions/RabbitizerInstrId.h"
 
-#define RABBITIZER_DEF_INSTR_ID_ALTNAME(prefix, caseBits, name, altname, ...) \
-    RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
 
-typedef enum RabbitizerInstrId {
-    #include "instr_id/RabbitizerInstrId_cpu.inc"
+#define RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, ...)                   { "InstrId", #prefix "_" #name, RABBITIZER_INSTR_ID_##prefix##_##name, false, NULL },
+#define RABBITIZER_DEF_INSTR_ID_ALTNAME(prefix, caseBits, name, altname, ...)  RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
 
-    #include "instr_id/RabbitizerInstrId_rsp.inc"
+RabbitizerEnumMetadata rabbitizer_enum_InstrId_enumvalues[] = {
+    #include "instructions/InstrIds.inc"
 
-    #include "instr_id/RabbitizerInstrId_r3000gte.inc"
-
-    #include "instr_id/RabbitizerInstrId_r5900.inc"
-
-    RABBITIZER_INSTR_ID_ALL_MAX = RABBITIZER_DEF_INSTR_ID(r5900, , MAX, )
-} RabbitizerInstrId;
+    RABBITIZER_DEF_INSTR_ID(ALL, , MAX, )
+    { 0 },
+};
 
 #undef RABBITIZER_DEF_INSTR_ID
 #undef RABBITIZER_DEF_INSTR_ID_ALTNAME
+
+static PyMethodDef rabbitizer_enum_InstrId_methods[] = {
+    { 0 },
+};
+
+DEF_ENUM(InstrId, "")
```

### Comparing `rabbitizer-1.7.0/include/instructions/OperandType_function_declarations.table.h` & `rabbitizer-1.7.1/include/instructions/OperandType_function_declarations.table.h`

 * *Files 16% similar despite different names*

```diff
@@ -2,81 +2,81 @@
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
 #ifndef OperandType_function_declarations_table_h_automatic
 #define OperandType_function_declarations_table_h_automatic
 
-size_t RabbitizerOperandType_process_cpu_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_rt (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_rd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_sa (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_zero (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_cop0d (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_fs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_ft (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_fd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_cop1cs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_cop2t (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_cop2cd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_op (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_code (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_code_lower (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_copraw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_label (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_immediate (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_branch_target_label (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_immediate_base (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_cpu_maybe_rd_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_rt (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_rd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_cop0d (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_cop2t (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_cop2cd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_vs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_vt (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_vd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_vt_elementhigh (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_vt_elementlow (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_vd_de (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_vs_index (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_offset_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_immediate_base (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_rsp_maybe_rd_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_rt (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_rd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_sa (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_zero (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_cop0d (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_fs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_ft (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_fd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_cop1cs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_cop2t (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_cop2cd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_op (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_code (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_code_lower (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_copraw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_label (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_immediate (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_branch_target_label (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_immediate_base (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_cpu_maybe_rd_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_rt (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_rd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_cop0d (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_cop2t (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_cop2cd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_vs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_vt (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_vd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_vt_elementhigh (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_vt_elementlow (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_vd_de (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_vs_index (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_offset_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_immediate_base (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_rsp_maybe_rd_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_r3000gte_sf (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_r3000gte_mx (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_r3000gte_v (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_r3000gte_cv (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_r3000gte_lm (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_I (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_Q (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_R (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_ACC (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_ACCxyzw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vft (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfsxyzw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vftxyzw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfdxyzw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfsn (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vftn (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfdn (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfsl (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vftl (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfdl (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfsm (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vftm (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vfdm (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vis (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vit (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vid (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vis_predecr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vit_predecr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vid_predecr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vis_postincr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vit_postincr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_vid_postincr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
-size_t RabbitizerOperandType_process_r5900_immediate5 (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_I (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_Q (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_R (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_ACC (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_ACCxyzw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vft (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfsxyzw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vftxyzw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfdxyzw (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfsn (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vftn (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfdn (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfsl (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vftl (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfdl (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfsm (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vftm (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vfdm (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vis (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vit (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vid (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vis_predecr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vit_predecr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vid_predecr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vis_postincr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vit_postincr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_vid_postincr (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
+    size_t RabbitizerOperandType_process_r5900_immediate5 (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
 
 #endif
```

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerInstrDescriptor.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerInstrDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerInstrId.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerInstrId.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerInstrSuffix.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerInstrSuffix.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerInstruction.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerInstruction.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerInstructionR3000GTE.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerInstructionR3000GTE.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerInstructionR5900.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerInstructionR5900.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerInstructionRsp.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerInstructionRsp.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerOperandType.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerOperandType.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerRegister.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerRegister.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/RabbitizerRegisterDescriptor.h` & `rabbitizer-1.7.1/include/instructions/RabbitizerRegisterDescriptor.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/Registers_enums.table.h` & `rabbitizer-1.7.1/include/instructions/Registers_enums.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/Registers_enums.table.template` & `rabbitizer-1.7.1/include/instructions/Registers_enums.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/RabbitizerInstrId_cpu.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_cpu.inc`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,109 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , INVALID,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate}
-)
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , INVALID,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate}
+    )
 
-#include "cpu/cpu_normal.inc"
-#include "cpu/cpu_special.inc"
-#include "cpu/cpu_regimm.inc"
-#include "cpu/cpu_cop0.inc"
-#include "cpu/cpu_cop0_bc0.inc"
-#include "cpu/cpu_cop0_tlb.inc"
-#include "cpu/cpu_cop1.inc"
-#include "cpu/cpu_cop1_bc1.inc"
-#include "cpu/cpu_cop1_fpu_s.inc"
-#include "cpu/cpu_cop1_fpu_d.inc"
-#include "cpu/cpu_cop1_fpu_w.inc"
-#include "cpu/cpu_cop1_fpu_l.inc"
-#include "cpu/cpu_cop2.inc"
+    #include "cpu/cpu_normal.inc"
+    #include "cpu/cpu_special.inc"
+    #include "cpu/cpu_regimm.inc"
+    #include "cpu/cpu_cop0.inc"
+    #include "cpu/cpu_cop0_bc0.inc"
+    #include "cpu/cpu_cop0_tlb.inc"
+    #include "cpu/cpu_cop1.inc"
+    #include "cpu/cpu_cop1_bc1.inc"
+    #include "cpu/cpu_cop1_fpu_s.inc"
+    #include "cpu/cpu_cop1_fpu_d.inc"
+    #include "cpu/cpu_cop1_fpu_w.inc"
+    #include "cpu/cpu_cop1_fpu_l.inc"
+    #include "cpu/cpu_cop2.inc"
 
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_00,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_01,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_02,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_03,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_04,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_05,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_06,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_07,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_08,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_09,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_10,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_11,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_12,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_13,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_14,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_15,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_16,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_17,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_18,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , USERDEF_19,
-    .operands={0}
-)
+#ifndef INSTRID_AVOID_USERDEF
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_00,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_01,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_02,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_03,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_04,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_05,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_06,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_07,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_08,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_09,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_10,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_11,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_12,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_13,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_14,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_15,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_16,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_17,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_18,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , USERDEF_19,
+        .operands={0}
+    )
+#endif
 
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , MAX,
-    .operands={0}
-)
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , MAX,
+        .operands={0}
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/RabbitizerInstrId_r5900.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_r5900.inc`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,115 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , INVALID,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN
-)
-
-#include "r5900/r5900_normal.inc"
-#include "r5900/r5900_special.inc"
-#include "r5900/r5900_regimm.inc"
-
-#include "r5900/r5900_mmi.inc"
-#include "r5900/r5900_mmi_0.inc"
-#include "r5900/r5900_mmi_1.inc"
-#include "r5900/r5900_mmi_2.inc"
-#include "r5900/r5900_mmi_3.inc"
-
-#include "r5900/r5900_cop0_tlb.inc"
-
-#include "r5900/r5900_cop1_fpu_s.inc"
-
-#include "r5900/r5900_cop2.inc"
-#include "r5900/r5900_cop2_bc2.inc"
-#include "r5900/r5900_cop2_special1.inc"
-#include "r5900/r5900_cop2_special2.inc"
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_00,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_01,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_02,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_03,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_04,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_05,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_06,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_07,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_08,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_09,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_10,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_11,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_12,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_13,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_14,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_15,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_16,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_17,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_18,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , USERDEF_19,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, , MAX,
-    .operands={0}
-)
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , INVALID,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN
+    )
+
+    #include "r5900/r5900_normal.inc"
+    #include "r5900/r5900_special.inc"
+    #include "r5900/r5900_regimm.inc"
+
+    #include "r5900/r5900_mmi.inc"
+    #include "r5900/r5900_mmi_0.inc"
+    #include "r5900/r5900_mmi_1.inc"
+    #include "r5900/r5900_mmi_2.inc"
+    #include "r5900/r5900_mmi_3.inc"
+
+    #include "r5900/r5900_cop0_tlb.inc"
+
+    #include "r5900/r5900_cop1_fpu_s.inc"
+
+    #include "r5900/r5900_cop2.inc"
+    #include "r5900/r5900_cop2_bc2.inc"
+    #include "r5900/r5900_cop2_special1.inc"
+    #include "r5900/r5900_cop2_special2.inc"
+
+#ifndef INSTRID_AVOID_USERDEF
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_00,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_01,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_02,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_03,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_04,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_05,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_06,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_07,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_08,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_09,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_10,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_11,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_12,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_13,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_14,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_15,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_16,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_17,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_18,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , USERDEF_19,
+        .operands={0}
+    )
+#endif
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, , MAX,
+        .operands={0}
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/RabbitizerInstrId_rsp.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_rsp.inc`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,110 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// RSP instructions
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , INVALID,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-
-#include "rsp/rsp_cop2.inc"
-#include "rsp/rsp_cop2_vu.inc"
-
-#include "rsp/rsp_normal_lwc2.inc"
-#include "rsp/rsp_normal_swc2.inc"
-
-// CPU instructions but with rsp registers
-
-#include "rsp/rsp_normal.inc"
-#include "rsp/rsp_special.inc"
-#include "rsp/rsp_regimm.inc"
-#include "rsp/rsp_cop0.inc"
-
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_00,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_01,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_02,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_03,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_04,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_05,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_06,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_07,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_08,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_09,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_10,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_11,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_12,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_13,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_14,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_15,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_16,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_17,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_18,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , USERDEF_19,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    rsp, , MAX,
-    .operands={0}
-)
+    // RSP instructions
+
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , INVALID,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+
+    #include "rsp/rsp_cop2.inc"
+    #include "rsp/rsp_cop2_vu.inc"
+
+    #include "rsp/rsp_normal_lwc2.inc"
+    #include "rsp/rsp_normal_swc2.inc"
+
+    // CPU instructions but with rsp registers
+
+    #include "rsp/rsp_normal.inc"
+    #include "rsp/rsp_special.inc"
+    #include "rsp/rsp_regimm.inc"
+    #include "rsp/rsp_cop0.inc"
+
+#ifndef INSTRID_AVOID_USERDEF
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_00,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_01,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_02,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_03,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_04,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_05,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_06,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_07,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_08,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_09,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_10,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_11,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_12,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_13,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_14,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_15,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_16,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_17,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_18,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , USERDEF_19,
+        .operands={0}
+    )
+#endif
+
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, , MAX,
+        .operands={0}
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop0.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0.inc`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP rt, cop0d
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x00, mfc0,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .modifiesRt=true,
-    .notEmittedByCompilers=true
-) // Move word From CP0
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x01, dmfc0,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .modifiesRt=true,
-    .notEmittedByCompilers=true
-) // Doubleword Move From CP0
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x02, cfc0,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .modifiesRt=true,
-    .notEmittedByCompilers=true
-) // Move control word From CP0
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x04, mtc0,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .readsRt=true,
-    .notEmittedByCompilers=true
-) // Move word to CP0
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x05, dmtc0,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .readsRt=true,
-    .notEmittedByCompilers=true
-) // Doubleword Move To CP0
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x06, ctc0,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .readsRt=true,
-    .notEmittedByCompilers=true
-) // Move control word To CP0
+    // OP rt, cop0d
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x00, mfc0,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .modifiesRt=true,
+        .notEmittedByCompilers=true
+    ) // Move word From CP0
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x01, dmfc0,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .modifiesRt=true,
+        .notEmittedByCompilers=true
+    ) // Doubleword Move From CP0
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x02, cfc0,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .modifiesRt=true,
+        .notEmittedByCompilers=true
+    ) // Move control word From CP0
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x04, mtc0,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .readsRt=true,
+        .notEmittedByCompilers=true
+    ) // Move word to CP0
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x05, dmtc0,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .readsRt=true,
+        .notEmittedByCompilers=true
+    ) // Doubleword Move To CP0
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x06, ctc0,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .readsRt=true,
+        .notEmittedByCompilers=true
+    ) // Move control word To CP0
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP IMM
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x00, bc0f,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isBranch=true
-) // Branch on FP False
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x01, bc0t,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isBranch=true
-) // Branch on FP True
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x02, bc0fl,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isBranch=true,
-    .isBranchLikely=true
-) // Branch on FP False Likely
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x03, bc0tl,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isBranch=true,
-    .isBranchLikely=true
-) // Branch on FP True Likely
+    // OP IMM
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x00, bc0f,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isBranch=true
+    ) // Branch on FP False
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x01, bc0t,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isBranch=true
+    ) // Branch on FP True
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x02, bc0fl,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isBranch=true,
+        .isBranchLikely=true
+    ) // Branch on FP False Likely
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x03, bc0tl,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isBranch=true,
+        .isBranchLikely=true
+    ) // Branch on FP True Likely
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x01, tlbr,
-    .operands={0},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .notEmittedByCompilers=true
-) // Read Indexed TLB Entry
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x02, tlbwi,
-    .operands={0},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .notEmittedByCompilers=true
-) // Write Indexed TLB Entry
+    // OP
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x01, tlbr,
+        .operands={0},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .notEmittedByCompilers=true
+    ) // Read Indexed TLB Entry
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x02, tlbwi,
+        .operands={0},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .notEmittedByCompilers=true
+    ) // Write Indexed TLB Entry
 
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x06, tlbwr,
-    .operands={0},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN
-) // Write Random TLB Entry
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x06, tlbwr,
+        .operands={0},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN
+    ) // Write Random TLB Entry
 
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x08, tlbp,
-    .operands={0},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .notEmittedByCompilers=true
-) // Probe TLB for Matching Entry
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x08, tlbp,
+        .operands={0},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .notEmittedByCompilers=true
+    ) // Probe TLB for Matching Entry
 
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x18, eret,
-    .operands={0},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .notEmittedByCompilers=true
-) // Return from Exception
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x18, eret,
+        .operands={0},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .notEmittedByCompilers=true
+    ) // Return from Exception
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1.inc`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP rt, fs
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x00, mfc1,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesRt=true,
-    .readsFs=true
-) // Move Word From Floating-Point
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x01, dmfc1,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesRt=true,
-    .readsFs=true
-) // Doubleword Move From Floating-Point
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x04, mtc1,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsRt=true,
-    .modifiesFs=true
-) // Move Word to Floating-Point
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x05, dmtc1,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsRt=true,
-    .modifiesFs=true
-) // Doubleword Move To Floating-Point
+    // OP rt, fs
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x00, mfc1,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesRt=true,
+        .readsFs=true
+    ) // Move Word From Floating-Point
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x01, dmfc1,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesRt=true,
+        .readsFs=true
+    ) // Doubleword Move From Floating-Point
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x04, mtc1,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsRt=true,
+        .modifiesFs=true
+    ) // Move Word to Floating-Point
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x05, dmtc1,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsRt=true,
+        .modifiesFs=true
+    ) // Doubleword Move To Floating-Point
 
-// OP rt, cop1cs
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x02, cfc1,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop1cs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesRt=true
-) // Move Control Word from Floating-Point
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x06, ctc1,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop1cs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsRt=true
-) // Move Control Word to Floating-Point
+    // OP rt, cop1cs
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x02, cfc1,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop1cs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesRt=true
+    ) // Move Control Word from Floating-Point
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x06, ctc1,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop1cs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsRt=true
+    ) // Move Control Word to Floating-Point
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP IMM
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x00, bc1f,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isBranch=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x01, bc1t,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isBranch=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x02, bc1fl,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isBranch=true,
-    .isBranchLikely=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x03, bc1tl,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isBranch=true,
-    .isBranchLikely=true
-)
+    // OP IMM
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x00, bc1f,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isBranch=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x01, bc1t,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isBranch=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x02, bc1fl,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isBranch=true,
+        .isBranchLikely=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x03, bc1tl,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isBranch=true,
+        .isBranchLikely=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc`

 * *Files 21% similar despite different names*

```diff
@@ -1,300 +1,298 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP fd, fs, ft
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x00, add_d, add.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true,
-    .readsFt=true
-) // Floating-Point Add
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x01, sub_d, sub.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true,
-    .readsFt=true
-) // Floating-Point Sub
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x02, mul_d, mul.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true,
-    .readsFt=true
-) // Floating-Point Multiply
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x03, div_d, div.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true,
-    .readsFt=true
-) // Floating-Point Divide
+    // OP fd, fs, ft
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x00, add_s, add.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true,
+        .readsFt=true
+    ) // Floating-Point Add
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x01, sub_s, sub.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true,
+        .readsFt=true
+    ) // Floating-Point Sub
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x02, mul_s, mul.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true,
+        .readsFt=true
+    ) // Floating-Point Multiply
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x03, div_s, div.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true,
+        .readsFt=true
+    ) // Floating-Point Divide
 
-// OP fd, fs
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x04, sqrt_d, sqrt.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Square Root
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x05, abs_d, abs.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Absolute Value
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x06, mov_d, mov.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Move
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x07, neg_d, neg.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Negate
+    // OP fd, fs
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x04, sqrt_s, sqrt.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Square Root
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x05, abs_s, abs.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Absolute Value
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x06, mov_s, mov.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Move
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x07, neg_s, neg.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Negate
 
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x08, round_l_d, round.l.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Round to Long Fixed-Point
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x09, trunc_l_d, trunc.l.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Truncate to Long Fixed-Point
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x0A, ceil_l_d, ceil.l.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Ceiling Convert to Long Fixed-Point
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x0B, floor_l_d, floor.l.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Floor Convert to Long Fixed-Point
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x08, round_l_s, round.l.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Round to Long Fixed-Point
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x09, trunc_l_s, trunc.l.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Truncate to Long Fixed-Point
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x0A, ceil_l_s, ceil.l.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Ceiling Convert to Long Fixed-Point
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x0B, floor_l_s, floor.l.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Floor Convert to Long Fixed-Point
 
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x0C, round_w_d, round.w.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Round to Word Fixed-Point
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x0D, trunc_w_d, trunc.w.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Truncate to Word Fixed-Point
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x0E, ceil_w_d, ceil.w.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Ceiling Convert to Word Fixed-Point
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x0F, floor_w_d, floor.w.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-) // Floating-Point Floor Convert to Word Fixed-Point
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x0C, round_w_s, round.w.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Round to Word Fixed-Point
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x0D, trunc_w_s, trunc.w.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Truncate to Word Fixed-Point
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x0E, ceil_w_s, ceil.w.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Ceiling Convert to Word Fixed-Point
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x0F, floor_w_s, floor.w.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    ) // Floating-Point Floor Convert to Word Fixed-Point
 
-// OP fd, fs
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x20, cvt_s_d, cvt.s.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .isDouble=true,
-    .modifiesFd=true,
-    .readsFs=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x24, cvt_w_d, cvt.w.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .isDouble=true,
-    .modifiesFd=true,
-    .readsFs=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x25, cvt_l_d, cvt.l.d,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .isDouble=true,
-    .modifiesFd=true,
-    .readsFs=true
-)
+    // OP fd, fs
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x21, cvt_d_s, cvt.d.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .isDouble=true,
+        .modifiesFd=true,
+        .readsFs=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x24, cvt_w_s, cvt.w.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x25, cvt_l_s, cvt.l.s,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    )
 
-// OP fs, ft
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x30, c_f_d, c.f.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x31, c_un_d, c.un.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x32, c_eq_d, c.eq.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x33, c_ueq_d, c.ueq.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x34, c_olt_d, c.olt.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x35, c_ult_d, c.ult.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x36, c_ole_d, c.ole.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x37, c_ule_d, c.ule.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
+    // OP fs, ft
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x30, c_f_s, c.f.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x31, c_un_s, c.un.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x32, c_eq_s, c.eq.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x33, c_ueq_s, c.ueq.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x34, c_olt_s, c.olt.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x35, c_ult_s, c.ult.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x36, c_ole_s, c.ole.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x37, c_ule_s, c.ule.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
 
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x38, c_df_d, c.df.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x39, c_ngle_d, c.ngle.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x3A, c_deq_d, c.deq.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x3B, c_ngl_d, c.ngl.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x3C, c_lt_d, c.lt.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x3D, c_nge_d, c.nge.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x3E, c_le_d, c.le.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x3F, c_ngt_d, c.ngt.d,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x38, c_sf_s, c.sf.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x39, c_ngle_s, c.ngle.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x3A, c_seq_s, c.seq.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x3B, c_ngl_s, c.ngl.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x3C, c_lt_s, c.lt.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x3D, c_nge_s, c.nge.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x3E, c_le_s, c.le.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x3F, c_ngt_s, c.ngt.s,
+        .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .readsFs=true,
+        .readsFt=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop0.inc`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP fd, fs
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x20, cvt_s_l, cvt.s.l,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x21, cvt_d_l, cvt.d.l,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .isDouble=true,
-    .modifiesFd=true,
-    .readsFs=true
-)
+    // OP rt, cop0d
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x00, mfc0,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_cop0d},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .modifiesRt=true,
+        .notEmittedByCompilers=true
+    ) // Move word From CP0
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x04, mtc0,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_cop0d},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .readsRt=true,
+        .notEmittedByCompilers=true
+    ) // Move word to CP0
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP fd, fs
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x20, cvt_s_w, cvt.s.w,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, 0x21, cvt_d_w, cvt.d.w,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .isFloat=true,
-    .isDouble=true,
-    .modifiesFd=true,
-    .readsFs=true
-)
+    // OP fd, fs
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x20, cvt_s_w, cvt.s.w,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x21, cvt_d_w, cvt.d.w,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .isDouble=true,
+        .modifiesFd=true,
+        .readsFs=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_cop2.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop2.inc`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP rt, cop2cd
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x00, mfc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd},
-    .modifiesRt=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x04, mtc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd},
-    .readsRt=true
-)
+    // OP rt, cop2cd
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x00, mfc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd},
+        .modifiesRt=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x04, mtc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd},
+        .readsRt=true
+    )
 
-// OP rt, cop2cd
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x02, cfc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd},
-    .modifiesRt=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x06, ctc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd},
-    .readsRt=true
-)
+    // OP rt, cop2cd
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x02, cfc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd},
+        .modifiesRt=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x06, ctc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd},
+        .readsRt=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_normal.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_normal.inc`

 * *Files 18% similar despite different names*

```diff
@@ -1,557 +1,557 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP LABEL
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x02, j,
-    .operands={RAB_OPERAND_cpu_label},
-    .instrType=RABBITIZER_INSTR_TYPE_J,
-    .isJump=true,
-    .isJumpWithAddress=true
-) // Jump
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x03, jal,
-    .operands={RAB_OPERAND_cpu_label},
-    .instrType=RABBITIZER_INSTR_TYPE_J,
-    .isJump=true,
-    .isJumpWithAddress=true,
-    .doesLink=true
-) // Jump And Link
-
-// OP rs, rt, IMM
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x04, beq,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isBranch=true,
-    .readsRs=true,
-    .readsRt=true
-) // Branch on EQual
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x05, bne,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isBranch=true,
-    .readsRs=true,
-    .readsRt=true
-) // Branch on Not Equal
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x14, beql,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isBranch=true,
-    .isBranchLikely=true,
-    .readsRs=true,
-    .readsRt=true
-) // Branch on EQual Likely
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x15, bnel,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isBranch=true,
-    .isBranchLikely=true,
-    .readsRs=true,
-    .readsRt=true
-) // Branch on Not Equal Likely
-
-// OP rs, IMM
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x06, blez,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isBranch=true,
-    .readsRs=true
-) // Branch on Less than or Equal to Zero
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x16, blezl,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isBranch=true,
-    .isBranchLikely=true,
-    .readsRs=true
-) // Branch on Less than or Equal to Zero Likely
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x07, bgtz,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isBranch=true,
-    .readsRs=true
-) // Branch on Greater Than Zero
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x17, bgtzl,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isBranch=true,
-    .isBranchLikely=true,
-    .readsRs=true
-) // Branch on Greater Than Zero Likely
-
-// OP rt, rs, IMM
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x08, addi,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true,
-    .canBeLo=true
-) // Add Immediate
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x09, addiu,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true
-) // Add Immediate Unsigned Word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0A, slti,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true
-) // Set on Less Than Immediate
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0B, sltiu,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true
-) // Set on Less Than Immediate Unsigned
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0C, andi,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isUnsigned=true,
-    .modifiesRt=true,
-    .readsRs=true
-) // And Immediate
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0D, ori,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isUnsigned=true,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true
-) // Or Immediate
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0E, xori,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isUnsigned=true,
-    .modifiesRt=true,
-    .readsRs=true
-) // eXclusive OR Immediate
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x18, daddi,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true
-) // Doubleword add Immediate
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x19, daddiu,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true
-) // Doubleword add Immediate Unsigned
-
-// OP rt, IMM
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0F, lui,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isUnsigned=true,
-    .modifiesRt=true,
-    .canBeHi=true
-) // Load Upper Immediate
-
-// OP rt, IMM(base)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x1A, ldl,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-) // Load Doubleword Left
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x1B, ldr,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-) // Load Doubleword Right
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x20, lb,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_BYTE
-) // Load Byte
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x21, lh,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_SHORT
-) // Load Halfword
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x22, lwl,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-) // Load Word Left
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x23, lw,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_WORD
-) // Load Word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x24, lbu,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_BYTE,
-    .doesUnsignedMemoryAccess=true
-) // Load Byte Insigned
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x25, lhu,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_SHORT,
-    .doesUnsignedMemoryAccess=true
-) // Load Halfword Unsigned
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x26, lwr,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-) // Load Word Right
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x27, lwu,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_WORD,
-    .doesUnsignedMemoryAccess=true
-) // Load Word Unsigned
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x28, sb,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true,
-    .accessType=RAB_ACCESSTYPE_BYTE
-) // Store Byte
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x29, sh,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true,
-    .accessType=RAB_ACCESSTYPE_SHORT
-) // Store Halfword
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2A, swl,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-) // Store Word Left
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2B, sw,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true,
-    .accessType=RAB_ACCESSTYPE_WORD
-) // Store Word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2C, sdl,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-) // Store Doubleword Left
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2D, sdr,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-) // Store Doubleword Right
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2E, swr,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-) // Store Word Right
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x30, ll,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-) // Load Linked word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x33, pref,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true
-) // Prefetch
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x34, lld,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-) // Load Linked Doubleword
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x37, ld,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_DOUBLEWORD
-) // Load Doubleword
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x38, sc,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .notEmittedByCompilers=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-) // Store Conditional word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3C, scd,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .notEmittedByCompilers=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-) // Store Conditional Doubleword
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3F, sd,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true,
-    .accessType=RAB_ACCESSTYPE_DOUBLEWORD
-) // Store Doubleword
-
-// OP op, IMM(base)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2F, cache,
-    .operands={RAB_OPERAND_cpu_op, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .notEmittedByCompilers=true
-) // Cache
-
-// OP ft, IMM(base)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x31, lwc1,
-    .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isFloat=true,
-    .readsRs=true,
-    .modifiesFt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_FLOAT
-) // Load Word to Coprocessor z
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x35, ldc1,
-    .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isFloat=true,
-    .isDouble=true,
-    .readsRs=true,
-    .modifiesFt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_DOUBLEFLOAT
-) // Load Doubleword to Coprocessor z
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x39, swc1,
-    .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isFloat=true,
-    .readsRs=true,
-    .readsFt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true,
-    .accessType=RAB_ACCESSTYPE_FLOAT
-) // Store Word from Coprocessor z
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3D, sdc1,
-    .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isFloat=true,
-    .isDouble=true,
-    .readsRs=true,
-    .readsFt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true,
-    .accessType=RAB_ACCESSTYPE_DOUBLEFLOAT
-) // Store Doubleword from Coprocessor z
-
-// OP cop2t, IMM(base)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x32, lwc2,
-    .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-) // Load Word to Coprocessor z
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x36, ldc2,
-    .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-) // Load Doubleword to Coprocessor z
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3A, swc2,
-    .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-) // Store Word from Coprocessor z
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3E, sdc2,
-    .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-) // Store Doubleword from Coprocessor z
-
-
-// Pseudo-Instruction Unique IDs
-
-// OP IMM
-RABBITIZER_DEF_INSTR_ID(
-    cpu, -0x03, b,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isBranch=true,
-    .isPseudo=true
-) // Branch (unconditional)
-
-// OP rs, IMM
-RABBITIZER_DEF_INSTR_ID(
-    cpu, -0x04, beqz,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .isBranch=true,
-    .isPseudo=true
-) // Branch on EQual Zero
-RABBITIZER_DEF_INSTR_ID(
-    cpu, -0x05, bnez,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .isBranch=true,
-    .isPseudo=true
-) // Branch on Not Equal Zero
+    // OP LABEL
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x02, j,
+        .operands={RAB_OPERAND_cpu_label},
+        .instrType=RABBITIZER_INSTR_TYPE_J,
+        .isJump=true,
+        .isJumpWithAddress=true
+    ) // Jump
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x03, jal,
+        .operands={RAB_OPERAND_cpu_label},
+        .instrType=RABBITIZER_INSTR_TYPE_J,
+        .isJump=true,
+        .isJumpWithAddress=true,
+        .doesLink=true
+    ) // Jump And Link
+
+    // OP rs, rt, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x04, beq,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isBranch=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Branch on EQual
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x05, bne,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isBranch=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Branch on Not Equal
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x14, beql,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isBranch=true,
+        .isBranchLikely=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Branch on EQual Likely
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x15, bnel,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isBranch=true,
+        .isBranchLikely=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Branch on Not Equal Likely
+
+    // OP rs, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x06, blez,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isBranch=true,
+        .readsRs=true
+    ) // Branch on Less than or Equal to Zero
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x16, blezl,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isBranch=true,
+        .isBranchLikely=true,
+        .readsRs=true
+    ) // Branch on Less than or Equal to Zero Likely
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x07, bgtz,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isBranch=true,
+        .readsRs=true
+    ) // Branch on Greater Than Zero
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x17, bgtzl,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isBranch=true,
+        .isBranchLikely=true,
+        .readsRs=true
+    ) // Branch on Greater Than Zero Likely
+
+    // OP rt, rs, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x08, addi,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true,
+        .canBeLo=true
+    ) // Add Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x09, addiu,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true
+    ) // Add Immediate Unsigned Word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0A, slti,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true
+    ) // Set on Less Than Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0B, sltiu,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true
+    ) // Set on Less Than Immediate Unsigned
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0C, andi,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isUnsigned=true,
+        .modifiesRt=true,
+        .readsRs=true
+    ) // And Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0D, ori,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isUnsigned=true,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true
+    ) // Or Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0E, xori,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isUnsigned=true,
+        .modifiesRt=true,
+        .readsRs=true
+    ) // eXclusive OR Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x18, daddi,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true
+    ) // Doubleword add Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x19, daddiu,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true
+    ) // Doubleword add Immediate Unsigned
+
+    // OP rt, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0F, lui,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isUnsigned=true,
+        .modifiesRt=true,
+        .canBeHi=true
+    ) // Load Upper Immediate
+
+    // OP rt, IMM(base)
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x1A, ldl,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Load Doubleword Left
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x1B, ldr,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Load Doubleword Right
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x20, lb,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_BYTE
+    ) // Load Byte
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x21, lh,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_SHORT
+    ) // Load Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x22, lwl,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Load Word Left
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x23, lw,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_WORD
+    ) // Load Word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x24, lbu,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_BYTE,
+        .doesUnsignedMemoryAccess=true
+    ) // Load Byte Insigned
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x25, lhu,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_SHORT,
+        .doesUnsignedMemoryAccess=true
+    ) // Load Halfword Unsigned
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x26, lwr,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Load Word Right
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x27, lwu,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_WORD,
+        .doesUnsignedMemoryAccess=true
+    ) // Load Word Unsigned
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x28, sb,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true,
+        .accessType=RAB_ACCESSTYPE_BYTE
+    ) // Store Byte
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x29, sh,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true,
+        .accessType=RAB_ACCESSTYPE_SHORT
+    ) // Store Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2A, swl,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Store Word Left
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2B, sw,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true,
+        .accessType=RAB_ACCESSTYPE_WORD
+    ) // Store Word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2C, sdl,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Store Doubleword Left
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2D, sdr,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Store Doubleword Right
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2E, swr,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Store Word Right
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x30, ll,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Load Linked word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x33, pref,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true
+    ) // Prefetch
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x34, lld,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Load Linked Doubleword
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x37, ld,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_DOUBLEWORD
+    ) // Load Doubleword
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x38, sc,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .notEmittedByCompilers=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Store Conditional word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3C, scd,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .notEmittedByCompilers=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Store Conditional Doubleword
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3F, sd,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true,
+        .accessType=RAB_ACCESSTYPE_DOUBLEWORD
+    ) // Store Doubleword
+
+    // OP op, IMM(base)
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2F, cache,
+        .operands={RAB_OPERAND_cpu_op, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .notEmittedByCompilers=true
+    ) // Cache
+
+    // OP ft, IMM(base)
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x31, lwc1,
+        .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isFloat=true,
+        .readsRs=true,
+        .modifiesFt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_FLOAT
+    ) // Load Word to Coprocessor z
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x35, ldc1,
+        .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isFloat=true,
+        .isDouble=true,
+        .readsRs=true,
+        .modifiesFt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_DOUBLEFLOAT
+    ) // Load Doubleword to Coprocessor z
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x39, swc1,
+        .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isFloat=true,
+        .readsRs=true,
+        .readsFt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true,
+        .accessType=RAB_ACCESSTYPE_FLOAT
+    ) // Store Word from Coprocessor z
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3D, sdc1,
+        .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isFloat=true,
+        .isDouble=true,
+        .readsRs=true,
+        .readsFt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true,
+        .accessType=RAB_ACCESSTYPE_DOUBLEFLOAT
+    ) // Store Doubleword from Coprocessor z
+
+    // OP cop2t, IMM(base)
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x32, lwc2,
+        .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Load Word to Coprocessor z
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x36, ldc2,
+        .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Load Doubleword to Coprocessor z
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3A, swc2,
+        .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Store Word from Coprocessor z
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3E, sdc2,
+        .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Store Doubleword from Coprocessor z
+
+
+    // Pseudo-Instruction Unique IDs
+
+    // OP IMM
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, -0x03, b,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isBranch=true,
+        .isPseudo=true
+    ) // Branch (unconditional)
+
+    // OP rs, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, -0x04, beqz,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .isBranch=true,
+        .isPseudo=true
+    ) // Branch on EQual Zero
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, -0x05, bnez,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .isBranch=true,
+        .isPseudo=true
+    ) // Branch on Not Equal Zero
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_regimm.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_regimm.inc`

 * *Files 11% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP rs, IMM
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x00, bltz,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .readsRs=true
-) // Branch on Less Than Zero
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x01, bgez,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .readsRs=true
-) // Branch on Greater than or Equal to Zero
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x02, bltzl,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .isBranchLikely=true,
-    .readsRs=true
-) // Branch on Less Than Zero Likely
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x03, bgezl,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .isBranchLikely=true,
-    .readsRs=true
-) // Branch on Greater than or Equal to Zero Likely
-
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x08, tgei,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isTrap=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x09, tgeiu,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isTrap=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0A, tlti,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isTrap=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0B, tltiu,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isTrap=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0C, teqi,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isTrap=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0E, tnei,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isTrap=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x10, bltzal,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .readsRs=true,
-    .doesLink=true
-) // Branch on Less Than Zero and Link
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x11, bgezal,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .readsRs=true,
-    .doesLink=true
-) // Branch on Greater Than or Equal to Zero and Link
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x12, bltzall,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .isBranchLikely=true,
-    .readsRs=true,
-    .doesLink=true
-) // Branch on Less Than Zero and Link Likely
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x13, bgezall,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .isBranchLikely=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true,
-    .doesLink=true
-) // Branch on Greater Than or Equal to Zero and Link Likely
-
-
-// Pseudo-Instruction Unique IDs
-
-RABBITIZER_DEF_INSTR_ID(
-    cpu, -0x11, bal,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .notEmittedByCompilers=true,
-    .doesLink=true,
-    .isPseudo=true
-) // Branch and Link
+    // OP rs, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x00, bltz,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .readsRs=true
+    ) // Branch on Less Than Zero
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x01, bgez,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .readsRs=true
+    ) // Branch on Greater than or Equal to Zero
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x02, bltzl,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .isBranchLikely=true,
+        .readsRs=true
+    ) // Branch on Less Than Zero Likely
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x03, bgezl,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .isBranchLikely=true,
+        .readsRs=true
+    ) // Branch on Greater than or Equal to Zero Likely
+
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x08, tgei,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isTrap=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x09, tgeiu,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isTrap=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0A, tlti,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isTrap=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0B, tltiu,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isTrap=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0C, teqi,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isTrap=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0E, tnei,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isTrap=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x10, bltzal,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .readsRs=true,
+        .doesLink=true
+    ) // Branch on Less Than Zero and Link
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x11, bgezal,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .readsRs=true,
+        .doesLink=true
+    ) // Branch on Greater Than or Equal to Zero and Link
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x12, bltzall,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .isBranchLikely=true,
+        .readsRs=true,
+        .doesLink=true
+    ) // Branch on Less Than Zero and Link Likely
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x13, bgezall,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .isBranchLikely=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true,
+        .doesLink=true
+    ) // Branch on Greater Than or Equal to Zero and Link Likely
+
+
+    // Pseudo-Instruction Unique IDs
+
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, -0x11, bal,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .notEmittedByCompilers=true,
+        .doesLink=true,
+        .isPseudo=true
+    ) // Branch and Link
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/cpu/cpu_special.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_special.inc`

 * *Files 14% similar despite different names*

```diff
@@ -1,534 +1,534 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP rd, rt, sa
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x00, sll,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Shift word Left Logical
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x02, srl,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Shift word Right Logical
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x03, sra,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Shift word Right Arithmetic
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x38, dsll,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Doubleword Shift Left Logical
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3A, dsrl,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Doubleword Shift Right Logical
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3B, dsra,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Doubleword Shift Right Arithmetic
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3C, dsll32,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Doubleword Shift Left Logical plus 32
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3E, dsrl32,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Doubleword Shift Right Logical plus 32
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x3F, dsra32,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Doubleword Shift Right Arithmetic plus 32
-
-// OP rd, rt, rs
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x14, dsllv,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Doubleword Shift Left Logical Variable
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x16, dsrlv,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Doubleword Shift Right Logical Variable
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x17, dsrav,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Doubleword Shift Right Arithmetic Variable
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x04, sllv,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Shift word Left Logical Variable
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x06, srlv,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Shift word Right Logical Variable
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x07, srav,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Shift word Right Arithmetic Variable
-
-// OP rs
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x11, mthi,
-    .operands={RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .modifiesHI=true
-) // Move To HI register
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x13, mtlo,
-    .operands={RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .modifiesLO=true
-) // Move To LO register
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x08, jr,
-    .operands={RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .isJump=true
-) // Jump Register
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x09, jalr,
-    .operands={RAB_OPERAND_cpu_maybe_rd_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .isJump=true,
-    .modifiesRd=true,
-    .readsRs=true,
-    .doesLink=true
-) // Jump And Link Register
-
-// OP rd
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x10, mfhi,
-    .operands={RAB_OPERAND_cpu_rd},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsHI=true
-) // Move From HI register
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x12, mflo,
-    .operands={RAB_OPERAND_cpu_rd},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsLO=true
-) // Move From LO register
-
-// OP rd, rs, rt
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0A, movz,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // MOVe conditional on Zero
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0B, movn,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // MOVe conditional on Not zero
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x1A, div,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .readsRd=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // DIVide word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x1B, divu,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .readsRd=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // DIVide Unsigned word
-
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, -0x1A, sn64_div, div,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // DIVide word
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    cpu, -0x1B, sn64_divu, divu,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // DIVide Unsigned word
-
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x1E, ddiv,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .readsRd=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // Doubleword DIVide
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x1F, ddivu,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .readsRd=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // Doubleword DIVide Unsigned
-
-/*
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , ddiv,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-)
-*/
-/*
-RABBITIZER_DEF_INSTR_ID(
-    cpu, , ddivu,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-)
-*/
-
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x20, add,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true,
-    .notEmittedByCompilers=true
-) // ADD word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x21, addu,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true,
-    .maybeIsMove=true
-) // ADD Unsigned word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x22, sub,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .notEmittedByCompilers=true,
-    .readsRs=true,
-    .readsRt=true
-) // Subtract word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x23, subu,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // SUBtract Unsigned word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x24, and,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // AND
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x25, or,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .maybeIsMove=true,
-    .readsRs=true,
-    .readsRt=true
-) // OR
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x26, xor,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // eXclusive OR
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x27, nor,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Not OR
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2A, slt,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Set on Less Than
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2B, sltu,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Set on Less Than Unsigned
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2C, dadd,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Doubleword Add
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2D, daddu,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true,
-    .maybeIsMove=true
-) // Doubleword Add Unsigned
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2E, dsub,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Doubleword SUBtract
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x2F, dsubu,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Doubleword SUBtract Unsigned
-
-// OP code
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0C, syscall,
-    .operands={RAB_OPERAND_cpu_code},
-    .instrType=RABBITIZER_INSTR_TYPE_R
-) // SYStem CALL
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0D, break,
-    .operands={RAB_OPERAND_cpu_code},
-    .instrType=RABBITIZER_INSTR_TYPE_R
-) // Break
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x0F, sync,
-    .operands={0},
-    .instrType=RABBITIZER_INSTR_TYPE_R
-) // Sync
-
-// OP rs, rt
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x18, mult,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // MULTtiply word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x19, multu,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // MULTtiply Unsigned word
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x1C, dmult,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // Doubleword MULTiply
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x1D, dmultu,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .modifiesHI=true,
-    .modifiesLO=true
-) // Doubleword MULTiply Unsigned
-
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x30, tge,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .isTrap=true,
-    .notEmittedByCompilers=true
-) // Trap if Greater or Equal
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x31, tgeu,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .isTrap=true,
-    .notEmittedByCompilers=true
-) // Trap if Greater or Equal Unsigned
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x32, tlt,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .isTrap=true,
-    .notEmittedByCompilers=true
-) // Trap if Less Than
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x33, tltu,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .isTrap=true,
-    .notEmittedByCompilers=true
-) // Trap if Less Than Unsigned
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x34, teq,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .isTrap=true,
-    .notEmittedByCompilers=true
-) // Trap if EQual
-RABBITIZER_DEF_INSTR_ID(
-    cpu, 0x36, tne,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .readsRt=true,
-    .isTrap=true,
-    .notEmittedByCompilers=true
-) // Trap if Not Equal
-
-
-// Pseudo-Instruction Unique IDs
-
-// OP
-RABBITIZER_DEF_INSTR_ID(
-    cpu, -0x01, nop,
-    .operands={0},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .isPseudo=true
-) // No OPeration
-
-// OP rd, rs
-RABBITIZER_DEF_INSTR_ID(
-    cpu, -0x25, move,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .maybeIsMove=true,
-    .isPseudo=true
-) // Move
-RABBITIZER_DEF_INSTR_ID(
-    cpu, -0x27, not,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .isPseudo=true
-) // Not
-
-// OP rd, rt
-RABBITIZER_DEF_INSTR_ID(
-    cpu, -0x23, negu,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true,
-    .isPseudo=true
-)
+    // OP rd, rt, sa
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x00, sll,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Shift word Left Logical
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x02, srl,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Shift word Right Logical
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x03, sra,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Shift word Right Arithmetic
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x38, dsll,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Doubleword Shift Left Logical
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3A, dsrl,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Doubleword Shift Right Logical
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3B, dsra,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Doubleword Shift Right Arithmetic
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3C, dsll32,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Doubleword Shift Left Logical plus 32
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3E, dsrl32,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Doubleword Shift Right Logical plus 32
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x3F, dsra32,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Doubleword Shift Right Arithmetic plus 32
+
+    // OP rd, rt, rs
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x14, dsllv,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Doubleword Shift Left Logical Variable
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x16, dsrlv,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Doubleword Shift Right Logical Variable
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x17, dsrav,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Doubleword Shift Right Arithmetic Variable
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x04, sllv,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Shift word Left Logical Variable
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x06, srlv,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Shift word Right Logical Variable
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x07, srav,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Shift word Right Arithmetic Variable
+
+    // OP rs
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x11, mthi,
+        .operands={RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .modifiesHI=true
+    ) // Move To HI register
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x13, mtlo,
+        .operands={RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .modifiesLO=true
+    ) // Move To LO register
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x08, jr,
+        .operands={RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .isJump=true
+    ) // Jump Register
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x09, jalr,
+        .operands={RAB_OPERAND_cpu_maybe_rd_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .isJump=true,
+        .modifiesRd=true,
+        .readsRs=true,
+        .doesLink=true
+    ) // Jump And Link Register
+
+    // OP rd
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x10, mfhi,
+        .operands={RAB_OPERAND_cpu_rd},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsHI=true
+    ) // Move From HI register
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x12, mflo,
+        .operands={RAB_OPERAND_cpu_rd},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsLO=true
+    ) // Move From LO register
+
+    // OP rd, rs, rt
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0A, movz,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // MOVe conditional on Zero
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0B, movn,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // MOVe conditional on Not zero
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x1A, div,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .readsRd=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // DIVide word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x1B, divu,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .readsRd=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // DIVide Unsigned word
+
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, -0x1A, sn64_div, div,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // DIVide word
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, -0x1B, sn64_divu, divu,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // DIVide Unsigned word
+
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x1E, ddiv,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .readsRd=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // Doubleword DIVide
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x1F, ddivu,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .readsRd=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // Doubleword DIVide Unsigned
+
+    /*
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , ddiv,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    )
+    */
+    /*
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, , ddivu,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    )
+    */
+
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x20, add,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true,
+        .notEmittedByCompilers=true
+    ) // ADD word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x21, addu,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true,
+        .maybeIsMove=true
+    ) // ADD Unsigned word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x22, sub,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .notEmittedByCompilers=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Subtract word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x23, subu,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // SUBtract Unsigned word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x24, and,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // AND
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x25, or,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .maybeIsMove=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // OR
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x26, xor,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // eXclusive OR
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x27, nor,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Not OR
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2A, slt,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Set on Less Than
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2B, sltu,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Set on Less Than Unsigned
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2C, dadd,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Doubleword Add
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2D, daddu,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true,
+        .maybeIsMove=true
+    ) // Doubleword Add Unsigned
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2E, dsub,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Doubleword SUBtract
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x2F, dsubu,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Doubleword SUBtract Unsigned
+
+    // OP code
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0C, syscall,
+        .operands={RAB_OPERAND_cpu_code},
+        .instrType=RABBITIZER_INSTR_TYPE_R
+    ) // SYStem CALL
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0D, break,
+        .operands={RAB_OPERAND_cpu_code},
+        .instrType=RABBITIZER_INSTR_TYPE_R
+    ) // Break
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x0F, sync,
+        .operands={0},
+        .instrType=RABBITIZER_INSTR_TYPE_R
+    ) // Sync
+
+    // OP rs, rt
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x18, mult,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // MULTtiply word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x19, multu,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // MULTtiply Unsigned word
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x1C, dmult,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // Doubleword MULTiply
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x1D, dmultu,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .modifiesHI=true,
+        .modifiesLO=true
+    ) // Doubleword MULTiply Unsigned
+
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x30, tge,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .isTrap=true,
+        .notEmittedByCompilers=true
+    ) // Trap if Greater or Equal
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x31, tgeu,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .isTrap=true,
+        .notEmittedByCompilers=true
+    ) // Trap if Greater or Equal Unsigned
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x32, tlt,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .isTrap=true,
+        .notEmittedByCompilers=true
+    ) // Trap if Less Than
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x33, tltu,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .isTrap=true,
+        .notEmittedByCompilers=true
+    ) // Trap if Less Than Unsigned
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x34, teq,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .isTrap=true,
+        .notEmittedByCompilers=true
+    ) // Trap if EQual
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, 0x36, tne,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .readsRt=true,
+        .isTrap=true,
+        .notEmittedByCompilers=true
+    ) // Trap if Not Equal
+
+
+    // Pseudo-Instruction Unique IDs
+
+    // OP
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, -0x01, nop,
+        .operands={0},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .isPseudo=true
+    ) // No OPeration
+
+    // OP rd, rs
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, -0x25, move,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .maybeIsMove=true,
+        .isPseudo=true
+    ) // Move
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, -0x27, not,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .isPseudo=true
+    ) // Not
+
+    // OP rd, rt
+    RABBITIZER_DEF_INSTR_ID(
+        cpu, -0x23, negu,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true,
+        .isPseudo=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r3000gte/r3000gte_cop2_gte.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r3000gte/r3000gte_cop2_gte.inc`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,114 @@
 /* SPDX-FileCopyrightText: © 2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-/* Indexed by "function" operand */
+    /* Indexed by "function" operand */
 
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x01, RTPS,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x30, RTPT,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x29, DPCL,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x10, DPCS,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x2A, DPCT,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x11, INTPL,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x1E, NCS,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x20, NCT,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x13, NCDS,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x16, NCDT,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x1B, NCCS,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x3F, NCCT,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x14, CDP,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x1C, CC,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x06, NCLIP,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x2D, AVSZ3,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x2E, AVSZ4,
-    .operands={0}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x12, MVMVA,
-    .operands={RAB_OPERAND_r3000gte_sf, RAB_OPERAND_r3000gte_mx, RAB_OPERAND_r3000gte_v, RAB_OPERAND_r3000gte_cv, RAB_OPERAND_r3000gte_lm}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x28, SQR,
-    .operands={RAB_OPERAND_r3000gte_sf}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x0C, OP,
-    .operands={RAB_OPERAND_r3000gte_sf}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x3D, GPF,
-    .operands={RAB_OPERAND_r3000gte_sf}
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r3000gte, 0x3E, GPL,
-    .operands={RAB_OPERAND_r3000gte_sf}
-)
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x01, RTPS,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x30, RTPT,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x29, DPCL,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x10, DPCS,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x2A, DPCT,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x11, INTPL,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x1E, NCS,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x20, NCT,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x13, NCDS,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x16, NCDT,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x1B, NCCS,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x3F, NCCT,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x14, CDP,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x1C, CC,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x06, NCLIP,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x2D, AVSZ3,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x2E, AVSZ4,
+        .operands={0}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x12, MVMVA,
+        .operands={RAB_OPERAND_r3000gte_sf, RAB_OPERAND_r3000gte_mx, RAB_OPERAND_r3000gte_v, RAB_OPERAND_r3000gte_cv, RAB_OPERAND_r3000gte_lm}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x28, SQR,
+        .operands={RAB_OPERAND_r3000gte_sf}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x0C, OP,
+        .operands={RAB_OPERAND_r3000gte_sf}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x3D, GPF,
+        .operands={RAB_OPERAND_r3000gte_sf}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r3000gte, 0x3E, GPL,
+        .operands={RAB_OPERAND_r3000gte_sf}
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
     31--------26-25------21--------------------------------5--------0
     |  = COP0   |   TLB   |                                |  fmt   |
     ------6----------5-----------------------------------------------
     |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
@@ -13,17 +13,17 @@
 100 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
 101 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
 110 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
 111 |  EI   |  DI   |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
  hi |-------|-------|-------|-------|-------|-------|-------|-------|
 */
 
-// The other instructions are implemented using the main CPU table
+    // The other instructions are implemented using the main CPU table
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x38, ei,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x39, di,
-    .operands={0}
-)
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x38, ei,
+        .operands={0}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x39, di,
+        .operands={0}
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_3.inc`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,107 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
-    31--------26-25------21 -------------------------------5--------0
-    |  = COP1   |  = S    |                               | function|
-    ------6----------5-----------------------------------------6-----
-    |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
-000 | ADD.S | SUB.S | MUL.S | DIV.S | SQRT.S| ABS.S | MOV.S | NEG.S |
-001 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  | ---   |
-010 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |RSQRT.S|  ---  |
-011 | ADDA.S| SUBA.S| MULA.S|  ---  | MADD.S| MSUB.S|MADDA.S|MSUBA.S|
-100 |  ---  | ---   |  ---  |  ---  | CVT.W |  ---  |  ---  |  ---  |
-101 | MAX.S | MIN.S |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
-110 | C.F   | ---   | C.EQ  |  ---  | C.LT  |  ---  |  C.LE |  ---  |
-111 | ---   | ---   |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
- hi |-------|-------|-------|-------|-------|-------|-------|-------|
+    31---------26------------------------------------------5--------0
+    |           |                               |function  |  MMI3  |
+    ------6----------------------------------------------------6-----
+    |---00--|---01--|---10--|---11--| lo
+000 |PMADDUW|  ---  |  ---  |PSRAVW |
+001 |  ---  |  ---  |  ---  |  ---  |
+010 |PMTHI  | PMTLO |PINTEH |  ---  |
+011 |PMULTUW| PDIVUW|PCPYUD |  ---  |
+100 |  ---  |  ---  |  POR  | PNOR  |
+101 |  ---  |  ---  |  ---  |  ---  |
+110 |  ---  |  ---  | PEXCH | PCPYH |
+111 |  ---  |  ---  | PEXCW |  ---  |
+ hi |-------|-------|-------|-------|
 */
 
-// The other instructions are implemented using the main CPU table
-
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x04, c1__sqrt_s, c1,
-    .operands={RAB_OPERAND_cpu_copraw}
-)
-
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x16, rsqrt_s, rsqrt.s,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true,
-    .readsFt=true
-) // floating point Reciprocal SQuare RooT
-
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x18, adda_s, adda.s,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .modifiesFs=true,
-    .readsFt=true
-) // floating point ADD to Accumulator
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x19, suba_s, suba.s,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .modifiesFs=true,
-    .readsFt=true
-) // floating point SUBtract to Accumulator
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x1A, mula_s, mula.s,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .modifiesFs=true,
-    .readsFt=true
-) // floating point MULtiply to Accumulator
-
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x1C, madd_s, madd.s,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true,
-    .readsFt=true
-) // floating point Multiply-ADD
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x1D, msub_s, msub.s,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true,
-    .readsFt=true
-) // floating point Multiply abd SUBtract
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x1E, madda_s, madda.s,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-) // floating point Multiply-ADD Accumulator
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x1F, msuba_s, msuba.s,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-) // floating point Multiply SUBtract from Accumulator
-
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x28, max_s, max.s,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true,
-    .readsFt=true
-) // floating point MAXimum
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x29, min_s, min.s,
-    .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .modifiesFd=true,
-    .readsFs=true,
-    .readsFt=true
-) // floating point MINimum
-
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x34, c_lt_s, c.lt.s,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, 0x36, c_le_s, c.le.s,
-    .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft},
-    .isFloat=true,
-    .readsFs=true,
-    .readsFt=true
-)
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x00, pmadduw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Multiply-ADD Unsigned Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x03, psravw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Shift Right Arithmetic Variable Word
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x08, pmthi,
+        .operands={RAB_OPERAND_cpu_rs},
+        .readsRs=true
+    ) // Parallel Move To HI register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x09, pmtlo,
+        .operands={RAB_OPERAND_cpu_rs},
+        .readsRs=true
+    ) // Parallel Move To LO register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0A, pinteh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel INTerleave Even Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0C, pmultuw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel MULTiply Unsigned Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0D, pdivuw,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .readsRs=true,
+        .readsRt=true
+    ) // Prallel DIVide Unsigned Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0E, pcpyud,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel CoPY Upper Doubleword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x12, por,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel OR
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x13, pnor,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Not OR
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1A, pexch,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel EXchange Center Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1B, pcpyh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel CoPY Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1E, pexcw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel EXchange Center Word
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop2.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2.inc`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
     31--------26-25------21 ----------------------------------------0
     |  = COP2   |   fmt   |                                         |
     ------6----------5-----------------------------------------------
     |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
@@ -10,28 +10,28 @@
  01 | *1    |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
  10 | *2    | *2    | *2    | *2    | *2    | *2    | *2    | *2    |
  11 | *2    | *2    | *2    | *2    | *2    | *2    | *2    | *2    |
  hi |-------|-------|-------|-------|-------|-------|-------|-------|
      *1 = BC instructions, see BC2 list   *2 =see special1 table
 */
 
-// TODO: properties
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x01, qmfc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs},
-    .modifiesRt=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x02, cfc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis},
-    .modifiesRt=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x05, qmtc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs},
-    .readsRt=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x06, ctc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis},
-    .readsRt=true
-)
+    // TODO: properties
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x01, qmfc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs},
+        .modifiesRt=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x02, cfc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis},
+        .modifiesRt=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x05, qmtc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs},
+        .readsRt=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x06, ctc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis},
+        .readsRt=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
     31--------26-25------21-20------16------------------------------0
     |  = COP0   |   BC2   |   fmt   |                               |
     ------6----------5----------5------------------------------------
     |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
  00 | BC2F  | BC2T  | BC2FL | BC2TL |  ---  |  ---  |  ---  |  ---  |
  01 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
  10 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
  11 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
  hi |-------|-------|-------|-------|-------|-------|-------|-------|
 */
 
-// TODO: operands and properties
+    // TODO: operands and properties
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x00, bc2f,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .isBranch=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x01, bc2t,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .isBranch=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x02, bc2fl,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .isBranch=true,
-    .isBranchLikely=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x03, bc2tl,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .isBranch=true,
-    .isBranchLikely=true
-)
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x00, bc2f,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .isBranch=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x01, bc2t,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .isBranch=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x02, bc2fl,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .isBranch=true,
+        .isBranchLikely=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x03, bc2tl,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .isBranch=true,
+        .isBranchLikely=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_cop2_special1.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_special2.inc`

 * *Files 19% similar despite different names*

```diff
@@ -1,343 +1,443 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
-    31---------26-25-----21-20-----------------------------5--------0
-    |  =COP2   | Special1 |                                |function|
-    ------6----------5------------------------------------------6----
-    |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
-000 |VADDx  |VADDy  |VADDz  |VADDw  |VSUBx  |VSUBy  |VSUBz  |VSUBw  |
-001 |VMADDx |VMADDy |VMADDz |VMADDw |VMSUBx |VMSUBy |VMSUBz |VMSUBw |
-010 |VMAXx  |VMAXy  |VMAXz  |VMAXw  |VMINIx |VMINIy |VMINIz |VMINIw |
-011 |VMULx  |VMULy  |VMULz  |VMULw  |VMULq  |VMAXi  |VMULi  |VMINIi |
-100 |VADDq  |VMADDq |VADDi  |VMADDi |VSUBq  |VMSUBq |VSUbi  |VMSUBi |
-101 |VADD   |VMADD  |VMUL   |VMAX   |VSUB   |VMSUB  |VOPMSUB|VMINI  |
-110 |VIADD  |VISUB  |VIADDI |  ---  |VIAND  |VIOR   |  ---  |  ---  |
-111 |VCALLMS|VCALLMSR| ---  |  ---  |  *1   |  *1   |  *1   |  *1   |
- hi |-------|-------|-------|-------|-------|-------|-------|-------|
-    *1=see special2 table
+    31---------26-25-----21-20------------------11-10------6-5-2-1--0
+    |  =COP2   | Special2 |                        |  fhi  |1111|flo|
+    ------6----------5-----------------------------------------------
+Note: opcode is flo | (
+    fhi * 4
+).
+     |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
+0000 |VADDAx |VADDAy |VADDAz |VADDAw |VSUBAx |VSUBAy |VSUBAz |VSUBAw |
+0001 |VMADDAx|VMADDAy|VMADDAz|VMADDAw|VMSUBAx|VMSUBAy|VMSUBAz|VMSUBAw|
+0010 |VITOF0 |VITOF4 |VITOF12|VITOF15|VFTOI0 |VFTOI4 |VFTOI12|VFTOI15|
+0011 |VMULAx |VMULAy |VMULAz |VMULAw |VMULAq |VABS   |VMULAi |VCLIPw |
+0100 |VADDAq |VMADDAq|VADDAi |VMADDAi|VSUBAq |VMSUBAq|VSUBAi |VMSUBAi|
+0101 |VADDA  |VMADDA |VMULA  |  ---  |VSUBA  |VMSUBA |VOPMULA|VNOP   |
+0110 |VMOVE  |VMR32  |  ---  |  ---  |VLQI   |VSQI   |VLQD   |VSQD   |
+0111 |VDIV   |VSQRT  |VRSQRT |VWAITQ |VMTIR  |VMFIR  |VILWR  |VISWR  |
+1000 |VRNEXT |VRGET  |VRINIT |VRXOR  |  ---  |  ---  |  ---  |  ---  |
+1001 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
+1010 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
+1011 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
+1100 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
+1101 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
+1110 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
+1111 |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
+ hi  |-------|-------|-------|-------|-------|-------|-------|-------|
 */
 
-// TODO: properties
+    // TODO: operands and properties
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x00, vaddx,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // ADD broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x01, vaddy,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // ADD broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x02, vaddz,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // ADD broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x03, vaddw,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // ADD broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x04, vsubx,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // SUBtract broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x05, vsuby,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // SUBtract broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x06, vsubz,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // SUBtract broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x07, vsubw,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // SUBtract broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x08, vmaddx,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-ADD broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x09, vmaddy,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-ADD broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0A, vmaddz,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-ADD broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0B, vmaddw,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-ADD broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0C, vmsubx,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-SUBtract broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0D, vmsuby,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-SUBtract broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0E, vmsubz,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-SUBtract broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0F, vmsubw,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-SUBtract broadcast
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x10, vmaxx,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MAXimum broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x11, vmaxy,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MAXimum broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x12, vmaxz,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MAXimum broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x13, vmaxw,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MAXimum broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x14, vminix,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MINimum broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x15, vminiy,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MINimum broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x16, vminiz,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MINimum broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x17, vminiw,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MINimum broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x18, vmulx,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MULtiply broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x19, vmuly,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MULtiply broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1A, vmulz,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MULtiply broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1B, vmulw,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MULtiply broadcast
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1C, vmulq,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MULtiply Q
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1D, vmaxi,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MAXimum I
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1E, vmuli,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MULtiply I
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1F, vminii,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MINImum I
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x20, vaddq,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // ADD Q
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x21, vmaddq,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-ADD Q
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x22, vaddi,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // ADD I
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x23, vmaddi,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-ADD I
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x24, vsubq,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // SUBtract Q
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x25, vmsubq,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-SUBtract Q
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x26, vsubi,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // SUBtract I
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x27, vmsubi,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-SUBtract I
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x28, vadd,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // ADD
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x29, vmadd,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-ADD
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x2A, vmul,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MULtiply
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x2B, vmax,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MAXimum
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x2C, vsub,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // SUBtract
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x2D, vmsub,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Multiply-SUBtract
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x2E, vopmsub,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // Outer product post decrement
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x2F, vmini,
-    .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
-    .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
-    .isFloat=true
-) // MINImum
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x30, viadd,
-    .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit}
-) // Integer ADD
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x31, visub,
-    .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit}
-) // Integer SUBtract
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x32, viaddi,
-    .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_immediate5}
-) // Integer ADD Immediate
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x34, viand,
-    .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit}
-) // Integer AND
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x35, vior,
-    .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit}
-) // Integer OR
-
-// TODO: operands and properties
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x38, vcallms,
-    .operands={0}
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x39, vcallmsr,
-    .operands={RAB_OPERAND_r5900_vis}
-)
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x00, vaddax,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Add accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x01, vadday,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Add accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x02, vaddaz,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Add accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x03, vaddaw,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Add accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x04, vsubax,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and substract accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x05, vsubay,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and substract accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x06, vsubaz,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and substract accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x07, vsubaw,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and substract accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x08, vmaddax,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    ) // Multiply and add accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x09, vmadday,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    ) // Multiply and add accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0A, vmaddaz,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    ) // Multiply and add accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0B, vmaddaw,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    ) // Multiply and add accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0C, vmsubax,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and substract accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0D, vmsubay,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and substract accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0E, vmsubaz,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and substract accumulator broadcast
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0F, vmsubaw,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and substract accumulator broadcast
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x10, vitof0,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Integer to floating point
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x11, vitof4,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Integer to floating point
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x12, vitof12,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Integer to floating point
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x13, vitof15,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Integer to floating point
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x14, vftoi0,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Floating to integer
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x15, vftoi4,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Floating to integer
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x16, vftoi12,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Floating to integer
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x17, vftoi15,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Floating to integer
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x18, vmulax,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x19, vmulay,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1A, vmulaz,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1B, vmulaw,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    )
+    // TODO
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1C, vmulaq,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1D, vabs,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Absolute
+
+    // TODO
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1E, vmulai,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1F, vclipw,
+        .operands={RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Clip
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x20, vaddaq,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Add accumulator Q
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x21, vmaddaq,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and add accumulator Q
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x22, vaddai,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Add accumulator I
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x23, vmaddai,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and add accumulator I
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x24, vsubaq,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Subtract accumulator Q
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x25, vmsubaq,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and Subtract accumulator Q
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x26, vsubai,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Subtract accumulator I
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x27, vmsubai,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and Subtract accumulator I
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x28, vadda,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Add accumulator
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x29, vmadda,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and add accumulator
+
+    // TODO
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x2A, vmula,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x2C, vsuba,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x2D, vmsuba,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Multiply and substract accumulator
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x2E, vopmula,
+        .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Outer product pre increment
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x2F, vnop,
+        .operands={0}
+    ) // No operation
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x30, vmove,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Move floating point registers
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x31, vmr32,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Move and rotate per word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x34, vlqi,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vis_postincr},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Load quadraword post increment
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x35, vsqi,
+        .operands={RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vit_postincr},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Store quadraword post increment
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x36, vlqd,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vis_predecr},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Load quadraword pre decrement
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x37, vsqd,
+        .operands={RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vit_predecr},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Store quadraword pre decrement
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x38, vdiv,
+        .operands={RAB_OPERAND_r5900_Q, RAB_OPERAND_r5900_vfsl, RAB_OPERAND_r5900_vftm}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x39, vsqrt,
+        .operands={RAB_OPERAND_r5900_Q, RAB_OPERAND_r5900_vftm}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3A, vrsqrt,
+        .operands={RAB_OPERAND_r5900_Q, RAB_OPERAND_r5900_vfsl,RAB_OPERAND_r5900_vftm}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3B, vwaitq,
+        .operands={0}
+    ) // Wait Q operation
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3C, vmtir,
+        .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vfsl}
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3D, vmfir,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vis},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // Move from integer register
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3E, vilwr,
+        .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vis},
+        .isFloat=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Integer load word register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3F, viswr,
+        .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vis},
+        .isFloat=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Integer store word register
+    /*
+    "vilwr.w",		RAB_OPERAND_r5900_vit,(
+        RAB_OPERAND_r5900_vis
+    )
+    "vilwr.x",		RAB_OPERAND_r5900_vit,(
+        RAB_OPERAND_r5900_vis
+    )
+    "vilwr.y",		RAB_OPERAND_r5900_vit,(
+        RAB_OPERAND_r5900_vis
+    )
+    "vilwr.z",		RAB_OPERAND_r5900_vit,(
+        RAB_OPERAND_r5900_vis
+    )
+    "viswr.w",		RAB_OPERAND_r5900_vit,(
+        RAB_OPERAND_r5900_vis
+    )
+    "viswr.x",		RAB_OPERAND_r5900_vit,(
+        RAB_OPERAND_r5900_vis
+    )
+    "viswr.y",		RAB_OPERAND_r5900_vit,(
+        RAB_OPERAND_r5900_vis
+    )
+    "viswr.z",		RAB_OPERAND_r5900_vit,(
+        RAB_OPERAND_r5900_vis
+    )
+    */
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x40, vrnext,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_R},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // R next
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x41, vrget,
+        .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_R},
+        .instrSuffix=RABINSTRSUFFIX_R5900_xyzw,
+        .isFloat=true
+    ) // R move
+
+    // TODO
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x42, vrinit,
+        .operands={RAB_OPERAND_r5900_R, RAB_OPERAND_r5900_vfsl}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x43, vrxor,
+        .operands={RAB_OPERAND_r5900_R, RAB_OPERAND_r5900_vfsl}
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_mmi.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi.inc`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
     31---------26------------------------------------------5--------0
     | = MMI     |                                         | function|
     ------6----------------------------------------------------6-----
     |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
@@ -15,140 +15,140 @@
 110 | PMFHL | PMTHL |  ---  |  ---  | PSLLH |  ---  | PSRLH | PSRAH |
 111 |  ---  |  ---  |  ---  |  ---  | PSLLW |  ---  | PSRLW | PSRAW |
  hi |-------|-------|-------|-------|-------|-------|-------|-------|
      *1 = MMI0 list                    *2 = MMI2 list
      *3 = MMI1 list                    *4 = MMI3 list
 */
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x00, madd,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Multiply-ADD word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x01, maddu,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Multiply-ADD Unsigned word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x04, plzcw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs},
-    .modifiesRd=true,
-    .readsRs=true
-) // Parallel Leading Zero or one Count Word
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x10, mfhi1,
-    .operands={RAB_OPERAND_cpu_rd},
-    .modifiesRd=true
-) // Move From HI1 register
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x11, mthi1,
-    .operands={RAB_OPERAND_cpu_rs},
-    .readsRs=true
-) // Move To HI1 register
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x12, mflo1,
-    .operands={RAB_OPERAND_cpu_rd},
-    .readsRd=true
-) // Move From LO1 register
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x13, mtlo1,
-    .operands={RAB_OPERAND_cpu_rs},
-    .readsRs=true
-) // Move To LO1 register
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x18, mult1,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // MULTiply word pipeline 1
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x19, multu1,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // MULTiply Unsigned word pipeline 1
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1A, div1,
-    .operands={RAB_OPERAND_cpu_zero, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .readsRs=true,
-    .readsRt=true
-) // DIVide word pipeline 1
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1B, divu1,
-    .operands={RAB_OPERAND_cpu_zero, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .readsRs=true,
-    .readsRt=true
-) // DIVide Unsigned word pipeline 1
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x20, madd1,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Multiply-ADD word pipeline 1
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x21, maddu1,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Multiply-ADD Unsigned word pipeline 1
-
-// TODO: check this two instruction, it is supposed to have an extra .fmt
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x30, pmfhl,
-    .operands={RAB_OPERAND_cpu_rd},
-    .modifiesRd=true
-) // Parallel Move From Hi/Lo register
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x31, pmthl,
-    .operands={RAB_OPERAND_cpu_rs},
-    .readsRs=true
-) // Parallel Move To Hi/Lo register
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x34, psllh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel Shift Left Logical Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x36, psrlh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel Shift Right Logical Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x37, psrah,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel Shift Right Arithmetic Halfword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x3C, psllw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel Shift Left Logical Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x3E, psrlw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel Shift Right Logical Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x3F, psraw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel Shift Right Arithmetic Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x00, madd,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Multiply-ADD word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x01, maddu,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Multiply-ADD Unsigned word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x04, plzcw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs},
+        .modifiesRd=true,
+        .readsRs=true
+    ) // Parallel Leading Zero or one Count Word
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x10, mfhi1,
+        .operands={RAB_OPERAND_cpu_rd},
+        .modifiesRd=true
+    ) // Move From HI1 register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x11, mthi1,
+        .operands={RAB_OPERAND_cpu_rs},
+        .readsRs=true
+    ) // Move To HI1 register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x12, mflo1,
+        .operands={RAB_OPERAND_cpu_rd},
+        .readsRd=true
+    ) // Move From LO1 register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x13, mtlo1,
+        .operands={RAB_OPERAND_cpu_rs},
+        .readsRs=true
+    ) // Move To LO1 register
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x18, mult1,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // MULTiply word pipeline 1
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x19, multu1,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // MULTiply Unsigned word pipeline 1
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1A, div1,
+        .operands={RAB_OPERAND_cpu_zero, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .readsRs=true,
+        .readsRt=true
+    ) // DIVide word pipeline 1
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1B, divu1,
+        .operands={RAB_OPERAND_cpu_zero, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .readsRs=true,
+        .readsRt=true
+    ) // DIVide Unsigned word pipeline 1
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x20, madd1,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Multiply-ADD word pipeline 1
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x21, maddu1,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Multiply-ADD Unsigned word pipeline 1
+
+    // TODO: check this two instruction, it is supposed to have an extra .fmt
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x30, pmfhl,
+        .operands={RAB_OPERAND_cpu_rd},
+        .modifiesRd=true
+    ) // Parallel Move From Hi/Lo register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x31, pmthl,
+        .operands={RAB_OPERAND_cpu_rs},
+        .readsRs=true
+    ) // Parallel Move To Hi/Lo register
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x34, psllh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel Shift Left Logical Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x36, psrlh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel Shift Right Logical Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x37, psrah,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel Shift Right Arithmetic Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3C, psllw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel Shift Left Logical Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3E, psrlw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel Shift Right Logical Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3F, psraw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel Shift Right Arithmetic Word
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_mmi_0.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_1.inc`

 * *Files 20% similar despite different names*

```diff
@@ -1,198 +1,149 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
-    31---------26------------------------------10--------6-5--------0
-    |          |                              |function  |   MMI0   |
+    31---------26------------------------------------------5--------0
+    |           |                               |function  |  MMI1  |
     ------6----------------------------------------------------6-----
     |---00--|---01--|---10--|---11--| lo
-000 |PADDW  | PSUBW | PCGTW | PMAXW |
-001 |PADDH  | PSUBH | PCGTH | PMAXH |
-010 |PADDB  | PSUBB | PCGTB |  ---  |
-011 | ---   | ---   |  ---  |  ---  |
-100 |PADDSW |PSUBSW |PEXTLW | PPACW |
-101 |PADDSH |PSUBSH |PEXTLH | PPACH |
-110 |PADDSB |PSUBSB |PEXTLB | PPACB |
-111 | ---   |  ---  | PEXT5 | PPAC5 |
+000 |  ---  | PABSW | PCEQW | PMINW |
+001 |PADSBH | PABSH | PCEQH | PMINH |
+010 |  ---  |  ---  | PCEQB |  ---  |
+011 |  ---  |  ---  |  ---  |  ---  |
+100 |PADDUW |PSUBUW |PEXTUW |  ---  |
+101 |PADDUH |PSUBUH |PEXTUH |  ---  |
+110 |PADDUB |PSUBUB |PEXTUB | QFSRV |
+111 |  ---  |  ---  |  ---  |  ---  |
  hi |-------|-------|-------|-------|
 */
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x00, paddw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADD Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x01, psubw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel SUBtract Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x02, pcgtw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Compare for Greater Than Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x03, pmaxw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel MAXimum Word
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x04, paddh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADD Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x05, psubh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel SUBtract Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x06, pcgth,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Compare for Greater Than Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x07, pmaxh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel MAXimum Halfword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x08, paddb,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADD Byte
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x09, psubb,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel SUBtract Byte
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0A, pcgtb,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Compare for Greater Than Byte
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x10, paddsw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADD with Signed saturation Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x11, psubsw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel SUBtract with Signed saturation Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x12, pextlw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel EXTend Lower from Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x13, ppacw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel PACk to Word
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x14, paddsh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADD with Signed saturation Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x15, psubsh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel SUBtract with Signed saturation Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x16, pextlh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel EXTend Lower from Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x17, ppach,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel PACk to Halfword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x18, paddsb,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADD with Signed saturation Bytes
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x19, psubsb,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel SUBtract with Signed saturation Bytes
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1A, pextlb,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel EXTend Lower from Bytes
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1B, ppacb,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel PACk to Bytes
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1E, pext5,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel EXTend from 5-bits
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1F, ppac5,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel PACk to 5-bits
+    // TODO: operands and properties
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x01, pabsw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel ABSolute Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x02, pceqw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Compare for EQual Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x03, pminw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel MINimum Word
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x04, padsbh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADd/SuBtract Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x05, pabsh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel ABSolute Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x06, pceqh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Compare for EQual Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x07, pminh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel MINimum Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0A, pceqb,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Compare for EQual Byte
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x10, padduw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADD Unsigned saturation Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x11, psubuw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel SUBtract Unsigned saturation Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x12, pextuw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel EXTend Upper from Word
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x14, padduh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADD Unsigned saturation Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x15, psubuh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel SUBtract Unsigned saturation Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x16, pextuh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel EXTend Upper from Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x18, paddub,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADD Unsigned saturation Byte
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x19, psubub,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel SUBtract Unsigned saturation Byte
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1A, pextub,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel EXTend Upper from Byte
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1B, qfsrv,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Quadword Funnel Shift Right Variable
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_mmi_1.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_2.inc`

 * *Files 20% similar despite different names*

```diff
@@ -1,149 +1,170 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
     31---------26------------------------------------------5--------0
-    |           |                               |function  |  MMI1  |
+    |           |                              |function   |  MMI2  |
     ------6----------------------------------------------------6-----
     |---00--|---01--|---10--|---11--| lo
-000 |  ---  | PABSW | PCEQW | PMINW |
-001 |PADSBH | PABSH | PCEQH | PMINH |
-010 |  ---  |  ---  | PCEQB |  ---  |
-011 |  ---  |  ---  |  ---  |  ---  |
-100 |PADDUW |PSUBUW |PEXTUW |  ---  |
-101 |PADDUH |PSUBUH |PEXTUH |  ---  |
-110 |PADDUB |PSUBUB |PEXTUB | QFSRV |
-111 |  ---  |  ---  |  ---  |  ---  |
+000 |PMADDW |  ---  |PSLLVW |PSRLVW |
+001 |PMSUBW |  ---  |  ---  |  ---  |
+010 |PMFHI  |PMFLO  |PINTH  |  ---  |
+011 |PMULTW |PDIVW  |PCPYLD |  ---  |
+100 |PMADDH |PHMADH | PAND  |  PXOR |
+101 |PMSUBH |PHMSBH |  ---  |  ---  |
+110 | ---   |  ---  | PEXEH | PREVH |
+111 |PMULTH |PDIVBW | PEXEW |PROT3W |
  hi |-------|-------|-------|-------|
 */
 
-// TODO: operands and properties
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x01, pabsw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel ABSolute Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x02, pceqw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Compare for EQual Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x03, pminw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel MINimum Word
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x04, padsbh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADd/SuBtract Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x05, pabsh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel ABSolute Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x06, pceqh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Compare for EQual Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x07, pminh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel MINimum Halfword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0A, pceqb,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Compare for EQual Byte
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x10, padduw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADD Unsigned saturation Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x11, psubuw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel SUBtract Unsigned saturation Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x12, pextuw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel EXTend Upper from Word
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x14, padduh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADD Unsigned saturation Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x15, psubuh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel SUBtract Unsigned saturation Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x16, pextuh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel EXTend Upper from Halfword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x18, paddub,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel ADD Unsigned saturation Byte
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x19, psubub,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel SUBtract Unsigned saturation Byte
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1A, pextub,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel EXTend Upper from Byte
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1B, qfsrv,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Quadword Funnel Shift Right Variable
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x00, pmaddw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Multiply-ADD Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x02, psllvw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Shift Left Logical Variable Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x03, psrlvw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Shift Right Logical Variable Word
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x04, pmsubw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Multiply-SUBtract Word
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x08, pmfhi,
+        .operands={RAB_OPERAND_cpu_rd},
+        .modifiesRd=true
+    ) // Parallel Move From HI register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x09, pmflo,
+        .operands={RAB_OPERAND_cpu_rd},
+        .modifiesRd=true
+    ) // Parallel Move From LO register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0A, pinth,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel INTerleave Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0C, pmultw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel MULTiply Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0D, pdivw,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel DIVide Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0E, pcpyld,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel CoPY Lower Doubleword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x10, pmaddh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Multiply-ADD Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x11, phmadh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Horizontal Multiply-ADd Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x12, pand,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel AND
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x13, pxor,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel eXclusive OR
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x14, pmsubh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Multiply-SUBtract Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x15, phmsbh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Horizontal Multiply-Subtract Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1A, pexeh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel EXchange Even Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1B, prevh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel REVerse Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1C, pmulth,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Multiply Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1D, pdivbw,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel DIVide Broadcast Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1E, pexew,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel EXchange Even Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1F, prot3w,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel ROTate 3 Words left
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_mmi_2.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_0.inc`

 * *Files 18% similar despite different names*

```diff
@@ -1,170 +1,198 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
-    31---------26------------------------------------------5--------0
-    |           |                              |function   |  MMI2  |
+    31---------26------------------------------10--------6-5--------0
+    |          |                              |function  |   MMI0   |
     ------6----------------------------------------------------6-----
     |---00--|---01--|---10--|---11--| lo
-000 |PMADDW |  ---  |PSLLVW |PSRLVW |
-001 |PMSUBW |  ---  |  ---  |  ---  |
-010 |PMFHI  |PMFLO  |PINTH  |  ---  |
-011 |PMULTW |PDIVW  |PCPYLD |  ---  |
-100 |PMADDH |PHMADH | PAND  |  PXOR |
-101 |PMSUBH |PHMSBH |  ---  |  ---  |
-110 | ---   |  ---  | PEXEH | PREVH |
-111 |PMULTH |PDIVBW | PEXEW |PROT3W |
+000 |PADDW  | PSUBW | PCGTW | PMAXW |
+001 |PADDH  | PSUBH | PCGTH | PMAXH |
+010 |PADDB  | PSUBB | PCGTB |  ---  |
+011 | ---   | ---   |  ---  |  ---  |
+100 |PADDSW |PSUBSW |PEXTLW | PPACW |
+101 |PADDSH |PSUBSH |PEXTLH | PPACH |
+110 |PADDSB |PSUBSB |PEXTLB | PPACB |
+111 | ---   |  ---  | PEXT5 | PPAC5 |
  hi |-------|-------|-------|-------|
 */
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x00, pmaddw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Multiply-ADD Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x02, psllvw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Shift Left Logical Variable Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x03, psrlvw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Shift Right Logical Variable Word
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x04, pmsubw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Multiply-SUBtract Word
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x08, pmfhi,
-    .operands={RAB_OPERAND_cpu_rd},
-    .modifiesRd=true
-) // Parallel Move From HI register
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x09, pmflo,
-    .operands={RAB_OPERAND_cpu_rd},
-    .modifiesRd=true
-) // Parallel Move From LO register
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0A, pinth,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel INTerleave Halfword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0C, pmultw,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel MULTiply Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0D, pdivw,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .readsRs=true,
-    .readsRt=true
-) // Parallel DIVide Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x0E, pcpyld,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel CoPY Lower Doubleword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x10, pmaddh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Multiply-ADD Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x11, phmadh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Horizontal Multiply-ADd Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x12, pand,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel AND
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x13, pxor,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel eXclusive OR
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x14, pmsubh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Multiply-SUBtract Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x15, phmsbh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Horizontal Multiply-Subtract Halfword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1A, pexeh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel EXchange Even Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1B, prevh,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel REVerse Halfword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1C, pmulth,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Parallel Multiply Halfword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1D, pdivbw,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .readsRs=true,
-    .readsRt=true
-) // Parallel DIVide Broadcast Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1E, pexew,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel EXchange Even Word
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1F, prot3w,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
-    .modifiesRd=true,
-    .readsRt=true
-) // Parallel ROTate 3 Words left
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x00, paddw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADD Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x01, psubw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel SUBtract Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x02, pcgtw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Compare for Greater Than Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x03, pmaxw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel MAXimum Word
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x04, paddh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADD Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x05, psubh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel SUBtract Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x06, pcgth,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Compare for Greater Than Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x07, pmaxh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel MAXimum Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x08, paddb,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADD Byte
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x09, psubb,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel SUBtract Byte
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x0A, pcgtb,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel Compare for Greater Than Byte
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x10, paddsw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADD with Signed saturation Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x11, psubsw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel SUBtract with Signed saturation Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x12, pextlw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel EXTend Lower from Word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x13, ppacw,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel PACk to Word
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x14, paddsh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADD with Signed saturation Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x15, psubsh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel SUBtract with Signed saturation Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x16, pextlh,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel EXTend Lower from Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x17, ppach,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel PACk to Halfword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x18, paddsb,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel ADD with Signed saturation Bytes
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x19, psubsb,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel SUBtract with Signed saturation Bytes
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1A, pextlb,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel EXTend Lower from Bytes
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1B, ppacb,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Parallel PACk to Bytes
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1E, pext5,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel EXTend from 5-bits
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1F, ppac5,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt},
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Parallel PACk to 5-bits
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_normal.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_normal.inc`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
     31---------26---------------------------------------------------0
     |  opcode   |                                                   |
     ------6----------------------------------------------------------
     |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
@@ -16,48 +16,48 @@
 111 | ---   | SWC1  | ---   | ---   | ---   | ---   | SQC2  | SD    |
  hi |-------|-------|-------|-------|-------|-------|-------|-------|
      *1 = SPECIAL, see SPECIAL list    *2 = REGIMM, see REGIMM list
      *3 = COP0                         *4 = COP1
      *5 = COP2                         *6 = MMI table
 */
 
-// The other instructions are implemented using the main CPU table
+    // The other instructions are implemented using the main CPU table
 
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1E, lq,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-) // Load Quadword
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x1F, sq,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-) // Store Quadword
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x36, lqc2,
-    .operands={RAB_OPERAND_r5900_vft, RAB_OPERAND_cpu_immediate_base},
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true
-)
-
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x3E, sqc2,
-    .operands={RAB_OPERAND_r5900_vft, RAB_OPERAND_cpu_immediate_base},
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true
-)
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1E, lq,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    ) // Load Quadword
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x1F, sq,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    ) // Store Quadword
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x36, lqc2,
+        .operands={RAB_OPERAND_r5900_vft, RAB_OPERAND_cpu_immediate_base},
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x3E, sqc2,
+        .operands={RAB_OPERAND_r5900_vft, RAB_OPERAND_cpu_immediate_base},
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_regimm.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_regimm.inc`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
     31---------26----------20-------16------------------------------0
     | = REGIMM  |          |   rt    |                              |
     ------6---------------------5------------------------------------
     |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
  00 | BLTZ  | BGEZ  | BLTZL | BGEZL |  ---  |  ---  |  ---  |  ---  |
  01 | TGEI  | TGEIU | TLTI  | TLTIU | TEQI  |  ---  | TNEI  |  ---  |
  10 | BLTZAL| BGEZAL|BLTZALL|BGEZALL|  ---  |  ---  |  ---  |  ---  |
  11 | MTSAB | MTSAH |  ---  |  ---  |  ---  |  ---  |  ---  |  ---  |
  hi |-------|-------|-------|-------|-------|-------|-------|-------|
 */
 
-// The other instructions are implemented using the main CPU table
+    // The other instructions are implemented using the main CPU table
 
-// OP rs, IMM
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x18, mtsab,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x19, mtsah,
-    .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true
-)
+    // OP rs, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x18, mtsab,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x19, mtsah,
+        .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/r5900/r5900_special.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_special.inc`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /*
     31---------26------------------------------------------5--------0
     | = SPECIAL |                                         | function|
     ------6----------------------------------------------------6-----
     |--000--|--001--|--010--|--011--|--100--|--101--|--110--|--111--| lo
@@ -13,34 +13,34 @@
 100 | ADD   | ADDU  | SUB   | SUBU  | AND   | OR    | XOR   | NOR   |
 101 | MFSA  | MTSA  | SLT   | SLTU  | DADD  | DADDU | DSUB  | DSUBU |
 110 | TGE   | TGEU  | TLT   | TLTU  | TEQ   |  ---  | TNE   |  ---  |
 111 | DSLL  |  ---  | DSRL  | DSRA  |DSLL32 |  ---  |DSRL32 |DSRA32 |
  hi |-------|-------|-------|-------|-------|-------|-------|-------|
 */
 
-// The other instructions are implemented using the main CPU table
+    // The other instructions are implemented using the main CPU table
 
-RABBITIZER_DEF_INSTR_ID_ALTNAME(
-    r5900, -0x0F, sync_p, sync.p,
-    .operands={0},
-    .instrType=RABBITIZER_INSTR_TYPE_R
-) // Sync
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        r5900, -0x0F, sync_p, sync.p,
+        .operands={0},
+        .instrType=RABBITIZER_INSTR_TYPE_R
+    ) // Sync
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x18, mult,
-    .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // MULTtiply word
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x18, mult,
+        .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // MULTtiply word
 
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x28, mfsa,
-    .operands={RAB_OPERAND_cpu_rd},
-    .modifiesRd=true
-) // Move From Shift Amount register
-RABBITIZER_DEF_INSTR_ID(
-    r5900, 0x29, mtsa,
-    .operands={RAB_OPERAND_cpu_rs},
-    .readsRs=true
-) // Move To Shift Amount register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x28, mfsa,
+        .operands={RAB_OPERAND_cpu_rd},
+        .modifiesRd=true
+    ) // Move From Shift Amount register
+    RABBITIZER_DEF_INSTR_ID(
+        r5900, 0x29, mtsa,
+        .operands={RAB_OPERAND_cpu_rs},
+        .readsRs=true
+    ) // Move To Shift Amount register
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_cop0.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP rt, cop0d
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x00, mfc0,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_cop0d},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .modifiesRt=true,
-    .notEmittedByCompilers=true
-) // Move word From CP0
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x04, mtc0,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_cop0d},
-    .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
-    .readsRt=true,
-    .notEmittedByCompilers=true
-) // Move word to CP0
+    // OP fd, fs
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x20, cvt_s_l, cvt.s.l,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .modifiesFd=true,
+        .readsFs=true
+    )
+    RABBITIZER_DEF_INSTR_ID_ALTNAME(
+        cpu, 0x21, cvt_d_l, cvt.d.l,
+        .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs},
+        .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN,
+        .isFloat=true,
+        .isDouble=true,
+        .modifiesFd=true,
+        .readsFs=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_cop2.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop2.inc`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP cop2t, vd[index]
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x00, mfc2,
-    .operands={RAB_OPERAND_rsp_cop2t, RAB_OPERAND_rsp_vs_index}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x04, mtc2,
-    .operands={RAB_OPERAND_rsp_cop2t, RAB_OPERAND_rsp_vs_index}
-)
+    // OP cop2t, vd[index]
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x00, mfc2,
+        .operands={RAB_OPERAND_rsp_cop2t, RAB_OPERAND_rsp_vs_index}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x04, mtc2,
+        .operands={RAB_OPERAND_rsp_cop2t, RAB_OPERAND_rsp_vs_index}
+    )
 
-// OP rt, cop2cd
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x02, cfc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_rsp_cop2cd},
-    .modifiesRt=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x06, ctc2,
-    .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_rsp_cop2cd},
-    .readsRt=true
-)
+    // OP rt, cop2cd
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x02, cfc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_rsp_cop2cd},
+        .modifiesRt=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x06, ctc2,
+        .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_rsp_cop2cd},
+        .readsRt=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_cop2_vu.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop2_vu.inc`

 * *Files 7% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP vd, vs, vt[elementhigh]
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x00, vmulf,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x01, vmulu,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x02, vrndp,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x03, vmulq,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x04, vmudl,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x05, vmudm,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x06, vmudn,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x07, vmudh,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x08, vmacf,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x09, vmacu,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0A, vrndn,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0B, vmacq,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0C, vmadl,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0D, vmadm,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0E, vmadn,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0F, vmadh,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x10, vadd,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x11, vsub,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x13, vabs,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x14, vaddc,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x15, vsubc,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x1D, vsar,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x28, vand,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x29, vnand,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x2A, vor,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x2B, vnor,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x2C, vxor,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x2D, vnxor,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
+    // OP vd, vs, vt[elementhigh]
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x00, vmulf,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x01, vmulu,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x02, vrndp,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x03, vmulq,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x04, vmudl,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x05, vmudm,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x06, vmudn,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x07, vmudh,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x08, vmacf,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x09, vmacu,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0A, vrndn,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0B, vmacq,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0C, vmadl,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0D, vmadm,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0E, vmadn,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0F, vmadh,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x10, vadd,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x11, vsub,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x13, vabs,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x14, vaddc,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x15, vsubc,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x1D, vsar,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x28, vand,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x29, vnand,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x2A, vor,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x2B, vnor,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x2C, vxor,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x2D, vnxor,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
 
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x20, vlt,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x21, veq,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x22, vne,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x23, vge,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x24, vcl,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x25, vch,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x26, vcr,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x27, vmrg,
-    .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
-)
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x20, vlt,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x21, veq,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x22, vne,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x23, vge,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x24, vcl,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x25, vch,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x26, vcr,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x27, vmrg,
+        .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh}
+    )
 
-// OP vd[de], vt[elementhigh]
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x30, vrcp,
-    .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x31, vrcpl,
-    .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
-) // operands may be wrong
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x32, vrcph,
-    .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x33, vmov,
-    .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x34, vrsq,
-    .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x35, vrsql,
-    .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x36, vrsqh,
-    .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
-)
+    // OP vd[de], vt[elementhigh]
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x30, vrcp,
+        .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x31, vrcpl,
+        .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
+    ) // operands may be wrong
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x32, vrcph,
+        .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x33, vmov,
+        .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x34, vrsq,
+        .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x35, vrsql,
+        .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x36, vrsqh,
+        .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh}
+    )
 
-// OP
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x37, vnop,
-    .operands={0}
-)
+    // OP
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x37, vnop,
+        .operands={0}
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_normal.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal.inc`

 * *Files 6% similar despite different names*

```diff
@@ -1,247 +1,247 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP LABEL
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x02, j,
-    .operands={RAB_OPERAND_cpu_label},
-    .instrType=RABBITIZER_INSTR_TYPE_J,
-    .isJump=true,
-    .isJumpWithAddress=true
-) // Jump
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x03, jal,
-    .operands={RAB_OPERAND_cpu_label},
-    .instrType=RABBITIZER_INSTR_TYPE_J,
-    .isJump=true,
-    .isJumpWithAddress=true,
-    .doesLink=true
-) // Jump And Link
-
-// OP rs, rt, IMM
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x04, beq,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .readsRt=true,
-    .isBranch=true
-) // Branch on EQual
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x05, bne,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .readsRt=true,
-    .isBranch=true
-) // Branch on Not Equal
-
-// OP rs, IMM
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x06, blez,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .isBranch=true
-) // Branch on Less than or Equal to Zero
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x07, bgtz,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .isBranch=true
-) // Branch on Greater Than Zero
-
-// OP rt, rs, IMM
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x08, addi,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .notEmittedByCompilers=true,
-    .canBeLo=true
-) // Add Immediate
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x09, addiu,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true
-) // Add Immediate Unsigned Word
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0A, slti,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true
-) // Set on Less Than Immediate
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0B, sltiu,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true
-) // Set on Less Than Immediate Unsigned
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0C, andi,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isUnsigned=true,
-    .modifiesRt=true,
-    .readsRs=true
-) // And Immediate
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0D, ori,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isUnsigned=true,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true
-) // Or Immediate
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0E, xori,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isUnsigned=true,
-    .modifiesRt=true,
-    .readsRs=true
-) // eXclusive OR Immediate
-
-// OP rt, IMM
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0F, lui,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_immediate},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .isUnsigned=true,
-    .modifiesRt=true,
-    .canBeHi=true
-) // Load Upper Immediate
-
-// OP rt, IMM(base)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x20, lb,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_BYTE
-) // Load Byte
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x21, lh,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_SHORT
-) // Load Halfword
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x23, lw,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_WORD
-) // Load Word
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x24, lbu,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_BYTE,
-    .doesUnsignedMemoryAccess=true
-) // Load Byte Insigned
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x25, lhu,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .modifiesRt=true,
-    .readsRs=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesLoad=true,
-    .accessType=RAB_ACCESSTYPE_SHORT,
-    .doesUnsignedMemoryAccess=true
-) // Load Halfword Unsigned
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x28, sb,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true,
-    .accessType=RAB_ACCESSTYPE_BYTE
-) // Store Byte
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x29, sh,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true,
-    .accessType=RAB_ACCESSTYPE_SHORT
-) // Store Halfword
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x2B, sw,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true,
-    .canBeLo=true,
-    .doesDereference=true,
-    .doesStore=true,
-    .accessType=RAB_ACCESSTYPE_WORD
-) // Store Word
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x33, pref,
-    .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
-    .instrType=RABBITIZER_INSTR_TYPE_I,
-    .readsRs=true,
-    .readsRt=true
-) // Prefetch
-
-
-// Pseudo-Instruction Unique IDs
-
-// OP IMM
-RABBITIZER_DEF_INSTR_ID(
-    rsp, -0x03, b,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true
-) // Branch (unconditional)
-
-// OP rs, IMM
-RABBITIZER_DEF_INSTR_ID(
-    rsp, -0x04, beqz,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .isBranch=true
-) // Branch on EQual Zero
-RABBITIZER_DEF_INSTR_ID(
-    rsp, -0x05, bnez,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .isBranch=true
-) // Branch on Not Equal Zero
+    // OP LABEL
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x02, j,
+        .operands={RAB_OPERAND_cpu_label},
+        .instrType=RABBITIZER_INSTR_TYPE_J,
+        .isJump=true,
+        .isJumpWithAddress=true
+    ) // Jump
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x03, jal,
+        .operands={RAB_OPERAND_cpu_label},
+        .instrType=RABBITIZER_INSTR_TYPE_J,
+        .isJump=true,
+        .isJumpWithAddress=true,
+        .doesLink=true
+    ) // Jump And Link
+
+    // OP rs, rt, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x04, beq,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .readsRt=true,
+        .isBranch=true
+    ) // Branch on EQual
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x05, bne,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .readsRt=true,
+        .isBranch=true
+    ) // Branch on Not Equal
+
+    // OP rs, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x06, blez,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .isBranch=true
+    ) // Branch on Less than or Equal to Zero
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x07, bgtz,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .isBranch=true
+    ) // Branch on Greater Than Zero
+
+    // OP rt, rs, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x08, addi,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .notEmittedByCompilers=true,
+        .canBeLo=true
+    ) // Add Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x09, addiu,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true
+    ) // Add Immediate Unsigned Word
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0A, slti,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true
+    ) // Set on Less Than Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0B, sltiu,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true
+    ) // Set on Less Than Immediate Unsigned
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0C, andi,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isUnsigned=true,
+        .modifiesRt=true,
+        .readsRs=true
+    ) // And Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0D, ori,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isUnsigned=true,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true
+    ) // Or Immediate
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0E, xori,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isUnsigned=true,
+        .modifiesRt=true,
+        .readsRs=true
+    ) // eXclusive OR Immediate
+
+    // OP rt, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0F, lui,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_immediate},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .isUnsigned=true,
+        .modifiesRt=true,
+        .canBeHi=true
+    ) // Load Upper Immediate
+
+    // OP rt, IMM(base)
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x20, lb,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_BYTE
+    ) // Load Byte
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x21, lh,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_SHORT
+    ) // Load Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x23, lw,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_WORD
+    ) // Load Word
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x24, lbu,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_BYTE,
+        .doesUnsignedMemoryAccess=true
+    ) // Load Byte Insigned
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x25, lhu,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .modifiesRt=true,
+        .readsRs=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesLoad=true,
+        .accessType=RAB_ACCESSTYPE_SHORT,
+        .doesUnsignedMemoryAccess=true
+    ) // Load Halfword Unsigned
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x28, sb,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true,
+        .accessType=RAB_ACCESSTYPE_BYTE
+    ) // Store Byte
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x29, sh,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true,
+        .accessType=RAB_ACCESSTYPE_SHORT
+    ) // Store Halfword
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x2B, sw,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true,
+        .canBeLo=true,
+        .doesDereference=true,
+        .doesStore=true,
+        .accessType=RAB_ACCESSTYPE_WORD
+    ) // Store Word
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x33, pref,
+        .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base},
+        .instrType=RABBITIZER_INSTR_TYPE_I,
+        .readsRs=true,
+        .readsRt=true
+    ) // Prefetch
+
+
+    // Pseudo-Instruction Unique IDs
+
+    // OP IMM
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, -0x03, b,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true
+    ) // Branch (unconditional)
+
+    // OP rs, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, -0x04, beqz,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .isBranch=true
+    ) // Branch on EQual Zero
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, -0x05, bnez,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .isBranch=true
+    ) // Branch on Not Equal Zero
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal_swc2.inc`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP vt[elementlow], offset(vs)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x00, lbv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x01, lsv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x02, llv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x03, ldv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x04, lqv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x05, lrv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x06, lpv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x07, luv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x08, lhv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x09, lfv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0B, ltv,
-    .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
-    .readsRs=true
-)
+    // OP vt[elementlow], offset(vs)
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x00, sbv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x01, ssv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x02, slv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x03, sdv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x04, sqv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x05, srv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x06, spv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x07, suv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x08, shv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x09, sfv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0B, stv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
+
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, -0x07, swv,
+        .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs},
+        .readsRs=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_regimm.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_regimm.inc`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP rs, IMM
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x00, bltz,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .isBranch=true
-) // Branch on Less Than Zero
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x01, bgez,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .isBranch=true
-) // Branch on Greater than or Equal to Zero
+    // OP rs, IMM
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x00, bltz,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .isBranch=true
+    ) // Branch on Less Than Zero
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x01, bgez,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .isBranch=true
+    ) // Branch on Greater than or Equal to Zero
 
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x10, bltzal,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .isBranch=true,
-    .doesLink=true
-) // Branch on Less Than Zero and Link
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x11, bgezal,
-    .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .readsRs=true,
-    .isBranch=true,
-    .notEmittedByCompilers=true,
-    .doesLink=true
-) // Branch on Greater Than or Equal to Zero and Link
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x10, bltzal,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .isBranch=true,
+        .doesLink=true
+    ) // Branch on Less Than Zero and Link
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x11, bgezal,
+        .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .readsRs=true,
+        .isBranch=true,
+        .notEmittedByCompilers=true,
+        .doesLink=true
+    ) // Branch on Greater Than or Equal to Zero and Link
 
 
-// Pseudo-Instruction Unique IDs
+    // Pseudo-Instruction Unique IDs
 
-RABBITIZER_DEF_INSTR_ID(
-    rsp, -0x11, bal,
-    .operands={RAB_OPERAND_cpu_branch_target_label},
-    .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
-    .isBranch=true,
-    .notEmittedByCompilers=true,
-    .doesLink=true,
-    .isPseudo=true
-) // Branch and Link
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, -0x11, bal,
+        .operands={RAB_OPERAND_cpu_branch_target_label},
+        .instrType=RABBITIZER_INSTR_TYPE_REGIMM,
+        .isBranch=true,
+        .notEmittedByCompilers=true,
+        .doesLink=true,
+        .isPseudo=true
+    ) // Branch and Link
```

### Comparing `rabbitizer-1.7.0/include/instructions/instr_id/rsp/rsp_special.inc` & `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_special.inc`

 * *Files 17% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-// OP rd, rt, sa
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x00, sll,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Shift word Left Logical
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x02, srl,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Shift word Right Logical
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x03, sra,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true
-) // Shift word Right Arithmetic
-
-// OP rd, rt, rs
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x04, sllv,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Shift word Left Logical Variable
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x06, srlv,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Shift word Right Logical Variable
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x07, srav,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Shift word Right Arithmetic Variable
-
-// OP rs
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x08, jr,
-    .operands={RAB_OPERAND_rsp_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .readsRs=true,
-    .isJump=true
-) // Jump Register
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x09, jalr,
-    .operands={RAB_OPERAND_rsp_maybe_rd_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .isJump=true,
-    .modifiesRd=true,
-    .readsRs=true,
-    .doesLink=true
-) // Jump And Link Register
-
-// OP rd, rs, rt
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0A, movz,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // MOVe conditional on Zero
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0B, movn,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // MOVe conditional on Not zero
-
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x20, add,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true,
-    .notEmittedByCompilers=true
-) // ADD word
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x21, addu,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // ADD Unsigned word
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x22, sub,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .notEmittedByCompilers=true,
-    .readsRs=true,
-    .readsRt=true
-) // Subtract word
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x23, subu,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // SUBtract Unsigned word
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x24, and,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // AND
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x25, or,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // OR
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x26, xor,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // eXclusive OR
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x27, nor,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Not OR
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x2A, slt,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Set on Less Than
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x2B, sltu,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .readsRt=true
-) // Set on Less Than Unsigned
-
-// OP code
-RABBITIZER_DEF_INSTR_ID(
-    rsp, 0x0D, break,
-    .operands={RAB_OPERAND_cpu_code},
-    .instrType=RABBITIZER_INSTR_TYPE_R
-) // Break
-
-
-// Pseudo-Instruction Unique IDs
-// OP
-RABBITIZER_DEF_INSTR_ID(
-    rsp, -0x01, nop,
-    .operands={0},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .isPseudo=true
-) // No OPeration
-
-// OP rd, rs
-RABBITIZER_DEF_INSTR_ID(
-    rsp, -0x25, move,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .isPseudo=true
-) // Move
-RABBITIZER_DEF_INSTR_ID(
-    rsp, -0x27, not,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRs=true,
-    .isPseudo=true
-) // Not
-
-// OP rd, rt
-RABBITIZER_DEF_INSTR_ID(
-    rsp, -0x23, negu,
-    .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt},
-    .instrType=RABBITIZER_INSTR_TYPE_R,
-    .modifiesRd=true,
-    .readsRt=true,
-    .isPseudo=true
-)
+    // OP rd, rt, sa
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x00, sll,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Shift word Left Logical
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x02, srl,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Shift word Right Logical
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x03, sra,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true
+    ) // Shift word Right Arithmetic
+
+    // OP rd, rt, rs
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x04, sllv,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Shift word Left Logical Variable
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x06, srlv,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Shift word Right Logical Variable
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x07, srav,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Shift word Right Arithmetic Variable
+
+    // OP rs
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x08, jr,
+        .operands={RAB_OPERAND_rsp_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .readsRs=true,
+        .isJump=true
+    ) // Jump Register
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x09, jalr,
+        .operands={RAB_OPERAND_rsp_maybe_rd_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .isJump=true,
+        .modifiesRd=true,
+        .readsRs=true,
+        .doesLink=true
+    ) // Jump And Link Register
+
+    // OP rd, rs, rt
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0A, movz,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // MOVe conditional on Zero
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0B, movn,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // MOVe conditional on Not zero
+
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x20, add,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true,
+        .notEmittedByCompilers=true
+    ) // ADD word
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x21, addu,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // ADD Unsigned word
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x22, sub,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .notEmittedByCompilers=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Subtract word
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x23, subu,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // SUBtract Unsigned word
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x24, and,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // AND
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x25, or,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // OR
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x26, xor,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // eXclusive OR
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x27, nor,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Not OR
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x2A, slt,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Set on Less Than
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x2B, sltu,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .readsRt=true
+    ) // Set on Less Than Unsigned
+
+    // OP code
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, 0x0D, break,
+        .operands={RAB_OPERAND_cpu_code},
+        .instrType=RABBITIZER_INSTR_TYPE_R
+    ) // Break
+
+
+    // Pseudo-Instruction Unique IDs
+    // OP
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, -0x01, nop,
+        .operands={0},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .isPseudo=true
+    ) // No OPeration
+
+    // OP rd, rs
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, -0x25, move,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .isPseudo=true
+    ) // Move
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, -0x27, not,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRs=true,
+        .isPseudo=true
+    ) // Not
+
+    // OP rd, rt
+    RABBITIZER_DEF_INSTR_ID(
+        rsp, -0x23, negu,
+        .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt},
+        .instrType=RABBITIZER_INSTR_TYPE_R,
+        .modifiesRd=true,
+        .readsRt=true,
+        .isPseudo=true
+    )
```

### Comparing `rabbitizer-1.7.0/include/instructions/operands/RabbitizerOperandType_cpu.inc` & `rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_cpu.inc`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-RAB_DEF_OPERAND(cpu, rs)
-RAB_DEF_OPERAND(cpu, rt)
-RAB_DEF_OPERAND(cpu, rd)
-RAB_DEF_OPERAND(cpu, sa)
-RAB_DEF_OPERAND(cpu, zero) // $zero
-// RAB_DEF_OPERAND(cpu, function)
-RAB_DEF_OPERAND(cpu, cop0d)
-RAB_DEF_OPERAND(cpu, fs)
-RAB_DEF_OPERAND(cpu, ft)
-RAB_DEF_OPERAND(cpu, fd)
-RAB_DEF_OPERAND(cpu, cop1cs) // Coprocessor 1 control fs
-RAB_DEF_OPERAND(cpu, cop2t)
-RAB_DEF_OPERAND(cpu, cop2cd) // Coprocessor 2 control rd
-RAB_DEF_OPERAND(cpu, op)
-RAB_DEF_OPERAND(cpu, code)
-RAB_DEF_OPERAND(cpu, code_lower)
-RAB_DEF_OPERAND(cpu, copraw)
-RAB_DEF_OPERAND(cpu, label)
-RAB_DEF_OPERAND(cpu, immediate)
-RAB_DEF_OPERAND(cpu, branch_target_label)
+    RAB_DEF_OPERAND(cpu, rs)
+    RAB_DEF_OPERAND(cpu, rt)
+    RAB_DEF_OPERAND(cpu, rd)
+    RAB_DEF_OPERAND(cpu, sa)
+    RAB_DEF_OPERAND(cpu, zero) // $zero
+    // RAB_DEF_OPERAND(cpu, function)
+    RAB_DEF_OPERAND(cpu, cop0d)
+    RAB_DEF_OPERAND(cpu, fs)
+    RAB_DEF_OPERAND(cpu, ft)
+    RAB_DEF_OPERAND(cpu, fd)
+    RAB_DEF_OPERAND(cpu, cop1cs) // Coprocessor 1 control fs
+    RAB_DEF_OPERAND(cpu, cop2t)
+    RAB_DEF_OPERAND(cpu, cop2cd) // Coprocessor 2 control rd
+    RAB_DEF_OPERAND(cpu, op)
+    RAB_DEF_OPERAND(cpu, code)
+    RAB_DEF_OPERAND(cpu, code_lower)
+    RAB_DEF_OPERAND(cpu, copraw)
+    RAB_DEF_OPERAND(cpu, label)
+    RAB_DEF_OPERAND(cpu, immediate)
+    RAB_DEF_OPERAND(cpu, branch_target_label)
 
-// composed/aliased operands
-RAB_DEF_OPERAND(cpu, immediate_base)
-RAB_DEF_OPERAND(cpu, maybe_rd_rs) // $rd is omitted if it is $ra
+    // composed/aliased operands
+    RAB_DEF_OPERAND(cpu, immediate_base)
+    RAB_DEF_OPERAND(cpu, maybe_rd_rs) // $rd is omitted if it is $ra
```

### Comparing `rabbitizer-1.7.0/include/instructions/operands/RabbitizerOperandType_rsp.inc` & `rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_rsp.inc`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
-RAB_DEF_OPERAND(rsp, rs)
-RAB_DEF_OPERAND(rsp, rt)
-RAB_DEF_OPERAND(rsp, rd)
-RAB_DEF_OPERAND(rsp, cop0d)
-RAB_DEF_OPERAND(rsp, cop2t)
-RAB_DEF_OPERAND(rsp, cop2cd) // Coprocessor 2 control rd
-RAB_DEF_OPERAND(rsp, vs)
-RAB_DEF_OPERAND(rsp, vt)
-RAB_DEF_OPERAND(rsp, vd)
-// RAB_DEF_OPERAND(rsp, elementhigh)
-// RAB_DEF_OPERAND(rsp, elementlow)
-// RAB_DEF_OPERAND(rsp, index)
-// RAB_DEF_OPERAND(rsp, offset)
+    RAB_DEF_OPERAND(rsp, rs)
+    RAB_DEF_OPERAND(rsp, rt)
+    RAB_DEF_OPERAND(rsp, rd)
+    RAB_DEF_OPERAND(rsp, cop0d)
+    RAB_DEF_OPERAND(rsp, cop2t)
+    RAB_DEF_OPERAND(rsp, cop2cd) // Coprocessor 2 control rd
+    RAB_DEF_OPERAND(rsp, vs)
+    RAB_DEF_OPERAND(rsp, vt)
+    RAB_DEF_OPERAND(rsp, vd)
+    // RAB_DEF_OPERAND(rsp, elementhigh)
+    // RAB_DEF_OPERAND(rsp, elementlow)
+    // RAB_DEF_OPERAND(rsp, index)
+    // RAB_DEF_OPERAND(rsp, offset)
 
-// composed/aliased operands
-RAB_DEF_OPERAND(rsp, vt_elementhigh)
-RAB_DEF_OPERAND(rsp, vt_elementlow)
-RAB_DEF_OPERAND(rsp, vd_de)
-RAB_DEF_OPERAND(rsp, vs_index)
-RAB_DEF_OPERAND(rsp, offset_rs)
-RAB_DEF_OPERAND(rsp, immediate_base)
-RAB_DEF_OPERAND(rsp, maybe_rd_rs)
+    // composed/aliased operands
+    RAB_DEF_OPERAND(rsp, vt_elementhigh)
+    RAB_DEF_OPERAND(rsp, vt_elementlow)
+    RAB_DEF_OPERAND(rsp, vd_de)
+    RAB_DEF_OPERAND(rsp, vs_index)
+    RAB_DEF_OPERAND(rsp, offset_rs)
+    RAB_DEF_OPERAND(rsp, immediate_base)
+    RAB_DEF_OPERAND(rsp, maybe_rd_rs)
```

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop0.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop1Control.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop1N32.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1N32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop1N64.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1N64.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop1O32.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1O32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_Cop2.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_GprN32.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_GprN32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_GprO32.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_GprO32.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_R5900VF.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_R5900VF.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_R5900VI.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_R5900VI.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspCop0.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspCop2.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspGpr.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspGpr.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/instructions/registers/RabbitizerRegister_RspVector.inc` & `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspVector.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/include/rabbitizer.h` & `rabbitizer-1.7.1/include/rabbitizer.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/pyproject.toml` & `rabbitizer-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "rabbitizer"
 # Version should be synced with include/common/RabbitizerVersion.h
-version = "1.7.0"
+version = "1.7.1"
 description = "MIPS instruction decoder"
 # license = "MIT"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     { name="Anghelo Carvajal", email="angheloalf95@gmail.com" },
 ]
```

### Comparing `rabbitizer-1.7.0/rabbitizer/Config.pyi` & `rabbitizer-1.7.1/rabbitizer/Config.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,15 @@
 
 # SPDX-FileCopyrightText: © 2022 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from .Enum import Enum
-
-
-class Abi:
-    NUMERIC: Enum
-    O32: Enum
-    N32: Enum
-    N64: Enum
-
-    @staticmethod
-    def fromStr(name: str | None) -> Enum: ...
-
+from .Abi import Abi
 
 class _RabbitizerConfig:
     regNames_namedRegisters: bool = True
     regNames_gprAbiNames: Enum = Abi.O32
     regNames_fprAbiNames: Enum = Abi.NUMERIC
     regNames_userFpcCsr: bool = True
     regNames_vr4300Cop0NamedRegisters: bool = True
```

### Comparing `rabbitizer-1.7.0/rabbitizer/Enum.pyi` & `rabbitizer-1.7.1/rabbitizer/Enum.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/InstrId.pyi` & `rabbitizer-1.7.1/rabbitizer/InstrId.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,110 +1,38 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
-from __future__ import annotations
+# Automatically generated. DO NOT MODIFY
 
+from __future__ import annotations
 from .Enum import Enum
-
-
 class InstrId:
     cpu_INVALID: Enum
-    cpu_mthi: Enum
-    cpu_mtlo: Enum
-    cpu_jr: Enum
-    cpu_jalr: Enum
-    cpu_mfhi: Enum
-    cpu_mflo: Enum
-    cpu_mult: Enum
-    cpu_multu: Enum
-    cpu_dmult: Enum
-    cpu_dmultu: Enum
-    cpu_tge: Enum
-    cpu_tgeu: Enum
-    cpu_tlt: Enum
-    cpu_tltu: Enum
-    cpu_teq: Enum
-    cpu_tne: Enum
-    cpu_movz: Enum
-    cpu_movn: Enum
-    cpu_div: Enum
-    cpu_divu: Enum
-    cpu_sn64_div: Enum
-    cpu_sn64_divu: Enum
-    cpu_ddiv: Enum
-    cpu_ddivu: Enum
-    cpu_add: Enum
-    cpu_addu: Enum
-    cpu_sub: Enum
-    cpu_subu: Enum
-    cpu_and: Enum
-    cpu_or: Enum
-    cpu_xor: Enum
-    cpu_nor: Enum
-    cpu_slt: Enum
-    cpu_sltu: Enum
-    cpu_dadd: Enum
-    cpu_daddu: Enum
-    cpu_dsub: Enum
-    cpu_dsubu: Enum
-    cpu_syscall: Enum
-    cpu_break: Enum
-    cpu_sync: Enum
-    cpu_dsllv: Enum
-    cpu_dsrlv: Enum
-    cpu_dsrav: Enum
-    cpu_sllv: Enum
-    cpu_srlv: Enum
-    cpu_srav: Enum
-    cpu_sll: Enum
-    cpu_srl: Enum
-    cpu_sra: Enum
-    cpu_dsll: Enum
-    cpu_dsrl: Enum
-    cpu_dsra: Enum
-    cpu_dsll32: Enum
-    cpu_dsrl32: Enum
-    cpu_dsra32: Enum
-    cpu_bltz: Enum
-    cpu_bgez: Enum
-    cpu_bltzl: Enum
-    cpu_bgezl: Enum
-    cpu_tgei: Enum
-    cpu_tgeiu: Enum
-    cpu_tlti: Enum
-    cpu_tltiu: Enum
-    cpu_bltzal: Enum
-    cpu_bgezal: Enum
-    cpu_bltzall: Enum
-    cpu_bgezall: Enum
-    cpu_bal: Enum
-    cpu_teqi: Enum
-    cpu_tnei: Enum
     cpu_j: Enum
     cpu_jal: Enum
     cpu_beq: Enum
     cpu_bne: Enum
     cpu_beql: Enum
     cpu_bnel: Enum
     cpu_blez: Enum
-    cpu_bgtz: Enum
     cpu_blezl: Enum
+    cpu_bgtz: Enum
     cpu_bgtzl: Enum
-    cpu_lui: Enum
+    cpu_addi: Enum
+    cpu_addiu: Enum
+    cpu_slti: Enum
+    cpu_sltiu: Enum
     cpu_andi: Enum
     cpu_ori: Enum
     cpu_xori: Enum
-    cpu_addi: Enum
-    cpu_addiu: Enum
     cpu_daddi: Enum
     cpu_daddiu: Enum
-    cpu_slti: Enum
-    cpu_sltiu: Enum
+    cpu_lui: Enum
     cpu_ldl: Enum
     cpu_ldr: Enum
     cpu_lb: Enum
     cpu_lh: Enum
     cpu_lwl: Enum
     cpu_lw: Enum
     cpu_lbu: Enum
@@ -121,135 +49,210 @@
     cpu_ll: Enum
     cpu_pref: Enum
     cpu_lld: Enum
     cpu_ld: Enum
     cpu_sc: Enum
     cpu_scd: Enum
     cpu_sd: Enum
+    cpu_cache: Enum
     cpu_lwc1: Enum
     cpu_ldc1: Enum
     cpu_swc1: Enum
     cpu_sdc1: Enum
     cpu_lwc2: Enum
     cpu_ldc2: Enum
     cpu_swc2: Enum
     cpu_sdc2: Enum
+    cpu_b: Enum
+    cpu_beqz: Enum
+    cpu_bnez: Enum
+    cpu_sll: Enum
+    cpu_srl: Enum
+    cpu_sra: Enum
+    cpu_dsll: Enum
+    cpu_dsrl: Enum
+    cpu_dsra: Enum
+    cpu_dsll32: Enum
+    cpu_dsrl32: Enum
+    cpu_dsra32: Enum
+    cpu_dsllv: Enum
+    cpu_dsrlv: Enum
+    cpu_dsrav: Enum
+    cpu_sllv: Enum
+    cpu_srlv: Enum
+    cpu_srav: Enum
+    cpu_mthi: Enum
+    cpu_mtlo: Enum
+    cpu_jr: Enum
+    cpu_jalr: Enum
+    cpu_mfhi: Enum
+    cpu_mflo: Enum
+    cpu_movz: Enum
+    cpu_movn: Enum
+    cpu_div: Enum
+    cpu_divu: Enum
+    cpu_sn64_div: Enum
+    cpu_sn64_divu: Enum
+    cpu_ddiv: Enum
+    cpu_ddivu: Enum
+    cpu_add: Enum
+    cpu_addu: Enum
+    cpu_sub: Enum
+    cpu_subu: Enum
+    cpu_and: Enum
+    cpu_or: Enum
+    cpu_xor: Enum
+    cpu_nor: Enum
+    cpu_slt: Enum
+    cpu_sltu: Enum
+    cpu_dadd: Enum
+    cpu_daddu: Enum
+    cpu_dsub: Enum
+    cpu_dsubu: Enum
+    cpu_syscall: Enum
+    cpu_break: Enum
+    cpu_sync: Enum
+    cpu_mult: Enum
+    cpu_multu: Enum
+    cpu_dmult: Enum
+    cpu_dmultu: Enum
+    cpu_tge: Enum
+    cpu_tgeu: Enum
+    cpu_tlt: Enum
+    cpu_tltu: Enum
+    cpu_teq: Enum
+    cpu_tne: Enum
+    cpu_nop: Enum
+    cpu_move: Enum
+    cpu_not: Enum
+    cpu_negu: Enum
+    cpu_bltz: Enum
+    cpu_bgez: Enum
+    cpu_bltzl: Enum
+    cpu_bgezl: Enum
+    cpu_tgei: Enum
+    cpu_tgeiu: Enum
+    cpu_tlti: Enum
+    cpu_tltiu: Enum
+    cpu_teqi: Enum
+    cpu_tnei: Enum
+    cpu_bltzal: Enum
+    cpu_bgezal: Enum
+    cpu_bltzall: Enum
+    cpu_bgezall: Enum
+    cpu_bal: Enum
     cpu_mfc0: Enum
     cpu_dmfc0: Enum
     cpu_cfc0: Enum
     cpu_mtc0: Enum
     cpu_dmtc0: Enum
     cpu_ctc0: Enum
+    cpu_bc0f: Enum
+    cpu_bc0t: Enum
+    cpu_bc0fl: Enum
+    cpu_bc0tl: Enum
     cpu_tlbr: Enum
     cpu_tlbwi: Enum
     cpu_tlbwr: Enum
     cpu_tlbp: Enum
     cpu_eret: Enum
-    cpu_bc0t: Enum
-    cpu_bc0f: Enum
-    cpu_bc0tl: Enum
-    cpu_bc0fl: Enum
     cpu_mfc1: Enum
     cpu_dmfc1: Enum
     cpu_mtc1: Enum
     cpu_dmtc1: Enum
     cpu_cfc1: Enum
     cpu_ctc1: Enum
     cpu_bc1f: Enum
     cpu_bc1t: Enum
     cpu_bc1fl: Enum
     cpu_bc1tl: Enum
     cpu_add_s: Enum
     cpu_sub_s: Enum
     cpu_mul_s: Enum
     cpu_div_s: Enum
-    cpu_add_d: Enum
-    cpu_sub_d: Enum
-    cpu_mul_d: Enum
-    cpu_div_d: Enum
     cpu_sqrt_s: Enum
     cpu_abs_s: Enum
     cpu_mov_s: Enum
     cpu_neg_s: Enum
-    cpu_sqrt_d: Enum
-    cpu_abs_d: Enum
-    cpu_mov_d: Enum
-    cpu_neg_d: Enum
     cpu_round_l_s: Enum
     cpu_trunc_l_s: Enum
     cpu_ceil_l_s: Enum
     cpu_floor_l_s: Enum
-    cpu_round_l_d: Enum
-    cpu_trunc_l_d: Enum
-    cpu_ceil_l_d: Enum
-    cpu_floor_l_d: Enum
     cpu_round_w_s: Enum
     cpu_trunc_w_s: Enum
     cpu_ceil_w_s: Enum
     cpu_floor_w_s: Enum
-    cpu_round_w_d: Enum
-    cpu_trunc_w_d: Enum
-    cpu_ceil_w_d: Enum
-    cpu_floor_w_d: Enum
+    cpu_cvt_d_s: Enum
+    cpu_cvt_w_s: Enum
+    cpu_cvt_l_s: Enum
     cpu_c_f_s: Enum
     cpu_c_un_s: Enum
     cpu_c_eq_s: Enum
     cpu_c_ueq_s: Enum
     cpu_c_olt_s: Enum
     cpu_c_ult_s: Enum
     cpu_c_ole_s: Enum
     cpu_c_ule_s: Enum
-    cpu_c_f_d: Enum
-    cpu_c_un_d: Enum
-    cpu_c_eq_d: Enum
-    cpu_c_ueq_d: Enum
-    cpu_c_olt_d: Enum
-    cpu_c_ult_d: Enum
-    cpu_c_ole_d: Enum
-    cpu_c_ule_d: Enum
     cpu_c_sf_s: Enum
     cpu_c_ngle_s: Enum
     cpu_c_seq_s: Enum
     cpu_c_ngl_s: Enum
     cpu_c_lt_s: Enum
     cpu_c_nge_s: Enum
     cpu_c_le_s: Enum
     cpu_c_ngt_s: Enum
-    cpu_c_sf_d: Enum
+    cpu_add_d: Enum
+    cpu_sub_d: Enum
+    cpu_mul_d: Enum
+    cpu_div_d: Enum
+    cpu_sqrt_d: Enum
+    cpu_abs_d: Enum
+    cpu_mov_d: Enum
+    cpu_neg_d: Enum
+    cpu_round_l_d: Enum
+    cpu_trunc_l_d: Enum
+    cpu_ceil_l_d: Enum
+    cpu_floor_l_d: Enum
+    cpu_round_w_d: Enum
+    cpu_trunc_w_d: Enum
+    cpu_ceil_w_d: Enum
+    cpu_floor_w_d: Enum
+    cpu_cvt_s_d: Enum
+    cpu_cvt_w_d: Enum
+    cpu_cvt_l_d: Enum
+    cpu_c_f_d: Enum
+    cpu_c_un_d: Enum
+    cpu_c_eq_d: Enum
+    cpu_c_ueq_d: Enum
+    cpu_c_olt_d: Enum
+    cpu_c_ult_d: Enum
+    cpu_c_ole_d: Enum
+    cpu_c_ule_d: Enum
+    cpu_c_df_d: Enum
     cpu_c_ngle_d: Enum
-    cpu_c_seq_d: Enum
+    cpu_c_deq_d: Enum
     cpu_c_ngl_d: Enum
     cpu_c_lt_d: Enum
     cpu_c_nge_d: Enum
     cpu_c_le_d: Enum
     cpu_c_ngt_d: Enum
-    cpu_cvt_s_d: Enum
     cpu_cvt_s_w: Enum
-    cpu_cvt_s_l: Enum
-    cpu_cvt_d_s: Enum
     cpu_cvt_d_w: Enum
+    cpu_cvt_s_l: Enum
     cpu_cvt_d_l: Enum
     cpu_mfc2: Enum
     cpu_mtc2: Enum
     cpu_cfc2: Enum
     cpu_ctc2: Enum
-    cpu_cvt_w_s: Enum
-    cpu_cvt_w_d: Enum
-    cpu_cvt_l_s: Enum
-    cpu_cvt_l_d: Enum
-    cpu_nop: Enum
-    cpu_beqz: Enum
-    cpu_bnez: Enum
-    cpu_b: Enum
-    cpu_move: Enum
-    cpu_not: Enum
-    cpu_negu: Enum
     cpu_MAX: Enum
-
     rsp_INVALID: Enum
+    rsp_mfc2: Enum
+    rsp_mtc2: Enum
+    rsp_cfc2: Enum
+    rsp_ctc2: Enum
     rsp_vmulf: Enum
     rsp_vmulu: Enum
     rsp_vrndp: Enum
     rsp_vmulq: Enum
     rsp_vmudl: Enum
     rsp_vmudm: Enum
     rsp_vmudn: Enum
@@ -286,101 +289,96 @@
     rsp_vrcpl: Enum
     rsp_vrcph: Enum
     rsp_vmov: Enum
     rsp_vrsq: Enum
     rsp_vrsql: Enum
     rsp_vrsqh: Enum
     rsp_vnop: Enum
-    rsp_mfc2: Enum
-    rsp_mtc2: Enum
-    rsp_cfc2: Enum
-    rsp_ctc2: Enum
-    rsp_sbv: Enum
-    rsp_ssv: Enum
-    rsp_slv: Enum
-    rsp_sdv: Enum
-    rsp_sqv: Enum
-    rsp_srv: Enum
-    rsp_spv: Enum
-    rsp_suv: Enum
-    rsp_swv: Enum
-    rsp_shv: Enum
-    rsp_sfv: Enum
-    rsp_stv: Enum
     rsp_lbv: Enum
     rsp_lsv: Enum
     rsp_llv: Enum
     rsp_ldv: Enum
     rsp_lqv: Enum
     rsp_lrv: Enum
     rsp_lpv: Enum
     rsp_luv: Enum
     rsp_lhv: Enum
     rsp_lfv: Enum
     rsp_ltv: Enum
-    rsp_jr: Enum
-    rsp_jalr: Enum
-    rsp_movz: Enum
-    rsp_movn: Enum
-    rsp_add: Enum
-    rsp_addu: Enum
-    rsp_sub: Enum
-    rsp_subu: Enum
-    rsp_and: Enum
-    rsp_or: Enum
-    rsp_xor: Enum
-    rsp_nor: Enum
-    rsp_slt: Enum
-    rsp_sltu: Enum
-    rsp_break: Enum
-    rsp_sllv: Enum
-    rsp_srlv: Enum
-    rsp_srav: Enum
-    rsp_sll: Enum
-    rsp_srl: Enum
-    rsp_sra: Enum
-    rsp_bltz: Enum
-    rsp_bgez: Enum
-    rsp_bltzal: Enum
-    rsp_bgezal: Enum
-    rsp_bal: Enum
+    rsp_sbv: Enum
+    rsp_ssv: Enum
+    rsp_slv: Enum
+    rsp_sdv: Enum
+    rsp_sqv: Enum
+    rsp_srv: Enum
+    rsp_spv: Enum
+    rsp_suv: Enum
+    rsp_shv: Enum
+    rsp_sfv: Enum
+    rsp_stv: Enum
+    rsp_swv: Enum
     rsp_j: Enum
     rsp_jal: Enum
     rsp_beq: Enum
     rsp_bne: Enum
     rsp_blez: Enum
     rsp_bgtz: Enum
-    rsp_lui: Enum
-    rsp_andi: Enum
-    rsp_ori: Enum
-    rsp_xori: Enum
     rsp_addi: Enum
     rsp_addiu: Enum
     rsp_slti: Enum
     rsp_sltiu: Enum
+    rsp_andi: Enum
+    rsp_ori: Enum
+    rsp_xori: Enum
+    rsp_lui: Enum
     rsp_lb: Enum
     rsp_lh: Enum
     rsp_lw: Enum
     rsp_lbu: Enum
     rsp_lhu: Enum
     rsp_sb: Enum
     rsp_sh: Enum
     rsp_sw: Enum
     rsp_pref: Enum
-    rsp_mfc0: Enum
-    rsp_mtc0: Enum
-    rsp_nop: Enum
+    rsp_b: Enum
     rsp_beqz: Enum
     rsp_bnez: Enum
-    rsp_b: Enum
+    rsp_sll: Enum
+    rsp_srl: Enum
+    rsp_sra: Enum
+    rsp_sllv: Enum
+    rsp_srlv: Enum
+    rsp_srav: Enum
+    rsp_jr: Enum
+    rsp_jalr: Enum
+    rsp_movz: Enum
+    rsp_movn: Enum
+    rsp_add: Enum
+    rsp_addu: Enum
+    rsp_sub: Enum
+    rsp_subu: Enum
+    rsp_and: Enum
+    rsp_or: Enum
+    rsp_xor: Enum
+    rsp_nor: Enum
+    rsp_slt: Enum
+    rsp_sltu: Enum
+    rsp_break: Enum
+    rsp_nop: Enum
     rsp_move: Enum
     rsp_not: Enum
     rsp_negu: Enum
+    rsp_bltz: Enum
+    rsp_bgez: Enum
+    rsp_bltzal: Enum
+    rsp_bgezal: Enum
+    rsp_bal: Enum
+    rsp_mfc0: Enum
+    rsp_mtc0: Enum
     rsp_MAX: Enum
-
     r3000gte_INVALID: Enum
     r3000gte_RTPS: Enum
     r3000gte_RTPT: Enum
     r3000gte_DPCL: Enum
     r3000gte_DPCS: Enum
     r3000gte_DPCT: Enum
     r3000gte_INTPL: Enum
@@ -397,21 +395,21 @@
     r3000gte_AVSZ4: Enum
     r3000gte_MVMVA: Enum
     r3000gte_SQR: Enum
     r3000gte_OP: Enum
     r3000gte_GPF: Enum
     r3000gte_GPL: Enum
     r3000gte_MAX: Enum
-
     r5900_INVALID: Enum
     r5900_lq: Enum
     r5900_sq: Enum
     r5900_lqc2: Enum
     r5900_sqc2: Enum
     r5900_sync_p: Enum
+    r5900_mult: Enum
     r5900_mfsa: Enum
     r5900_mtsa: Enum
     r5900_mtsab: Enum
     r5900_mtsah: Enum
     r5900_madd: Enum
     r5900_maddu: Enum
     r5900_plzcw: Enum
@@ -509,24 +507,27 @@
     r5900_por: Enum
     r5900_pnor: Enum
     r5900_pexch: Enum
     r5900_pcpyh: Enum
     r5900_pexcw: Enum
     r5900_ei: Enum
     r5900_di: Enum
+    r5900_c1__sqrt_s: Enum
     r5900_rsqrt_s: Enum
     r5900_adda_s: Enum
     r5900_suba_s: Enum
     r5900_mula_s: Enum
     r5900_madd_s: Enum
     r5900_msub_s: Enum
     r5900_madda_s: Enum
     r5900_msuba_s: Enum
     r5900_max_s: Enum
     r5900_min_s: Enum
+    r5900_c_lt_s: Enum
+    r5900_c_le_s: Enum
     r5900_qmfc2: Enum
     r5900_cfc2: Enum
     r5900_qmtc2: Enum
     r5900_ctc2: Enum
     r5900_bc2f: Enum
     r5900_bc2t: Enum
     r5900_bc2fl: Enum
@@ -581,27 +582,27 @@
     r5900_vmini: Enum
     r5900_viadd: Enum
     r5900_visub: Enum
     r5900_viaddi: Enum
     r5900_viand: Enum
     r5900_vior: Enum
     r5900_vcallms: Enum
-    r5900_callmsr: Enum
+    r5900_vcallmsr: Enum
     r5900_vaddax: Enum
     r5900_vadday: Enum
     r5900_vaddaz: Enum
     r5900_vaddaw: Enum
     r5900_vsubax: Enum
     r5900_vsubay: Enum
     r5900_vsubaz: Enum
     r5900_vsubaw: Enum
-    r5900_vvmaddx: Enum
-    r5900_vvmaddy: Enum
-    r5900_vvmaddz: Enum
-    r5900_vvmaddw: Enum
+    r5900_vmaddax: Enum
+    r5900_vmadday: Enum
+    r5900_vmaddaz: Enum
+    r5900_vmaddaw: Enum
     r5900_vmsubax: Enum
     r5900_vmsubay: Enum
     r5900_vmsubaz: Enum
     r5900_vmsubaw: Enum
     r5900_vitof0: Enum
     r5900_vitof4: Enum
     r5900_vitof12: Enum
@@ -648,9 +649,8 @@
     r5900_vilwr: Enum
     r5900_viswr: Enum
     r5900_vrnext: Enum
     r5900_vrget: Enum
     r5900_vrinit: Enum
     r5900_vrxor: Enum
     r5900_MAX: Enum
-
     ALL_MAX: Enum
```

### Comparing `rabbitizer-1.7.0/rabbitizer/OperandType.pyi` & `rabbitizer-1.7.1/rabbitizer/OperandType.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
-from __future__ import annotations
+# Automatically generated. DO NOT MODIFY
 
+from __future__ import annotations
 from .Enum import Enum
-
-
 class OperandType:
     ALL_INVALID: Enum
-
     cpu_rs: Enum
     cpu_rt: Enum
     cpu_rd: Enum
     cpu_sa: Enum
     cpu_zero: Enum
     cpu_cop0d: Enum
     cpu_fs: Enum
     cpu_ft: Enum
     cpu_fd: Enum
     cpu_cop1cs: Enum
     cpu_cop2t: Enum
+    cpu_cop2cd: Enum
     cpu_op: Enum
     cpu_code: Enum
     cpu_code_lower: Enum
     cpu_copraw: Enum
     cpu_label: Enum
     cpu_immediate: Enum
     cpu_branch_target_label: Enum
     cpu_immediate_base: Enum
     cpu_maybe_rd_rs: Enum
-
     rsp_rs: Enum
     rsp_rt: Enum
     rsp_rd: Enum
     rsp_cop0d: Enum
     rsp_cop2t: Enum
     rsp_cop2cd: Enum
     rsp_vs: Enum
@@ -44,21 +42,19 @@
     rsp_vt_elementhigh: Enum
     rsp_vt_elementlow: Enum
     rsp_vd_de: Enum
     rsp_vs_index: Enum
     rsp_offset_rs: Enum
     rsp_immediate_base: Enum
     rsp_maybe_rd_rs: Enum
-
     r3000gte_sf: Enum
     r3000gte_mx: Enum
     r3000gte_v: Enum
     r3000gte_cv: Enum
     r3000gte_lm: Enum
-
     r5900_I: Enum
     r5900_Q: Enum
     r5900_R: Enum
     r5900_ACC: Enum
     r5900_ACCxyzw: Enum
     r5900_vfs: Enum
     r5900_vft: Enum
@@ -81,9 +77,8 @@
     r5900_vis_predecr: Enum
     r5900_vit_predecr: Enum
     r5900_vid_predecr: Enum
     r5900_vis_postincr: Enum
     r5900_vit_postincr: Enum
     r5900_vid_postincr: Enum
     r5900_immediate5: Enum
-
     ALL_MAX: Enum
```

### Comparing `rabbitizer-1.7.0/rabbitizer/RegCop1N32.pyi` & `rabbitizer-1.7.1/rabbitizer/RegCop1N32.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2023 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
-from __future__ import annotations
+# Automatically generated. DO NOT MODIFY
 
+from __future__ import annotations
 from .Enum import Enum
-
-
 class RegCop1N32:
     fv0: Enum
     ft14: Enum
     fv1: Enum
     ft15: Enum
     ft0: Enum
     ft1: Enum
```

### Comparing `rabbitizer-1.7.0/rabbitizer/RegGprN32.pyi` & `rabbitizer-1.7.1/rabbitizer/RegGprN32.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
-from __future__ import annotations
+# Automatically generated. DO NOT MODIFY
 
+from __future__ import annotations
 from .Enum import Enum
-
-
 class RegGprN32:
     zero: Enum
     at: Enum
     v0: Enum
     v1: Enum
     a0: Enum
     a1: Enum
```

### Comparing `rabbitizer-1.7.0/rabbitizer/RegGprO32.pyi` & `rabbitizer-1.7.1/rabbitizer/RegGprO32.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
-from __future__ import annotations
+# Automatically generated. DO NOT MODIFY
 
+from __future__ import annotations
 from .Enum import Enum
-
-
 class RegGprO32:
     zero: Enum
     at: Enum
     v0: Enum
     v1: Enum
     a0: Enum
     a1: Enum
```

### Comparing `rabbitizer-1.7.0/rabbitizer/RegistersTracker.pyi` & `rabbitizer-1.7.1/rabbitizer/RegistersTracker.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/enums_utils.c` & `rabbitizer-1.7.1/rabbitizer/enums/enums_utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/enums_utils.h` & `rabbitizer-1.7.1/rabbitizer/enums/enums_utils.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_enum_Abi.c` & `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_Abi.c`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 /* SPDX-License-Identifier: MIT */
 
 #include "enums_utils.h"
 #include "common/RabbitizerConfig.h"
 #include "common/Utils.h"
 
 
-#define RABBITIZER_DEF_ABI(name) { "Abi", #name, RABBITIZER_ABI_##name, false, NULL }
+#define RABBITIZER_DEF_ABI(name) { "Abi", #name, RABBITIZER_ABI_##name, false, NULL },
 
 RabbitizerEnumMetadata rabbitizer_enum_Abi_enumvalues[] = {
     #include "common/Abi.inc"
-    RABBITIZER_DEF_ABI(MAX),
+    RABBITIZER_DEF_ABI(MAX)
 
     { 0 },
 };
 
 #undef RABBITIZER_DEF_ABI
```

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_enum_AccessType.c` & `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_AccessType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_enum_InstrCategory.c` & `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_InstrCategory.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "enums_utils.h"
 #include "instructions/RabbitizerInstruction.h"
 
 
-#define RABBITIZER_DEF_INSTR_CATEGORY(name) { "InstrCategory", #name, RABBITIZER_INSTRCAT_##name, false, NULL }
+#define RABBITIZER_DEF_INSTR_CATEGORY(name) { "InstrCategory", #name, RABBITIZER_INSTRCAT_##name, false, NULL },
 
 RabbitizerEnumMetadata rabbitizer_enum_InstrCategory_enumvalues[] = {
     #include "instructions/InstrCategory.inc"
-    RABBITIZER_DEF_INSTR_CATEGORY(MAX),
+    RABBITIZER_DEF_INSTR_CATEGORY(MAX)
 
     { 0 },
 };
 
 #undef RABBITIZER_DEF_INSTR_CATEGORY
```

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/rabbitizer_type_Enum.c` & `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_type_Enum.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c` & `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c` & `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c` & `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c` & `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c` & `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/rabbitizer.pyi` & `rabbitizer-1.7.1/rabbitizer/rabbitizer.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/rabbitizer_global_config.c` & `rabbitizer-1.7.1/rabbitizer/rabbitizer_global_config.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/rabbitizer_module.c` & `rabbitizer-1.7.1/rabbitizer/rabbitizer_module.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/rabbitizer_module.h` & `rabbitizer-1.7.1/rabbitizer/rabbitizer_module.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/rabbitizer_submodule_Utils.c` & `rabbitizer-1.7.1/rabbitizer/rabbitizer_submodule_Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/rabbitizer_type_Instruction.c` & `rabbitizer-1.7.1/rabbitizer/rabbitizer_type_Instruction.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/rabbitizer_type_LoPairingInfo.c` & `rabbitizer-1.7.1/rabbitizer/rabbitizer_type_LoPairingInfo.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/rabbitizer_type_RegistersTracker.c` & `rabbitizer-1.7.1/rabbitizer/rabbitizer_type_RegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer/rabbitizer_type_TrackedRegisterState.c` & `rabbitizer-1.7.1/rabbitizer/rabbitizer_type_TrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/rabbitizer.egg-info/PKG-INFO` & `rabbitizer-1.7.1/rabbitizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.7.0
+Version: 1.7.1
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.7.0/rabbitizer.egg-info/SOURCES.txt` & `rabbitizer-1.7.1/rabbitizer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 include/instructions/AccessType_enum.table.h
 include/instructions/AccessType_enum.table.template
 include/instructions/InstrCategory.inc
 include/instructions/InstrCategory_enum.table.h
 include/instructions/InstrCategory_enum.table.template
 include/instructions/InstrId_enum.table.h
 include/instructions/InstrId_enum.table.template
+include/instructions/InstrIds.inc
 include/instructions/InstrSuffix.inc
 include/instructions/InstrSuffix_enum.table.h
 include/instructions/InstrSuffix_enum.table.template
 include/instructions/OperandType_enum.table.h
 include/instructions/OperandType_enum.table.template
 include/instructions/OperandType_function_declarations.table.h
 include/instructions/OperandType_function_declarations.table.template
+include/instructions/OperandTypes.inc
 include/instructions/RabbitizerAccessType.h
 include/instructions/RabbitizerInstrCategory.h
 include/instructions/RabbitizerInstrDescriptor.h
 include/instructions/RabbitizerInstrId.h
 include/instructions/RabbitizerInstrSuffix.h
 include/instructions/RabbitizerInstruction.h
 include/instructions/RabbitizerInstructionR3000GTE.h
@@ -97,14 +99,15 @@
 include/instructions/registers/RabbitizerRegister_R5900VF.inc
 include/instructions/registers/RabbitizerRegister_R5900VI.inc
 include/instructions/registers/RabbitizerRegister_RspCop0.inc
 include/instructions/registers/RabbitizerRegister_RspCop2.inc
 include/instructions/registers/RabbitizerRegister_RspCop2Control.inc
 include/instructions/registers/RabbitizerRegister_RspGpr.inc
 include/instructions/registers/RabbitizerRegister_RspVector.inc
+rabbitizer/Abi.pyi
 rabbitizer/AccessType.pyi
 rabbitizer/Config.pyi
 rabbitizer/Enum.pyi
 rabbitizer/InstrCategory.pyi
 rabbitizer/InstrId.pyi
 rabbitizer/LoPairingInfo.pyi
 rabbitizer/OperandType.pyi
```

### Comparing `rabbitizer-1.7.0/setup.py` & `rabbitizer-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/analysis/RabbitizerRegistersTracker.c` & `rabbitizer-1.7.1/src/analysis/RabbitizerRegistersTracker.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/analysis/RabbitizerTrackedRegisterState.c` & `rabbitizer-1.7.1/src/analysis/RabbitizerTrackedRegisterState.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/common/RabbitizerConfig.c` & `rabbitizer-1.7.1/src/common/RabbitizerConfig.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/common/Utils.c` & `rabbitizer-1.7.1/src/common/Utils.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/InstrDescriptor_Descriptors_array.table.h` & `rabbitizer-1.7.1/src/instructions/InstrDescriptor_Descriptors_array.table.h`

 * *Files 12% similar despite different names*

```diff
@@ -3,735 +3,735 @@
 
 /* Automatically generated. DO NOT MODIFY */
 
 #ifndef InstrDescriptor_Descriptors_array_table_h_automatic
 #define InstrDescriptor_Descriptors_array_table_h_automatic
 
 const RabbitizerInstrDescriptor RabbitizerInstrDescriptor_Descriptors[] = {
-[RABBITIZER_INSTR_ID_cpu_INVALID] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate} },
-[RABBITIZER_INSTR_ID_cpu_j] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true },
-[RABBITIZER_INSTR_ID_cpu_jal] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_cpu_beq] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_bne] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_beql] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isBranchLikely=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_bnel] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isBranchLikely=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_blez] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_blezl] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isBranchLikely=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_bgtz] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_bgtzl] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isBranchLikely=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_addi] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .notEmittedByCompilers=true, .canBeLo=true },
-[RABBITIZER_INSTR_ID_cpu_addiu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true },
-[RABBITIZER_INSTR_ID_cpu_slti] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_sltiu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_andi] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_ori] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true, .canBeLo=true },
-[RABBITIZER_INSTR_ID_cpu_xori] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_daddi] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true },
-[RABBITIZER_INSTR_ID_cpu_daddiu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true },
-[RABBITIZER_INSTR_ID_cpu_lui] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .canBeHi=true },
-[RABBITIZER_INSTR_ID_cpu_ldl] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_cpu_ldr] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_cpu_lb] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_BYTE },
-[RABBITIZER_INSTR_ID_cpu_lh] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_SHORT },
-[RABBITIZER_INSTR_ID_cpu_lwl] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_cpu_lw] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_WORD },
-[RABBITIZER_INSTR_ID_cpu_lbu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_BYTE, .doesUnsignedMemoryAccess=true },
-[RABBITIZER_INSTR_ID_cpu_lhu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_SHORT, .doesUnsignedMemoryAccess=true },
-[RABBITIZER_INSTR_ID_cpu_lwr] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_cpu_lwu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_WORD, .doesUnsignedMemoryAccess=true },
-[RABBITIZER_INSTR_ID_cpu_sb] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_BYTE },
-[RABBITIZER_INSTR_ID_cpu_sh] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_SHORT },
-[RABBITIZER_INSTR_ID_cpu_swl] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_cpu_sw] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_WORD },
-[RABBITIZER_INSTR_ID_cpu_sdl] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_cpu_sdr] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_cpu_swr] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_cpu_ll] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .notEmittedByCompilers=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_cpu_pref] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_lld] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .notEmittedByCompilers=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_cpu_ld] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_DOUBLEWORD },
-[RABBITIZER_INSTR_ID_cpu_sc] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .notEmittedByCompilers=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_cpu_scd] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .notEmittedByCompilers=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_cpu_sd] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_DOUBLEWORD },
-[RABBITIZER_INSTR_ID_cpu_cache] = { .operands={RAB_OPERAND_cpu_op, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_lwc1] = { .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .isFloat=true, .readsRs=true, .modifiesFt=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_FLOAT },
-[RABBITIZER_INSTR_ID_cpu_ldc1] = { .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .isFloat=true, .isDouble=true, .readsRs=true, .modifiesFt=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_DOUBLEFLOAT },
-[RABBITIZER_INSTR_ID_cpu_swc1] = { .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .isFloat=true, .readsRs=true, .readsFt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_FLOAT },
-[RABBITIZER_INSTR_ID_cpu_sdc1] = { .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .isFloat=true, .isDouble=true, .readsRs=true, .readsFt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_DOUBLEFLOAT },
-[RABBITIZER_INSTR_ID_cpu_lwc2] = { .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_cpu_ldc2] = { .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_cpu_swc2] = { .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_cpu_sdc2] = { .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_cpu_b] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_cpu_beqz] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .isBranch=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_cpu_bnez] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .isBranch=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_cpu_sll] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_srl] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_sra] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsll] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsrl] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsra] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsll32] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsrl32] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsra32] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsllv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsrlv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsrav] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_sllv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_srlv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_srav] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_mthi] = { .operands={RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .modifiesHI=true },
-[RABBITIZER_INSTR_ID_cpu_mtlo] = { .operands={RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_jr] = { .operands={RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .isJump=true },
-[RABBITIZER_INSTR_ID_cpu_jalr] = { .operands={RAB_OPERAND_cpu_maybe_rd_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .isJump=true, .modifiesRd=true, .readsRs=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_cpu_mfhi] = { .operands={RAB_OPERAND_cpu_rd}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsHI=true },
-[RABBITIZER_INSTR_ID_cpu_mflo] = { .operands={RAB_OPERAND_cpu_rd}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsLO=true },
-[RABBITIZER_INSTR_ID_cpu_movz] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_movn] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_div] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .readsRd=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_divu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .readsRd=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_sn64_div] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_sn64_divu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_ddiv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .readsRd=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_ddivu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .readsRd=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_add] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_addu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true, .maybeIsMove=true },
-[RABBITIZER_INSTR_ID_cpu_sub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .notEmittedByCompilers=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_subu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_and] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_or] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .maybeIsMove=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_xor] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_nor] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_slt] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_sltu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dadd] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_daddu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true, .maybeIsMove=true },
-[RABBITIZER_INSTR_ID_cpu_dsub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_dsubu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_syscall] = { .operands={RAB_OPERAND_cpu_code}, .instrType=RABBITIZER_INSTR_TYPE_R },
-[RABBITIZER_INSTR_ID_cpu_break] = { .operands={RAB_OPERAND_cpu_code}, .instrType=RABBITIZER_INSTR_TYPE_R },
-[RABBITIZER_INSTR_ID_cpu_sync] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_R },
-[RABBITIZER_INSTR_ID_cpu_mult] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_multu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_dmult] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_dmultu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
-[RABBITIZER_INSTR_ID_cpu_tge] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tgeu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tlt] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tltu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_teq] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tne] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_nop] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_R, .isPseudo=true },
-[RABBITIZER_INSTR_ID_cpu_move] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .maybeIsMove=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_cpu_not] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_cpu_negu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_cpu_bltz] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_bgez] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_bltzl] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .isBranchLikely=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_bgezl] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .isBranchLikely=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_cpu_tgei] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tgeiu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tlti] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tltiu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_teqi] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tnei] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_bltzal] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .readsRs=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_cpu_bgezal] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .readsRs=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_cpu_bltzall] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .isBranchLikely=true, .readsRs=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_cpu_bgezall] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .isBranchLikely=true, .readsRs=true, .notEmittedByCompilers=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_cpu_bal] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .notEmittedByCompilers=true, .doesLink=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_cpu_mfc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .modifiesRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_dmfc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .modifiesRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_cfc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .modifiesRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_mtc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .readsRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_dmtc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .readsRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_ctc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .readsRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_bc0f] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true },
-[RABBITIZER_INSTR_ID_cpu_bc0t] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true },
-[RABBITIZER_INSTR_ID_cpu_bc0fl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true, .isBranchLikely=true },
-[RABBITIZER_INSTR_ID_cpu_bc0tl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true, .isBranchLikely=true },
-[RABBITIZER_INSTR_ID_cpu_tlbr] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tlbwi] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_tlbwr] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN },
-[RABBITIZER_INSTR_ID_cpu_tlbp] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_eret] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_cpu_mfc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesRt=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_dmfc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesRt=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_mtc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsRt=true, .modifiesFs=true },
-[RABBITIZER_INSTR_ID_cpu_dmtc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsRt=true, .modifiesFs=true },
-[RABBITIZER_INSTR_ID_cpu_cfc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop1cs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesRt=true },
-[RABBITIZER_INSTR_ID_cpu_ctc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop1cs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_bc1f] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true },
-[RABBITIZER_INSTR_ID_cpu_bc1t] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true },
-[RABBITIZER_INSTR_ID_cpu_bc1fl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true, .isBranchLikely=true },
-[RABBITIZER_INSTR_ID_cpu_bc1tl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true, .isBranchLikely=true },
-[RABBITIZER_INSTR_ID_cpu_add_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_sub_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_mul_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_div_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_sqrt_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_abs_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_mov_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_neg_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_round_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_trunc_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_ceil_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_floor_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_round_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_trunc_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_ceil_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_floor_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_d_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_c_f_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_un_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_eq_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ueq_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_olt_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ult_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ole_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ule_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_sf_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ngle_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_seq_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ngl_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_lt_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_nge_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_le_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ngt_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_add_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_sub_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_mul_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_div_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_sqrt_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_abs_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_mov_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_neg_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_round_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_trunc_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_ceil_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_floor_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_round_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_trunc_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_ceil_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_floor_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_s_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_c_f_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_un_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_eq_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ueq_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_olt_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ult_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ole_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ule_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_df_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ngle_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_deq_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ngl_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_lt_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_nge_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_le_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_c_ngt_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_s_w] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_d_w] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_s_l] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_cvt_d_l] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
-[RABBITIZER_INSTR_ID_cpu_mfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd}, .modifiesRt=true },
-[RABBITIZER_INSTR_ID_cpu_mtc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd}, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_cfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd}, .modifiesRt=true },
-[RABBITIZER_INSTR_ID_cpu_ctc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd}, .readsRt=true },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_00] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_01] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_02] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_03] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_04] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_05] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_06] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_07] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_08] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_09] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_10] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_11] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_12] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_13] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_14] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_15] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_16] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_17] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_18] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_USERDEF_19] = { .operands={0} },
-[RABBITIZER_INSTR_ID_cpu_MAX] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_INVALID] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_mfc2] = { .operands={RAB_OPERAND_rsp_cop2t, RAB_OPERAND_rsp_vs_index} },
-[RABBITIZER_INSTR_ID_rsp_mtc2] = { .operands={RAB_OPERAND_rsp_cop2t, RAB_OPERAND_rsp_vs_index} },
-[RABBITIZER_INSTR_ID_rsp_cfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_rsp_cop2cd}, .modifiesRt=true },
-[RABBITIZER_INSTR_ID_rsp_ctc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_rsp_cop2cd}, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_vmulf] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmulu] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vrndp] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmulq] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmudl] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmudm] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmudn] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmudh] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmacf] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmacu] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vrndn] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmacq] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmadl] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmadm] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmadn] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmadh] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vadd] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vsub] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vabs] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vaddc] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vsubc] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vsar] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vand] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vnand] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vor] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vnor] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vxor] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vnxor] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vlt] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_veq] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vne] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vge] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vcl] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vch] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vcr] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmrg] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vrcp] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vrcpl] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vrcph] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vmov] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vrsq] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vrsql] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vrsqh] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
-[RABBITIZER_INSTR_ID_rsp_vnop] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_lbv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_lsv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_llv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_ldv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_lqv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_lrv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_lpv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_luv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_lhv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_lfv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_ltv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_sbv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_ssv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_slv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_sdv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_sqv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_srv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_spv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_suv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_shv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_sfv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_stv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_swv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_j] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true },
-[RABBITIZER_INSTR_ID_rsp_jal] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_rsp_beq] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .readsRt=true, .isBranch=true },
-[RABBITIZER_INSTR_ID_rsp_bne] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .readsRt=true, .isBranch=true },
-[RABBITIZER_INSTR_ID_rsp_blez] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
-[RABBITIZER_INSTR_ID_rsp_bgtz] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
-[RABBITIZER_INSTR_ID_rsp_addi] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .notEmittedByCompilers=true, .canBeLo=true },
-[RABBITIZER_INSTR_ID_rsp_addiu] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true },
-[RABBITIZER_INSTR_ID_rsp_slti] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_sltiu] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_andi] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_ori] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true, .canBeLo=true },
-[RABBITIZER_INSTR_ID_rsp_xori] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_rsp_lui] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .canBeHi=true },
-[RABBITIZER_INSTR_ID_rsp_lb] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_BYTE },
-[RABBITIZER_INSTR_ID_rsp_lh] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_SHORT },
-[RABBITIZER_INSTR_ID_rsp_lw] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_WORD },
-[RABBITIZER_INSTR_ID_rsp_lbu] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_BYTE, .doesUnsignedMemoryAccess=true },
-[RABBITIZER_INSTR_ID_rsp_lhu] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_SHORT, .doesUnsignedMemoryAccess=true },
-[RABBITIZER_INSTR_ID_rsp_sb] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_BYTE },
-[RABBITIZER_INSTR_ID_rsp_sh] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_SHORT },
-[RABBITIZER_INSTR_ID_rsp_sw] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_WORD },
-[RABBITIZER_INSTR_ID_rsp_pref] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_b] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true },
-[RABBITIZER_INSTR_ID_rsp_beqz] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
-[RABBITIZER_INSTR_ID_rsp_bnez] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
-[RABBITIZER_INSTR_ID_rsp_sll] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_srl] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_sra] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_sllv] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_srlv] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_srav] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_jr] = { .operands={RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .isJump=true },
-[RABBITIZER_INSTR_ID_rsp_jalr] = { .operands={RAB_OPERAND_rsp_maybe_rd_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .isJump=true, .modifiesRd=true, .readsRs=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_rsp_movz] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_movn] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_add] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_rsp_addu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_sub] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .notEmittedByCompilers=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_subu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_and] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_or] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_xor] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_nor] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_slt] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_sltu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_rsp_break] = { .operands={RAB_OPERAND_cpu_code}, .instrType=RABBITIZER_INSTR_TYPE_R },
-[RABBITIZER_INSTR_ID_rsp_nop] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_R, .isPseudo=true },
-[RABBITIZER_INSTR_ID_rsp_move] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_rsp_not] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_rsp_negu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_rsp_bltz] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
-[RABBITIZER_INSTR_ID_rsp_bgez] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
-[RABBITIZER_INSTR_ID_rsp_bltzal] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_rsp_bgezal] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true, .notEmittedByCompilers=true, .doesLink=true },
-[RABBITIZER_INSTR_ID_rsp_bal] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .notEmittedByCompilers=true, .doesLink=true, .isPseudo=true },
-[RABBITIZER_INSTR_ID_rsp_mfc0] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .modifiesRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_rsp_mtc0] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .readsRt=true, .notEmittedByCompilers=true },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_00] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_01] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_02] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_03] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_04] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_05] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_06] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_07] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_08] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_09] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_10] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_11] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_12] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_13] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_14] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_15] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_16] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_17] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_18] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_USERDEF_19] = { .operands={0} },
-[RABBITIZER_INSTR_ID_rsp_MAX] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_INVALID] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN },
-[RABBITIZER_INSTR_ID_r3000gte_RTPS] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_RTPT] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_DPCL] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_DPCS] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_DPCT] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_INTPL] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_NCS] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_NCT] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_NCDS] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_NCDT] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_NCCS] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_NCCT] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_CDP] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_CC] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_NCLIP] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_AVSZ3] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_AVSZ4] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_MVMVA] = { .operands={RAB_OPERAND_r3000gte_sf, RAB_OPERAND_r3000gte_mx, RAB_OPERAND_r3000gte_v, RAB_OPERAND_r3000gte_cv, RAB_OPERAND_r3000gte_lm} },
-[RABBITIZER_INSTR_ID_r3000gte_SQR] = { .operands={RAB_OPERAND_r3000gte_sf} },
-[RABBITIZER_INSTR_ID_r3000gte_OP] = { .operands={RAB_OPERAND_r3000gte_sf} },
-[RABBITIZER_INSTR_ID_r3000gte_GPF] = { .operands={RAB_OPERAND_r3000gte_sf} },
-[RABBITIZER_INSTR_ID_r3000gte_GPL] = { .operands={RAB_OPERAND_r3000gte_sf} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_00] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_01] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_02] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_03] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_04] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_05] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_06] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_07] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_08] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_09] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_10] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_11] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_12] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_13] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_14] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_15] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_16] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_17] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_18] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_USERDEF_19] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r3000gte_MAX] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_INVALID] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN },
-[RABBITIZER_INSTR_ID_r5900_lq] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_r5900_sq] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_r5900_lqc2] = { .operands={RAB_OPERAND_r5900_vft, RAB_OPERAND_cpu_immediate_base}, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_r5900_sqc2] = { .operands={RAB_OPERAND_r5900_vft, RAB_OPERAND_cpu_immediate_base}, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_r5900_sync_p] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_R },
-[RABBITIZER_INSTR_ID_r5900_mult] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_mfsa] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
-[RABBITIZER_INSTR_ID_r5900_mtsa] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_r5900_mtsab] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true },
-[RABBITIZER_INSTR_ID_r5900_mtsah] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true },
-[RABBITIZER_INSTR_ID_r5900_madd] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_maddu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_plzcw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true },
-[RABBITIZER_INSTR_ID_r5900_mfhi1] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
-[RABBITIZER_INSTR_ID_r5900_mthi1] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_r5900_mflo1] = { .operands={RAB_OPERAND_cpu_rd}, .readsRd=true },
-[RABBITIZER_INSTR_ID_r5900_mtlo1] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_r5900_mult1] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_multu1] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_div1] = { .operands={RAB_OPERAND_cpu_zero, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_divu1] = { .operands={RAB_OPERAND_cpu_zero, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_madd1] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_maddu1] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmfhl] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
-[RABBITIZER_INSTR_ID_r5900_pmthl] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_r5900_psllh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psrlh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psrah] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psllw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psrlw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psraw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_paddw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psubw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pcgtw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmaxw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_paddh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psubh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pcgth] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmaxh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_paddb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psubb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pcgtb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_paddsw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psubsw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pextlw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_ppacw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_paddsh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psubsh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pextlh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_ppach] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_paddsb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psubsb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pextlb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_ppacb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pext5] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_ppac5] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pabsw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pceqw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pminw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_padsbh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pabsh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pceqh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pminh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pceqb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_padduw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psubuw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pextuw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_padduh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psubuh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pextuh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_paddub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psubub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pextub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_qfsrv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmaddw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psllvw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psrlvw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmsubw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmfhi] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
-[RABBITIZER_INSTR_ID_r5900_pmflo] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
-[RABBITIZER_INSTR_ID_r5900_pinth] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmultw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pdivw] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pcpyld] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmaddh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_phmadh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pand] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pxor] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmsubh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_phmsbh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pexeh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_prevh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmulth] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pdivbw] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pexew] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_prot3w] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmadduw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_psravw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmthi] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_r5900_pmtlo] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
-[RABBITIZER_INSTR_ID_r5900_pinteh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pmultuw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pdivuw] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pcpyud] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_por] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pnor] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pexch] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pcpyh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_pexcw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_ei] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_di] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_c1__sqrt_s] = { .operands={RAB_OPERAND_cpu_copraw} },
-[RABBITIZER_INSTR_ID_r5900_rsqrt_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_adda_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_suba_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_mula_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_madd_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_msub_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_madda_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_msuba_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_max_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_min_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_c_lt_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_c_le_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
-[RABBITIZER_INSTR_ID_r5900_qmfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs}, .modifiesRt=true },
-[RABBITIZER_INSTR_ID_r5900_cfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis}, .modifiesRt=true },
-[RABBITIZER_INSTR_ID_r5900_qmtc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs}, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_ctc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis}, .readsRt=true },
-[RABBITIZER_INSTR_ID_r5900_bc2f] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .isBranch=true },
-[RABBITIZER_INSTR_ID_r5900_bc2t] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .isBranch=true },
-[RABBITIZER_INSTR_ID_r5900_bc2fl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .isBranch=true, .isBranchLikely=true },
-[RABBITIZER_INSTR_ID_r5900_bc2tl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .isBranch=true, .isBranchLikely=true },
-[RABBITIZER_INSTR_ID_r5900_vaddx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vaddy] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vaddz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vaddw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsuby] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaddx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaddy] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaddz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaddw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsuby] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaxx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaxy] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaxz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaxw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vminix] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vminiy] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vminiz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vminiw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmulx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmuly] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmulz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmulw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmulq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaxi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmuli] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vminii] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vaddq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaddq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vaddi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaddi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vadd] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmadd] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmul] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmax] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsub] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsub] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vopmsub] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmini] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_viadd] = { .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit} },
-[RABBITIZER_INSTR_ID_r5900_visub] = { .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit} },
-[RABBITIZER_INSTR_ID_r5900_viaddi] = { .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_immediate5} },
-[RABBITIZER_INSTR_ID_r5900_viand] = { .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit} },
-[RABBITIZER_INSTR_ID_r5900_vior] = { .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit} },
-[RABBITIZER_INSTR_ID_r5900_vcallms] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_vcallmsr] = { .operands={RAB_OPERAND_r5900_vis} },
-[RABBITIZER_INSTR_ID_r5900_vaddax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vadday] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vaddaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vaddaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubay] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaddax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vmadday] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vmaddaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vmaddaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vmsubax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubay] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vitof0] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vitof4] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vitof12] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vitof15] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vftoi0] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vftoi4] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vftoi12] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vftoi15] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmulax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vmulay] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vmulaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vmulaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vmulaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vabs] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmulai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vclipw] = { .operands={RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vaddaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaddaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vaddai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmaddai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsubai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsubai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vadda] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmadda] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmula] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
-[RABBITIZER_INSTR_ID_r5900_vsuba] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmsuba] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vopmula] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vnop] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_vmove] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vmr32] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vlqi] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vis_postincr}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsqi] = { .operands={RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vit_postincr}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vlqd] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vis_predecr}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vsqd] = { .operands={RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vit_predecr}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vdiv] = { .operands={RAB_OPERAND_r5900_Q, RAB_OPERAND_r5900_vfsl, RAB_OPERAND_r5900_vftm} },
-[RABBITIZER_INSTR_ID_r5900_vsqrt] = { .operands={RAB_OPERAND_r5900_Q, RAB_OPERAND_r5900_vftm} },
-[RABBITIZER_INSTR_ID_r5900_vrsqrt] = { .operands={RAB_OPERAND_r5900_Q, RAB_OPERAND_r5900_vfsl,RAB_OPERAND_r5900_vftm} },
-[RABBITIZER_INSTR_ID_r5900_vwaitq] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_vmtir] = { .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vfsl} },
-[RABBITIZER_INSTR_ID_r5900_vmfir] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vis}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vilwr] = { .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vis}, .isFloat=true, .doesDereference=true, .doesLoad=true },
-[RABBITIZER_INSTR_ID_r5900_viswr] = { .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vis}, .isFloat=true, .doesDereference=true, .doesStore=true },
-[RABBITIZER_INSTR_ID_r5900_vrnext] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_R}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vrget] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_R}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
-[RABBITIZER_INSTR_ID_r5900_vrinit] = { .operands={RAB_OPERAND_r5900_R, RAB_OPERAND_r5900_vfsl} },
-[RABBITIZER_INSTR_ID_r5900_vrxor] = { .operands={RAB_OPERAND_r5900_R, RAB_OPERAND_r5900_vfsl} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_00] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_01] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_02] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_03] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_04] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_05] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_06] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_07] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_08] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_09] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_10] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_11] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_12] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_13] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_14] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_15] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_16] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_17] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_18] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_USERDEF_19] = { .operands={0} },
-[RABBITIZER_INSTR_ID_r5900_MAX] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_INVALID] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate} },
+    [RABBITIZER_INSTR_ID_cpu_j] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true },
+    [RABBITIZER_INSTR_ID_cpu_jal] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_cpu_beq] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_bne] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_beql] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isBranchLikely=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_bnel] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isBranchLikely=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_blez] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_blezl] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isBranchLikely=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_bgtz] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_bgtzl] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isBranchLikely=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_addi] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .notEmittedByCompilers=true, .canBeLo=true },
+    [RABBITIZER_INSTR_ID_cpu_addiu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true },
+    [RABBITIZER_INSTR_ID_cpu_slti] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_sltiu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_andi] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_ori] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true, .canBeLo=true },
+    [RABBITIZER_INSTR_ID_cpu_xori] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_daddi] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true },
+    [RABBITIZER_INSTR_ID_cpu_daddiu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true },
+    [RABBITIZER_INSTR_ID_cpu_lui] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .canBeHi=true },
+    [RABBITIZER_INSTR_ID_cpu_ldl] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_cpu_ldr] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_cpu_lb] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_BYTE },
+    [RABBITIZER_INSTR_ID_cpu_lh] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_SHORT },
+    [RABBITIZER_INSTR_ID_cpu_lwl] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_cpu_lw] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_WORD },
+    [RABBITIZER_INSTR_ID_cpu_lbu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_BYTE, .doesUnsignedMemoryAccess=true },
+    [RABBITIZER_INSTR_ID_cpu_lhu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_SHORT, .doesUnsignedMemoryAccess=true },
+    [RABBITIZER_INSTR_ID_cpu_lwr] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_cpu_lwu] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_WORD, .doesUnsignedMemoryAccess=true },
+    [RABBITIZER_INSTR_ID_cpu_sb] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_BYTE },
+    [RABBITIZER_INSTR_ID_cpu_sh] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_SHORT },
+    [RABBITIZER_INSTR_ID_cpu_swl] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_cpu_sw] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_WORD },
+    [RABBITIZER_INSTR_ID_cpu_sdl] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_cpu_sdr] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_cpu_swr] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_cpu_ll] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .notEmittedByCompilers=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_cpu_pref] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_lld] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .notEmittedByCompilers=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_cpu_ld] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_DOUBLEWORD },
+    [RABBITIZER_INSTR_ID_cpu_sc] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .notEmittedByCompilers=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_cpu_scd] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .notEmittedByCompilers=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_cpu_sd] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_DOUBLEWORD },
+    [RABBITIZER_INSTR_ID_cpu_cache] = { .operands={RAB_OPERAND_cpu_op, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_lwc1] = { .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .isFloat=true, .readsRs=true, .modifiesFt=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_FLOAT },
+    [RABBITIZER_INSTR_ID_cpu_ldc1] = { .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .isFloat=true, .isDouble=true, .readsRs=true, .modifiesFt=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_DOUBLEFLOAT },
+    [RABBITIZER_INSTR_ID_cpu_swc1] = { .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .isFloat=true, .readsRs=true, .readsFt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_FLOAT },
+    [RABBITIZER_INSTR_ID_cpu_sdc1] = { .operands={RAB_OPERAND_cpu_ft, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .isFloat=true, .isDouble=true, .readsRs=true, .readsFt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_DOUBLEFLOAT },
+    [RABBITIZER_INSTR_ID_cpu_lwc2] = { .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_cpu_ldc2] = { .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_cpu_swc2] = { .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_cpu_sdc2] = { .operands={RAB_OPERAND_cpu_cop2t, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_cpu_b] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_cpu_beqz] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .isBranch=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_cpu_bnez] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .isBranch=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_cpu_sll] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_srl] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_sra] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsll] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsrl] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsra] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsll32] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsrl32] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsra32] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsllv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsrlv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsrav] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_sllv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_srlv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_srav] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_mthi] = { .operands={RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .modifiesHI=true },
+    [RABBITIZER_INSTR_ID_cpu_mtlo] = { .operands={RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_jr] = { .operands={RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .isJump=true },
+    [RABBITIZER_INSTR_ID_cpu_jalr] = { .operands={RAB_OPERAND_cpu_maybe_rd_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .isJump=true, .modifiesRd=true, .readsRs=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_cpu_mfhi] = { .operands={RAB_OPERAND_cpu_rd}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsHI=true },
+    [RABBITIZER_INSTR_ID_cpu_mflo] = { .operands={RAB_OPERAND_cpu_rd}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsLO=true },
+    [RABBITIZER_INSTR_ID_cpu_movz] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_movn] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_div] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .readsRd=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_divu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .readsRd=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_sn64_div] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_sn64_divu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_ddiv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .readsRd=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_ddivu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .readsRd=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_add] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_addu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true, .maybeIsMove=true },
+    [RABBITIZER_INSTR_ID_cpu_sub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .notEmittedByCompilers=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_subu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_and] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_or] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .maybeIsMove=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_xor] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_nor] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_slt] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_sltu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dadd] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_daddu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true, .maybeIsMove=true },
+    [RABBITIZER_INSTR_ID_cpu_dsub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_dsubu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_syscall] = { .operands={RAB_OPERAND_cpu_code}, .instrType=RABBITIZER_INSTR_TYPE_R },
+    [RABBITIZER_INSTR_ID_cpu_break] = { .operands={RAB_OPERAND_cpu_code}, .instrType=RABBITIZER_INSTR_TYPE_R },
+    [RABBITIZER_INSTR_ID_cpu_sync] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_R },
+    [RABBITIZER_INSTR_ID_cpu_mult] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_multu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_dmult] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_dmultu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .modifiesHI=true, .modifiesLO=true },
+    [RABBITIZER_INSTR_ID_cpu_tge] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tgeu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tlt] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tltu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_teq] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tne] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_code_lower}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .readsRt=true, .isTrap=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_nop] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_R, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_cpu_move] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .maybeIsMove=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_cpu_not] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_cpu_negu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_cpu_bltz] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_bgez] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_bltzl] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .isBranchLikely=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_bgezl] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .isBranchLikely=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_cpu_tgei] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tgeiu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tlti] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tltiu] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_teqi] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tnei] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isTrap=true, .readsRs=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_bltzal] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .readsRs=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_cpu_bgezal] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .readsRs=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_cpu_bltzall] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .isBranchLikely=true, .readsRs=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_cpu_bgezall] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .isBranchLikely=true, .readsRs=true, .notEmittedByCompilers=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_cpu_bal] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .notEmittedByCompilers=true, .doesLink=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_cpu_mfc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .modifiesRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_dmfc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .modifiesRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_cfc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .modifiesRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_mtc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .readsRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_dmtc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .readsRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_ctc0] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .readsRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_bc0f] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true },
+    [RABBITIZER_INSTR_ID_cpu_bc0t] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true },
+    [RABBITIZER_INSTR_ID_cpu_bc0fl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true, .isBranchLikely=true },
+    [RABBITIZER_INSTR_ID_cpu_bc0tl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true, .isBranchLikely=true },
+    [RABBITIZER_INSTR_ID_cpu_tlbr] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tlbwi] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_tlbwr] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN },
+    [RABBITIZER_INSTR_ID_cpu_tlbp] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_eret] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_cpu_mfc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesRt=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_dmfc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesRt=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_mtc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsRt=true, .modifiesFs=true },
+    [RABBITIZER_INSTR_ID_cpu_dmtc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsRt=true, .modifiesFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cfc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop1cs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesRt=true },
+    [RABBITIZER_INSTR_ID_cpu_ctc1] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop1cs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_bc1f] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true },
+    [RABBITIZER_INSTR_ID_cpu_bc1t] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true },
+    [RABBITIZER_INSTR_ID_cpu_bc1fl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true, .isBranchLikely=true },
+    [RABBITIZER_INSTR_ID_cpu_bc1tl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isBranch=true, .isBranchLikely=true },
+    [RABBITIZER_INSTR_ID_cpu_add_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_sub_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_mul_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_div_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_sqrt_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_abs_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_mov_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_neg_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_round_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_trunc_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_ceil_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_floor_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_round_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_trunc_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_ceil_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_floor_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_d_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_w_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_l_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_c_f_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_un_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_eq_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ueq_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_olt_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ult_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ole_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ule_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_sf_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ngle_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_seq_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ngl_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_lt_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_nge_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_le_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ngt_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_add_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_sub_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_mul_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_div_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_sqrt_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_abs_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_mov_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_neg_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_round_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_trunc_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_ceil_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_floor_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_round_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_trunc_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_ceil_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_floor_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_s_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_w_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_l_d] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_c_f_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_un_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_eq_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ueq_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_olt_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ult_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ole_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ule_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_df_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ngle_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_deq_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ngl_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_lt_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_nge_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_le_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_c_ngt_d] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_s_w] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_d_w] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_s_l] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_cvt_d_l] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .isFloat=true, .isDouble=true, .modifiesFd=true, .readsFs=true },
+    [RABBITIZER_INSTR_ID_cpu_mfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd}, .modifiesRt=true },
+    [RABBITIZER_INSTR_ID_cpu_mtc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd}, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_cfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd}, .modifiesRt=true },
+    [RABBITIZER_INSTR_ID_cpu_ctc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_cop2cd}, .readsRt=true },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_00] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_01] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_02] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_03] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_04] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_05] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_06] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_07] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_08] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_09] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_10] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_11] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_12] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_13] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_14] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_15] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_16] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_17] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_18] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_USERDEF_19] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_cpu_MAX] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_INVALID] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_mfc2] = { .operands={RAB_OPERAND_rsp_cop2t, RAB_OPERAND_rsp_vs_index} },
+    [RABBITIZER_INSTR_ID_rsp_mtc2] = { .operands={RAB_OPERAND_rsp_cop2t, RAB_OPERAND_rsp_vs_index} },
+    [RABBITIZER_INSTR_ID_rsp_cfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_rsp_cop2cd}, .modifiesRt=true },
+    [RABBITIZER_INSTR_ID_rsp_ctc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_rsp_cop2cd}, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_vmulf] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmulu] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vrndp] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmulq] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmudl] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmudm] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmudn] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmudh] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmacf] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmacu] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vrndn] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmacq] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmadl] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmadm] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmadn] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmadh] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vadd] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vsub] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vabs] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vaddc] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vsubc] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vsar] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vand] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vnand] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vor] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vnor] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vxor] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vnxor] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vlt] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_veq] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vne] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vge] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vcl] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vch] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vcr] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmrg] = { .operands={RAB_OPERAND_rsp_vd, RAB_OPERAND_rsp_vs, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vrcp] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vrcpl] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vrcph] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vmov] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vrsq] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vrsql] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vrsqh] = { .operands={RAB_OPERAND_rsp_vd_de, RAB_OPERAND_rsp_vt_elementhigh} },
+    [RABBITIZER_INSTR_ID_rsp_vnop] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_lbv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_lsv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_llv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_ldv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_lqv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_lrv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_lpv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_luv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_lhv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_lfv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_ltv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_sbv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_ssv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_slv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_sdv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_sqv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_srv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_spv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_suv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_shv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_sfv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_stv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_swv] = { .operands={RAB_OPERAND_rsp_vt_elementlow, RAB_OPERAND_rsp_offset_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_j] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true },
+    [RABBITIZER_INSTR_ID_rsp_jal] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_rsp_beq] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .readsRt=true, .isBranch=true },
+    [RABBITIZER_INSTR_ID_rsp_bne] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .readsRt=true, .isBranch=true },
+    [RABBITIZER_INSTR_ID_rsp_blez] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
+    [RABBITIZER_INSTR_ID_rsp_bgtz] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
+    [RABBITIZER_INSTR_ID_rsp_addi] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .notEmittedByCompilers=true, .canBeLo=true },
+    [RABBITIZER_INSTR_ID_rsp_addiu] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true },
+    [RABBITIZER_INSTR_ID_rsp_slti] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_sltiu] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_andi] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_ori] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true, .canBeLo=true },
+    [RABBITIZER_INSTR_ID_rsp_xori] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_rsp_lui] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_I, .isUnsigned=true, .modifiesRt=true, .canBeHi=true },
+    [RABBITIZER_INSTR_ID_rsp_lb] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_BYTE },
+    [RABBITIZER_INSTR_ID_rsp_lh] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_SHORT },
+    [RABBITIZER_INSTR_ID_rsp_lw] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_WORD },
+    [RABBITIZER_INSTR_ID_rsp_lbu] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_BYTE, .doesUnsignedMemoryAccess=true },
+    [RABBITIZER_INSTR_ID_rsp_lhu] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true, .accessType=RAB_ACCESSTYPE_SHORT, .doesUnsignedMemoryAccess=true },
+    [RABBITIZER_INSTR_ID_rsp_sb] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_BYTE },
+    [RABBITIZER_INSTR_ID_rsp_sh] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_SHORT },
+    [RABBITIZER_INSTR_ID_rsp_sw] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true, .accessType=RAB_ACCESSTYPE_WORD },
+    [RABBITIZER_INSTR_ID_rsp_pref] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_b] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true },
+    [RABBITIZER_INSTR_ID_rsp_beqz] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
+    [RABBITIZER_INSTR_ID_rsp_bnez] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
+    [RABBITIZER_INSTR_ID_rsp_sll] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_srl] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_sra] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_cpu_sa}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_sllv] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_srlv] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_srav] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_jr] = { .operands={RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .readsRs=true, .isJump=true },
+    [RABBITIZER_INSTR_ID_rsp_jalr] = { .operands={RAB_OPERAND_rsp_maybe_rd_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .isJump=true, .modifiesRd=true, .readsRs=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_rsp_movz] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_movn] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_add] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_rsp_addu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_sub] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .notEmittedByCompilers=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_subu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_and] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_or] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_xor] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_nor] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_slt] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_sltu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_rsp_break] = { .operands={RAB_OPERAND_cpu_code}, .instrType=RABBITIZER_INSTR_TYPE_R },
+    [RABBITIZER_INSTR_ID_rsp_nop] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_R, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_rsp_move] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_rsp_not] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rs}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_rsp_negu] = { .operands={RAB_OPERAND_rsp_rd, RAB_OPERAND_rsp_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRt=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_rsp_bltz] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
+    [RABBITIZER_INSTR_ID_rsp_bgez] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true },
+    [RABBITIZER_INSTR_ID_rsp_bltzal] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_rsp_bgezal] = { .operands={RAB_OPERAND_rsp_rs, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true, .isBranch=true, .notEmittedByCompilers=true, .doesLink=true },
+    [RABBITIZER_INSTR_ID_rsp_bal] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .isBranch=true, .notEmittedByCompilers=true, .doesLink=true, .isPseudo=true },
+    [RABBITIZER_INSTR_ID_rsp_mfc0] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .modifiesRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_rsp_mtc0] = { .operands={RAB_OPERAND_rsp_rt, RAB_OPERAND_rsp_cop0d}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN, .readsRt=true, .notEmittedByCompilers=true },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_00] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_01] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_02] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_03] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_04] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_05] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_06] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_07] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_08] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_09] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_10] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_11] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_12] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_13] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_14] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_15] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_16] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_17] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_18] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_USERDEF_19] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_rsp_MAX] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_INVALID] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN },
+    [RABBITIZER_INSTR_ID_r3000gte_RTPS] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_RTPT] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_DPCL] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_DPCS] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_DPCT] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_INTPL] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_NCS] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_NCT] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_NCDS] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_NCDT] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_NCCS] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_NCCT] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_CDP] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_CC] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_NCLIP] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_AVSZ3] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_AVSZ4] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_MVMVA] = { .operands={RAB_OPERAND_r3000gte_sf, RAB_OPERAND_r3000gte_mx, RAB_OPERAND_r3000gte_v, RAB_OPERAND_r3000gte_cv, RAB_OPERAND_r3000gte_lm} },
+    [RABBITIZER_INSTR_ID_r3000gte_SQR] = { .operands={RAB_OPERAND_r3000gte_sf} },
+    [RABBITIZER_INSTR_ID_r3000gte_OP] = { .operands={RAB_OPERAND_r3000gte_sf} },
+    [RABBITIZER_INSTR_ID_r3000gte_GPF] = { .operands={RAB_OPERAND_r3000gte_sf} },
+    [RABBITIZER_INSTR_ID_r3000gte_GPL] = { .operands={RAB_OPERAND_r3000gte_sf} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_00] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_01] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_02] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_03] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_04] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_05] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_06] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_07] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_08] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_09] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_10] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_11] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_12] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_13] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_14] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_15] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_16] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_17] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_18] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_USERDEF_19] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r3000gte_MAX] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_INVALID] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_UNKNOWN },
+    [RABBITIZER_INSTR_ID_r5900_lq] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .modifiesRt=true, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_r5900_sq] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate_base}, .instrType=RABBITIZER_INSTR_TYPE_I, .readsRs=true, .readsRt=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_r5900_lqc2] = { .operands={RAB_OPERAND_r5900_vft, RAB_OPERAND_cpu_immediate_base}, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_r5900_sqc2] = { .operands={RAB_OPERAND_r5900_vft, RAB_OPERAND_cpu_immediate_base}, .readsRs=true, .canBeLo=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_r5900_sync_p] = { .operands={0}, .instrType=RABBITIZER_INSTR_TYPE_R },
+    [RABBITIZER_INSTR_ID_r5900_mult] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .instrType=RABBITIZER_INSTR_TYPE_R, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_mfsa] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
+    [RABBITIZER_INSTR_ID_r5900_mtsa] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_r5900_mtsab] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true },
+    [RABBITIZER_INSTR_ID_r5900_mtsah] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_immediate}, .instrType=RABBITIZER_INSTR_TYPE_REGIMM, .readsRs=true },
+    [RABBITIZER_INSTR_ID_r5900_madd] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_maddu] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_plzcw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true },
+    [RABBITIZER_INSTR_ID_r5900_mfhi1] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
+    [RABBITIZER_INSTR_ID_r5900_mthi1] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_r5900_mflo1] = { .operands={RAB_OPERAND_cpu_rd}, .readsRd=true },
+    [RABBITIZER_INSTR_ID_r5900_mtlo1] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_r5900_mult1] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_multu1] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_div1] = { .operands={RAB_OPERAND_cpu_zero, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_divu1] = { .operands={RAB_OPERAND_cpu_zero, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_madd1] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_maddu1] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmfhl] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
+    [RABBITIZER_INSTR_ID_r5900_pmthl] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_r5900_psllh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psrlh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psrah] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psllw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psrlw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psraw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_sa}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_paddw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psubw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pcgtw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmaxw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_paddh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psubh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pcgth] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmaxh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_paddb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psubb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pcgtb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_paddsw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psubsw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pextlw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_ppacw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_paddsh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psubsh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pextlh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_ppach] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_paddsb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psubsb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pextlb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_ppacb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pext5] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_ppac5] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pabsw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pceqw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pminw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_padsbh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pabsh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pceqh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pminh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pceqb] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_padduw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psubuw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pextuw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_padduh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psubuh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pextuh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_paddub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psubub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pextub] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_qfsrv] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmaddw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psllvw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psrlvw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmsubw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmfhi] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
+    [RABBITIZER_INSTR_ID_r5900_pmflo] = { .operands={RAB_OPERAND_cpu_rd}, .modifiesRd=true },
+    [RABBITIZER_INSTR_ID_r5900_pinth] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmultw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pdivw] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pcpyld] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmaddh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_phmadh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pand] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pxor] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmsubh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_phmsbh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pexeh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_prevh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmulth] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pdivbw] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pexew] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_prot3w] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmadduw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_psravw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_rs}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmthi] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_r5900_pmtlo] = { .operands={RAB_OPERAND_cpu_rs}, .readsRs=true },
+    [RABBITIZER_INSTR_ID_r5900_pinteh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pmultuw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pdivuw] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pcpyud] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_por] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pnor] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRs=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pexch] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pcpyh] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_pexcw] = { .operands={RAB_OPERAND_cpu_rd, RAB_OPERAND_cpu_rt}, .modifiesRd=true, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_ei] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_di] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_c1__sqrt_s] = { .operands={RAB_OPERAND_cpu_copraw} },
+    [RABBITIZER_INSTR_ID_r5900_rsqrt_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_adda_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_suba_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_mula_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_madd_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_msub_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_madda_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_msuba_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_max_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_min_s] = { .operands={RAB_OPERAND_cpu_fd, RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .modifiesFd=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_c_lt_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_c_le_s] = { .operands={RAB_OPERAND_cpu_fs, RAB_OPERAND_cpu_ft}, .isFloat=true, .readsFs=true, .readsFt=true },
+    [RABBITIZER_INSTR_ID_r5900_qmfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs}, .modifiesRt=true },
+    [RABBITIZER_INSTR_ID_r5900_cfc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis}, .modifiesRt=true },
+    [RABBITIZER_INSTR_ID_r5900_qmtc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vfs}, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_ctc2] = { .operands={RAB_OPERAND_cpu_rt, RAB_OPERAND_r5900_vis}, .readsRt=true },
+    [RABBITIZER_INSTR_ID_r5900_bc2f] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .isBranch=true },
+    [RABBITIZER_INSTR_ID_r5900_bc2t] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .isBranch=true },
+    [RABBITIZER_INSTR_ID_r5900_bc2fl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .isBranch=true, .isBranchLikely=true },
+    [RABBITIZER_INSTR_ID_r5900_bc2tl] = { .operands={RAB_OPERAND_cpu_branch_target_label}, .isBranch=true, .isBranchLikely=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddy] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsuby] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaddx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaddy] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaddz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaddw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsuby] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaxx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaxy] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaxz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaxw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vminix] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vminiy] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vminiz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vminiw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmulx] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmuly] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmulz] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmulw] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmulq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaxi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmuli] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vminii] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaddq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaddi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubq] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubi] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vadd] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmadd] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmul] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmax] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsub] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsub] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vopmsub] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmini] = { .operands={RAB_OPERAND_r5900_vfdxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_viadd] = { .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit} },
+    [RABBITIZER_INSTR_ID_r5900_visub] = { .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit} },
+    [RABBITIZER_INSTR_ID_r5900_viaddi] = { .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_immediate5} },
+    [RABBITIZER_INSTR_ID_r5900_viand] = { .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit} },
+    [RABBITIZER_INSTR_ID_r5900_vior] = { .operands={RAB_OPERAND_r5900_vid, RAB_OPERAND_r5900_vis, RAB_OPERAND_r5900_vit} },
+    [RABBITIZER_INSTR_ID_r5900_vcallms] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_vcallmsr] = { .operands={RAB_OPERAND_r5900_vis} },
+    [RABBITIZER_INSTR_ID_r5900_vaddax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vadday] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubay] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaddax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vmadday] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vmaddaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vmaddaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vmsubax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubay] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vitof0] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vitof4] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vitof12] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vitof15] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vftoi0] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vftoi4] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vftoi12] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vftoi15] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmulax] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vmulay] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vmulaz] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vmulaw] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vmulaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vabs] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmulai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vclipw] = { .operands={RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftn}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaddaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vaddai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmaddai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubaq] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_Q}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsubai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsubai] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_I}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vadda] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmadda] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmula] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw },
+    [RABBITIZER_INSTR_ID_r5900_vsuba] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmsuba] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vopmula] = { .operands={RAB_OPERAND_r5900_ACCxyzw, RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vftxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vnop] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_vmove] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vmr32] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vfsxyzw}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vlqi] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vis_postincr}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsqi] = { .operands={RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vit_postincr}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vlqd] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vis_predecr}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vsqd] = { .operands={RAB_OPERAND_r5900_vfsxyzw, RAB_OPERAND_r5900_vit_predecr}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vdiv] = { .operands={RAB_OPERAND_r5900_Q, RAB_OPERAND_r5900_vfsl, RAB_OPERAND_r5900_vftm} },
+    [RABBITIZER_INSTR_ID_r5900_vsqrt] = { .operands={RAB_OPERAND_r5900_Q, RAB_OPERAND_r5900_vftm} },
+    [RABBITIZER_INSTR_ID_r5900_vrsqrt] = { .operands={RAB_OPERAND_r5900_Q, RAB_OPERAND_r5900_vfsl,RAB_OPERAND_r5900_vftm} },
+    [RABBITIZER_INSTR_ID_r5900_vwaitq] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_vmtir] = { .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vfsl} },
+    [RABBITIZER_INSTR_ID_r5900_vmfir] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_vis}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vilwr] = { .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vis}, .isFloat=true, .doesDereference=true, .doesLoad=true },
+    [RABBITIZER_INSTR_ID_r5900_viswr] = { .operands={RAB_OPERAND_r5900_vit, RAB_OPERAND_r5900_vis}, .isFloat=true, .doesDereference=true, .doesStore=true },
+    [RABBITIZER_INSTR_ID_r5900_vrnext] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_R}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vrget] = { .operands={RAB_OPERAND_r5900_vftxyzw, RAB_OPERAND_r5900_R}, .instrSuffix=RABINSTRSUFFIX_R5900_xyzw, .isFloat=true },
+    [RABBITIZER_INSTR_ID_r5900_vrinit] = { .operands={RAB_OPERAND_r5900_R, RAB_OPERAND_r5900_vfsl} },
+    [RABBITIZER_INSTR_ID_r5900_vrxor] = { .operands={RAB_OPERAND_r5900_R, RAB_OPERAND_r5900_vfsl} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_00] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_01] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_02] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_03] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_04] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_05] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_06] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_07] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_08] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_09] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_10] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_11] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_12] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_13] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_14] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_15] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_16] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_17] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_18] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_USERDEF_19] = { .operands={0} },
+    [RABBITIZER_INSTR_ID_r5900_MAX] = { .operands={0} },
 };
 
 #endif
```

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstrCategory.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstrCategory.c`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 #include <string.h>
 
 #include "InstrCategory_Names_array.table.h"
 
 RabbitizerInstrCategory RabbitizerInstrCategory_fromStr(const char *name) {
     if (name == NULL) {
-        return -2;
+        return (RabbitizerInstrCategory)-2;
     }
 
-    for (size_t i = 0; i < RABBITIZER_INSTRCAT_MAX; i++) {
+    for (RabbitizerInstrCategory i = 0; i < RABBITIZER_INSTRCAT_MAX; i++) {
         if (strcmp(RabbitizerInstrCategory_Names[i], name) == 0) {
             return i;
         }
     }
 
-    return -1;
+    return (RabbitizerInstrCategory)-1;
 }
```

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstrDescriptor.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstrDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstrId.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstrId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstrSuffix.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstrSuffix.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerRegister.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerRegister.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RabbitizerRegisterDescriptor.c` & `rabbitizer-1.7.1/src/instructions/RabbitizerRegisterDescriptor.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h` & `rabbitizer-1.7.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template` & `rabbitizer-1.7.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/Registers_Names_arrays.table.h` & `rabbitizer-1.7.1/src/instructions/Registers_Names_arrays.table.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.0/src/instructions/Registers_Names_arrays.table.template` & `rabbitizer-1.7.1/src/instructions/Registers_Names_arrays.table.template`

 * *Files identical despite different names*

