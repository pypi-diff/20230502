# Comparing `tmp/vessel_manoeuvring_models-0.0.4.tar.gz` & `tmp/vessel_manoeuvring_models-0.0.6.tar.gz`

## Comparing `vessel_manoeuvring_models-0.0.4.tar` & `vessel_manoeuvring_models-0.0.6.tar`

### file list

```diff
@@ -1,273 +1,273 @@
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/Makefile
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/requirements.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/requirements_build.txt
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/test_environment.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tox.ini
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/binder/apt.txt
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/binder/environment.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/binder/postBuild
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/data/external/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/data/interim/.gitkeep
--rw-r--r--   0        0        0    41828 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/data/interim/run_selection.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/data/processed/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/data/raw/.gitkeep
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/Makefile
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/commands.rst
--rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/conf.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/getting-started.rst
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/index.rst
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/make.bat
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/00.01_intro.md
--rw-r--r--   0        0        0    15206 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/00.02_intro_example.ipynb
--rw-r--r--   0        0        0    42000 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/01.01_manoeuvring_simulation.ipynb
--rw-r--r--   0        0        0    34911 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/02.01_manoeuvring_PIT.ipynb
--rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/10.03_OLS_covariance.ipynb
--rw-r--r--   0        0        0    29754 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/10.04_bias_variance.ipynb
--rw-r--r--   0        0        0    20341 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/15.39_KF_nomoto.ipynb
--rw-r--r--   0        0        0    19838 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/15.40_EKF_nomoto.ipynb
--rw-r--r--   0        0        0    18606 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/30.01_maximum_likelihood.ipynb
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/_config.yml
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/_toc.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/bibligraphy.md
--rw-r--r--   0        0        0    34134 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/book.mplstyle
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/chapter.ipynb
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/example_1.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/imports.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/kalman_filters.md
--rw-r--r--   0        0        0   469672 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/logo.png
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/markdown.md
--rw-r--r--   0        0        0   238911 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/references.bib
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/book/requirements.txt
--rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/01.1_seaman_matematical_model.ipynb
--rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/02.1_seaman_sway_hull_equation.ipynb
--rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/03.1_seaman_yaw_hull_equation.ipynb
--rw-r--r--   0        0        0    17435 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/04.1_seaman_rudder_equation.ipynb
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/04.2_seaman_rudder_equation_modified_drag.ipynb
--rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/05.1_seaman_surge_hull_equation.ipynb
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/06.1_seaman_roll_hull_equation.ipynb
--rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/10_seaman_rigid_body.ipynb
--rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/11_manoeuvring_simulation.ipynb
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/X_function.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/Y_function.py
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/__init__.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/bis_system.py
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/cd.png
--rw-r--r--   0        0        0   130907 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/coordinateSystem.png
--rw-r--r--   0        0        0    30237 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/coordinate_system.png
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/curve_fit.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/generate_input.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/notebooks_to_html.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/regression.py
--rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/regression_old.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/roll_hull_equations.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/roll_hull_lambda_functions.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/rudder_equations.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/rudder_lambda_functions.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/run_real_seaman.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/save_lambda_functions.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/seaman_symbol.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/seaman_symbols.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/substitute_dynamic_symbols.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/surge_hull_equations.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/surge_hull_lambda_functions.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/sway_hull_equations.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/sway_hull_lambda_functions.py
--rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/test_ship.ship
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/total_equations.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/total_lambda_functions.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/yaw_hull_equations.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/docs/seaman/yaw_hull_lambda_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/models/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/.gitkeep
--rw-r--r--   0        0        0   332654 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/01.00_MDL_select_runs.ipynb
--rw-r--r--   0        0        0    27865 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/02.00_MDL_load_runs.ipynb
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/03.00_test_overview.ipynb
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/04.01_PIT_nomoto.ipynb
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/04.02_PIT_linear_VMM.ipynb
--rw-r--r--   0        0        0     9376 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/04.02_PIT_nomotos.ipynb
--rw-r--r--   0        0        0    19255 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/04.02_PIT_nonlinear_VMM.ipynb
--rw-r--r--   0        0        0    31214 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/04.03_PIT_VCT_linear_VMM.ipynb
--rw-r--r--   0        0        0    32154 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/04.03_PIT_VCT_nonlinear_VMM.ipynb
--rw-r--r--   0        0        0    34957 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/04.03_PIT_linear_VMM.ipynb
--rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/05.01_acceleration_Kalman.ipynb
--rw-r--r--   0        0        0   274069 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/05.02_transform_to_ship.ipynb
--rw-r--r--   0        0        0   879206 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/05.03_cutting.ipynb
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/05.semiempirical_rudder_wpcc.ipynb
--rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/06.01_linear_VMM.ipynb
--rw-r--r--   0        0        0    23562 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/06.01_linear_simplified_VMM.ipynb
--rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/06.02_linear_VMM_wPCC_brix.ipynb
--rw-r--r--   0        0        0  1165028 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/07.03_PIT_static_forces_nonlinear.ipynb
--rw-r--r--   0        0        0    37675 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/07_01_static_forces_from_model_test.ipynb
--rw-r--r--   0        0        0  1176968 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/07_02_static_forces_from_spirals.ipynb
--rw-r--r--   0        0        0    48697 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/07_05_static_forces_from_model_test-many.ipynb
--rw-r--r--   0        0        0    49041 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/08_01_PIT_summary.ipynb
--rw-r--r--   0        0        0    44439 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/08_02_PIT_nonlinear_summary.ipynb
--rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/09_01_PIT_tongton.ipynb
--rw-r--r--   0        0        0    23537 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/09_02_PIT_tongton_SI.ipynb
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/10.01_EOM_air.ipynb
--rw-r--r--   0        0        0    19914 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/10.02_kalman_PIT_sensitivity.ipynb
--rw-r--r--   0        0        0    33006 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/10.03_lowpass_PIT.ipynb
--rw-r--r--   0        0        0    30697 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/11.01_regression_revisited.ipynb
--rw-r--r--   0        0        0    25508 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.01_regression_simulated_data.ipynb
--rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.02_regression_simulated_data_nonlinear_EOM.ipynb
--rw-r--r--   0        0        0    37550 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.03_regression_simulated_data_mariner.ipynb
--rw-r--r--   0        0        0    24478 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.04_regression_too_little_simulated_data.ipynb
--rw-r--r--   0        0        0    28072 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.05.5_regression_simulated_data_simple_nonlinear_BDF.ipynb
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.05_regression_simulated_data_acc_thrust.ipynb
--rw-r--r--   0        0        0    27714 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.05_regression_simulated_data_simple_nonlinear.ipynb
--rw-r--r--   0        0        0    24448 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.06.5_regression_simulated_data_BDF_numerical_gradient.ipynb
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.06_regression_simulated_data_numerical_gradient.ipynb
--rw-r--r--   0        0        0    27318 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.07_regression_simulated_data_better_numerical_gradient.ipynb
--rw-r--r--   0        0        0    22934 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.08_regression_simulated_data_gausian_noise.ipynb
--rw-r--r--   0        0        0    24594 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/12.08_regression_simulated_more_data_gausian_noise.ipynb
--rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/13.01_solve_ivp.ipynb
--rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/14.01_EM_algorithm.ipynb
--rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/14.01_hidden_states.ipynb
--rw-r--r--   0        0        0    23581 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/14.02_hidden_states_gradient_regression.ipynb
--rw-r--r--   0        0        0    24046 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/14.03_hidden_states_gradient_regression_linear.ipynb
--rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.01_kalman_filter_unvariate.ipynb
--rw-r--r--   0        0        0    21616 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.10_kalman_filter_multivariate.ipynb
--rw-r--r--   0        0        0    31286 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.11_kalman_filter_linear_manoeuvring.ipynb
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.20_EM-algorithm.ipynb
--rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.30_KF_fossen.ipynb
--rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.31_EKF_fossen.ipynb
--rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.39_KF_nomoto.ipynb
--rw-r--r--   0        0        0    15487 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.40_EKF_nomoto.ipynb
--rw-r--r--   0        0        0    18938 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.41_EKF_PIT_nomoto.ipynb
--rw-r--r--   0        0        0    21033 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.42_EKF_EM_nomoto.ipynb
--rw-r--r--   0        0        0    19373 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.42_EKF_PIT_2_nomoto.ipynb
--rw-r--r--   0        0        0    17287 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.44_KF_EM_RTS_nomoto.ipynb
--rw-r--r--   0        0        0   299798 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.45_KF_EM_RTS_nomoto.ipynb
--rw-r--r--   0        0        0    14125 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.46_EKF_Abkowitz.ipynb
--rw-r--r--   0        0        0    45662 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.47_EKF_3DOF.ipynb
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.47_EKF_3DOF.py
--rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.48_EK_smoother_3DOF.ipynb
--rw-r--r--   0        0        0    29295 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.49_EK_smoother_3DOF_thrust.ipynb
--rw-r--r--   0        0        0    15522 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.50_KF_EM_RTS_nomoto.ipynb
--rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.51_EK_inverse_dynamics.ipynb
--rw-r--r--   0        0        0    10993 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/15.52_inverse_static.ipynb
--rw-r--r--   0        0        0    17497 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/16.01_PIT_VCT_revisited_linear.ipynb
--rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/16.02_PIT_VCT_revisited_nonlinear.ipynb
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/16.03_model_simulate.ipynb
--rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/17.01_RTS_manoeuvring_PIT.ipynb
--rw-r--r--   0        0        0    19422 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/21.01_parameter_drift.ipynb
--rw-r--r--   0        0        0    17265 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/21.02_parameter_drift.ipynb
--rw-r--r--   0        0        0    23816 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/21.03_parameter_drift.ipynb
--rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/21.04_perfect_captive.ipynb
--rw-r--r--   0        0        0    13073 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/21.05_perfect_captive_truncated.ipynb
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/22.01_scaling_VCT_captive.ipynb
--rw-r--r--   0        0        0   334166 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/30.01_joke.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/__init__.py
--rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/ai_research.png
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/example_ship2.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/imports.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/logbook.ipynb
--rw-r--r--   0        0        0    33486 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/matplotlibrc
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/research.ipynb
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/model_simulate/01.01_run_simulations.py
--rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/model_simulate/02.01_analyze_runs.ipynb
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/notebooks/model_simulate/templates/16.03_model_simulate.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/references/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/reports/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/reports/figures/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/.gitkeep
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_EKF_PIT_Nomot.py
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_KF_Nomoto.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_extended_kalman_filter.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_extended_kalman_vmm.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_force_regression.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_kalman_filter.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_linear_vmm.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_model_simulator.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_parameter_denominator.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_prime_system.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_rts_smoother.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/tests/test_vmm_simple_nonliear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/__init__.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/bias_variance_tradeoff.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/equations.py
--rw-r--r--   0        0        0    12310 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/extended_kalman_filter.py
--rw-r--r--   0        0        0    21125 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/extended_kalman_vmm.py
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/feature_selection.py
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/kalman_filter.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/linear_vmm_equations.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/linear_vmm_simplified_equations.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/logger.py
--rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/mlflow_utils.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/nonlinear_abkowitz_vmm_equations.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/nonlinear_martin_vmm_equations.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/nonlinear_vmm_equations.py
--rw-r--r--   0        0        0    12924 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/notebook_to_latex.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/parameter_helpers.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/parameters.py
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/prime_system.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/substitute_dynamic_symbols.py
--rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/symbols.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/system_equations.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/to_mlflow.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/twin_simulations.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/vct_scaling.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/vmm_equations_VCT.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/__init__.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/case_0.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/case_1.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/kalman_filter.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/lowpass_filter.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/make_dataset.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/mdl.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/wpcc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/features/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/features/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/features/build_features.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/.gitkeep
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/MMG_hull.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/MMG_propeller.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/MMG_rudder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/__init__.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/brix_coefficients.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/captive_variation.py
--rw-r--r--   0        0        0     9394 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/diff_eq_to_matrix.py
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/force_from_motion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/linear_nomoto.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/linear_vmm.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/nonlinear_martin_vmm.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/nonlinear_vmm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/predict_model.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/propeller.py
--rw-r--r--   0        0        0    22018 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/regression.py
--rw-r--r--   0        0        0    12128 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/result.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/train_model.py
--rw-r--r--   0        0        0    29108 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_MMG.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_VCT.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_abkowitz.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_abkowitz_expanded.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_abkowitz_no_thrust.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_air.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_gsi.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_linear.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_mariner.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_martin.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_martin_linear.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_martin_simple.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_nonlinear_EOM.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_perturbed.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_simple.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_simple_nonlinear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vessels/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vessels/mariner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/__init__.py
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/book_format.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/equation.py
--rw-r--r--   0        0        0    12833 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/plot.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/regression.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/visualize.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/LICENSE
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/README.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/Makefile
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/requirements.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/requirements_build.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/test_environment.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tox.ini
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/binder/apt.txt
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/binder/environment.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/binder/postBuild
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/external/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/interim/.gitkeep
+-rw-r--r--   0        0        0    41828 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/interim/run_selection.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/processed/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/data/raw/.gitkeep
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/Makefile
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/commands.rst
+-rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/conf.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/getting-started.rst
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/index.rst
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/make.bat
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/00.01_intro.md
+-rw-r--r--   0        0        0    15206 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/00.02_intro_example.ipynb
+-rw-r--r--   0        0        0    42000 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/01.01_manoeuvring_simulation.ipynb
+-rw-r--r--   0        0        0    34911 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/02.01_manoeuvring_PIT.ipynb
+-rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/10.03_OLS_covariance.ipynb
+-rw-r--r--   0        0        0    29754 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/10.04_bias_variance.ipynb
+-rw-r--r--   0        0        0    20341 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/15.39_KF_nomoto.ipynb
+-rw-r--r--   0        0        0    19838 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/15.40_EKF_nomoto.ipynb
+-rw-r--r--   0        0        0    18606 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/30.01_maximum_likelihood.ipynb
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/_config.yml
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/_toc.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/bibligraphy.md
+-rw-r--r--   0        0        0    34134 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/book.mplstyle
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/chapter.ipynb
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/example_1.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/imports.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/kalman_filters.md
+-rw-r--r--   0        0        0   469672 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/logo.png
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/markdown.md
+-rw-r--r--   0        0        0   238911 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/references.bib
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/book/requirements.txt
+-rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/01.1_seaman_matematical_model.ipynb
+-rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/02.1_seaman_sway_hull_equation.ipynb
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/03.1_seaman_yaw_hull_equation.ipynb
+-rw-r--r--   0        0        0    17435 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/04.1_seaman_rudder_equation.ipynb
+-rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/04.2_seaman_rudder_equation_modified_drag.ipynb
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/05.1_seaman_surge_hull_equation.ipynb
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/06.1_seaman_roll_hull_equation.ipynb
+-rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/10_seaman_rigid_body.ipynb
+-rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/11_manoeuvring_simulation.ipynb
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/X_function.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/Y_function.py
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/__init__.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/bis_system.py
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/cd.png
+-rw-r--r--   0        0        0   130907 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/coordinateSystem.png
+-rw-r--r--   0        0        0    30237 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/coordinate_system.png
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/curve_fit.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/generate_input.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/notebooks_to_html.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/regression.py
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/regression_old.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/roll_hull_equations.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/roll_hull_lambda_functions.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/rudder_equations.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/rudder_lambda_functions.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/run_real_seaman.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/save_lambda_functions.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/seaman_symbol.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/seaman_symbols.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/substitute_dynamic_symbols.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/surge_hull_equations.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/surge_hull_lambda_functions.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/sway_hull_equations.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/sway_hull_lambda_functions.py
+-rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/test_ship.ship
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/total_equations.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/total_lambda_functions.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/yaw_hull_equations.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/docs/seaman/yaw_hull_lambda_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/models/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/.gitkeep
+-rw-r--r--   0        0        0   332654 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/01.00_MDL_select_runs.ipynb
+-rw-r--r--   0        0        0    27865 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/02.00_MDL_load_runs.ipynb
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/03.00_test_overview.ipynb
+-rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.01_PIT_nomoto.ipynb
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_linear_VMM.ipynb
+-rw-r--r--   0        0        0     9376 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_nomotos.ipynb
+-rw-r--r--   0        0        0    19255 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_nonlinear_VMM.ipynb
+-rw-r--r--   0        0        0    31214 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_VCT_linear_VMM.ipynb
+-rw-r--r--   0        0        0    32154 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_VCT_nonlinear_VMM.ipynb
+-rw-r--r--   0        0        0    34957 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_linear_VMM.ipynb
+-rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/05.01_acceleration_Kalman.ipynb
+-rw-r--r--   0        0        0   274069 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/05.02_transform_to_ship.ipynb
+-rw-r--r--   0        0        0   879206 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/05.03_cutting.ipynb
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/05.semiempirical_rudder_wpcc.ipynb
+-rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/06.01_linear_VMM.ipynb
+-rw-r--r--   0        0        0    23562 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/06.01_linear_simplified_VMM.ipynb
+-rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/06.02_linear_VMM_wPCC_brix.ipynb
+-rw-r--r--   0        0        0  1165028 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/07.03_PIT_static_forces_nonlinear.ipynb
+-rw-r--r--   0        0        0    37675 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/07_01_static_forces_from_model_test.ipynb
+-rw-r--r--   0        0        0  1176968 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/07_02_static_forces_from_spirals.ipynb
+-rw-r--r--   0        0        0    48697 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/07_05_static_forces_from_model_test-many.ipynb
+-rw-r--r--   0        0        0    49041 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/08_01_PIT_summary.ipynb
+-rw-r--r--   0        0        0    44439 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/08_02_PIT_nonlinear_summary.ipynb
+-rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/09_01_PIT_tongton.ipynb
+-rw-r--r--   0        0        0    23537 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/09_02_PIT_tongton_SI.ipynb
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/10.01_EOM_air.ipynb
+-rw-r--r--   0        0        0    19914 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/10.02_kalman_PIT_sensitivity.ipynb
+-rw-r--r--   0        0        0    33006 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/10.03_lowpass_PIT.ipynb
+-rw-r--r--   0        0        0    30697 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/11.01_regression_revisited.ipynb
+-rw-r--r--   0        0        0    25508 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.01_regression_simulated_data.ipynb
+-rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.02_regression_simulated_data_nonlinear_EOM.ipynb
+-rw-r--r--   0        0        0    37550 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.03_regression_simulated_data_mariner.ipynb
+-rw-r--r--   0        0        0    24478 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.04_regression_too_little_simulated_data.ipynb
+-rw-r--r--   0        0        0    28072 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.05.5_regression_simulated_data_simple_nonlinear_BDF.ipynb
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.05_regression_simulated_data_acc_thrust.ipynb
+-rw-r--r--   0        0        0    27714 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.05_regression_simulated_data_simple_nonlinear.ipynb
+-rw-r--r--   0        0        0    24448 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.06.5_regression_simulated_data_BDF_numerical_gradient.ipynb
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.06_regression_simulated_data_numerical_gradient.ipynb
+-rw-r--r--   0        0        0    27318 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.07_regression_simulated_data_better_numerical_gradient.ipynb
+-rw-r--r--   0        0        0    22934 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.08_regression_simulated_data_gausian_noise.ipynb
+-rw-r--r--   0        0        0    24594 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/12.08_regression_simulated_more_data_gausian_noise.ipynb
+-rw-r--r--   0        0        0    10947 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/13.01_solve_ivp.ipynb
+-rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/14.01_EM_algorithm.ipynb
+-rw-r--r--   0        0        0    13425 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/14.01_hidden_states.ipynb
+-rw-r--r--   0        0        0    23581 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/14.02_hidden_states_gradient_regression.ipynb
+-rw-r--r--   0        0        0    24046 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/14.03_hidden_states_gradient_regression_linear.ipynb
+-rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.01_kalman_filter_unvariate.ipynb
+-rw-r--r--   0        0        0    21616 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.10_kalman_filter_multivariate.ipynb
+-rw-r--r--   0        0        0    31286 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.11_kalman_filter_linear_manoeuvring.ipynb
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.20_EM-algorithm.ipynb
+-rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.30_KF_fossen.ipynb
+-rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.31_EKF_fossen.ipynb
+-rw-r--r--   0        0        0    15732 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.39_KF_nomoto.ipynb
+-rw-r--r--   0        0        0    15487 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.40_EKF_nomoto.ipynb
+-rw-r--r--   0        0        0    18938 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.41_EKF_PIT_nomoto.ipynb
+-rw-r--r--   0        0        0    21033 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.42_EKF_EM_nomoto.ipynb
+-rw-r--r--   0        0        0    19373 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.42_EKF_PIT_2_nomoto.ipynb
+-rw-r--r--   0        0        0    17287 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.44_KF_EM_RTS_nomoto.ipynb
+-rw-r--r--   0        0        0   299798 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.45_KF_EM_RTS_nomoto.ipynb
+-rw-r--r--   0        0        0    14125 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.46_EKF_Abkowitz.ipynb
+-rw-r--r--   0        0        0    45662 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.47_EKF_3DOF.ipynb
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.47_EKF_3DOF.py
+-rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.48_EK_smoother_3DOF.ipynb
+-rw-r--r--   0        0        0    29295 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.49_EK_smoother_3DOF_thrust.ipynb
+-rw-r--r--   0        0        0    15522 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.50_KF_EM_RTS_nomoto.ipynb
+-rw-r--r--   0        0        0    21888 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.51_EK_inverse_dynamics.ipynb
+-rw-r--r--   0        0        0    10993 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/15.52_inverse_static.ipynb
+-rw-r--r--   0        0        0    17497 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/16.01_PIT_VCT_revisited_linear.ipynb
+-rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/16.02_PIT_VCT_revisited_nonlinear.ipynb
+-rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/16.03_model_simulate.ipynb
+-rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/17.01_RTS_manoeuvring_PIT.ipynb
+-rw-r--r--   0        0        0    19422 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.01_parameter_drift.ipynb
+-rw-r--r--   0        0        0    17265 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.02_parameter_drift.ipynb
+-rw-r--r--   0        0        0    23816 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.03_parameter_drift.ipynb
+-rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.04_perfect_captive.ipynb
+-rw-r--r--   0        0        0    13073 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/21.05_perfect_captive_truncated.ipynb
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/22.01_scaling_VCT_captive.ipynb
+-rw-r--r--   0        0        0   334166 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/30.01_joke.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/__init__.py
+-rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/ai_research.png
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/example_ship2.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/imports.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/logbook.ipynb
+-rw-r--r--   0        0        0    33486 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/matplotlibrc
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/research.ipynb
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/01.01_run_simulations.py
+-rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/02.01_analyze_runs.ipynb
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/templates/16.03_model_simulate.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/references/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/reports/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/reports/figures/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/.gitkeep
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_EKF_PIT_Nomot.py
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_KF_Nomoto.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_extended_kalman_filter.py
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_extended_kalman_vmm.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_force_regression.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_kalman_filter.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_linear_vmm.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_model_simulator.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_parameter_denominator.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_prime_system.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_rts_smoother.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/tests/test_vmm_simple_nonliear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/__init__.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/bias_variance_tradeoff.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/equations.py
+-rw-r--r--   0        0        0    12310 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/extended_kalman_filter.py
+-rw-r--r--   0        0        0    21131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/extended_kalman_vmm.py
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/feature_selection.py
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/kalman_filter.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/linear_vmm_equations.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/linear_vmm_simplified_equations.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/logger.py
+-rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/mlflow_utils.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_abkowitz_vmm_equations.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_martin_vmm_equations.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_vmm_equations.py
+-rw-r--r--   0        0        0    12924 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/notebook_to_latex.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/parameter_helpers.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/parameters.py
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/prime_system.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/substitute_dynamic_symbols.py
+-rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/symbols.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/system_equations.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/to_mlflow.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/twin_simulations.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/vct_scaling.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/vmm_equations_VCT.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/__init__.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/case_0.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/case_1.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/kalman_filter.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/lowpass_filter.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/make_dataset.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/mdl.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/wpcc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/features/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/features/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/features/build_features.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/.gitkeep
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_hull.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_propeller.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_rudder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/__init__.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/brix_coefficients.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/captive_variation.py
+-rw-r--r--   0        0        0     9394 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/diff_eq_to_matrix.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/force_from_motion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/linear_nomoto.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/linear_vmm.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/nonlinear_martin_vmm.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/nonlinear_vmm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/predict_model.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/propeller.py
+-rw-r--r--   0        0        0    22054 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/regression.py
+-rw-r--r--   0        0        0    12128 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/result.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/train_model.py
+-rw-r--r--   0        0        0    29108 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_MMG.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_VCT.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz_expanded.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz_no_thrust.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_air.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_gsi.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_linear.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_mariner.py
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin_linear.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin_simple.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_nonlinear_EOM.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_perturbed.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_simple.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_simple_nonlinear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vessels/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vessels/mariner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/__init__.py
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/book_format.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/equation.py
+-rw-r--r--   0        0        0    12833 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/plot.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/regression.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/visualize.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/LICENSE
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/README.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 vessel_manoeuvring_models-0.0.6/PKG-INFO
```

