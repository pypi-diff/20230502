# Comparing `tmp/systemID-24.8.tar.gz` & `tmp/systemID-24.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systemID-24.8.tar", last modified: Tue Feb  7 22:49:16 2023, max compression
+gzip compressed data, was "systemID-24.9.tar", last modified: Tue Feb  7 23:13:22 2023, max compression
```

## Comparing `systemID-24.8.tar` & `systemID-24.9.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.838022 systemID-24.8/
--rw-r--r--   0 damiengueho   (501) staff       (20)      763 2023-02-07 22:49:16.837792 systemID-24.8/PKG-INFO
--rw-r--r--   0 damiengueho   (501) staff       (20)       38 2023-02-07 22:49:16.838147 systemID-24.8/setup.cfg
--rw-r--r--   0 damiengueho   (501) staff       (20)     1605 2023-02-07 22:48:34.000000 systemID-24.8/setup.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.789562 systemID-24.8/systemID/
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.800495 systemID-24.8/systemID/ClassesDynamics/
--rw-r--r--   0 damiengueho   (501) staff       (20)     2635 2023-02-07 20:15:31.000000 systemID-24.8/systemID/ClassesDynamics/ClassAutomobileCruiseControlDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4896 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassAutomobileSystemDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2558 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassBallAndBeamDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     6760 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassCircularRestrictedThreeBodyProblemDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      588 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassCustomizedDiscreteTimeInvariantDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3500 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassDCMotorDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    20095 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassDuffingOscillatorDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2475 2023-02-07 20:15:31.000000 systemID-24.8/systemID/ClassesDynamics/ClassFiniteElementTypeOscillatorChainDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     7135 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassFlutterAeroelasticWingDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5953 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassFreeThreeMassSpringDamperDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4131 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassInterceptProblemDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3569 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassInvertedPendulumDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3685 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassLorenzSystemDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5470 2023-02-07 20:15:31.000000 systemID-24.8/systemID/ClassesDynamics/ClassMassSpringDamperDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1140 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassOscillatorySystemZeroDampingDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    10908 2023-02-07 20:15:31.000000 systemID-24.8/systemID/ClassesDynamics/ClassPanelFlutterDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1532 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassPointMassInRotatingTubeDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2594 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassSlowManifoldDecoupledSystemDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1072 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassSystemWithAStableOriginDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5579 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassThreeMassSpringDamperDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     7834 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassTwoBodyProblemDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4349 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassTwoMassSpringDamperDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2476 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesDynamics/ClassVanDerPolOscillatorDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.8/systemID/ClassesDynamics/__init__.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.801768 systemID-24.8/systemID/ClassesGeneral/
--rw-r--r--   0 damiengueho   (501) staff       (20)     2516 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesGeneral/ClassExperiments.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    11747 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesGeneral/ClassSignal.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4344 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesGeneral/ClassSystem.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.8/systemID/ClassesGeneral/__init__.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.802270 systemID-24.8/systemID/ClassesSparseID/
--rw-r--r--   0 damiengueho   (501) staff       (20)     3668 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesSparseID/ClassSparseApproximation.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2021-11-12 18:54:37.000000 systemID-24.8/systemID/ClassesSparseID/__init__.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.803582 systemID-24.8/systemID/ClassesSystemID/
--rw-r--r--   0 damiengueho   (501) staff       (20)     1644 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesSystemID/ClassBilinear.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4836 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesSystemID/ClassERA.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3437 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesSystemID/ClassMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      446 2023-02-07 20:15:32.000000 systemID-24.8/systemID/ClassesSystemID/ClassQMarkov.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.8/systemID/ClassesSystemID/__init__.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.804909 systemID-24.8/systemID/Plotting/
--rw-r--r--   0 damiengueho   (501) staff       (20)     2315 2023-02-07 20:15:32.000000 systemID-24.8/systemID/Plotting/PlotEigenValues.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      993 2023-02-07 20:15:32.000000 systemID-24.8/systemID/Plotting/PlotMarkovParameters2.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1175 2023-02-07 20:15:32.000000 systemID-24.8/systemID/Plotting/PlotSignals.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      750 2023-02-07 20:15:32.000000 systemID-24.8/systemID/Plotting/PlotSingularValues.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.8/systemID/Plotting/__init__.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.808724 systemID-24.8/systemID/SparseIDAlgorithms/
--rw-r--r--   0 damiengueho   (501) staff       (20)     3227 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/GeneratePolynomialBasisFunctions.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4620 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/GeneratePolynomialIndex.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      819 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/NormalizeSignals.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     6328 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    18012 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation1stOrder.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     8017 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    14388 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     9204 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem_polar.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    16894 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem_v2.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     9024 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2ndOrder.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      140 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation3rdOrder.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     6630 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation_v2.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2021-11-12 18:54:37.000000 systemID-24.8/systemID/SparseIDAlgorithms/__init__.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.824126 systemID-24.8/systemID/SystemIDAlgorithms/
--rw-r--r--   0 damiengueho   (501) staff       (20)    10567 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/BilinearSystemID.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1195 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/CalculateNaturalFrequenciesAndDampingRatios.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1497 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/ComputeStatisticalMoments.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3402 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/CorrectSystemForEigenvaluesCheck.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4921 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/CreateAugmentedSignal.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    12540 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/DepartureDynamics.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      770 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/DynamicModeDecompositionAlgorithm.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5485 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithm.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5991 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmFromInitialConditionResponse.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     6424 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmWithDataCorrelation.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     7056 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmWithDataCorrelationFromInitialConditionResponse.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      642 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetCovarianceMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2535 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetDeltaMatrix.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1399 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetInitialConditionResponseMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1253 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetMACandMSV.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1550 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4513 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetMarkovParametersFromFrequencyResponseFunctions.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1741 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetMarkovParametersFromObserverControllerMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1709 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetMarkovParametersFromObserverMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2069 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetObservabilityMatrix.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1812 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetObserverGainMarkovParametersFromObserverMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1027 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetObserverGainMatrix.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1024 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetObserverMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1597 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetOptimizedHankelMatrixSize.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1470 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetPowerOf2.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1747 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetTVMarkovParametersFromTVObserverMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1559 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetTVObserverGainMarkovParametersFromTVObserverMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4740 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetTimeVaryingMarkovParameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1207 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/GetTimeVaryingObserverGainMatrix.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5707 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/HigherOrderMomentsPropagation.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    20238 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/HigherOrderStateTransitionTensorsPropagation.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2639 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/IdentificationInitialCondition.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1373 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/Integrate.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     7752 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/ObserverControllerKalmanIdentificationAlgorithmWithObserver.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     6826 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/ObserverKalmanIdentificationAlgorithm.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     7207 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/ObserverKalmanIdentificationAlgorithmWithObserver.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4724 2022-09-08 23:56:43.000000 systemID-24.8/systemID/SystemIDAlgorithms/ParticleSwarmOptimization.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    12826 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/Prediction.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    27483 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/Propagation.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2569 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/QMarkovCover.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     7437 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithm.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4798 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmFromInitialConditionResponse.py
--rw-r--r--   0 damiengueho   (501) staff       (20)    12377 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmWithDataCorrelation.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5772 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmWithDataCorrelationFromInitialConditionResponse.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3654 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingObserverKalmanIdentificationAlgorithmWithObserver.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3739 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/WeightingSequenceDescription.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1004 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmFull.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1398 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmObserver.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1418 2023-02-07 20:15:31.000000 systemID-24.8/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmObserverFull.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1594 2023-02-07 20:15:32.000000 systemID-24.8/systemID/SystemIDAlgorithms/ZZZTimeVaryingObserverKalmanIdentificationAlgorithmObserver.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.8/systemID/SystemIDAlgorithms/__init__.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      223 2023-02-07 22:45:02.000000 systemID-24.8/systemID/__init__.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.824333 systemID-24.8/systemID/dynamics/
--rw-r--r--   0 damiengueho   (501) staff       (20)       15 2023-02-07 22:23:56.000000 systemID-24.8/systemID/dynamics/__init__.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.830481 systemID-24.8/systemID/functions/
--rw-r--r--   0 damiengueho   (501) staff       (20)       57 2023-02-07 22:48:07.000000 systemID-24.8/systemID/functions/__init__.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5436 2023-02-07 20:14:46.000000 systemID-24.8/systemID/functions/eigensystem_realization_algorithm.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5630 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/eigensystem_realization_algorithm_from_initial_condition_response.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     6374 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/eigensystem_realization_algorithm_with_data_correlation.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     6703 2023-02-07 20:14:46.000000 systemID-24.8/systemID/functions/eigensystem_realization_algorithm_with_data_correlation_from_initial_condition_response.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1216 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/mac_and_msv.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1680 2023-02-07 20:14:48.000000 systemID-24.8/systemID/functions/markov_parameters_from_observer_markov_parameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1785 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/observer_gain_markov_parameters_from_observer_markov_parameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     6706 2023-02-07 20:14:48.000000 systemID-24.8/systemID/functions/observer_kalman_identification_algorithm.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     7176 2023-02-07 20:14:48.000000 systemID-24.8/systemID/functions/observer_kalman_identification_algorithm_with_observer.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3191 2023-02-07 20:14:46.000000 systemID-24.8/systemID/functions/polynomial_basis_functions.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4582 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/polynomial_index.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      120 2022-12-06 03:38:29.000000 systemID-24.8/systemID/functions/test.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      148 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/time_invariant_koopman_operator.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     5417 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/time_varying_eigensystem_realization_algorithm.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     4085 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/time_varying_eigensystem_realization_algorithm_from_initial_condition_response.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1740 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/time_varying_markov_parameters_from_time_varying_observer_markov_parameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1554 2023-02-07 20:14:47.000000 systemID-24.8/systemID/functions/time_varying_observer_gain_markov_parameters_from_time_varying_observer_markov_parameters.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3744 2023-02-07 20:14:48.000000 systemID-24.8/systemID/functions/time_varying_observer_kalman_identification_algorithm_with_observer.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.832191 systemID-24.8/systemID/input_output_identification/
--rw-r--r--   0 damiengueho   (501) staff       (20)       15 2023-02-07 22:23:43.000000 systemID-24.8/systemID/input_output_identification/__init__.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3220 2022-12-10 04:18:38.000000 systemID-24.8/systemID/input_output_identification/autoregressive_identification.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     3236 2022-12-09 03:09:22.000000 systemID-24.8/systemID/input_output_identification/autoregressive_with_exogeneous_input_identification.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1923 2023-02-07 20:14:46.000000 systemID-24.8/systemID/input_output_identification/time_invariant.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      533 2023-02-07 20:14:47.000000 systemID-24.8/systemID/input_output_identification/time_varying.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.834836 systemID-24.8/systemID/input_output_model/
--rw-r--r--   0 damiengueho   (501) staff       (20)       15 2023-02-07 22:23:35.000000 systemID-24.8/systemID/input_output_model/__init__.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:24:17.000000 systemID-24.8/systemID/input_output_model/autoregressive_integrated_moving_average_model.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:24:30.000000 systemID-24.8/systemID/input_output_model/autoregressive_integrated_moving_average_with_exogeneous_input_model.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      777 2023-02-06 21:08:45.000000 systemID-24.8/systemID/input_output_model/autoregressive_model.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:23:32.000000 systemID-24.8/systemID/input_output_model/autoregressive_moving_average_model.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:23:46.000000 systemID-24.8/systemID/input_output_model/autoregressive_moving_average_with_exogeneous_input_model.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1117 2023-02-06 21:08:45.000000 systemID-24.8/systemID/input_output_model/autoregressive_with_exogeneous_input_model.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:24:47.000000 systemID-24.8/systemID/input_output_model/volterra_series_model.py
--rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:24:59.000000 systemID-24.8/systemID/input_output_model/volterra_series_with_exogeneous_input_model.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.835590 systemID-24.8/systemID/signals/
--rw-r--r--   0 damiengueho   (501) staff       (20)       50 2023-02-07 22:47:53.000000 systemID-24.8/systemID/signals/__init__.py
--rw-r--r--   0 damiengueho   (501) staff       (20)      267 2023-02-07 20:14:47.000000 systemID-24.8/systemID/signals/continuous.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1229 2023-02-07 22:26:36.000000 systemID-24.8/systemID/signals/discrete.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.836393 systemID-24.8/systemID/state_space_identification/
--rw-r--r--   0 damiengueho   (501) staff       (20)       15 2023-02-07 22:23:17.000000 systemID-24.8/systemID/state_space_identification/__init__.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2796 2023-02-07 20:14:47.000000 systemID-24.8/systemID/state_space_identification/time_invariant.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2244 2023-02-07 20:14:47.000000 systemID-24.8/systemID/state_space_identification/time_varying.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.837442 systemID-24.8/systemID/state_space_model/
--rw-r--r--   0 damiengueho   (501) staff       (20)       15 2023-02-07 22:23:09.000000 systemID-24.8/systemID/state_space_model/__init__.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     2896 2023-02-07 20:14:47.000000 systemID-24.8/systemID/state_space_model/continuous.py
--rw-r--r--   0 damiengueho   (501) staff       (20)     1509 2023-02-07 20:14:47.000000 systemID-24.8/systemID/state_space_model/discrete.py
-drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 22:49:16.793104 systemID-24.8/systemID.egg-info/
--rw-r--r--   0 damiengueho   (501) staff       (20)      763 2023-02-07 22:49:16.000000 systemID-24.8/systemID.egg-info/PKG-INFO
--rw-r--r--   0 damiengueho   (501) staff       (20)     9244 2023-02-07 22:49:16.000000 systemID-24.8/systemID.egg-info/SOURCES.txt
--rw-r--r--   0 damiengueho   (501) staff       (20)        1 2023-02-07 22:49:16.000000 systemID-24.8/systemID.egg-info/dependency_links.txt
--rw-r--r--   0 damiengueho   (501) staff       (20)       23 2023-02-07 22:49:16.000000 systemID-24.8/systemID.egg-info/requires.txt
--rw-r--r--   0 damiengueho   (501) staff       (20)        9 2023-02-07 22:49:16.000000 systemID-24.8/systemID.egg-info/top_level.txt
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.494742 systemID-24.9/
+-rw-r--r--   0 damiengueho   (501) staff       (20)      763 2023-02-07 23:13:22.494452 systemID-24.9/PKG-INFO
+-rw-r--r--   0 damiengueho   (501) staff       (20)       38 2023-02-07 23:13:22.494827 systemID-24.9/setup.cfg
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1605 2023-02-07 23:12:03.000000 systemID-24.9/setup.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.441858 systemID-24.9/systemID/
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.451335 systemID-24.9/systemID/ClassesDynamics/
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2635 2023-02-07 20:15:31.000000 systemID-24.9/systemID/ClassesDynamics/ClassAutomobileCruiseControlDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4896 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassAutomobileSystemDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2558 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassBallAndBeamDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     6760 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassCircularRestrictedThreeBodyProblemDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      588 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassCustomizedDiscreteTimeInvariantDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3500 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassDCMotorDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    20095 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassDuffingOscillatorDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2475 2023-02-07 20:15:31.000000 systemID-24.9/systemID/ClassesDynamics/ClassFiniteElementTypeOscillatorChainDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     7135 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassFlutterAeroelasticWingDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5953 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassFreeThreeMassSpringDamperDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4131 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassInterceptProblemDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3569 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassInvertedPendulumDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3685 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassLorenzSystemDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5470 2023-02-07 20:15:31.000000 systemID-24.9/systemID/ClassesDynamics/ClassMassSpringDamperDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1140 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassOscillatorySystemZeroDampingDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    10908 2023-02-07 20:15:31.000000 systemID-24.9/systemID/ClassesDynamics/ClassPanelFlutterDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1532 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassPointMassInRotatingTubeDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2594 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassSlowManifoldDecoupledSystemDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1072 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassSystemWithAStableOriginDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5579 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassThreeMassSpringDamperDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     7834 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassTwoBodyProblemDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4349 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassTwoMassSpringDamperDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2476 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesDynamics/ClassVanDerPolOscillatorDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.9/systemID/ClassesDynamics/__init__.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.452516 systemID-24.9/systemID/ClassesGeneral/
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2516 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesGeneral/ClassExperiments.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    11747 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesGeneral/ClassSignal.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4344 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesGeneral/ClassSystem.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.9/systemID/ClassesGeneral/__init__.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.453492 systemID-24.9/systemID/ClassesSparseID/
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3668 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesSparseID/ClassSparseApproximation.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2021-11-12 18:54:37.000000 systemID-24.9/systemID/ClassesSparseID/__init__.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.455891 systemID-24.9/systemID/ClassesSystemID/
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1644 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesSystemID/ClassBilinear.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4836 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesSystemID/ClassERA.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3437 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesSystemID/ClassMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      446 2023-02-07 20:15:32.000000 systemID-24.9/systemID/ClassesSystemID/ClassQMarkov.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.9/systemID/ClassesSystemID/__init__.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.457936 systemID-24.9/systemID/Plotting/
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2315 2023-02-07 20:15:32.000000 systemID-24.9/systemID/Plotting/PlotEigenValues.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      993 2023-02-07 20:15:32.000000 systemID-24.9/systemID/Plotting/PlotMarkovParameters2.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1175 2023-02-07 20:15:32.000000 systemID-24.9/systemID/Plotting/PlotSignals.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      750 2023-02-07 20:15:32.000000 systemID-24.9/systemID/Plotting/PlotSingularValues.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.9/systemID/Plotting/__init__.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.462169 systemID-24.9/systemID/SparseIDAlgorithms/
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3227 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/GeneratePolynomialBasisFunctions.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4620 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/GeneratePolynomialIndex.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      819 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/NormalizeSignals.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     6328 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    18012 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation1stOrder.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     8017 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    14388 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     9204 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem_polar.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    16894 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem_v2.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     9024 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2ndOrder.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      140 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation3rdOrder.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     6630 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation_v2.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2021-11-12 18:54:37.000000 systemID-24.9/systemID/SparseIDAlgorithms/__init__.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.481468 systemID-24.9/systemID/SystemIDAlgorithms/
+-rw-r--r--   0 damiengueho   (501) staff       (20)    10567 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/BilinearSystemID.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1195 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/CalculateNaturalFrequenciesAndDampingRatios.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1497 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/ComputeStatisticalMoments.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3402 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/CorrectSystemForEigenvaluesCheck.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4921 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/CreateAugmentedSignal.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    12540 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/DepartureDynamics.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      770 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/DynamicModeDecompositionAlgorithm.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5485 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithm.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5991 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmFromInitialConditionResponse.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     6424 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmWithDataCorrelation.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     7056 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmWithDataCorrelationFromInitialConditionResponse.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      642 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetCovarianceMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2535 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetDeltaMatrix.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1399 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetInitialConditionResponseMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1253 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetMACandMSV.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1550 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4513 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetMarkovParametersFromFrequencyResponseFunctions.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1741 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetMarkovParametersFromObserverControllerMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1709 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetMarkovParametersFromObserverMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2069 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetObservabilityMatrix.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1812 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetObserverGainMarkovParametersFromObserverMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1027 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetObserverGainMatrix.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1024 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetObserverMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1597 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetOptimizedHankelMatrixSize.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1470 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetPowerOf2.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1747 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetTVMarkovParametersFromTVObserverMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1559 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetTVObserverGainMarkovParametersFromTVObserverMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4740 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetTimeVaryingMarkovParameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1207 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/GetTimeVaryingObserverGainMatrix.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5707 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/HigherOrderMomentsPropagation.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    20238 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/HigherOrderStateTransitionTensorsPropagation.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2639 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/IdentificationInitialCondition.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1373 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/Integrate.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     7752 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/ObserverControllerKalmanIdentificationAlgorithmWithObserver.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     6826 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/ObserverKalmanIdentificationAlgorithm.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     7207 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/ObserverKalmanIdentificationAlgorithmWithObserver.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4724 2022-09-08 23:56:43.000000 systemID-24.9/systemID/SystemIDAlgorithms/ParticleSwarmOptimization.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    12826 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/Prediction.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    27483 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/Propagation.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2569 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/QMarkovCover.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     7437 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithm.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4798 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmFromInitialConditionResponse.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)    12377 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmWithDataCorrelation.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5772 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmWithDataCorrelationFromInitialConditionResponse.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3654 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingObserverKalmanIdentificationAlgorithmWithObserver.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3739 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/WeightingSequenceDescription.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1004 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmFull.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1398 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmObserver.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1418 2023-02-07 20:15:31.000000 systemID-24.9/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmObserverFull.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1594 2023-02-07 20:15:32.000000 systemID-24.9/systemID/SystemIDAlgorithms/ZZZTimeVaryingObserverKalmanIdentificationAlgorithmObserver.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2020-08-30 20:47:42.000000 systemID-24.9/systemID/SystemIDAlgorithms/__init__.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      223 2023-02-07 22:45:02.000000 systemID-24.9/systemID/__init__.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.481781 systemID-24.9/systemID/dynamics/
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:07:34.000000 systemID-24.9/systemID/dynamics/__init__.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.487443 systemID-24.9/systemID/functions/
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1190 2023-02-07 23:11:40.000000 systemID-24.9/systemID/functions/__init__.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5436 2023-02-07 20:14:46.000000 systemID-24.9/systemID/functions/eigensystem_realization_algorithm.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5630 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/eigensystem_realization_algorithm_from_initial_condition_response.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     6374 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/eigensystem_realization_algorithm_with_data_correlation.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     6703 2023-02-07 20:14:46.000000 systemID-24.9/systemID/functions/eigensystem_realization_algorithm_with_data_correlation_from_initial_condition_response.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1216 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/mac_and_msv.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1680 2023-02-07 20:14:48.000000 systemID-24.9/systemID/functions/markov_parameters_from_observer_markov_parameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1785 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/observer_gain_markov_parameters_from_observer_markov_parameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     6706 2023-02-07 20:14:48.000000 systemID-24.9/systemID/functions/observer_kalman_identification_algorithm.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     7176 2023-02-07 20:14:48.000000 systemID-24.9/systemID/functions/observer_kalman_identification_algorithm_with_observer.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3191 2023-02-07 20:14:46.000000 systemID-24.9/systemID/functions/polynomial_basis_functions.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4582 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/polynomial_index.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      120 2022-12-06 03:38:29.000000 systemID-24.9/systemID/functions/test.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      148 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/time_invariant_koopman_operator.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     5417 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/time_varying_eigensystem_realization_algorithm.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     4085 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/time_varying_eigensystem_realization_algorithm_from_initial_condition_response.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1740 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/time_varying_markov_parameters_from_time_varying_observer_markov_parameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1554 2023-02-07 20:14:47.000000 systemID-24.9/systemID/functions/time_varying_observer_gain_markov_parameters_from_time_varying_observer_markov_parameters.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3744 2023-02-07 20:14:48.000000 systemID-24.9/systemID/functions/time_varying_observer_kalman_identification_algorithm_with_observer.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.489016 systemID-24.9/systemID/input_output_identification/
+-rw-r--r--   0 damiengueho   (501) staff       (20)      170 2023-02-07 23:08:13.000000 systemID-24.9/systemID/input_output_identification/__init__.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3220 2022-12-10 04:18:38.000000 systemID-24.9/systemID/input_output_identification/autoregressive_identification.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     3236 2022-12-09 03:09:22.000000 systemID-24.9/systemID/input_output_identification/autoregressive_with_exogeneous_input_identification.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1923 2023-02-07 20:14:46.000000 systemID-24.9/systemID/input_output_identification/time_invariant.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      533 2023-02-07 20:14:47.000000 systemID-24.9/systemID/input_output_identification/time_varying.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.491471 systemID-24.9/systemID/input_output_model/
+-rw-r--r--   0 damiengueho   (501) staff       (20)      460 2023-02-07 23:10:29.000000 systemID-24.9/systemID/input_output_model/__init__.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:24:17.000000 systemID-24.9/systemID/input_output_model/autoregressive_integrated_moving_average_model.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:24:30.000000 systemID-24.9/systemID/input_output_model/autoregressive_integrated_moving_average_with_exogeneous_input_model.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      777 2023-02-06 21:08:45.000000 systemID-24.9/systemID/input_output_model/autoregressive_model.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:23:32.000000 systemID-24.9/systemID/input_output_model/autoregressive_moving_average_model.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:23:46.000000 systemID-24.9/systemID/input_output_model/autoregressive_moving_average_with_exogeneous_input_model.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1117 2023-02-06 21:08:45.000000 systemID-24.9/systemID/input_output_model/autoregressive_with_exogeneous_input_model.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:24:47.000000 systemID-24.9/systemID/input_output_model/volterra_series_model.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)        0 2022-11-09 03:24:59.000000 systemID-24.9/systemID/input_output_model/volterra_series_with_exogeneous_input_model.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.492394 systemID-24.9/systemID/signals/
+-rw-r--r--   0 damiengueho   (501) staff       (20)       50 2023-02-07 22:47:53.000000 systemID-24.9/systemID/signals/__init__.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)      267 2023-02-07 20:14:47.000000 systemID-24.9/systemID/signals/continuous.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1229 2023-02-07 22:26:36.000000 systemID-24.9/systemID/signals/discrete.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.493245 systemID-24.9/systemID/state_space_identification/
+-rw-r--r--   0 damiengueho   (501) staff       (20)       57 2023-02-07 23:10:52.000000 systemID-24.9/systemID/state_space_identification/__init__.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2796 2023-02-07 20:14:47.000000 systemID-24.9/systemID/state_space_identification/time_invariant.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2244 2023-02-07 20:14:47.000000 systemID-24.9/systemID/state_space_identification/time_varying.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.494070 systemID-24.9/systemID/state_space_model/
+-rw-r--r--   0 damiengueho   (501) staff       (20)       50 2023-02-07 23:11:07.000000 systemID-24.9/systemID/state_space_model/__init__.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     2896 2023-02-07 20:14:47.000000 systemID-24.9/systemID/state_space_model/continuous.py
+-rw-r--r--   0 damiengueho   (501) staff       (20)     1509 2023-02-07 20:14:47.000000 systemID-24.9/systemID/state_space_model/discrete.py
+drwxr-xr-x   0 damiengueho   (501) staff       (20)        0 2023-02-07 23:13:22.443411 systemID-24.9/systemID.egg-info/
+-rw-r--r--   0 damiengueho   (501) staff       (20)      763 2023-02-07 23:13:21.000000 systemID-24.9/systemID.egg-info/PKG-INFO
+-rw-r--r--   0 damiengueho   (501) staff       (20)     9244 2023-02-07 23:13:22.000000 systemID-24.9/systemID.egg-info/SOURCES.txt
+-rw-r--r--   0 damiengueho   (501) staff       (20)        1 2023-02-07 23:13:21.000000 systemID-24.9/systemID.egg-info/dependency_links.txt
+-rw-r--r--   0 damiengueho   (501) staff       (20)       23 2023-02-07 23:13:22.000000 systemID-24.9/systemID.egg-info/requires.txt
+-rw-r--r--   0 damiengueho   (501) staff       (20)        9 2023-02-07 23:13:22.000000 systemID-24.9/systemID.egg-info/top_level.txt
```

### Comparing `systemID-24.8/PKG-INFO` & `systemID-24.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemID
-Version: 24.8
+Version: 24.9
 Summary: Package for time domain system identification. LTI and LTV systems, bilinear systems and nonlinear systems.
 Author: Damien Gueho
 Author-email: <systemidtechnologies@gmail.com>
 License: UNKNOWN
 Keywords: python,system identification
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `systemID-24.8/setup.py` & `systemID-24.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '24.8'
+VERSION = '24.9'
 DESCRIPTION = 'Package for time domain system identification. LTI and LTV systems, bilinear systems and nonlinear systems.'
 LONG_DESCRIPTION = 'Package for time domain system identification. Supports linear time-invariant (LTI) and linear time-varying (LTV) dynamics, bilinear dynamics and nonlinear dynamics.'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="systemID",
```

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassAutomobileCruiseControlDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassAutomobileCruiseControlDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassAutomobileSystemDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassAutomobileSystemDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassBallAndBeamDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassBallAndBeamDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassCircularRestrictedThreeBodyProblemDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassCircularRestrictedThreeBodyProblemDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassCustomizedDiscreteTimeInvariantDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassCustomizedDiscreteTimeInvariantDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassDCMotorDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassDCMotorDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassDuffingOscillatorDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassDuffingOscillatorDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassFiniteElementTypeOscillatorChainDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassFiniteElementTypeOscillatorChainDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassFlutterAeroelasticWingDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassFlutterAeroelasticWingDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassFreeThreeMassSpringDamperDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassFreeThreeMassSpringDamperDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassInterceptProblemDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassInterceptProblemDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassInvertedPendulumDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassInvertedPendulumDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassLorenzSystemDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassLorenzSystemDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassMassSpringDamperDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassMassSpringDamperDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassOscillatorySystemZeroDampingDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassOscillatorySystemZeroDampingDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassPanelFlutterDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassPanelFlutterDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassPointMassInRotatingTubeDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassPointMassInRotatingTubeDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassSlowManifoldDecoupledSystemDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassSlowManifoldDecoupledSystemDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassSystemWithAStableOriginDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassSystemWithAStableOriginDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassThreeMassSpringDamperDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassThreeMassSpringDamperDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassTwoBodyProblemDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassTwoBodyProblemDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassTwoMassSpringDamperDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassTwoMassSpringDamperDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesDynamics/ClassVanDerPolOscillatorDynamics.py` & `systemID-24.9/systemID/ClassesDynamics/ClassVanDerPolOscillatorDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesGeneral/ClassExperiments.py` & `systemID-24.9/systemID/ClassesGeneral/ClassExperiments.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesGeneral/ClassSignal.py` & `systemID-24.9/systemID/ClassesGeneral/ClassSignal.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesGeneral/ClassSystem.py` & `systemID-24.9/systemID/ClassesGeneral/ClassSystem.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesSparseID/ClassSparseApproximation.py` & `systemID-24.9/systemID/ClassesSparseID/ClassSparseApproximation.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesSystemID/ClassBilinear.py` & `systemID-24.9/systemID/ClassesSystemID/ClassBilinear.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesSystemID/ClassERA.py` & `systemID-24.9/systemID/ClassesSystemID/ClassERA.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/ClassesSystemID/ClassMarkovParameters.py` & `systemID-24.9/systemID/ClassesSystemID/ClassMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/Plotting/PlotEigenValues.py` & `systemID-24.9/systemID/Plotting/PlotEigenValues.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/Plotting/PlotMarkovParameters2.py` & `systemID-24.9/systemID/Plotting/PlotMarkovParameters2.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/Plotting/PlotSignals.py` & `systemID-24.9/systemID/Plotting/PlotSignals.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/Plotting/PlotSingularValues.py` & `systemID-24.9/systemID/Plotting/PlotSingularValues.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/GeneratePolynomialBasisFunctions.py` & `systemID-24.9/systemID/SparseIDAlgorithms/GeneratePolynomialBasisFunctions.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/GeneratePolynomialIndex.py` & `systemID-24.9/systemID/SparseIDAlgorithms/GeneratePolynomialIndex.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/NormalizeSignals.py` & `systemID-24.9/systemID/SparseIDAlgorithms/NormalizeSignals.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation.py` & `systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation1stOrder.py` & `systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation1stOrder.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2.py` & `systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem.py` & `systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem_polar.py` & `systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem_polar.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem_v2.py` & `systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2_TwoBodyProblem_v2.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation2ndOrder.py` & `systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation2ndOrder.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SparseIDAlgorithms/SparseApproximation_v2.py` & `systemID-24.9/systemID/SparseIDAlgorithms/SparseApproximation_v2.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/BilinearSystemID.py` & `systemID-24.9/systemID/SystemIDAlgorithms/BilinearSystemID.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/CalculateNaturalFrequenciesAndDampingRatios.py` & `systemID-24.9/systemID/SystemIDAlgorithms/CalculateNaturalFrequenciesAndDampingRatios.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/ComputeStatisticalMoments.py` & `systemID-24.9/systemID/SystemIDAlgorithms/ComputeStatisticalMoments.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/CorrectSystemForEigenvaluesCheck.py` & `systemID-24.9/systemID/SystemIDAlgorithms/CorrectSystemForEigenvaluesCheck.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/CreateAugmentedSignal.py` & `systemID-24.9/systemID/SystemIDAlgorithms/CreateAugmentedSignal.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/DepartureDynamics.py` & `systemID-24.9/systemID/SystemIDAlgorithms/DepartureDynamics.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/DynamicModeDecompositionAlgorithm.py` & `systemID-24.9/systemID/SystemIDAlgorithms/DynamicModeDecompositionAlgorithm.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithm.py` & `systemID-24.9/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithm.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmFromInitialConditionResponse.py` & `systemID-24.9/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmFromInitialConditionResponse.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmWithDataCorrelation.py` & `systemID-24.9/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmWithDataCorrelation.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmWithDataCorrelationFromInitialConditionResponse.py` & `systemID-24.9/systemID/SystemIDAlgorithms/EigenSystemRealizationAlgorithmWithDataCorrelationFromInitialConditionResponse.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetCovarianceMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetCovarianceMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetDeltaMatrix.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetDeltaMatrix.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetInitialConditionResponseMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetInitialConditionResponseMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetMACandMSV.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetMACandMSV.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetMarkovParametersFromFrequencyResponseFunctions.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetMarkovParametersFromFrequencyResponseFunctions.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetMarkovParametersFromObserverControllerMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetMarkovParametersFromObserverControllerMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetMarkovParametersFromObserverMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetMarkovParametersFromObserverMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetObservabilityMatrix.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetObservabilityMatrix.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetObserverGainMarkovParametersFromObserverMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetObserverGainMarkovParametersFromObserverMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetObserverGainMatrix.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetObserverGainMatrix.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetObserverMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetObserverMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetOptimizedHankelMatrixSize.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetOptimizedHankelMatrixSize.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetPowerOf2.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetPowerOf2.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetTVMarkovParametersFromTVObserverMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetTVMarkovParametersFromTVObserverMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetTVObserverGainMarkovParametersFromTVObserverMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetTVObserverGainMarkovParametersFromTVObserverMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetTimeVaryingMarkovParameters.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetTimeVaryingMarkovParameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/GetTimeVaryingObserverGainMatrix.py` & `systemID-24.9/systemID/SystemIDAlgorithms/GetTimeVaryingObserverGainMatrix.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/HigherOrderMomentsPropagation.py` & `systemID-24.9/systemID/SystemIDAlgorithms/HigherOrderMomentsPropagation.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/HigherOrderStateTransitionTensorsPropagation.py` & `systemID-24.9/systemID/SystemIDAlgorithms/HigherOrderStateTransitionTensorsPropagation.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/IdentificationInitialCondition.py` & `systemID-24.9/systemID/SystemIDAlgorithms/IdentificationInitialCondition.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/Integrate.py` & `systemID-24.9/systemID/SystemIDAlgorithms/Integrate.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/ObserverControllerKalmanIdentificationAlgorithmWithObserver.py` & `systemID-24.9/systemID/SystemIDAlgorithms/ObserverControllerKalmanIdentificationAlgorithmWithObserver.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/ObserverKalmanIdentificationAlgorithm.py` & `systemID-24.9/systemID/SystemIDAlgorithms/ObserverKalmanIdentificationAlgorithm.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/ObserverKalmanIdentificationAlgorithmWithObserver.py` & `systemID-24.9/systemID/SystemIDAlgorithms/ObserverKalmanIdentificationAlgorithmWithObserver.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/ParticleSwarmOptimization.py` & `systemID-24.9/systemID/SystemIDAlgorithms/ParticleSwarmOptimization.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/Prediction.py` & `systemID-24.9/systemID/SystemIDAlgorithms/Prediction.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/Propagation.py` & `systemID-24.9/systemID/SystemIDAlgorithms/Propagation.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/QMarkovCover.py` & `systemID-24.9/systemID/SystemIDAlgorithms/QMarkovCover.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithm.py` & `systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithm.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmFromInitialConditionResponse.py` & `systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmFromInitialConditionResponse.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmWithDataCorrelation.py` & `systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmWithDataCorrelation.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmWithDataCorrelationFromInitialConditionResponse.py` & `systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingEigenSystemRealizationAlgorithmWithDataCorrelationFromInitialConditionResponse.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/TimeVaryingObserverKalmanIdentificationAlgorithmWithObserver.py` & `systemID-24.9/systemID/SystemIDAlgorithms/TimeVaryingObserverKalmanIdentificationAlgorithmWithObserver.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/WeightingSequenceDescription.py` & `systemID-24.9/systemID/SystemIDAlgorithms/WeightingSequenceDescription.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmFull.py` & `systemID-24.9/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmFull.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmObserver.py` & `systemID-24.9/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmObserver.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmObserverFull.py` & `systemID-24.9/systemID/SystemIDAlgorithms/ZZZObserverKalmanIdentificationAlgorithmObserverFull.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/SystemIDAlgorithms/ZZZTimeVaryingObserverKalmanIdentificationAlgorithmObserver.py` & `systemID-24.9/systemID/SystemIDAlgorithms/ZZZTimeVaryingObserverKalmanIdentificationAlgorithmObserver.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/eigensystem_realization_algorithm.py` & `systemID-24.9/systemID/functions/eigensystem_realization_algorithm.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/eigensystem_realization_algorithm_from_initial_condition_response.py` & `systemID-24.9/systemID/functions/eigensystem_realization_algorithm_from_initial_condition_response.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/eigensystem_realization_algorithm_with_data_correlation.py` & `systemID-24.9/systemID/functions/eigensystem_realization_algorithm_with_data_correlation.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/eigensystem_realization_algorithm_with_data_correlation_from_initial_condition_response.py` & `systemID-24.9/systemID/functions/eigensystem_realization_algorithm_with_data_correlation_from_initial_condition_response.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/mac_and_msv.py` & `systemID-24.9/systemID/functions/mac_and_msv.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/markov_parameters_from_observer_markov_parameters.py` & `systemID-24.9/systemID/functions/markov_parameters_from_observer_markov_parameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/observer_gain_markov_parameters_from_observer_markov_parameters.py` & `systemID-24.9/systemID/functions/observer_gain_markov_parameters_from_observer_markov_parameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/observer_kalman_identification_algorithm.py` & `systemID-24.9/systemID/functions/observer_kalman_identification_algorithm.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/observer_kalman_identification_algorithm_with_observer.py` & `systemID-24.9/systemID/functions/observer_kalman_identification_algorithm_with_observer.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/polynomial_basis_functions.py` & `systemID-24.9/systemID/functions/polynomial_basis_functions.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/polynomial_index.py` & `systemID-24.9/systemID/functions/polynomial_index.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/time_varying_eigensystem_realization_algorithm.py` & `systemID-24.9/systemID/functions/time_varying_eigensystem_realization_algorithm.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/time_varying_eigensystem_realization_algorithm_from_initial_condition_response.py` & `systemID-24.9/systemID/functions/time_varying_eigensystem_realization_algorithm_from_initial_condition_response.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/time_varying_markov_parameters_from_time_varying_observer_markov_parameters.py` & `systemID-24.9/systemID/functions/time_varying_markov_parameters_from_time_varying_observer_markov_parameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/time_varying_observer_gain_markov_parameters_from_time_varying_observer_markov_parameters.py` & `systemID-24.9/systemID/functions/time_varying_observer_gain_markov_parameters_from_time_varying_observer_markov_parameters.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/functions/time_varying_observer_kalman_identification_algorithm_with_observer.py` & `systemID-24.9/systemID/functions/time_varying_observer_kalman_identification_algorithm_with_observer.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/input_output_identification/autoregressive_identification.py` & `systemID-24.9/systemID/input_output_identification/autoregressive_identification.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/input_output_identification/autoregressive_with_exogeneous_input_identification.py` & `systemID-24.9/systemID/input_output_identification/autoregressive_with_exogeneous_input_identification.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/input_output_identification/time_invariant.py` & `systemID-24.9/systemID/input_output_identification/time_invariant.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/input_output_identification/time_varying.py` & `systemID-24.9/systemID/input_output_identification/time_varying.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/input_output_model/autoregressive_model.py` & `systemID-24.9/systemID/input_output_model/autoregressive_model.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/input_output_model/autoregressive_with_exogeneous_input_model.py` & `systemID-24.9/systemID/input_output_model/autoregressive_with_exogeneous_input_model.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/signals/discrete.py` & `systemID-24.9/systemID/signals/discrete.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/state_space_identification/time_invariant.py` & `systemID-24.9/systemID/state_space_identification/time_invariant.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/state_space_identification/time_varying.py` & `systemID-24.9/systemID/state_space_identification/time_varying.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/state_space_model/continuous.py` & `systemID-24.9/systemID/state_space_model/continuous.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID/state_space_model/discrete.py` & `systemID-24.9/systemID/state_space_model/discrete.py`

 * *Files identical despite different names*

### Comparing `systemID-24.8/systemID.egg-info/PKG-INFO` & `systemID-24.9/systemID.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemID
-Version: 24.8
+Version: 24.9
 Summary: Package for time domain system identification. LTI and LTV systems, bilinear systems and nonlinear systems.
 Author: Damien Gueho
 Author-email: <systemidtechnologies@gmail.com>
 License: UNKNOWN
 Keywords: python,system identification
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `systemID-24.8/systemID.egg-info/SOURCES.txt` & `systemID-24.9/systemID.egg-info/SOURCES.txt`

 * *Files identical despite different names*