### Comparing `vessel_manoeuvring_models-0.0.4/Makefile` & `vessel_manoeuvring_models-0.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/test_environment.py` & `vessel_manoeuvring_models-0.0.6/test_environment.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/data/interim/run_selection.csv` & `vessel_manoeuvring_models-0.0.6/data/interim/run_selection.csv`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/Makefile` & `vessel_manoeuvring_models-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/conf.py` & `vessel_manoeuvring_models-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/make.bat` & `vessel_manoeuvring_models-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/00.01_intro.md` & `vessel_manoeuvring_models-0.0.6/docs/book/00.01_intro.md`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/00.02_intro_example.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/book/00.02_intro_example.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/01.01_manoeuvring_simulation.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/book/01.01_manoeuvring_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/02.01_manoeuvring_PIT.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/book/02.01_manoeuvring_PIT.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/10.03_OLS_covariance.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/book/10.03_OLS_covariance.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/10.04_bias_variance.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/book/10.04_bias_variance.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/15.39_KF_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/book/15.39_KF_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/15.40_EKF_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/book/15.40_EKF_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/30.01_maximum_likelihood.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/book/30.01_maximum_likelihood.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/_config.yml` & `vessel_manoeuvring_models-0.0.6/docs/book/_config.yml`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/book.mplstyle` & `vessel_manoeuvring_models-0.0.6/docs/book/book.mplstyle`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/chapter.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/book/chapter.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/example_1.py` & `vessel_manoeuvring_models-0.0.6/docs/book/example_1.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/imports.py` & `vessel_manoeuvring_models-0.0.6/docs/book/imports.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/logo.png` & `vessel_manoeuvring_models-0.0.6/docs/book/logo.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/markdown.md` & `vessel_manoeuvring_models-0.0.6/docs/book/markdown.md`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/book/references.bib` & `vessel_manoeuvring_models-0.0.6/docs/book/references.bib`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/01.1_seaman_matematical_model.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/seaman/01.1_seaman_matematical_model.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/02.1_seaman_sway_hull_equation.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/seaman/02.1_seaman_sway_hull_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/03.1_seaman_yaw_hull_equation.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/seaman/03.1_seaman_yaw_hull_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/04.1_seaman_rudder_equation.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/seaman/04.1_seaman_rudder_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/04.2_seaman_rudder_equation_modified_drag.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/seaman/04.2_seaman_rudder_equation_modified_drag.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/05.1_seaman_surge_hull_equation.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/seaman/05.1_seaman_surge_hull_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/06.1_seaman_roll_hull_equation.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/seaman/06.1_seaman_roll_hull_equation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/10_seaman_rigid_body.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/seaman/10_seaman_rigid_body.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/11_manoeuvring_simulation.ipynb` & `vessel_manoeuvring_models-0.0.6/docs/seaman/11_manoeuvring_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/X_function.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/X_function.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/Y_function.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/Y_function.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/__init__.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/__init__.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/bis_system.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/bis_system.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/cd.png` & `vessel_manoeuvring_models-0.0.6/docs/seaman/cd.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/coordinateSystem.png` & `vessel_manoeuvring_models-0.0.6/docs/seaman/coordinateSystem.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/coordinate_system.png` & `vessel_manoeuvring_models-0.0.6/docs/seaman/coordinate_system.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/curve_fit.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/curve_fit.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/generate_input.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/generate_input.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/notebooks_to_html.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/notebooks_to_html.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/regression.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/regression.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/regression_old.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/regression_old.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/roll_hull_equations.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/roll_hull_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/rudder_equations.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/rudder_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/rudder_lambda_functions.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/rudder_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/run_real_seaman.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/run_real_seaman.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/save_lambda_functions.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/save_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/seaman_symbol.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/seaman_symbol.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/seaman_symbols.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/seaman_symbols.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/substitute_dynamic_symbols.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/substitute_dynamic_symbols.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/sway_hull_equations.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/sway_hull_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/sway_hull_lambda_functions.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/sway_hull_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/test_ship.ship` & `vessel_manoeuvring_models-0.0.6/docs/seaman/test_ship.ship`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/total_equations.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/total_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/total_lambda_functions.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/total_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/yaw_hull_equations.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/yaw_hull_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/docs/seaman/yaw_hull_lambda_functions.py` & `vessel_manoeuvring_models-0.0.6/docs/seaman/yaw_hull_lambda_functions.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/01.00_MDL_select_runs.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/01.00_MDL_select_runs.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/02.00_MDL_load_runs.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/02.00_MDL_load_runs.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/03.00_test_overview.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/03.00_test_overview.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/04.01_PIT_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/04.01_PIT_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/04.02_PIT_linear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_linear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/04.02_PIT_nomotos.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_nomotos.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/04.02_PIT_nonlinear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/04.02_PIT_nonlinear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/04.03_PIT_VCT_linear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_VCT_linear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/04.03_PIT_VCT_nonlinear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_VCT_nonlinear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/04.03_PIT_linear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/04.03_PIT_linear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/05.01_acceleration_Kalman.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/05.01_acceleration_Kalman.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/05.02_transform_to_ship.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/05.02_transform_to_ship.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/05.03_cutting.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/05.03_cutting.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/05.semiempirical_rudder_wpcc.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/05.semiempirical_rudder_wpcc.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/06.01_linear_VMM.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/06.01_linear_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/06.01_linear_simplified_VMM.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/06.01_linear_simplified_VMM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/06.02_linear_VMM_wPCC_brix.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/06.02_linear_VMM_wPCC_brix.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/07.03_PIT_static_forces_nonlinear.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/07.03_PIT_static_forces_nonlinear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/07_01_static_forces_from_model_test.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/07_01_static_forces_from_model_test.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/07_02_static_forces_from_spirals.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/07_02_static_forces_from_spirals.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/07_05_static_forces_from_model_test-many.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/07_05_static_forces_from_model_test-many.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/08_01_PIT_summary.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/08_01_PIT_summary.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/08_02_PIT_nonlinear_summary.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/08_02_PIT_nonlinear_summary.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/09_01_PIT_tongton.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/09_01_PIT_tongton.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/09_02_PIT_tongton_SI.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/09_02_PIT_tongton_SI.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/10.01_EOM_air.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/10.01_EOM_air.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/10.02_kalman_PIT_sensitivity.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/10.02_kalman_PIT_sensitivity.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/10.03_lowpass_PIT.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/10.03_lowpass_PIT.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/11.01_regression_revisited.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/11.01_regression_revisited.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.01_regression_simulated_data.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.01_regression_simulated_data.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.02_regression_simulated_data_nonlinear_EOM.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.02_regression_simulated_data_nonlinear_EOM.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.03_regression_simulated_data_mariner.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.03_regression_simulated_data_mariner.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.04_regression_too_little_simulated_data.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.04_regression_too_little_simulated_data.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.05.5_regression_simulated_data_simple_nonlinear_BDF.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.05.5_regression_simulated_data_simple_nonlinear_BDF.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.05_regression_simulated_data_acc_thrust.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.05_regression_simulated_data_acc_thrust.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.05_regression_simulated_data_simple_nonlinear.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.05_regression_simulated_data_simple_nonlinear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.06.5_regression_simulated_data_BDF_numerical_gradient.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.06.5_regression_simulated_data_BDF_numerical_gradient.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.06_regression_simulated_data_numerical_gradient.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.06_regression_simulated_data_numerical_gradient.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.07_regression_simulated_data_better_numerical_gradient.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.07_regression_simulated_data_better_numerical_gradient.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.08_regression_simulated_data_gausian_noise.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.08_regression_simulated_data_gausian_noise.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/12.08_regression_simulated_more_data_gausian_noise.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/12.08_regression_simulated_more_data_gausian_noise.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/13.01_solve_ivp.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/13.01_solve_ivp.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/14.01_EM_algorithm.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/14.01_EM_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/14.01_hidden_states.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/14.01_hidden_states.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/14.02_hidden_states_gradient_regression.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/14.02_hidden_states_gradient_regression.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/14.03_hidden_states_gradient_regression_linear.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/14.03_hidden_states_gradient_regression_linear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.01_kalman_filter_unvariate.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.01_kalman_filter_unvariate.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.10_kalman_filter_multivariate.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.10_kalman_filter_multivariate.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.11_kalman_filter_linear_manoeuvring.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.11_kalman_filter_linear_manoeuvring.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.20_EM-algorithm.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.20_EM-algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.30_KF_fossen.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.30_KF_fossen.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.31_EKF_fossen.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.31_EKF_fossen.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.39_KF_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.39_KF_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.40_EKF_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.40_EKF_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.41_EKF_PIT_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.41_EKF_PIT_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.42_EKF_EM_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.42_EKF_EM_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.42_EKF_PIT_2_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.42_EKF_PIT_2_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.44_KF_EM_RTS_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.44_KF_EM_RTS_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.45_KF_EM_RTS_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.45_KF_EM_RTS_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.46_EKF_Abkowitz.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.46_EKF_Abkowitz.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.47_EKF_3DOF.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.47_EKF_3DOF.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.47_EKF_3DOF.py` & `vessel_manoeuvring_models-0.0.6/notebooks/15.47_EKF_3DOF.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.48_EK_smoother_3DOF.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.48_EK_smoother_3DOF.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.49_EK_smoother_3DOF_thrust.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.49_EK_smoother_3DOF_thrust.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.50_KF_EM_RTS_nomoto.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.50_KF_EM_RTS_nomoto.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.51_EK_inverse_dynamics.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.51_EK_inverse_dynamics.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/15.52_inverse_static.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/15.52_inverse_static.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/16.01_PIT_VCT_revisited_linear.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/16.01_PIT_VCT_revisited_linear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/16.02_PIT_VCT_revisited_nonlinear.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/16.02_PIT_VCT_revisited_nonlinear.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/16.03_model_simulate.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/16.03_model_simulate.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/17.01_RTS_manoeuvring_PIT.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/17.01_RTS_manoeuvring_PIT.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/21.01_parameter_drift.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/21.01_parameter_drift.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/21.02_parameter_drift.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/21.02_parameter_drift.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/21.03_parameter_drift.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/21.03_parameter_drift.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/21.04_perfect_captive.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/21.04_perfect_captive.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/21.05_perfect_captive_truncated.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/21.05_perfect_captive_truncated.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/22.01_scaling_VCT_captive.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/22.01_scaling_VCT_captive.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/30.01_joke.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/30.01_joke.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/ai_research.png` & `vessel_manoeuvring_models-0.0.6/notebooks/ai_research.png`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/example_ship2.py` & `vessel_manoeuvring_models-0.0.6/notebooks/example_ship2.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/imports.py` & `vessel_manoeuvring_models-0.0.6/notebooks/imports.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/logbook.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/logbook.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/matplotlibrc` & `vessel_manoeuvring_models-0.0.6/notebooks/matplotlibrc`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/research.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/research.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/model_simulate/01.01_run_simulations.py` & `vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/01.01_run_simulations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/model_simulate/02.01_analyze_runs.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/02.01_analyze_runs.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/notebooks/model_simulate/templates/16.03_model_simulate.ipynb` & `vessel_manoeuvring_models-0.0.6/notebooks/model_simulate/templates/16.03_model_simulate.ipynb`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_EKF_PIT_Nomot.py` & `vessel_manoeuvring_models-0.0.6/tests/test_EKF_PIT_Nomot.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_KF_Nomoto.py` & `vessel_manoeuvring_models-0.0.6/tests/test_KF_Nomoto.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_extended_kalman_filter.py` & `vessel_manoeuvring_models-0.0.6/tests/test_extended_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_extended_kalman_vmm.py` & `vessel_manoeuvring_models-0.0.6/tests/test_extended_kalman_vmm.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_force_regression.py` & `vessel_manoeuvring_models-0.0.6/tests/test_force_regression.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_kalman_filter.py` & `vessel_manoeuvring_models-0.0.6/tests/test_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_linear_vmm.py` & `vessel_manoeuvring_models-0.0.6/tests/test_linear_vmm.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_model_simulator.py` & `vessel_manoeuvring_models-0.0.6/tests/test_model_simulator.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_parameter_denominator.py` & `vessel_manoeuvring_models-0.0.6/tests/test_parameter_denominator.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_prime_system.py` & `vessel_manoeuvring_models-0.0.6/tests/test_prime_system.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_rts_smoother.py` & `vessel_manoeuvring_models-0.0.6/tests/test_rts_smoother.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/tests/test_vmm_simple_nonliear.py` & `vessel_manoeuvring_models-0.0.6/tests/test_vmm_simple_nonliear.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/bias_variance_tradeoff.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/bias_variance_tradeoff.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/extended_kalman_filter.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/extended_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/extended_kalman_vmm.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/extended_kalman_vmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
                 len(missing_coefficients) == 0
             ), f"Missing parameters:{missing_coefficients}"
         else:
             replace = pd.Series(
                 data=np.zeros(len(missing_coefficients)),
                 index=list(missing_coefficients),
             )
-            parameters = parameters.append(replace)  # Set missing coefficients to 0!
+            parameters = pd.concat((parameters, replace))  # Set missing coefficients to 0!
 
         return parameters[coefficients].copy()
 
     def extract_needed_ship_parameters(self, ship_parameters):
 
         s = signature(self._lambda_f)
         keys = list(set(ship_parameters) & set(s.parameters.keys()))
```

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/feature_selection.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/feature_selection.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/kalman_filter.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/linear_vmm_equations.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/linear_vmm_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/linear_vmm_simplified_equations.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/linear_vmm_simplified_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/mlflow_utils.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/nonlinear_abkowitz_vmm_equations.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_abkowitz_vmm_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/nonlinear_martin_vmm_equations.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_martin_vmm_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/nonlinear_vmm_equations.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/nonlinear_vmm_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/notebook_to_latex.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/notebook_to_latex.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/parameters.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/parameters.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/prime_system.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/prime_system.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/substitute_dynamic_symbols.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/substitute_dynamic_symbols.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/symbols.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/symbols.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/system_equations.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/system_equations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/twin_simulations.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/twin_simulations.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/vct_scaling.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/vct_scaling.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/vmm_equations_VCT.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/vmm_equations_VCT.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/case_0.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/case_0.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/case_1.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/case_1.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/kalman_filter.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/make_dataset.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/make_dataset.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/mdl.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/mdl.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/data/wpcc.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/data/wpcc.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/MMG_hull.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_hull.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/MMG_propeller.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_propeller.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/MMG_rudder.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/MMG_rudder.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/brix_coefficients.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/brix_coefficients.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/captive_variation.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/captive_variation.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/diff_eq_to_matrix.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/diff_eq_to_matrix.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/force_from_motion.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/force_from_motion.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/nonlinear_vmm.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/nonlinear_vmm.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/propeller.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/propeller.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/regression.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 
         if data is None:
             data = self.data_prime
 
         X = diff_eq.calculate_features(data=data_prime)
 
         parameters_all = self.parameters["regressed"].copy()
-        parameters_all = parameters_all.append(self.exclude_parameters)
+        parameters_all = pd.concat((parameters_all, self.exclude_parameters))
 
         columns = list(set(parameters_all.index) & set(X.columns))
         parameters = parameters_all.loc[columns]
 
         force = X * parameters
         units = {key: unit for key in force.columns}
 
@@ -364,15 +364,15 @@
             df_parameters_all.drop(columns=["brix_lambda"], inplace=True)
 
         df_parameters_all["regressed"] = df_parameters_all["regressed"].combine_first(
             df_parameters_all["prime"]
         )  # prefer regressed
 
         parameters = df_parameters_all["regressed"]
-        parameters = parameters.append(self.exclude_parameters)
+        parameters = pd.concat((parameters, self.exclude_parameters))
 
         if model_pos is None:
 
             return ModelSimulator(
                 simulator=self.simulator,
                 parameters=parameters,
                 ship_parameters=self.ship_parameters,
@@ -562,33 +562,33 @@
         if "Yur" in self.result_summaries["Y"].index:
             self.result_summaries["Y"].loc["Yur", "decoupled"] += m_
 
         if "Nur" in self.result_summaries["N"].index:
             self.result_summaries["N"].loc["Nur", "decoupled"] += m_ * x_G_
 
         B_coeff_bse = self.model_Y.bse
-        B_coeff_bse = B_coeff_bse.append(
+        B_coeff_bse = pd.concat((B_coeff_bse, 
             pd.Series({key: 0 for key in self.connected_parameters_Y.keys()})
-        )
+        ))
         B_coeff_bse.sort_index(inplace=True)
 
         stds = run(
             A_lambda,
             A_coeff=self.model_X.bse.values,
             B_coeff=B_coeff_bse.values,
             C_coeff=self.model_N.bse.values,
             **self.parameters,
             **self.added_masses,
             **ship_parameters_prime,
         )
 
         self.std = pd.Series()
-        self.std = self.std.append(pd.Series(stds[0][0], index=self.model_X.bse.index))
-        self.std = self.std.append(pd.Series(stds[1][0], index=B_coeff_bse.index))
-        self.std = self.std.append(pd.Series(stds[2][0], index=self.model_N.bse.index))
+        self.std = pd.concat((self.std, pd.Series(stds[0][0], index=self.model_X.bse.index)))
+        self.std = pd.concat((self.std, pd.Series(stds[1][0], index=B_coeff_bse.index)))
+        self.std = pd.concat((self.std, pd.Series(stds[2][0], index=self.model_N.bse.index)))
 
         covs = run(
             A_lambda,
             A_coeff=self.model_X.cov_HC0,
             B_coeff=self.model_Y.cov_HC0,
             C_coeff=self.model_N.cov_HC0,
             **self.parameters,
```

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/result.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/result.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_MMG.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_MMG.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_abkowitz.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_abkowitz_expanded.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz_expanded.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_abkowitz_no_thrust.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_abkowitz_no_thrust.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_air.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_air.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_gsi.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_gsi.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_linear.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_linear.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_mariner.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_mariner.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_martin.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_martin_linear.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin_linear.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_martin_simple.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_martin_simple.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_nonlinear_EOM.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_nonlinear_EOM.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_perturbed.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_perturbed.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_simple.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_simple.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vmm_simple_nonlinear.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vmm_simple_nonlinear.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/models/vessels/mariner.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/models/vessels/mariner.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/book_format.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/book_format.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/equation.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/equation.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/plot.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/vessel_manoeuvring_models/visualization/regression.py` & `vessel_manoeuvring_models-0.0.6/vessel_manoeuvring_models/visualization/regression.py`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/LICENSE` & `vessel_manoeuvring_models-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vessel_manoeuvring_models-0.0.4/pyproject.toml` & `vessel_manoeuvring_models-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 description = "System identification of ship manoeuvring models"
 name = "vessel_manoeuvring_models"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.0.4"
+version = "0.0.6"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/martinlarsalbert/VesselManoeuvringModels/issues"
 "Homepage" = "https://github.com/martinlarsalbert/VesselManoeuvringModels"
 
 [build-system]
 build-backend = "hatchling.build"
```

### Comparing `vessel_manoeuvring_models-0.0.4/PKG-INFO` & `vessel_manoeuvring_models-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vessel_manoeuvring_models
-Version: 0.0.4
+Version: 0.0.6
 Summary: System identification of ship manoeuvring models
 Project-URL: Bug Tracker, https://github.com/martinlarsalbert/VesselManoeuvringModels/issues
 Project-URL: Homepage, https://github.com/martinlarsalbert/VesselManoeuvringModels
 Author-email: Martin Alexandersson <maralex@chalmers.se>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

