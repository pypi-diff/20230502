# Comparing `tmp/PyCBC-2.1.2.tar.gz` & `tmp/PyCBC-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyCBC-2.1.2.tar", last modified: Tue May  2 09:47:07 2023, max compression
+gzip compressed data, was "dist/PyCBC-2.2.0.tar", last modified: Thu Mar  9 21:19:37 2023, max compression
```

## Comparing `PyCBC-2.1.2.tar` & `PyCBC-2.2.0.tar`

### file list

```diff
@@ -1,825 +1,825 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35141 2023-05-02 09:46:59.000000 PyCBC-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-02 09:46:59.000000 PyCBC-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4018 2023-05-02 09:47:07.000000 PyCBC-2.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/PyCBC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4018 2023-05-02 09:47:07.000000 PyCBC-2.1.2/PyCBC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23744 2023-05-02 09:47:07.000000 PyCBC-2.1.2/PyCBC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 09:47:07.000000 PyCBC-2.1.2/PyCBC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      372 2023-05-02 09:47:07.000000 PyCBC-2.1.2/PyCBC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-02 09:47:07.000000 PyCBC-2.1.2/PyCBC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-05-02 09:46:59.000000 PyCBC-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/all_sky_search/
--rwxr-xr-x   0 runner    (1001) docker     (122)    29737 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_add_statmap
--rw-r--r--   0 runner    (1001) docker     (122)     4231 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_apply_rerank
--rw-r--r--   0 runner    (1001) docker     (122)     3897 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_average_psd
--rw-r--r--   0 runner    (1001) docker     (122)     6355 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_bin_trigger_rates_dq
--rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_calculate_dq
--rw-r--r--   0 runner    (1001) docker     (122)     2483 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_calculate_dqflag
--rwxr-xr-x   0 runner    (1001) docker     (122)     4844 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_calculate_psd
--rw-r--r--   0 runner    (1001) docker     (122)    22979 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_findtrigs
--rwxr-xr-x   0 runner    (1001) docker     (122)    14108 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_hdfinjfind
--rwxr-xr-x   0 runner    (1001) docker     (122)     6098 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_mergetrigs
--rwxr-xr-x   0 runner    (1001) docker     (122)    21534 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_statmap
--rw-r--r--   0 runner    (1001) docker     (122)     7186 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_statmap_inj
--rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_combine_coincident_events
--rwxr-xr-x   0 runner    (1001) docker     (122)     8387 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_combine_statmap
--rw-r--r--   0 runner    (1001) docker     (122)     6174 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_cut_merge_triggers_to_tmpltbank
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_distribute_background_bins
--rw-r--r--   0 runner    (1001) docker     (122)    11088 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_dtphase
--rw-r--r--   0 runner    (1001) docker     (122)     4732 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_exclude_zerolag
--rw-r--r--   0 runner    (1001) docker     (122)    19787 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_binned
--rwxr-xr-x   0 runner    (1001) docker     (122)    16852 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_by_template
--rwxr-xr-x   0 runner    (1001) docker     (122)    13721 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_over_multiparam
--rw-r--r--   0 runner    (1001) docker     (122)     9377 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_over_param
--rw-r--r--   0 runner    (1001) docker     (122)    21126 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_split_binned
--rw-r--r--   0 runner    (1001) docker     (122)     3445 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_followup_file
--rwxr-xr-x   0 runner    (1001) docker     (122)     2121 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_foreground_censor
--rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_get_loudest_params
--rwxr-xr-x   0 runner    (1001) docker     (122)     2490 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_merge_psds
--rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_plot_kde_vals
--rw-r--r--   0 runner    (1001) docker     (122)     2471 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_reduce_template_bank
--rw-r--r--   0 runner    (1001) docker     (122)     5084 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_rerank_dq
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_rerank_passthrough
--rw-r--r--   0 runner    (1001) docker     (122)     7429 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_sngls_findtrigs
--rw-r--r--   0 runner    (1001) docker     (122)    16771 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_sngls_pastro
--rwxr-xr-x   0 runner    (1001) docker     (122)    16627 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_sngls_statmap
--rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_sngls_statmap_inj
--rw-r--r--   0 runner    (1001) docker     (122)     2580 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_strip_injections
--rw-r--r--   0 runner    (1001) docker     (122)     8682 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_template_kde_calc
--rw-r--r--   0 runner    (1001) docker     (122)     4798 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/all_sky_search/pycbc_template_recovery_hist
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/bank/
--rw-r--r--   0 runner    (1001) docker     (122)     7665 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/bank/pycbc_aligned_bank_cat
--rw-r--r--   0 runner    (1001) docker     (122)    12145 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/bank/pycbc_aligned_stoch_bank
--rw-r--r--   0 runner    (1001) docker     (122)    12618 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/bank/pycbc_bank_verification
--rw-r--r--   0 runner    (1001) docker     (122)    17070 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/bank/pycbc_brute_bank
--rw-r--r--   0 runner    (1001) docker     (122)     4926 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/bank/pycbc_coinc_bank2hdf
--rw-r--r--   0 runner    (1001) docker     (122)    17389 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/bank/pycbc_geom_aligned_2dstack
--rw-r--r--   0 runner    (1001) docker     (122)    23518 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/bank/pycbc_geom_aligned_bank
--rw-r--r--   0 runner    (1001) docker     (122)    13737 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/bank/pycbc_geom_nonspinbank
--rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/bank/pycbc_tmpltbank_to_chi_params
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/hwinj/
--rw-r--r--   0 runner    (1001) docker     (122)    22443 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/hwinj/pycbc_generate_hwinj
--rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/hwinj/pycbc_generate_hwinj_from_xml
--rw-r--r--   0 runner    (1001) docker     (122)     2994 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/hwinj/pycbc_insert_frame_hwinj
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/hwinj/pycbc_plot_hwinj
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/inference/
--rw-r--r--   0 runner    (1001) docker     (122)     6405 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference
--rw-r--r--   0 runner    (1001) docker     (122)     4169 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_create_fits
--rw-r--r--   0 runner    (1001) docker     (122)     7268 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_extract_samples
--rw-r--r--   0 runner    (1001) docker     (122)     5736 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_model_stats
--rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_monitor
--rw-r--r--   0 runner    (1001) docker     (122)     3942 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_acceptance_rate
--rw-r--r--   0 runner    (1001) docker     (122)     5628 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_acf
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_acl
--rw-r--r--   0 runner    (1001) docker     (122)     2603 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_dynesty_run
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_dynesty_traceplot
--rw-r--r--   0 runner    (1001) docker     (122)     4461 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_gelman_rubin
--rw-r--r--   0 runner    (1001) docker     (122)     4883 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_geweke
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_inj_recovery
--rw-r--r--   0 runner    (1001) docker     (122)     6414 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_mcmc_history
--rw-r--r--   0 runner    (1001) docker     (122)    15034 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_movie
--rw-r--r--   0 runner    (1001) docker     (122)    13533 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_posterior
--rw-r--r--   0 runner    (1001) docker     (122)     5830 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_pp
--rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_prior
--rw-r--r--   0 runner    (1001) docker     (122)     4922 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_samples
--rw-r--r--   0 runner    (1001) docker     (122)     2241 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_skymap
--rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_plot_thermodynamic_integrand
--rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_pp_table_summary
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_start_from_samples
--rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_inference_table_summary
--rw-r--r--   0 runner    (1001) docker     (122)     2360 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/pycbc_validate_test_posterior
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/inference/run_pycbc_inference
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/live/
--rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/live/pycbc_live_combine_single_fits
--rw-r--r--   0 runner    (1001) docker     (122)     7531 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/live/pycbc_live_plot_combined_single_fits
--rw-r--r--   0 runner    (1001) docker     (122)     6561 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/live/pycbc_live_plot_single_trigger_fits
--rw-r--r--   0 runner    (1001) docker     (122)    17303 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/live/pycbc_live_single_trigger_fits
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/minifollowups/
--rw-r--r--   0 runner    (1001) docker     (122)    10521 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/minifollowups/pycbc_foreground_minifollowup
--rw-r--r--   0 runner    (1001) docker     (122)    13661 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/minifollowups/pycbc_injection_minifollowup
--rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/minifollowups/pycbc_page_coincinfo
--rw-r--r--   0 runner    (1001) docker     (122)     4476 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/minifollowups/pycbc_page_injinfo
--rw-r--r--   0 runner    (1001) docker     (122)     8423 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/minifollowups/pycbc_page_snglinfo
--rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/minifollowups/pycbc_plot_chigram
--rw-r--r--   0 runner    (1001) docker     (122)     4714 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/minifollowups/pycbc_plot_trigger_timeseries
--rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/minifollowups/pycbc_single_template_plot
--rw-r--r--   0 runner    (1001) docker     (122)     9897 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/minifollowups/pycbc_sngl_minifollowup
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     5543 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_banksim_plot_eff_fitting_factor
--rw-r--r--   0 runner    (1001) docker     (122)     5769 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_banksim_plot_fitting_factors
--rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_banksim_table_point_injs
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_create_html_snippet
--rwxr-xr-x   0 runner    (1001) docker     (122)     5359 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_faithsim_plots
--rw-r--r--   0 runner    (1001) docker     (122)    10855 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_ifar_catalog
--rw-r--r--   0 runner    (1001) docker     (122)     3604 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_mass_area_plot
--rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_mchirp_plots
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_banktriggerrate
--rw-r--r--   0 runner    (1001) docker     (122)     7937 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_coinc_snrchi
--rwxr-xr-x   0 runner    (1001) docker     (122)     8513 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_foreground
--rw-r--r--   0 runner    (1001) docker     (122)    10669 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_foundmissed
--rw-r--r--   0 runner    (1001) docker     (122)    13695 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_ifar
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_injtable
--rw-r--r--   0 runner    (1001) docker     (122)     9894 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_recovery
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_segments
--rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_segplot
--rw-r--r--   0 runner    (1001) docker     (122)     7188 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_segtable
--rwxr-xr-x   0 runner    (1001) docker     (122)    16396 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_sensitivity
--rw-r--r--   0 runner    (1001) docker     (122)     3263 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_snrchi
--rw-r--r--   0 runner    (1001) docker     (122)    15425 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_snrifar
--rwxr-xr-x   0 runner    (1001) docker     (122)    10377 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_snrratehist
--rw-r--r--   0 runner    (1001) docker     (122)     3452 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_page_vetotable
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_background_coincs
--rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_bank_bins
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_dq_likelihood_vs_time
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_dq_percentiles
--rwxr-xr-x   0 runner    (1001) docker     (122)     8101 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_gate_triggers
--rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_gating
--rw-r--r--   0 runner    (1001) docker     (122)     5504 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_hist
--rwxr-xr-x   0 runner    (1001) docker     (122)    11670 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_multiifo_dtphase
--rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_psd_file
--rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_psd_timefreq
--rw-r--r--   0 runner    (1001) docker     (122)    11089 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_qscan
--rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_range
--rw-r--r--   0 runner    (1001) docker     (122)     3544 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_range_vs_mtot
--rw-r--r--   0 runner    (1001) docker     (122)    10339 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_singles_timefreq
--rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_singles_vs_params
--rwxr-xr-x   0 runner    (1001) docker     (122)     2937 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_throughput
--rw-r--r--   0 runner    (1001) docker     (122)    12162 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_trigrate
--rw-r--r--   0 runner    (1001) docker     (122)     5888 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_vt_ratio
--rw-r--r--   0 runner    (1001) docker     (122)     8450 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/plotting/pycbc_plot_waveform
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/population/
--rw-r--r--   0 runner    (1001) docker     (122)    16341 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/population/pycbc_multiifo_pastro
--rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/population/pycbc_population_plots
--rw-r--r--   0 runner    (1001) docker     (122)     7417 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/population/pycbc_population_rates
--rw-r--r--   0 runner    (1001) docker     (122)    19520 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_banksim
--rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_banksim_combine_banks
--rw-r--r--   0 runner    (1001) docker     (122)     7343 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_banksim_match_combine
--rw-r--r--   0 runner    (1001) docker     (122)    22157 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_banksim_skymax
--rw-r--r--   0 runner    (1001) docker     (122)     7820 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_coinc_time
--rwxr-xr-x   0 runner    (1001) docker     (122)     9082 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_compress_bank
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_condition_strain
--rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_copy_output_map
--rw-r--r--   0 runner    (1001) docker     (122)    11438 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_create_injections
--rwxr-xr-x   0 runner    (1001) docker     (122)     1962 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_data_store
--rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_faithsim
--rwxr-xr-x   0 runner    (1001) docker     (122)     2395 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_faithsim_collect_results
--rw-r--r--   0 runner    (1001) docker     (122)    17380 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_fit_sngl_trigs
--rw-r--r--   0 runner    (1001) docker     (122)     9008 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_get_ffinal
--rwxr-xr-x   0 runner    (1001) docker     (122)     5952 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_hdf5_splitbank
--rw-r--r--   0 runner    (1001) docker     (122)     2356 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_hdf_splitinj
--rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_inj_cut
--rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_inspinj2hdf
--rw-r--r--   0 runner    (1001) docker     (122)    24465 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_inspiral
--rwxr-xr-x   0 runner    (1001) docker     (122)    18972 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_inspiral_skymax
--rwxr-xr-x   0 runner    (1001) docker     (122)    56280 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_live
--rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_live_nagios_monitor
--rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_losc_segment_query
--rw-r--r--   0 runner    (1001) docker     (122)    17345 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_make_banksim
--rw-r--r--   0 runner    (1001) docker     (122)    12546 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_make_faithsim
--rw-r--r--   0 runner    (1001) docker     (122)    11717 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_make_html_page
--rwxr-xr-x   0 runner    (1001) docker     (122)    25365 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_make_skymap
--rwxr-xr-x   0 runner    (1001) docker     (122)     3782 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_merge_inj_hdf
--rwxr-xr-x   0 runner    (1001) docker     (122)    30868 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_multi_inspiral
--rw-r--r--   0 runner    (1001) docker     (122)    15327 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_optimal_snr
--rwxr-xr-x   0 runner    (1001) docker     (122)    19574 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_optimize_snr
--rw-r--r--   0 runner    (1001) docker     (122)     5790 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_process_sngls
--rw-r--r--   0 runner    (1001) docker     (122)     9080 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_randomize_inj_dist_by_optsnr
--rwxr-xr-x   0 runner    (1001) docker     (122)    20942 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_single_template
--rwxr-xr-x   0 runner    (1001) docker     (122)     3992 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_source_probability_offline
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_split_inspinj
--rw-r--r--   0 runner    (1001) docker     (122)     6922 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_splitbank
--rw-r--r--   0 runner    (1001) docker     (122)     2740 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_stageout_failed_workflow
--rw-r--r--   0 runner    (1001) docker     (122)    10902 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_submit_dax
--rwxr-xr-x   0 runner    (1001) docker     (122)    11868 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pycbc_upload_xml_to_gracedb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/pygrb/
--rw-r--r--   0 runner    (1001) docker     (122)     7925 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_grb_inj_combiner
--rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_grb_inj_finder
--rw-r--r--   0 runner    (1001) docker     (122)     7661 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_grb_trig_cluster
--rw-r--r--   0 runner    (1001) docker     (122)    15754 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_grb_trig_combiner
--rw-r--r--   0 runner    (1001) docker     (122)    20351 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_make_offline_grb_workflow
--rw-r--r--   0 runner    (1001) docker     (122)    27308 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_efficiency
--rw-r--r--   0 runner    (1001) docker     (122)     4199 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_grb_info_table
--rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_minifollowups
--rw-r--r--   0 runner    (1001) docker     (122)    37060 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_page_tables
--rw-r--r--   0 runner    (1001) docker     (122)    10830 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_chisq_veto
--rw-r--r--   0 runner    (1001) docker     (122)    10435 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_coh_ifosnr
--rw-r--r--   0 runner    (1001) docker     (122)    21948 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_injs_results
--rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_null_stats
--rw-r--r--   0 runner    (1001) docker     (122)     3831 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_skygrid
--rw-r--r--   0 runner    (1001) docker     (122)     6795 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_snr_timeseries
--rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_stats_distribution
--rw-r--r--   0 runner    (1001) docker     (122)    30510 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_pp_workflow
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/workflow_comparisons/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/workflow_comparisons/offline_search/
--rwxr-xr-x   0 runner    (1001) docker     (122)    12151 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_combine_injection_comparisons
--rwxr-xr-x   0 runner    (1001) docker     (122)    21916 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_injection_set_comparison
--rwxr-xr-x   0 runner    (1001) docker     (122)     2768 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_plot_injections_found_both_workflows
--rwxr-xr-x   0 runner    (1001) docker     (122)     3072 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_plot_injections_missed_one_workflow
--rwxr-xr-x   0 runner    (1001) docker     (122)     4595 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_plot_vt_ratio_vs_ifar
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/bin/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)    16320 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflows/pycbc_make_bank_verifier_workflow
--rwxr-xr-x   0 runner    (1001) docker     (122)    36669 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflows/pycbc_make_coinc_search_workflow
--rwxr-xr-x   0 runner    (1001) docker     (122)     4599 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflows/pycbc_make_faithsim_workflow
--rw-r--r--   0 runner    (1001) docker     (122)    15794 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflows/pycbc_make_inference_inj_workflow
--rw-r--r--   0 runner    (1001) docker     (122)    10717 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflows/pycbc_make_inference_plots_workflow
--rw-r--r--   0 runner    (1001) docker     (122)    12772 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflows/pycbc_make_inference_workflow
--rw-r--r--   0 runner    (1001) docker     (122)     8159 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflows/pycbc_make_psd_estimation_workflow
--rw-r--r--   0 runner    (1001) docker     (122)    16316 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflows/pycbc_make_sbank_workflow
--rw-r--r--   0 runner    (1001) docker     (122)    12259 2023-05-02 09:46:59.000000 PyCBC-2.1.2/bin/workflows/pycbc_make_uberbank_workflow
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/banksim/
--rw-r--r--   0 runner    (1001) docker     (122)    21402 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/banksim/injection0.xml
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/banksim/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/cal/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/cal/foton_filter_esd_saturation/
--rw-r--r--   0 runner    (1001) docker     (122)     6703 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/cal/foton_filter_esd_saturation/pycbc_check_esd_saturation.sh
--rw-r--r--   0 runner    (1001) docker     (122)     4460 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/cal/foton_filter_esd_saturation/pycbc_check_pcal_saturation.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2582 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/cal/foton_filter_esd_saturation/run_pcal_saturation_example.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/catalog/
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/catalog/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/catalog/stat.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/catalog/what.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/dataquality/
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/dataquality/hwinj.py
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/dataquality/on.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/detector/
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/detector/ant.py
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/detector/delay.py
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/detector/loc.py
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/detector/travel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/distributions/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/distributions/list_distributions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/distributions/mass_examples.py
--rw-r--r--   0 runner    (1001) docker     (122)     1986 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/distributions/mchirp_q_from_uniform_m1m2_example.py
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/distributions/sampling_from_config_example.py
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/distributions/spin_examples.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/distributions/spin_spatial_distr_example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/faith/
--rw-r--r--   0 runner    (1001) docker     (122)    21402 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/faith/injection0.xml
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/faith/pegasus_workflow_create.sh
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/faith/pegasus_workflow_submit.sh
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/faith/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/filter/
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/filter/chisq.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/filter/fir.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/filter/pass.py
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/filter/snr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/gw150914/
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/gw150914/audio.py
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/gw150914/gw150914_h1_snr.py
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/gw150914/gw150914_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/analytic-normal2d/
--rwxr-xr-x   0 runner    (1001) docker     (122)      379 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/analytic-normal2d/make_movie.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      292 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/analytic-normal2d/plot.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      174 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/analytic-normal2d/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/bbh-injection/
--rwxr-xr-x   0 runner    (1001) docker     (122)      316 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/bbh-injection/make_injection.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      649 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/bbh-injection/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      967 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/bbh-injection/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/gw150914/
--rwxr-xr-x   0 runner    (1001) docker     (122)      582 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/gw150914/plot.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      656 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/gw150914/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1149 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/gw150914/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/hierarchical/
--rwxr-xr-x   0 runner    (1001) docker     (122)      269 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/hierarchical/make_injections.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      230 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/hierarchical/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      565 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/hierarchical/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/lisa_smbhb/
--rw-r--r--   0 runner    (1001) docker     (122)     2421 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/lisa_smbhb/advanced_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/lisa_smbhb/get.sh
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/lisa_smbhb/plot.sh
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/lisa_smbhb/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/list_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/margtime/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/margtime/get.sh
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/margtime/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/margtime/run_inj.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/multisignal/
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/multisignal/get.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      369 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/multisignal/make_injections.sh
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/multisignal/rel.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      151 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/multisignal/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/multisignal/single.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/relative/
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/relative/get.sh
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/relative/plot.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      139 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/relative/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/samplers/
--rwxr-xr-x   0 runner    (1001) docker     (122)      572 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/samplers/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inference/single/
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/single/get.sh
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/single/plot.sh
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/single/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/single/run_instant.sh
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inference/single/run_marg.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/inspiral/
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inspiral/check_GW150914_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inspiral/clean.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     3586 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/inspiral/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/live/
--rwxr-xr-x   0 runner    (1001) docker     (122)     7946 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/live/check_results.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1508 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/live/generate_injections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/live/make_singles_fits_file.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6584 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/live/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/make_skymap/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/make_skymap/GW150914.sh
--rw-r--r--   0 runner    (1001) docker     (122)      553 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/make_skymap/GW170817.sh
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/make_skymap/simulated_data.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/multi_inspiral/
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/multi_inspiral/check_faceon_faceaway_trigs.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/multi_inspiral/check_gw170817_trigs.py
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/multi_inspiral/clean.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     2736 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/multi_inspiral/faceon_faceaway.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     2530 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/multi_inspiral/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/noise/
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/noise/frequency.py
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/noise/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/overlap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/psd/
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/psd/analytic.py
--rw-r--r--   0 runner    (1001) docker     (122)      884 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/psd/estimate.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/psd/read.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/search/
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/search/bank.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/search/check_job.py
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/search/gen.sh
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/search/get.sh
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/search/master.sh
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/search/stats.sh
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/search/submit.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/tmpltbank/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/tmpltbank/bank_workflow_test/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/bank_workflow_test/gen.sh
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/cleanOutput.sh
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/make_cache.sh
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testAligned.sh
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testAligned2.sh
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testAligned3.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      649 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testNonspin.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      495 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testNonspin2.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      327 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testNonspin3.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      675 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testStoch.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      449 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testStoch2.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      355 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testStoch3.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      531 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/tmpltbank/testStoch4.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/waveform/
--rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/waveform/add_waveform.py
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/waveform/match_waveform.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/waveform/plot_detwaveform.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/waveform/plot_fd_td.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/waveform/plot_freq.py
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/waveform/plot_phase.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/waveform/plot_waveform.py
--rw-r--r--   0 runner    (1001) docker     (122)      426 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/waveform/what_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/data_checker/
--rwxr-xr-x   0 runner    (1001) docker     (122)     6801 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/data_checker/daily_test.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2162 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/data_checker/get_data_example.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/data_checker/run_daily_test.sh
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/data_checker/run_get_data_example.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/dayhopecheck/
--rwxr-xr-x   0 runner    (1001) docker     (122)     7198 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/dayhopecheck/dayhopecheck.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/dayhopecheck/run_dayhopecheck.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/generic/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/generic/multilevel_subworkflow_data/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/generic/multilevel_subworkflow_data/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/generic/multilevel_subworkflow_data/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/generic/simple_subworkflow_data/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/generic/simple_subworkflow_data/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/generic/simple_subworkflow_data/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/inference/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/inference/bbh_inj-dynesty/
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/inference/bbh_inj-dynesty/create_inj_workflow.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/inference/gw150914_gw170814-dynesty/
--rwxr-xr-x   0 runner    (1001) docker     (122)      486 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/inference/gw150914_gw170814-dynesty/create_workflow.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/inference/gw150914_gw170814-emcee_pt/
--rwxr-xr-x   0 runner    (1001) docker     (122)      480 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/inference/gw150914_gw170814-emcee_pt/create_workflow.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/inference/small_test/
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/inference/small_test/gen.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/pygrb/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/pygrb/ER7/
--rwxr-xr-x   0 runner    (1001) docker     (122)      739 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/pygrb/ER7/run_er7_pygrb_offline.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/pygrb/ER8/
--rwxr-xr-x   0 runner    (1001) docker     (122)      825 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/pygrb/ER8/run_er8_pygrb_offline.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      822 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/pygrb/ER8/run_er8_pygrb_online.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/examples/workflow/pygrb/S6/
--rwxr-xr-x   0 runner    (1001) docker     (122)      866 2023-05-02 09:46:59.000000 PyCBC-2.1.2/examples/workflow/pygrb/S6/run_s6_pygrb.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/
--rw-r--r--   0 runner    (1001) docker     (122)     6207 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3219 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     6380 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/_version_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    21555 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15026 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/boundaries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/catalog/
--rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)    56098 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4141 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (122)    23038 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (122)    28467 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/distributions/
--rw-r--r--   0 runner    (1001) docker     (122)     9279 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19645 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/angular.py
--rw-r--r--   0 runner    (1001) docker     (122)    13126 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (122)    13606 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/bounded.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/constraints.py
--rw-r--r--   0 runner    (1001) docker     (122)     8901 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/external.py
--rw-r--r--   0 runner    (1001) docker     (122)     6510 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/fixedsamples.py
--rw-r--r--   0 runner    (1001) docker     (122)     9342 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (122)    14330 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/joint.py
--rw-r--r--   0 runner    (1001) docker     (122)    10257 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/mass.py
--rw-r--r--   0 runner    (1001) docker     (122)     7732 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/power_law.py
--rw-r--r--   0 runner    (1001) docker     (122)    10564 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/qnm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/sky_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    12002 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/spins.py
--rw-r--r--   0 runner    (1001) docker     (122)     5286 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/uniform.py
--rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/uniform_log.py
--rw-r--r--   0 runner    (1001) docker     (122)     4617 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/distributions/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    16663 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/dq.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/events/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13726 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/coherent.py
--rw-r--r--   0 runner    (1001) docker     (122)    53275 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/coinc.py
--rw-r--r--   0 runner    (1001) docker     (122)     6808 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/coinc_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)    15820 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/cuts.py
--rw-r--r--   0 runner    (1001) docker     (122)    49942 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/eventmgr_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (122)    10863 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/ranking.py
--rw-r--r--   0 runner    (1001) docker     (122)    13205 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/significance.py
--rw-r--r--   0 runner    (1001) docker     (122)    13294 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/simd_threshold_ccode.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/simd_threshold_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     7717 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/single.py
--rw-r--r--   0 runner    (1001) docker     (122)    84395 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/stat.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/threshold_cpu.py
--rw-r--r--   0 runner    (1001) docker     (122)     8580 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/threshold_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     9465 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/trigger_fits.py
--rw-r--r--   0 runner    (1001) docker     (122)     8750 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/triggers.py
--rw-r--r--   0 runner    (1001) docker     (122)     7572 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/events/veto.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/fft/
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/backend_cpu.py
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/backend_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/backend_mkl.py
--rw-r--r--   0 runner    (1001) docker     (122)     3126 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/backend_support.py
--rw-r--r--   0 runner    (1001) docker     (122)     3391 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/class_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    11855 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/cuda_pyfft.py
--rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/cufft.py
--rw-r--r--   0 runner    (1001) docker     (122)     8478 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/fft_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)    22514 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/fftw.py
--rw-r--r--   0 runner    (1001) docker     (122)     7186 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/fftw_pruned.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/fftw_pruned_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/func_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     6192 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/mkl.py
--rw-r--r--   0 runner    (1001) docker     (122)     3765 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/npfft.py
--rw-r--r--   0 runner    (1001) docker     (122)     4879 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/fft/parser_support.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/filter/
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3609 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/fotonfilter.py
--rw-r--r--   0 runner    (1001) docker     (122)    83046 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/matchedfilter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/matchedfilter_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/matchedfilter_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/matchedfilter_numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/qtransform.py
--rw-r--r--   0 runner    (1001) docker     (122)    15735 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/resample.py
--rw-r--r--   0 runner    (1001) docker     (122)     3116 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/simd_correlate.py
--rw-r--r--   0 runner    (1001) docker     (122)    15271 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/simd_correlate_ccode.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/simd_correlate_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/filter/zpk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/frame/
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34138 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/frame/frame.py
--rw-r--r--   0 runner    (1001) docker     (122)     5736 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/frame/losc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/frame/store.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/inference/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30844 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/burn_in.py
--rw-r--r--   0 runner    (1001) docker     (122)     8796 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/entropy.py
--rw-r--r--   0 runner    (1001) docker     (122)     8936 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/evidence.py
--rw-r--r--   0 runner    (1001) docker     (122)     6652 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/gelman_rubin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/geweke.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/inference/io/
--rw-r--r--   0 runner    (1001) docker     (122)    32158 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38576 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/base_hdf.py
--rw-r--r--   0 runner    (1001) docker     (122)    36040 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/base_mcmc.py
--rw-r--r--   0 runner    (1001) docker     (122)    16944 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/base_multitemper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/base_nested_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5298 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/cpnest.py
--rw-r--r--   0 runner    (1001) docker     (122)     7473 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/dynesty.py
--rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/emcee.py
--rw-r--r--   0 runner    (1001) docker     (122)     4859 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/emcee_pt.py
--rw-r--r--   0 runner    (1001) docker     (122)    11226 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/epsie.py
--rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/multinest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3653 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/posterior.py
--rw-r--r--   0 runner    (1001) docker     (122)     5947 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/ptemcee.py
--rw-r--r--   0 runner    (1001) docker     (122)     2421 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/txt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/io/ultranest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/inference/jump/
--rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/jump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4775 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/jump/angular.py
--rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/jump/bounded_normal.py
--rw-r--r--   0 runner    (1001) docker     (122)     5794 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/jump/discrete.py
--rw-r--r--   0 runner    (1001) docker     (122)    20231 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/jump/normal.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/inference/models/
--rw-r--r--   0 runner    (1001) docker     (122)    11258 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8703 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/analytic.py
--rw-r--r--   0 runner    (1001) docker     (122)    33142 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5697 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/base_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7614 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/brute_marg.py
--rw-r--r--   0 runner    (1001) docker     (122)    23677 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    31219 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/gated_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (122)    49252 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (122)    24411 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (122)    32990 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/marginalized_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (122)    22631 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/relbin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8733 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/relbin_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     8435 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/single_template.py
--rw-r--r--   0 runner    (1001) docker     (122)    33243 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    16324 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/option_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/inference/sampler/
--rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8201 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/base_cube.py
--rw-r--r--   0 runner    (1001) docker     (122)    36376 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/base_mcmc.py
--rw-r--r--   0 runner    (1001) docker     (122)    16327 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/base_multitemper.py
--rw-r--r--   0 runner    (1001) docker     (122)     8274 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/cpnest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/dummy.py
--rw-r--r--   0 runner    (1001) docker     (122)    23999 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/dynesty.py
--rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/emcee.py
--rw-r--r--   0 runner    (1001) docker     (122)    18909 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/emcee_pt.py
--rw-r--r--   0 runner    (1001) docker     (122)    19831 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/epsie.py
--rw-r--r--   0 runner    (1001) docker     (122)    15427 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/multinest.py
--rw-r--r--   0 runner    (1001) docker     (122)    27259 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/ptemcee.py
--rw-r--r--   0 runner    (1001) docker     (122)     7359 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inference/sampler/ultranest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/inject/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48285 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inject/inject.py
--rw-r--r--   0 runner    (1001) docker     (122)    19409 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/inject/injfilterrejector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/io/
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    55604 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/io/hdf.py
--rw-r--r--   0 runner    (1001) docker     (122)    12494 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/io/ligolw.py
--rw-r--r--   0 runner    (1001) docker     (122)    25494 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/io/live.py
--rw-r--r--   0 runner    (1001) docker     (122)    77607 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/io/record.py
--rw-r--r--   0 runner    (1001) docker     (122)     9494 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/libutils.py
--rw-r--r--   0 runner    (1001) docker     (122)    13070 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/mchirp_area.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/neutron_stars/
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/neutron_stars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6861 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/neutron_stars/eos_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/neutron_stars/ns_data/
--rw-r--r--   0 runner    (1001) docker     (122)    53263 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/neutron_stars/ns_data/equil_2H.dat
--rw-r--r--   0 runner    (1001) docker     (122)    11046 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/neutron_stars/pg_isso_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/noise/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5192 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/noise/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (122)     8316 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/noise/reproduceable.py
--rw-r--r--   0 runner    (1001) docker     (122)     5385 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/opt.py
--rw-r--r--   0 runner    (1001) docker     (122)    39910 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/pnutils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5462 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/population/
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30477 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/population/fgmc_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/population/fgmc_laguerre.py
--rw-r--r--   0 runner    (1001) docker     (122)    10012 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/population/fgmc_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)    10265 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/population/live_pastro.py
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/population/live_pastro_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    16559 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/population/population_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    13826 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/population/rates_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    16956 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/population/scale_injections.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/psd/
--rw-r--r--   0 runner    (1001) docker     (122)    28796 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/psd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6263 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/psd/analytical.py
--rw-r--r--   0 runner    (1001) docker     (122)    22380 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/psd/analytical_space.py
--rw-r--r--   0 runner    (1001) docker     (122)    12318 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/psd/estimate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7153 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/psd/read.py
--rw-r--r--   0 runner    (1001) docker     (122)     8554 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/psd/variation.py
--rw-r--r--   0 runner    (1001) docker     (122)    12540 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/rate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/
--rw-r--r--   0 runner    (1001) docker     (122)      423 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/color.py
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/dq.py
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/followup.py
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/layout.py
--rw-r--r--   0 runner    (1001) docker     (122)     4692 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/legacy_grb.py
--rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/mpld3_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/psd.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/pygrb_plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    38592 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/pygrb_postprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7996 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/render.py
--rw-r--r--   0 runner    (1001) docker     (122)    33143 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/scatter_histograms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/css/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/css/bootstrap/3.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)   117150 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/css/bootstrap/3.3.2/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   117150 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/css/fancybox/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/css/fancybox/2.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)     4902 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/css/fancybox/2.1.5/jquery.fancybox.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/css/pycbc/
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/css/pycbc/orange.css
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/css/pycbc/red.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Light.css
--rw-r--r--   0 runner    (1001) docker     (122)   258264 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Light.eot
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Light.html
--rw-r--r--   0 runner    (1001) docker     (122)   658924 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   312760 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Light.woff
--rw-r--r--   0 runner    (1001) docker     (122)      436 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Semibold.css
--rw-r--r--   0 runner    (1001) docker     (122)   270560 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Semibold.eot
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Semibold.html
--rw-r--r--   0 runner    (1001) docker     (122)   702616 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Semibold.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   326132 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Semibold.woff
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/js/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/js/bootstrap/3.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35452 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/js/bootstrap/3.3.2/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (122)    35452 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/js/fancybox/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/js/fancybox/2.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/js/fancybox/2.1.5/fancybox-orange.js
--rwxr-xr-x   0 runner    (1001) docker     (122)    48706 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.js
--rwxr-xr-x   0 runner    (1001) docker     (122)    23135 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.pack.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/js/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/static/js/jquery/1.10.2/
--rw-r--r--   0 runner    (1001) docker     (122)    93107 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/js/jquery/1.10.2/jquery-1.10.2.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     1384 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/js/jquery/1.10.2/jquery.mousewheel-3.0.6.pack.js
--rw-r--r--   0 runner    (1001) docker     (122)    95786 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     9027 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4698 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/table_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/templates/files/
--rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/templates/files/file_default.html
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/templates/files/file_glitchgram.html
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/templates/files/file_img.html
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/templates/files/file_pre.html
--rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/templates/files/file_tmplt.html
--rw-r--r--   0 runner    (1001) docker     (122)    11740 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/templates/orange.html
--rw-r--r--   0 runner    (1001) docker     (122)    11734 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/templates/red.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/results/templates/wells/
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/templates/wells/sitemap.html
--rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/templates/wells/two_column.html
--rw-r--r--   0 runner    (1001) docker     (122)     7878 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/results/versioning.py
--rw-r--r--   0 runner    (1001) docker     (122)    10948 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/scheme.py
--rw-r--r--   0 runner    (1001) docker     (122)    11609 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/strain/
--rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/strain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/strain/calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     6383 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/strain/gate.py
--rw-r--r--   0 runner    (1001) docker     (122)     8123 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/strain/lines.py
--rw-r--r--   0 runner    (1001) docker     (122)    18783 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/strain/recalibrate.py
--rw-r--r--   0 runner    (1001) docker     (122)    91153 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/strain/strain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/tmpltbank/
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4865 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/bank_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    12504 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/bank_output_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    23515 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/brute_force_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)    23569 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/calc_moments.py
--rw-r--r--   0 runner    (1001) docker     (122)    33431 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/coord_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10726 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/lambda_mapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/lattice_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    57132 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/option_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    28137 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/tmpltbank/partitioned_bank.py
--rw-r--r--   0 runner    (1001) docker     (122)    84293 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/types/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/types/aligned.py
--rw-r--r--   0 runner    (1001) docker     (122)    39845 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/types/array.py
--rw-r--r--   0 runner    (1001) docker     (122)     5421 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/types/array_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (122)    11741 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/types/array_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)    26102 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/types/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    25727 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/types/frequencyseries.py
--rw-r--r--   0 runner    (1001) docker     (122)    21934 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/types/optparse.py
--rw-r--r--   0 runner    (1001) docker     (122)    45520 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/types/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)      768 2023-05-02 09:47:05.000000 PyCBC-2.1.2/pycbc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/vetoes/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/vetoes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12524 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/vetoes/autochisq.py
--rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/vetoes/bank_chisq.py
--rw-r--r--   0 runner    (1001) docker     (122)    19668 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/vetoes/chisq.py
--rw-r--r--   0 runner    (1001) docker     (122)     4964 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/vetoes/chisq_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (122)    12354 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/vetoes/chisq_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     7224 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/vetoes/sgchisq.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/waveform/
--rw-r--r--   0 runner    (1001) docker     (122)    18361 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/SpinTaylorF2.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    39507 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/bank.py
--rw-r--r--   0 runner    (1001) docker     (122)    30086 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/compress.py
--rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/decompress_cpu.py
--rw-r--r--   0 runner    (1001) docker     (122)     9811 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/decompress_cpu_ccode.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3580 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/decompress_cpu_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (122)    11138 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/decompress_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)    51496 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3724 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/multiband.py
--rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/nltides.py
--rw-r--r--   0 runner    (1001) docker     (122)    29135 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     4171 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/premerger.py
--rw-r--r--   0 runner    (1001) docker     (122)    15018 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/pycbc_phenomC_tmplt.py
--rw-r--r--   0 runner    (1001) docker     (122)    54746 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/ringdown.py
--rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/sinegauss.py
--rw-r--r--   0 runner    (1001) docker     (122)     8829 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/spa_tmplt.py
--rw-r--r--   0 runner    (1001) docker     (122)     6584 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/spa_tmplt_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     3243 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/spa_tmplt_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/supernovae.py
--rw-r--r--   0 runner    (1001) docker     (122)    19760 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4229 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/utils_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/utils_cuda.py
--rw-r--r--   0 runner    (1001) docker     (122)    57072 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/waveform.py
--rw-r--r--   0 runner    (1001) docker     (122)    11590 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/waveform/waveform_modes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/workflow/
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26619 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/coincidence.py
--rw-r--r--   0 runner    (1001) docker     (122)    10939 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/configparser_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    15824 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    88854 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    50017 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/datafind.py
--rw-r--r--   0 runner    (1001) docker     (122)     9556 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/dq.py
--rw-r--r--   0 runner    (1001) docker     (122)    21408 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/grb_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    42899 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/inference_followups.py
--rw-r--r--   0 runner    (1001) docker     (122)    13587 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/injection.py
--rw-r--r--   0 runner    (1001) docker     (122)    53624 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/jobsetup.py
--rw-r--r--   0 runner    (1001) docker     (122)    13905 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/matched_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)    36429 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/minifollowups.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/pycbc/workflow/pegasus_files/
--rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/pegasus_files/pegasus-properties.conf
--rw-r--r--   0 runner    (1001) docker     (122)    11840 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/pegasus_sites.py
--rw-r--r--   0 runner    (1001) docker     (122)    32699 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/pegasus_workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    23393 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/psd.py
--rw-r--r--   0 runner    (1001) docker     (122)     5160 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/psdfiles.py
--rw-r--r--   0 runner    (1001) docker     (122)    19177 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/segment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/splittable.py
--rw-r--r--   0 runner    (1001) docker     (122)    14333 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pycbc/workflow/tmpltbank.py
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-02 09:46:59.000000 PyCBC-2.1.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 09:47:07.000000 PyCBC-2.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)    12377 2023-05-02 09:46:59.000000 PyCBC-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/bankvetotest.py
--rw-r--r--   0 runner    (1001) docker     (122)    37722 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/fft_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16620 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/lalsim.py
--rw-r--r--   0 runner    (1001) docker     (122)    21211 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     5083 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_array_lal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6519 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_autochisq.py
--rw-r--r--   0 runner    (1001) docker     (122)     2989 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     4885 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_chisq.py
--rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_coinc_stat.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_correlate.py
--rw-r--r--   0 runner    (1001) docker     (122)     8904 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_cuts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)    11134 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_fft_mkl_threaded.py
--rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_fft_unthreaded.py
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_fftw_openmp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_fftw_pthreads.py
--rw-r--r--   0 runner    (1001) docker     (122)     6510 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (122)    24440 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_frequencyseries.py
--rw-r--r--   0 runner    (1001) docker     (122)     7338 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_infmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_injection.py
--rw-r--r--   0 runner    (1001) docker     (122)     6282 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_io_live.py
--rw-r--r--   0 runner    (1001) docker     (122)     6818 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_live_coinc_compare.py
--rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_matchedfilter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_pnutils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5934 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_psd.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (122)     7707 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_schemes.py
--rw-r--r--   0 runner    (1001) docker     (122)     7904 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_significance_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    19047 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_skymax.py
--rw-r--r--   0 runner    (1001) docker     (122)     3434 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_spatmplt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_threshold.py
--rw-r--r--   0 runner    (1001) docker     (122)    25115 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (122)    26649 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_tmpltbank.py
--rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (122)     7464 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_waveform.py
--rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/test_waveform_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    38174 2023-05-02 09:46:59.000000 PyCBC-2.1.2/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/tools/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/tools/benchmarking/
--rwxr-xr-x   0 runner    (1001) docker     (122)      822 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/benchmarking/absolute_times.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/tools/einsteinathome/
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/einsteinathome/check_GW150914_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/tools/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/tools/static/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)     3570 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/static/hooks/hook-pycbc.py
--rw-r--r--   0 runner    (1001) docker     (122)      734 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/static/runtime-scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/static/runtime-tkinter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/tools/timing/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2286 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/timing/arr_perf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 09:47:07.000000 PyCBC-2.1.2/tools/timing/banksim/
--rw-r--r--   0 runner    (1001) docker     (122)    12160 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/timing/banksim/banksim.py
--rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/timing/correlate_perf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2935 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/timing/fft_perf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3154 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/timing/match_perf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2472 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tools/timing/wav_perf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-02 09:46:59.000000 PyCBC-2.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35141 2023-03-09 21:19:31.000000 PyCBC-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-03-09 21:19:31.000000 PyCBC-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4018 2023-03-09 21:19:37.000000 PyCBC-2.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/PyCBC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4018 2023-03-09 21:19:37.000000 PyCBC-2.2.0/PyCBC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23744 2023-03-09 21:19:37.000000 PyCBC-2.2.0/PyCBC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 21:19:37.000000 PyCBC-2.2.0/PyCBC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2023-03-09 21:19:37.000000 PyCBC-2.2.0/PyCBC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-09 21:19:37.000000 PyCBC-2.2.0/PyCBC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-03-09 21:19:31.000000 PyCBC-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/all_sky_search/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    29737 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_add_statmap
+-rw-r--r--   0 runner    (1001) docker     (122)     4231 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_apply_rerank
+-rw-r--r--   0 runner    (1001) docker     (122)     3897 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_average_psd
+-rw-r--r--   0 runner    (1001) docker     (122)     6355 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_bin_trigger_rates_dq
+-rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_calculate_dq
+-rw-r--r--   0 runner    (1001) docker     (122)     2483 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_calculate_dqflag
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4844 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_calculate_psd
+-rw-r--r--   0 runner    (1001) docker     (122)    22979 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_findtrigs
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14108 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_hdfinjfind
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6098 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_mergetrigs
+-rwxr-xr-x   0 runner    (1001) docker     (122)    21534 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_statmap
+-rw-r--r--   0 runner    (1001) docker     (122)     7186 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_statmap_inj
+-rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_combine_coincident_events
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8387 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_combine_statmap
+-rw-r--r--   0 runner    (1001) docker     (122)     6174 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_cut_merge_triggers_to_tmpltbank
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_distribute_background_bins
+-rw-r--r--   0 runner    (1001) docker     (122)    11088 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_dtphase
+-rw-r--r--   0 runner    (1001) docker     (122)     4732 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_exclude_zerolag
+-rw-r--r--   0 runner    (1001) docker     (122)    19787 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_binned
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16852 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_by_template
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13721 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_over_multiparam
+-rw-r--r--   0 runner    (1001) docker     (122)     9377 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_over_param
+-rw-r--r--   0 runner    (1001) docker     (122)    21126 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_split_binned
+-rw-r--r--   0 runner    (1001) docker     (122)     3445 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_followup_file
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2121 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_foreground_censor
+-rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_get_loudest_params
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2490 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_merge_psds
+-rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_plot_kde_vals
+-rw-r--r--   0 runner    (1001) docker     (122)     2471 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_reduce_template_bank
+-rw-r--r--   0 runner    (1001) docker     (122)     5084 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_rerank_dq
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_rerank_passthrough
+-rw-r--r--   0 runner    (1001) docker     (122)     7429 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_sngls_findtrigs
+-rw-r--r--   0 runner    (1001) docker     (122)    16771 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_sngls_pastro
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16627 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_sngls_statmap
+-rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_sngls_statmap_inj
+-rw-r--r--   0 runner    (1001) docker     (122)     2580 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_strip_injections
+-rw-r--r--   0 runner    (1001) docker     (122)     8682 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_template_kde_calc
+-rw-r--r--   0 runner    (1001) docker     (122)     4798 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/all_sky_search/pycbc_template_recovery_hist
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/bank/
+-rw-r--r--   0 runner    (1001) docker     (122)     7665 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/bank/pycbc_aligned_bank_cat
+-rw-r--r--   0 runner    (1001) docker     (122)    12145 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/bank/pycbc_aligned_stoch_bank
+-rw-r--r--   0 runner    (1001) docker     (122)    12618 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/bank/pycbc_bank_verification
+-rw-r--r--   0 runner    (1001) docker     (122)    17070 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/bank/pycbc_brute_bank
+-rw-r--r--   0 runner    (1001) docker     (122)     4926 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/bank/pycbc_coinc_bank2hdf
+-rw-r--r--   0 runner    (1001) docker     (122)    17389 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/bank/pycbc_geom_aligned_2dstack
+-rw-r--r--   0 runner    (1001) docker     (122)    23518 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/bank/pycbc_geom_aligned_bank
+-rw-r--r--   0 runner    (1001) docker     (122)    13737 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/bank/pycbc_geom_nonspinbank
+-rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/bank/pycbc_tmpltbank_to_chi_params
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/hwinj/
+-rw-r--r--   0 runner    (1001) docker     (122)    22443 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/hwinj/pycbc_generate_hwinj
+-rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/hwinj/pycbc_generate_hwinj_from_xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2994 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/hwinj/pycbc_insert_frame_hwinj
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/hwinj/pycbc_plot_hwinj
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/inference/
+-rw-r--r--   0 runner    (1001) docker     (122)     6405 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference
+-rw-r--r--   0 runner    (1001) docker     (122)     4169 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_create_fits
+-rw-r--r--   0 runner    (1001) docker     (122)     7268 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_extract_samples
+-rw-r--r--   0 runner    (1001) docker     (122)     5736 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_model_stats
+-rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_monitor
+-rw-r--r--   0 runner    (1001) docker     (122)     3942 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_acceptance_rate
+-rw-r--r--   0 runner    (1001) docker     (122)     5628 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_acf
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_acl
+-rw-r--r--   0 runner    (1001) docker     (122)     2603 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_dynesty_run
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_dynesty_traceplot
+-rw-r--r--   0 runner    (1001) docker     (122)     4461 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_gelman_rubin
+-rw-r--r--   0 runner    (1001) docker     (122)     4883 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_geweke
+-rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_inj_recovery
+-rw-r--r--   0 runner    (1001) docker     (122)     6414 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_mcmc_history
+-rw-r--r--   0 runner    (1001) docker     (122)    15034 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_movie
+-rw-r--r--   0 runner    (1001) docker     (122)    13533 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_posterior
+-rw-r--r--   0 runner    (1001) docker     (122)     5830 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_pp
+-rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_prior
+-rw-r--r--   0 runner    (1001) docker     (122)     4922 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_samples
+-rw-r--r--   0 runner    (1001) docker     (122)     2241 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_skymap
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_plot_thermodynamic_integrand
+-rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_pp_table_summary
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_start_from_samples
+-rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_inference_table_summary
+-rw-r--r--   0 runner    (1001) docker     (122)     2360 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/pycbc_validate_test_posterior
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/inference/run_pycbc_inference
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/live/
+-rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/live/pycbc_live_combine_single_fits
+-rw-r--r--   0 runner    (1001) docker     (122)     7531 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/live/pycbc_live_plot_combined_single_fits
+-rw-r--r--   0 runner    (1001) docker     (122)     6561 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/live/pycbc_live_plot_single_trigger_fits
+-rw-r--r--   0 runner    (1001) docker     (122)    17164 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/live/pycbc_live_single_trigger_fits
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/minifollowups/
+-rw-r--r--   0 runner    (1001) docker     (122)    10521 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/minifollowups/pycbc_foreground_minifollowup
+-rw-r--r--   0 runner    (1001) docker     (122)    13661 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/minifollowups/pycbc_injection_minifollowup
+-rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/minifollowups/pycbc_page_coincinfo
+-rw-r--r--   0 runner    (1001) docker     (122)     4476 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/minifollowups/pycbc_page_injinfo
+-rw-r--r--   0 runner    (1001) docker     (122)     8423 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/minifollowups/pycbc_page_snglinfo
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/minifollowups/pycbc_plot_chigram
+-rw-r--r--   0 runner    (1001) docker     (122)     4714 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/minifollowups/pycbc_plot_trigger_timeseries
+-rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/minifollowups/pycbc_single_template_plot
+-rw-r--r--   0 runner    (1001) docker     (122)     9897 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/minifollowups/pycbc_sngl_minifollowup
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     5543 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_banksim_plot_eff_fitting_factor
+-rw-r--r--   0 runner    (1001) docker     (122)     5769 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_banksim_plot_fitting_factors
+-rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_banksim_table_point_injs
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_create_html_snippet
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5359 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_faithsim_plots
+-rw-r--r--   0 runner    (1001) docker     (122)    10855 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_ifar_catalog
+-rw-r--r--   0 runner    (1001) docker     (122)     3604 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_mass_area_plot
+-rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_mchirp_plots
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_banktriggerrate
+-rw-r--r--   0 runner    (1001) docker     (122)     7937 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_coinc_snrchi
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8513 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_foreground
+-rw-r--r--   0 runner    (1001) docker     (122)    10669 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_foundmissed
+-rw-r--r--   0 runner    (1001) docker     (122)    13695 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_ifar
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_injtable
+-rw-r--r--   0 runner    (1001) docker     (122)     9894 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_recovery
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_segments
+-rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_segplot
+-rw-r--r--   0 runner    (1001) docker     (122)     7188 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_segtable
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16396 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_sensitivity
+-rw-r--r--   0 runner    (1001) docker     (122)     3263 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_snrchi
+-rw-r--r--   0 runner    (1001) docker     (122)    15425 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_snrifar
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10377 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_snrratehist
+-rw-r--r--   0 runner    (1001) docker     (122)     3452 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_page_vetotable
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_background_coincs
+-rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_bank_bins
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_dq_likelihood_vs_time
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_dq_percentiles
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8101 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_gate_triggers
+-rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_gating
+-rw-r--r--   0 runner    (1001) docker     (122)     5504 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_hist
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11670 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_multiifo_dtphase
+-rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_psd_file
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_psd_timefreq
+-rw-r--r--   0 runner    (1001) docker     (122)    11089 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_qscan
+-rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_range
+-rw-r--r--   0 runner    (1001) docker     (122)     3544 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_range_vs_mtot
+-rw-r--r--   0 runner    (1001) docker     (122)    10339 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_singles_timefreq
+-rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_singles_vs_params
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2937 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_throughput
+-rw-r--r--   0 runner    (1001) docker     (122)    12162 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_trigrate
+-rw-r--r--   0 runner    (1001) docker     (122)     5888 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_vt_ratio
+-rw-r--r--   0 runner    (1001) docker     (122)     8450 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/plotting/pycbc_plot_waveform
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/population/
+-rw-r--r--   0 runner    (1001) docker     (122)    16341 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/population/pycbc_multiifo_pastro
+-rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/population/pycbc_population_plots
+-rw-r--r--   0 runner    (1001) docker     (122)     7417 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/population/pycbc_population_rates
+-rw-r--r--   0 runner    (1001) docker     (122)    19520 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_banksim
+-rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_banksim_combine_banks
+-rw-r--r--   0 runner    (1001) docker     (122)     7343 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_banksim_match_combine
+-rw-r--r--   0 runner    (1001) docker     (122)    22157 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_banksim_skymax
+-rw-r--r--   0 runner    (1001) docker     (122)     7820 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_coinc_time
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9082 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_compress_bank
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_condition_strain
+-rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_copy_output_map
+-rw-r--r--   0 runner    (1001) docker     (122)    11438 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_create_injections
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1962 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_data_store
+-rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_faithsim
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2395 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_faithsim_collect_results
+-rw-r--r--   0 runner    (1001) docker     (122)    17380 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_fit_sngl_trigs
+-rw-r--r--   0 runner    (1001) docker     (122)     9008 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_get_ffinal
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5952 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_hdf5_splitbank
+-rw-r--r--   0 runner    (1001) docker     (122)     2356 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_hdf_splitinj
+-rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_inj_cut
+-rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_inspinj2hdf
+-rw-r--r--   0 runner    (1001) docker     (122)    24465 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_inspiral
+-rwxr-xr-x   0 runner    (1001) docker     (122)    18972 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_inspiral_skymax
+-rwxr-xr-x   0 runner    (1001) docker     (122)    54408 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_live
+-rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_live_nagios_monitor
+-rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_losc_segment_query
+-rw-r--r--   0 runner    (1001) docker     (122)    17345 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_make_banksim
+-rw-r--r--   0 runner    (1001) docker     (122)    12546 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_make_faithsim
+-rw-r--r--   0 runner    (1001) docker     (122)    11717 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_make_html_page
+-rwxr-xr-x   0 runner    (1001) docker     (122)    25365 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_make_skymap
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3782 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_merge_inj_hdf
+-rwxr-xr-x   0 runner    (1001) docker     (122)    30868 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_multi_inspiral
+-rw-r--r--   0 runner    (1001) docker     (122)    15327 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_optimal_snr
+-rwxr-xr-x   0 runner    (1001) docker     (122)    19360 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_optimize_snr
+-rw-r--r--   0 runner    (1001) docker     (122)     5790 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_process_sngls
+-rw-r--r--   0 runner    (1001) docker     (122)     9080 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_randomize_inj_dist_by_optsnr
+-rwxr-xr-x   0 runner    (1001) docker     (122)    20946 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_single_template
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3992 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_source_probability_offline
+-rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_split_inspinj
+-rw-r--r--   0 runner    (1001) docker     (122)     6922 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_splitbank
+-rw-r--r--   0 runner    (1001) docker     (122)     2740 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_stageout_failed_workflow
+-rw-r--r--   0 runner    (1001) docker     (122)    10902 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_submit_dax
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11868 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pycbc_upload_xml_to_gracedb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/pygrb/
+-rw-r--r--   0 runner    (1001) docker     (122)     7925 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_grb_inj_combiner
+-rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_grb_inj_finder
+-rw-r--r--   0 runner    (1001) docker     (122)     7661 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_grb_trig_cluster
+-rw-r--r--   0 runner    (1001) docker     (122)    15754 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_grb_trig_combiner
+-rw-r--r--   0 runner    (1001) docker     (122)    20351 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_make_offline_grb_workflow
+-rw-r--r--   0 runner    (1001) docker     (122)    27308 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_efficiency
+-rw-r--r--   0 runner    (1001) docker     (122)     4199 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_grb_info_table
+-rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_minifollowups
+-rw-r--r--   0 runner    (1001) docker     (122)    37060 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_page_tables
+-rw-r--r--   0 runner    (1001) docker     (122)    10830 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_chisq_veto
+-rw-r--r--   0 runner    (1001) docker     (122)    10435 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_coh_ifosnr
+-rw-r--r--   0 runner    (1001) docker     (122)    21948 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_injs_results
+-rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_null_stats
+-rw-r--r--   0 runner    (1001) docker     (122)     3831 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_skygrid
+-rw-r--r--   0 runner    (1001) docker     (122)     6795 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_snr_timeseries
+-rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_stats_distribution
+-rw-r--r--   0 runner    (1001) docker     (122)    30510 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_pp_workflow
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/workflow_comparisons/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/workflow_comparisons/offline_search/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12151 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_combine_injection_comparisons
+-rwxr-xr-x   0 runner    (1001) docker     (122)    21916 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_injection_set_comparison
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2768 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_plot_injections_found_both_workflows
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3072 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_plot_injections_missed_one_workflow
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4595 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_plot_vt_ratio_vs_ifar
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/bin/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)    16320 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflows/pycbc_make_bank_verifier_workflow
+-rwxr-xr-x   0 runner    (1001) docker     (122)    36669 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflows/pycbc_make_coinc_search_workflow
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4599 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflows/pycbc_make_faithsim_workflow
+-rw-r--r--   0 runner    (1001) docker     (122)    15794 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflows/pycbc_make_inference_inj_workflow
+-rw-r--r--   0 runner    (1001) docker     (122)    10717 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflows/pycbc_make_inference_plots_workflow
+-rw-r--r--   0 runner    (1001) docker     (122)    12772 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflows/pycbc_make_inference_workflow
+-rw-r--r--   0 runner    (1001) docker     (122)     8159 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflows/pycbc_make_psd_estimation_workflow
+-rw-r--r--   0 runner    (1001) docker     (122)    16316 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflows/pycbc_make_sbank_workflow
+-rw-r--r--   0 runner    (1001) docker     (122)    12259 2023-03-09 21:19:31.000000 PyCBC-2.2.0/bin/workflows/pycbc_make_uberbank_workflow
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/banksim/
+-rw-r--r--   0 runner    (1001) docker     (122)    21402 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/banksim/injection0.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/banksim/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/cal/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/cal/foton_filter_esd_saturation/
+-rw-r--r--   0 runner    (1001) docker     (122)     6703 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/cal/foton_filter_esd_saturation/pycbc_check_esd_saturation.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     4460 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/cal/foton_filter_esd_saturation/pycbc_check_pcal_saturation.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2582 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/cal/foton_filter_esd_saturation/run_pcal_saturation_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/catalog/
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/catalog/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/catalog/stat.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/catalog/what.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/dataquality/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/dataquality/hwinj.py
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/dataquality/on.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/detector/
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/detector/ant.py
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/detector/delay.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/detector/loc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/detector/travel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/distributions/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/distributions/list_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/distributions/mass_examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1986 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/distributions/mchirp_q_from_uniform_m1m2_example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/distributions/sampling_from_config_example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/distributions/spin_examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/distributions/spin_spatial_distr_example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/faith/
+-rw-r--r--   0 runner    (1001) docker     (122)    21402 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/faith/injection0.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/faith/pegasus_workflow_create.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/faith/pegasus_workflow_submit.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/faith/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/filter/
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/filter/chisq.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/filter/fir.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/filter/pass.py
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/filter/snr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/gw150914/
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/gw150914/audio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/gw150914/gw150914_h1_snr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/gw150914/gw150914_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/analytic-normal2d/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      379 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/analytic-normal2d/make_movie.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      292 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/analytic-normal2d/plot.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      174 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/analytic-normal2d/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/bbh-injection/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      316 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/bbh-injection/make_injection.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      649 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/bbh-injection/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      967 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/bbh-injection/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/gw150914/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      582 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/gw150914/plot.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      656 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/gw150914/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1149 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/gw150914/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/hierarchical/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      269 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/hierarchical/make_injections.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      230 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/hierarchical/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      565 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/hierarchical/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/lisa_smbhb/
+-rw-r--r--   0 runner    (1001) docker     (122)     2421 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/lisa_smbhb/advanced_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/lisa_smbhb/get.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/lisa_smbhb/plot.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/lisa_smbhb/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/list_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/margtime/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/margtime/get.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/margtime/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/margtime/run_inj.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/multisignal/
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/multisignal/get.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      369 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/multisignal/make_injections.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/multisignal/rel.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      151 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/multisignal/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/multisignal/single.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/relative/
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/relative/get.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/relative/plot.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      139 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/relative/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/samplers/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      572 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/samplers/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inference/single/
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/single/get.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/single/plot.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/single/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/single/run_instant.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inference/single/run_marg.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/inspiral/
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inspiral/check_GW150914_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inspiral/clean.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3586 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/inspiral/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/live/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7946 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/live/check_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1508 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/live/generate_injections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/live/make_singles_fits_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6584 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/live/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/make_skymap/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/make_skymap/GW150914.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      553 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/make_skymap/GW170817.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/make_skymap/simulated_data.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/multi_inspiral/
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/multi_inspiral/check_faceon_faceaway_trigs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/multi_inspiral/check_gw170817_trigs.py
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/multi_inspiral/clean.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2736 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/multi_inspiral/faceon_faceaway.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2530 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/multi_inspiral/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/noise/
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/noise/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/noise/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/overlap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/psd/
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/psd/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      884 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/psd/estimate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/psd/read.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/search/bank.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/search/check_job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/search/gen.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/search/get.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/search/master.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/search/stats.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/search/submit.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/tmpltbank/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/tmpltbank/bank_workflow_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/bank_workflow_test/gen.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/cleanOutput.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/make_cache.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testAligned.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testAligned2.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testAligned3.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      649 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testNonspin.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      495 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testNonspin2.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      327 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testNonspin3.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      675 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testStoch.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      449 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testStoch2.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      355 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testStoch3.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      531 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/tmpltbank/testStoch4.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/waveform/
+-rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/waveform/add_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/waveform/match_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/waveform/plot_detwaveform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/waveform/plot_fd_td.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/waveform/plot_freq.py
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/waveform/plot_phase.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/waveform/plot_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/waveform/what_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/data_checker/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6801 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/data_checker/daily_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2162 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/data_checker/get_data_example.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/data_checker/run_daily_test.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/data_checker/run_get_data_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/dayhopecheck/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7198 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/dayhopecheck/dayhopecheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/dayhopecheck/run_dayhopecheck.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/generic/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/generic/multilevel_subworkflow_data/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/generic/multilevel_subworkflow_data/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/generic/multilevel_subworkflow_data/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/generic/simple_subworkflow_data/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/generic/simple_subworkflow_data/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/generic/simple_subworkflow_data/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/inference/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/inference/bbh_inj-dynesty/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/inference/bbh_inj-dynesty/create_inj_workflow.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/inference/gw150914_gw170814-dynesty/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      486 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/inference/gw150914_gw170814-dynesty/create_workflow.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/inference/gw150914_gw170814-emcee_pt/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      480 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/inference/gw150914_gw170814-emcee_pt/create_workflow.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/inference/small_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/inference/small_test/gen.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/pygrb/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/pygrb/ER7/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      739 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/pygrb/ER7/run_er7_pygrb_offline.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/pygrb/ER8/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      825 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/pygrb/ER8/run_er8_pygrb_offline.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      822 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/pygrb/ER8/run_er8_pygrb_online.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/examples/workflow/pygrb/S6/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      866 2023-03-09 21:19:31.000000 PyCBC-2.2.0/examples/workflow/pygrb/S6/run_s6_pygrb.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/
+-rw-r--r--   0 runner    (1001) docker     (122)     6207 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3219 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6380 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/_version_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21555 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15026 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/boundaries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/catalog/
+-rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56098 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4141 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23038 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28467 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (122)     9279 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19645 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/angular.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13126 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13606 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/bounded.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8901 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/external.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6510 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/fixedsamples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9342 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14330 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10257 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/mass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7732 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/power_law.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10564 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/qnm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/sky_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12002 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/spins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5286 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/uniform_log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4617 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/distributions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16663 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/dq.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/events/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13726 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/coherent.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52673 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/coinc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6808 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/coinc_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15820 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49942 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/eventmgr_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)    10863 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13205 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/significance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13294 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/simd_threshold_ccode.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/simd_threshold_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     7717 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/single.py
+-rw-r--r--   0 runner    (1001) docker     (122)    84395 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/stat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/threshold_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8580 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/threshold_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9465 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/trigger_fits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8750 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7572 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/events/veto.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/fft/
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/backend_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/backend_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/backend_mkl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3126 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/backend_support.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3391 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/class_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11855 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/cuda_pyfft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/cufft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8478 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/fft_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22514 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/fftw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7186 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/fftw_pruned.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/fftw_pruned_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/func_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6192 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/mkl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3765 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/npfft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4879 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/fft/parser_support.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/filter/
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3609 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/fotonfilter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82568 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/matchedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/matchedfilter_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/matchedfilter_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/matchedfilter_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/qtransform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15735 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/resample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3116 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/simd_correlate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15271 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/simd_correlate_ccode.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/simd_correlate_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/filter/zpk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/frame/
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34138 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/frame/frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5736 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/frame/losc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/frame/store.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/inference/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30844 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/burn_in.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8796 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8936 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6652 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/gelman_rubin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/geweke.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/inference/io/
+-rw-r--r--   0 runner    (1001) docker     (122)    32158 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38576 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/base_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36040 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/base_mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16944 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/base_multitemper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/base_nested_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5298 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/cpnest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7473 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/dynesty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4859 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/emcee_pt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11226 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/epsie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3653 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/posterior.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5947 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/ptemcee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2421 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/txt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/io/ultranest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/inference/jump/
+-rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/jump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4775 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/jump/angular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/jump/bounded_normal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5794 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/jump/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20231 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/jump/normal.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/inference/models/
+-rw-r--r--   0 runner    (1001) docker     (122)    11258 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8703 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33142 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5697 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/base_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7614 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/brute_marg.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23677 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31219 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/gated_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49252 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24411 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32990 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/marginalized_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22631 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/relbin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8733 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/relbin_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     8435 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/single_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33243 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16324 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/option_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/inference/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8201 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/base_cube.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36376 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/base_mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16327 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/base_multitemper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8274 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/cpnest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23999 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/dynesty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18909 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/emcee_pt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19831 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/epsie.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15427 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27259 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/ptemcee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7359 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inference/sampler/ultranest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/inject/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48285 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inject/inject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19409 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/inject/injfilterrejector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55604 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/io/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12494 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/io/ligolw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24724 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/io/live.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77607 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/io/record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9494 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/libutils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13070 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/mchirp_area.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/neutron_stars/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/neutron_stars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6861 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/neutron_stars/eos_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/neutron_stars/ns_data/
+-rw-r--r--   0 runner    (1001) docker     (122)    53263 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/neutron_stars/ns_data/equil_2H.dat
+-rw-r--r--   0 runner    (1001) docker     (122)    11046 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/neutron_stars/pg_isso_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/noise/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5192 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/noise/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8316 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/noise/reproduceable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5385 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/opt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39910 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/pnutils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5462 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/population/
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30477 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/population/fgmc_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/population/fgmc_laguerre.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10012 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/population/fgmc_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9061 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/population/live_pastro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/population/live_pastro_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16559 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/population/population_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13826 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/population/rates_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16956 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/population/scale_injections.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/psd/
+-rw-r--r--   0 runner    (1001) docker     (122)    28796 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/psd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6263 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/psd/analytical.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22380 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/psd/analytical_space.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12318 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/psd/estimate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7153 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/psd/read.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8554 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/psd/variation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12540 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/rate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/
+-rw-r--r--   0 runner    (1001) docker     (122)      423 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/dq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/followup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/layout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4692 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/legacy_grb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4769 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/mpld3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/psd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/pygrb_plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38592 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/pygrb_postprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7996 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/render.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33143 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/scatter_histograms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/css/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/css/bootstrap/3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)   117150 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/css/bootstrap/3.3.2/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)   117150 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/css/fancybox/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/css/fancybox/2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     4902 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/css/fancybox/2.1.5/jquery.fancybox.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/css/pycbc/
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/css/pycbc/orange.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/css/pycbc/red.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Light.css
+-rw-r--r--   0 runner    (1001) docker     (122)   258264 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Light.eot
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Light.html
+-rw-r--r--   0 runner    (1001) docker     (122)   658924 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   312760 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Semibold.css
+-rw-r--r--   0 runner    (1001) docker     (122)   270560 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Semibold.eot
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Semibold.html
+-rw-r--r--   0 runner    (1001) docker     (122)   702616 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Semibold.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   326132 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Semibold.woff
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/js/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/js/bootstrap/3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    35452 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/js/bootstrap/3.3.2/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    35452 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/js/fancybox/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/js/fancybox/2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/js/fancybox/2.1.5/fancybox-orange.js
+-rwxr-xr-x   0 runner    (1001) docker     (122)    48706 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.js
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23135 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.pack.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/js/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/static/js/jquery/1.10.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    93107 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/js/jquery/1.10.2/jquery-1.10.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1384 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/js/jquery/1.10.2/jquery.mousewheel-3.0.6.pack.js
+-rw-r--r--   0 runner    (1001) docker     (122)    95786 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9027 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4698 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/table_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/templates/files/
+-rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/templates/files/file_default.html
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/templates/files/file_glitchgram.html
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/templates/files/file_img.html
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/templates/files/file_pre.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/templates/files/file_tmplt.html
+-rw-r--r--   0 runner    (1001) docker     (122)    11740 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/templates/orange.html
+-rw-r--r--   0 runner    (1001) docker     (122)    11734 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/templates/red.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/results/templates/wells/
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/templates/wells/sitemap.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/templates/wells/two_column.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7878 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/results/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10948 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11609 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/strain/
+-rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/strain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/strain/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6383 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/strain/gate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8123 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/strain/lines.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18783 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/strain/recalibrate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    91091 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/strain/strain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/tmpltbank/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4865 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/bank_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12504 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/bank_output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23515 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/brute_force_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23569 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/calc_moments.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33431 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/coord_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10726 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/lambda_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/lattice_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57132 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/option_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28137 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/tmpltbank/partitioned_bank.py
+-rw-r--r--   0 runner    (1001) docker     (122)    84293 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/types/aligned.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39845 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5421 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/types/array_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)    11741 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/types/array_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26102 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25727 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/types/frequencyseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21934 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/types/optparse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45520 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/types/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-03-09 21:19:35.000000 PyCBC-2.2.0/pycbc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/vetoes/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/vetoes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12524 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/vetoes/autochisq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/vetoes/bank_chisq.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19668 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/vetoes/chisq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4964 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/vetoes/chisq_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)    12354 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/vetoes/chisq_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7224 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/vetoes/sgchisq.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/waveform/
+-rw-r--r--   0 runner    (1001) docker     (122)    18361 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/SpinTaylorF2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39507 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/bank.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30086 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/compress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/decompress_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9811 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/decompress_cpu_ccode.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3580 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/decompress_cpu_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)    11138 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/decompress_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51496 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3724 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/multiband.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/nltides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29135 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4171 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/premerger.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15018 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/pycbc_phenomC_tmplt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54746 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/ringdown.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/sinegauss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8829 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/spa_tmplt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6584 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/spa_tmplt_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     3243 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/spa_tmplt_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/supernovae.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19760 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4229 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/utils_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/utils_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57072 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11590 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/waveform/waveform_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/workflow/
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26619 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/coincidence.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10939 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/configparser_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15824 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    88854 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50017 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/datafind.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9556 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/dq.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21408 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/grb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42899 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/inference_followups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13587 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/injection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53624 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/jobsetup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13905 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/matched_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36429 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/minifollowups.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/pycbc/workflow/pegasus_files/
+-rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/pegasus_files/pegasus-properties.conf
+-rw-r--r--   0 runner    (1001) docker     (122)    11840 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/pegasus_sites.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32699 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/pegasus_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23393 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/psd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5160 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/psdfiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19177 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/segment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/splittable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14333 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pycbc/workflow/tmpltbank.py
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-03-09 21:19:31.000000 PyCBC-2.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-09 21:19:37.000000 PyCBC-2.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12377 2023-03-09 21:19:31.000000 PyCBC-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/bankvetotest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37722 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/fft_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16620 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/lalsim.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21211 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5083 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_array_lal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6519 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_autochisq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2989 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4885 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_chisq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_coinc_stat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_correlate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8904 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11134 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_fft_mkl_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_fft_unthreaded.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_fftw_openmp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_fftw_pthreads.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6510 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24440 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_frequencyseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7338 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_infmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_injection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6282 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_io_live.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6818 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_live_coinc_compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_matchedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_pnutils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5934 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_psd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7707 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7904 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_significance_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19047 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_skymax.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3434 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_spatmplt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25115 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26649 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_tmpltbank.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7464 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/test_waveform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38174 2023-03-09 21:19:31.000000 PyCBC-2.2.0/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/tools/benchmarking/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      822 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/benchmarking/absolute_times.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/tools/einsteinathome/
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/einsteinathome/check_GW150914_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/tools/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/tools/static/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)     3570 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/static/hooks/hook-pycbc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      734 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/static/runtime-scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/static/runtime-tkinter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/tools/timing/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2286 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/timing/arr_perf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:19:37.000000 PyCBC-2.2.0/tools/timing/banksim/
+-rw-r--r--   0 runner    (1001) docker     (122)    12160 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/timing/banksim/banksim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/timing/correlate_perf.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2935 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/timing/fft_perf.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3154 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/timing/match_perf.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2472 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tools/timing/wav_perf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-03-09 21:19:31.000000 PyCBC-2.2.0/tox.ini
```

### Comparing `PyCBC-2.1.2/LICENSE` & `PyCBC-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/PKG-INFO` & `PyCBC-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyCBC
-Version: 2.1.2
+Version: 2.2.0
 Summary: Core library to analyze gravitational-wave data, find signals, and study their parameters.
 Home-page: http://www.pycbc.org/
 Author: The PyCBC team
 Author-email: alex.nitz@gmail.org
 License: UNKNOWN
-Download-URL: https://github.com/gwastro/pycbc/tarball/v2.1.2
+Download-URL: https://github.com/gwastro/pycbc/tarball/v2.2.0
 Description: ![GW150914](https://raw.githubusercontent.com/gwastro/pycbc-logo/master/pycbc_logo_name.png)
         
         [PyCBC](http://pycbc.org) is a software package used to explore astrophysical sources of gravitational waves.
         It contains algorithms to analyze gravitational-wave data,
         detect coalescing compact binaries, and make bayesian inferences from gravitational-wave data.
         PyCBC was used in the [first direct detection of gravitational waves](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.116.061102) and
         is used in flagship analyses of LIGO and Virgo data.
```

### Comparing `PyCBC-2.1.2/PyCBC.egg-info/PKG-INFO` & `PyCBC-2.2.0/PyCBC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyCBC
-Version: 2.1.2
+Version: 2.2.0
 Summary: Core library to analyze gravitational-wave data, find signals, and study their parameters.
 Home-page: http://www.pycbc.org/
 Author: The PyCBC team
 Author-email: alex.nitz@gmail.org
 License: UNKNOWN
-Download-URL: https://github.com/gwastro/pycbc/tarball/v2.1.2
+Download-URL: https://github.com/gwastro/pycbc/tarball/v2.2.0
 Description: ![GW150914](https://raw.githubusercontent.com/gwastro/pycbc-logo/master/pycbc_logo_name.png)
         
         [PyCBC](http://pycbc.org) is a software package used to explore astrophysical sources of gravitational waves.
         It contains algorithms to analyze gravitational-wave data,
         detect coalescing compact binaries, and make bayesian inferences from gravitational-wave data.
         PyCBC was used in the [first direct detection of gravitational waves](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.116.061102) and
         is used in flagship analyses of LIGO and Virgo data.
```

### Comparing `PyCBC-2.1.2/PyCBC.egg-info/SOURCES.txt` & `PyCBC-2.2.0/PyCBC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/README.md` & `PyCBC-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_add_statmap` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_add_statmap`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_apply_rerank` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_apply_rerank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_average_psd` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_average_psd`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_bin_trigger_rates_dq` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_bin_trigger_rates_dq`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_calculate_dq` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_calculate_dq`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_calculate_dqflag` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_calculate_dqflag`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_calculate_psd` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_calculate_psd`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_findtrigs` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_findtrigs`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_hdfinjfind` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_hdfinjfind`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_mergetrigs` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_mergetrigs`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_statmap` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_statmap`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_coinc_statmap_inj` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_coinc_statmap_inj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_combine_coincident_events` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_combine_coincident_events`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_combine_statmap` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_combine_statmap`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_cut_merge_triggers_to_tmpltbank` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_cut_merge_triggers_to_tmpltbank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_distribute_background_bins` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_distribute_background_bins`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_dtphase` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_dtphase`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_exclude_zerolag` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_exclude_zerolag`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_binned` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_binned`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_by_template` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_by_template`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_over_multiparam` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_over_multiparam`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_over_param` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_over_param`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_fit_sngls_split_binned` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_fit_sngls_split_binned`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_followup_file` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_followup_file`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_foreground_censor` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_foreground_censor`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_get_loudest_params` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_get_loudest_params`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_merge_psds` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_merge_psds`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_plot_kde_vals` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_plot_kde_vals`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_reduce_template_bank` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_reduce_template_bank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_rerank_dq` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_rerank_dq`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_rerank_passthrough` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_rerank_passthrough`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_sngls_findtrigs` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_sngls_findtrigs`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_sngls_pastro` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_sngls_pastro`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_sngls_statmap` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_sngls_statmap`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_sngls_statmap_inj` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_sngls_statmap_inj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_strip_injections` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_strip_injections`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_template_kde_calc` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_template_kde_calc`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/all_sky_search/pycbc_template_recovery_hist` & `PyCBC-2.2.0/bin/all_sky_search/pycbc_template_recovery_hist`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/bank/pycbc_aligned_bank_cat` & `PyCBC-2.2.0/bin/bank/pycbc_aligned_bank_cat`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/bank/pycbc_aligned_stoch_bank` & `PyCBC-2.2.0/bin/bank/pycbc_aligned_stoch_bank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/bank/pycbc_bank_verification` & `PyCBC-2.2.0/bin/bank/pycbc_bank_verification`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/bank/pycbc_brute_bank` & `PyCBC-2.2.0/bin/bank/pycbc_brute_bank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/bank/pycbc_coinc_bank2hdf` & `PyCBC-2.2.0/bin/bank/pycbc_coinc_bank2hdf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/bank/pycbc_geom_aligned_2dstack` & `PyCBC-2.2.0/bin/bank/pycbc_geom_aligned_2dstack`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/bank/pycbc_geom_aligned_bank` & `PyCBC-2.2.0/bin/bank/pycbc_geom_aligned_bank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/bank/pycbc_geom_nonspinbank` & `PyCBC-2.2.0/bin/bank/pycbc_geom_nonspinbank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/bank/pycbc_tmpltbank_to_chi_params` & `PyCBC-2.2.0/bin/bank/pycbc_tmpltbank_to_chi_params`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/hwinj/pycbc_generate_hwinj` & `PyCBC-2.2.0/bin/hwinj/pycbc_generate_hwinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/hwinj/pycbc_generate_hwinj_from_xml` & `PyCBC-2.2.0/bin/hwinj/pycbc_generate_hwinj_from_xml`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/hwinj/pycbc_insert_frame_hwinj` & `PyCBC-2.2.0/bin/hwinj/pycbc_insert_frame_hwinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/hwinj/pycbc_plot_hwinj` & `PyCBC-2.2.0/bin/hwinj/pycbc_plot_hwinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference` & `PyCBC-2.2.0/bin/inference/pycbc_inference`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_create_fits` & `PyCBC-2.2.0/bin/inference/pycbc_inference_create_fits`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_extract_samples` & `PyCBC-2.2.0/bin/inference/pycbc_inference_extract_samples`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_model_stats` & `PyCBC-2.2.0/bin/inference/pycbc_inference_model_stats`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_monitor` & `PyCBC-2.2.0/bin/inference/pycbc_inference_monitor`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_acceptance_rate` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_acceptance_rate`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_acf` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_acf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_acl` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_acl`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_dynesty_run` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_dynesty_run`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_dynesty_traceplot` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_dynesty_traceplot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_gelman_rubin` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_gelman_rubin`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_geweke` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_geweke`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_inj_recovery` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_inj_recovery`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_mcmc_history` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_mcmc_history`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_movie` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_movie`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_posterior` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_posterior`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_pp` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_pp`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_prior` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_prior`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_samples` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_samples`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_skymap` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_skymap`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_plot_thermodynamic_integrand` & `PyCBC-2.2.0/bin/inference/pycbc_inference_plot_thermodynamic_integrand`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_pp_table_summary` & `PyCBC-2.2.0/bin/inference/pycbc_inference_pp_table_summary`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_start_from_samples` & `PyCBC-2.2.0/bin/inference/pycbc_inference_start_from_samples`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_inference_table_summary` & `PyCBC-2.2.0/bin/inference/pycbc_inference_table_summary`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/inference/pycbc_validate_test_posterior` & `PyCBC-2.2.0/bin/inference/pycbc_validate_test_posterior`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/live/pycbc_live_combine_single_fits` & `PyCBC-2.2.0/bin/live/pycbc_live_combine_single_fits`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/live/pycbc_live_plot_combined_single_fits` & `PyCBC-2.2.0/bin/live/pycbc_live_plot_combined_single_fits`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/live/pycbc_live_plot_single_trigger_fits` & `PyCBC-2.2.0/bin/live/pycbc_live_plot_single_trigger_fits`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/live/pycbc_live_single_trigger_fits` & `PyCBC-2.2.0/bin/live/pycbc_live_single_trigger_fits`

 * *Files 4% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 # criteria
 date_directory = os.path.join(args.top_directory, args.analysis_date)
 
 if not os.path.exists(date_directory):
     raise FileNotFoundError(f"The directory {date_directory} does not exist.")
 
 files = [f for f in os.listdir(date_directory)
-         if args.file_identifier in f and f.endswith('hdf')]
+         if args.file_identifier in f]
 
 events = {}
 counter = 0
 
 for filename in files:
     counter += 1
     if counter % 1000 == 0:
@@ -190,14 +190,15 @@
                 # In case of no triggers for an extended period
                 logging.info("%s: No data", ifo)
             else:
                 logging.info("%s: %d triggers in %.0fs", ifo,
                              events[ifo].data['snr'].size, live_time[ifo])
 
     f = os.path.join(date_directory, filename)
+    skipping_file = False
     # If there is an IOerror with the file, don't fail, just carry on
     try:
         h5py.File(f, 'r')
     except IOError:
         logging.info('IOError with file ' + f)
         continue
 
@@ -261,20 +262,19 @@
         triggers_cut[args.sngl_ranking] = sngls_value
 
         triggers_da = DictArray(data=triggers_cut)
 
         # If we are clustering, take the max sngl_ranking value
         if args.cluster:
             max_idx = sngls_value.argmax()
-            # Make sure that the DictArray has array data, not float
-            triggers_da = triggers_da.select([max_idx])
+            triggers_cut = triggers_da.select(max_idx)
 
-        if ifo in events:  # DictArray already exists for the ifo
+        if ifo in events:
             events[ifo] += triggers_da
-        else:  # Set up a new dictionary entry
+        else:
             events[ifo] = triggers_da
 
 logging.info("All events processed")
 
 logging.info("Number of events which meet all criteria:")
 for ifo in args.ifos:
     if ifo not in events:
```

### Comparing `PyCBC-2.1.2/bin/minifollowups/pycbc_foreground_minifollowup` & `PyCBC-2.2.0/bin/minifollowups/pycbc_foreground_minifollowup`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/minifollowups/pycbc_injection_minifollowup` & `PyCBC-2.2.0/bin/minifollowups/pycbc_injection_minifollowup`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/minifollowups/pycbc_page_coincinfo` & `PyCBC-2.2.0/bin/minifollowups/pycbc_page_coincinfo`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/minifollowups/pycbc_page_injinfo` & `PyCBC-2.2.0/bin/minifollowups/pycbc_page_injinfo`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/minifollowups/pycbc_page_snglinfo` & `PyCBC-2.2.0/bin/minifollowups/pycbc_page_snglinfo`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/minifollowups/pycbc_plot_chigram` & `PyCBC-2.2.0/bin/minifollowups/pycbc_plot_chigram`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/minifollowups/pycbc_plot_trigger_timeseries` & `PyCBC-2.2.0/bin/minifollowups/pycbc_plot_trigger_timeseries`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/minifollowups/pycbc_single_template_plot` & `PyCBC-2.2.0/bin/minifollowups/pycbc_single_template_plot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/minifollowups/pycbc_sngl_minifollowup` & `PyCBC-2.2.0/bin/minifollowups/pycbc_sngl_minifollowup`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_banksim_plot_eff_fitting_factor` & `PyCBC-2.2.0/bin/plotting/pycbc_banksim_plot_eff_fitting_factor`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_banksim_plot_fitting_factors` & `PyCBC-2.2.0/bin/plotting/pycbc_banksim_plot_fitting_factors`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_banksim_table_point_injs` & `PyCBC-2.2.0/bin/plotting/pycbc_banksim_table_point_injs`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_create_html_snippet` & `PyCBC-2.2.0/bin/plotting/pycbc_create_html_snippet`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_faithsim_plots` & `PyCBC-2.2.0/bin/plotting/pycbc_faithsim_plots`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_ifar_catalog` & `PyCBC-2.2.0/bin/plotting/pycbc_ifar_catalog`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_mass_area_plot` & `PyCBC-2.2.0/bin/plotting/pycbc_mass_area_plot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_mchirp_plots` & `PyCBC-2.2.0/bin/plotting/pycbc_mchirp_plots`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_banktriggerrate` & `PyCBC-2.2.0/bin/plotting/pycbc_page_banktriggerrate`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_coinc_snrchi` & `PyCBC-2.2.0/bin/plotting/pycbc_page_coinc_snrchi`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_foreground` & `PyCBC-2.2.0/bin/plotting/pycbc_page_foreground`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_foundmissed` & `PyCBC-2.2.0/bin/plotting/pycbc_page_foundmissed`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_ifar` & `PyCBC-2.2.0/bin/plotting/pycbc_page_ifar`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_injtable` & `PyCBC-2.2.0/bin/plotting/pycbc_page_injtable`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_recovery` & `PyCBC-2.2.0/bin/plotting/pycbc_page_recovery`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_segments` & `PyCBC-2.2.0/bin/plotting/pycbc_page_segments`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_segplot` & `PyCBC-2.2.0/bin/plotting/pycbc_page_segplot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_segtable` & `PyCBC-2.2.0/bin/plotting/pycbc_page_segtable`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_sensitivity` & `PyCBC-2.2.0/bin/plotting/pycbc_page_sensitivity`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_snrchi` & `PyCBC-2.2.0/bin/plotting/pycbc_page_snrchi`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_snrifar` & `PyCBC-2.2.0/bin/plotting/pycbc_page_snrifar`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_snrratehist` & `PyCBC-2.2.0/bin/plotting/pycbc_page_snrratehist`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_page_vetotable` & `PyCBC-2.2.0/bin/plotting/pycbc_page_vetotable`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_background_coincs` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_background_coincs`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_bank_bins` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_bank_bins`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_dq_likelihood_vs_time` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_dq_likelihood_vs_time`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_dq_percentiles` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_dq_percentiles`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_gate_triggers` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_gate_triggers`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_gating` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_gating`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_hist` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_hist`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_multiifo_dtphase` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_multiifo_dtphase`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_psd_file` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_psd_file`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_psd_timefreq` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_psd_timefreq`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_qscan` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_qscan`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_range` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_range`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_range_vs_mtot` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_range_vs_mtot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_singles_timefreq` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_singles_timefreq`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_singles_vs_params` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_singles_vs_params`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_throughput` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_throughput`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_trigrate` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_trigrate`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_vt_ratio` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_vt_ratio`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/plotting/pycbc_plot_waveform` & `PyCBC-2.2.0/bin/plotting/pycbc_plot_waveform`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/population/pycbc_multiifo_pastro` & `PyCBC-2.2.0/bin/population/pycbc_multiifo_pastro`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/population/pycbc_population_plots` & `PyCBC-2.2.0/bin/population/pycbc_population_plots`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/population/pycbc_population_rates` & `PyCBC-2.2.0/bin/population/pycbc_population_rates`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_banksim` & `PyCBC-2.2.0/bin/pycbc_banksim`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_banksim_combine_banks` & `PyCBC-2.2.0/bin/pycbc_banksim_combine_banks`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_banksim_match_combine` & `PyCBC-2.2.0/bin/pycbc_banksim_match_combine`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_banksim_skymax` & `PyCBC-2.2.0/bin/pycbc_banksim_skymax`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_coinc_time` & `PyCBC-2.2.0/bin/pycbc_coinc_time`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_compress_bank` & `PyCBC-2.2.0/bin/pycbc_compress_bank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_condition_strain` & `PyCBC-2.2.0/bin/pycbc_condition_strain`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_copy_output_map` & `PyCBC-2.2.0/bin/pycbc_copy_output_map`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_create_injections` & `PyCBC-2.2.0/bin/pycbc_create_injections`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_data_store` & `PyCBC-2.2.0/bin/pycbc_data_store`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_faithsim` & `PyCBC-2.2.0/bin/pycbc_faithsim`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_faithsim_collect_results` & `PyCBC-2.2.0/bin/pycbc_faithsim_collect_results`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_fit_sngl_trigs` & `PyCBC-2.2.0/bin/pycbc_fit_sngl_trigs`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_get_ffinal` & `PyCBC-2.2.0/bin/pycbc_get_ffinal`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_hdf5_splitbank` & `PyCBC-2.2.0/bin/pycbc_hdf5_splitbank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_hdf_splitinj` & `PyCBC-2.2.0/bin/pycbc_hdf_splitinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_inj_cut` & `PyCBC-2.2.0/bin/pycbc_inj_cut`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_inspinj2hdf` & `PyCBC-2.2.0/bin/pycbc_inspinj2hdf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_inspiral` & `PyCBC-2.2.0/bin/pycbc_inspiral`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_inspiral_skymax` & `PyCBC-2.2.0/bin/pycbc_inspiral_skymax`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_live` & `PyCBC-2.2.0/bin/pycbc_live`

 * *Files 2% similar despite different names*

```diff
@@ -91,21 +91,17 @@
 
         self.path = args.output_path
         self.mc_area_args = mchirp_area.from_cli(args, parser)
         self.padata = livepau.PAstroData(args.p_astro_spec, args.bank_file)
         self.use_date_prefix = args.day_hour_output_prefix
         self.ifar_upload_threshold = args.ifar_upload_threshold
         self.pvalue_livetime = args.pvalue_combination_livetime
-        self.gracedb_server = args.gracedb_server
-        self.gracedb_search = args.gracedb_search
-        self.gracedb_labels = args.gracedb_labels
         self.gracedb_testing = not args.enable_production_gracedb_upload
         self.enable_gracedb_upload = args.enable_gracedb_upload
         self.run_snr_optimization = args.run_snr_optimization
-        self.snr_opt_label = args.snr_opt_label
         self.gracedb = None
 
         # Keep track of which events have been uploaded
         self.last_few_coincs_uploaded = []
 
         if self.run_snr_optimization:
             # preestimate the number of CPU cores that we can afford giving
@@ -117,19 +113,14 @@
             if self.fu_cores <= 0:
                 logging.warning('Insufficient number of CPU cores (%d) to '
                                 'run search and trigger followups. Uploaded '
                                 'triggers will momentarily increase the lag',
                                 available_cores)
                 self.fu_cores = 1
 
-        if args.enable_embright_has_massgap:
-            if args.embright_massgap_max < self.mc_area_args['mass_bdary']['ns_max']:
-                parser.error('MAX_GAP value cannot be lower than MAX_NS limit')
-            self.mc_area_args['embright_mg_max'] = args.embright_massgap_max
-
     def commit_results(self, results):
         logging.info('Committing triggers')
         self.comm.gather(results, root=0)
 
     def barrier(self):
         self.comm.Barrier()
 
@@ -190,94 +181,67 @@
                 coinc_times[ifo],
                 check_state=False
             )
 
             if snr_series is not None:
                 out[ifo] = {'snr_series': snr_series}
 
-        # Determine if the other ifos can contribute to the coincident event,
-        # if so then update the info in `triggers` appropriately
+        # Determine if the other ifos can contribute to the coincident event
         for ifo in followup_ifos:
-            pvalue_info = followup_event_significance(
+            snr_series, ptime, pvalue, sigma2 = followup_event_significance(
                 ifo,
                 self.data_readers[ifo],
                 self.bank,
                 template_id,
                 coinc_times
             )
-            if pvalue_info is None:
-                continue
-            out[ifo] = {'snr_series': pvalue_info['snr_series']}
-            self.get_followup_info(
-                ifos[0],
-                ifo,
-                triggers,
-                pvalue_info,
-                recalculate_ifar=recalculate_ifar
-            )
+            if snr_series is not None:
+                out[ifo] = {'snr_series': snr_series}
+                self.get_followup_info(ifos[0], ifo, triggers, snr_series,
+                                       ptime, pvalue, sigma2,
+                                       recalculate_ifar=recalculate_ifar)
 
         # the SNR time series sample rate can vary slightly due to
         # rounding errors, so force all of them to be identical
         fix_delta_t = None
         for ifo in out:
             if 'snr_series' not in out[ifo]:
                 continue
             if fix_delta_t is None:
                 fix_delta_t = out[ifo]['snr_series']._delta_t
             else:
                 out[ifo]['snr_series']._delta_t = fix_delta_t
 
         return out
 
-    def get_followup_info(
-        self,
-        coinc_ifo,
-        ifo,
-        triggers,
-        pvalue_info,
-        recalculate_ifar=False
-    ):
-        peak_time = pvalue_info['peak_time']
-        pv = pvalue_info['pvalue']
-        pv_sat = pvalue_info['pvalue_saturated']
-
-        # Copy the common fields from the other detector;
+    def get_followup_info(self, coinc_ifo, ifo, triggers, snr_series, ptime,
+                          pvalue, sigma2, recalculate_ifar=False):
+        # Copy the common fields from the other detector
         # ignore fields that contain detector-specific data
-        fields_to_ignore = set([
-            'end_time', 'snr', 'stat', 'coa_phase',
-            'chisq', 'chisq_dof', 'sg_chisq', 'sigmasq'
-        ])
+        fields_to_ignore = set(['end_time', 'snr', 'stat', 'coa_phase',
+                                'chisq', 'chisq_dof', 'sg_chisq', 'sigmasq'])
         for key in set(triggers):
-            if f'foreground/{coinc_ifo}/' not in key:
-                continue
-            _, _, name = key.split('/')
-            if name in fields_to_ignore:
-                continue
-            triggers[f'foreground/{ifo}/{name}'] = triggers[key]
+            if 'foreground/{}/'.format(coinc_ifo) in key:
+                _, _, name = key.split('/')
+                if name in fields_to_ignore:
+                    continue
+                triggers['foreground/{}/{}'.format(ifo, name)] = triggers[key]
 
         # Set the detector-specific fields for which we have data
-        snr_series_peak = pvalue_info['snr_series'].at_time(
-            peak_time,
-            nearest_sample=True
-        )
-        base = f'foreground/{ifo}/'
-        triggers[base + 'end_time'] = float(peak_time)
+        snr_series_peak = snr_series.at_time(ptime, nearest_sample=True)
+        base = 'foreground/{}/'.format(ifo)
+        triggers[base + 'end_time'] = float(ptime)
         triggers[base + 'snr'] = triggers[base + 'stat'] = abs(snr_series_peak)
         triggers[base + 'coa_phase'] = numpy.angle(snr_series_peak)
-        triggers[base + 'sigmasq'] = pvalue_info['sigma2']
+        triggers[base + 'sigmasq'] = sigma2
         if recalculate_ifar:
             # Calculate new ifar
             triggers['foreground/ifar'] = combine_ifar_pvalue(
-                triggers['foreground/ifar'],
-                pv,
-                self.pvalue_livetime
-            )
-            triggers['foreground/ifar_saturated'] |= pv_sat
-            triggers[f'foreground/pvalue_{ifo}'] = pv
-            triggers[f'foreground/pvalue_{ifo}_saturated'] = pv_sat
+                    triggers['foreground/ifar'], pvalue, self.pvalue_livetime)
+            triggers['foreground/pvalue_{}'.format(ifo)] = pvalue
 
     def setup_optimize_snr(
         self, results, live_ifos, triggering_ifos, fname, gid
     ):
         """Setup and start the network SNR optimization process for a
         candidate event. See arXiv:2008.07494 for details.
 
@@ -360,21 +324,16 @@
 
             recursively_save_dict_contents_to_group(hdfp,
                                                     'mc_area_args/',
                                                     self.mc_area_args)
 
         cmd += '--params-file {} '.format(curr_fname)
         cmd += '--approximant {} '.format(apr)
-        cmd += '--gracedb-server {} '.format(self.gracedb_server)
-        cmd += '--gracedb-search {} '.format(self.gracedb_search)
-
-        labels = self.snr_opt_label
-        labels += ' '.join(self.gracedb_labels or [])
-        cmd += f'--gracedb-labels {labels} '
-
+        cmd += '--gracedb-server {} '.format(args.gracedb_server)
+        cmd += '--gracedb-search {} '.format(args.gracedb_search)
         if not self.gracedb_testing:
             cmd += '--production '
         cmd += '--verbose '
 
         # set up a place for storing the SNR optimization results and log
         out_dir_path = os.path.join(os.path.dirname(fname), 'optimize_snr')
         makedir(out_dir_path)
@@ -383,17 +342,17 @@
         if self.enable_gracedb_upload:
             cmd += '--enable-gracedb-upload '
 
         cmd += '--cores {} '.format(self.fu_cores)
         if args.processing_scheme:
             # we will use the cores for multiple workers of the
             # optimization routine, so we force the processing scheme
-            # to a single core here.  This may be enforcing some
+            # to a single core here.  this may be enforcing some
             # assumptions about the optimal way to do ffts on the
-            # machine. However, the dominant cost of pycbc_optimize_snr
+            # machine. however, the dominant cost of pycbc_optimize_snr
             # is expected to be in waveform generation, which is
             # unlikely to benefit from a processing scheme with more
             # than 1 thread anyway.
             opt_scheme = args.processing_scheme.split(':')[0]
             cmd += '--processing-scheme {}:1 '.format(opt_scheme)
 
         log_fname = os.path.join(out_dir_path, 'optimize_snr.log')
@@ -402,41 +361,38 @@
         with open(log_fname, "w") as logfile:
             subprocess.Popen(
                 cmd, shell=True, stdout=logfile, stderr=logfile
             )
 
     def create_gdb(self):
         """
-        Create a GraceDB session that will persist throughout the execution
-        of PyCBC Live.
+        Function to create GraceDB session.
         """
         from ligo.gracedb.rest import GraceDb
-
         logging.info('Creating GraceDB session')
         # Set up dict for args that reload the certificate if it will expire in the
         # reload_buffer time. These args are documented here:
         # https://ligo-gracedb.readthedocs.io/en/latest/api.html#ligo.gracedb.rest.GraceDb
         # Because we do not change any of the request session values when running the
         # code, it should remain thread safe. 
         gdbargs = {'reload_certificate': True, 'reload_buffer': 300}
-        if self.gracedb_server:
-            gdbargs['service_url'] = self.gracedb_server
+        if args.gracedb_server:
+            gdbargs['service_url'] = args.gracedb_server 
         self.gracedb = GraceDb(**gdbargs)
 
     def upload_in_thread(self, event, fname, comment, results, live_ifos, ifos,
-                         upload_checks, optimize_snr_checks):
+                         upload_checks, optimize_snr_checks, gracedb_server, gracedb_search):
         gid = None
         if upload_checks:
             gid = event.upload(
                 fname,
-                gracedb_server=self.gracedb_server,
+                gracedb_server=gracedb_server,
                 testing=self.gracedb_testing,
                 extra_strings=[comment],
-                search=self.gracedb_search,
-                labels=self.gracedb_labels
+                search=gracedb_search
             )
         if optimize_snr_checks:
             self.setup_optimize_snr(
                 results,
                 live_ifos,
                 ifos,
                 fname,
@@ -518,15 +474,16 @@
                 logging.info('Optimizing SNR for coinc above threshold ..')
                 # Tell snr optimized event about p_terr
                 if hasattr(event, 'p_terr') and event.p_terr is not None:
                     coinc_results['p_terr'] = event.p_terr
             live_ifos = [ifo for ifo in sld if 'snr_series' in sld[ifo]]
             thread_args = (
                 event, fname, comment, coinc_results, live_ifos, coinc_ifos,
-                upload_checks, optimize_snr_checks
+                upload_checks, optimize_snr_checks, args.gracedb_server, 
+                args.gracedb_search,
             )
             gdb_upload_thread = threading.Thread(target=self.upload_in_thread,
                                                  args=thread_args)
             gdb_upload_thread.start()
 
     def check_singles(self, results, psds):
         active = [k for k in results if results[k] is not None]
@@ -605,16 +562,17 @@
                     logging.info('Optimizing SNR for single above threshold ..')
                     # Tell snr optimized event about p_terr
                     if hasattr(event, 'p_terr') and event.p_terr is not None:
                         single['p_terr'] = event.p_terr
                 live_ifos = [ifo for ifo in sld if 'snr_series' in sld[ifo]]
                 thread_args = (
                     event, fname, comment, single, live_ifos, [ifo],
-                    upload_checks, optimize_snr_checks
-                )
+                    upload_checks, optimize_snr_checks, args.gracedb_server, 
+                    args.gracedb_search,
+                    )
                 gdb_upload_thread = threading.Thread(target=self.upload_in_thread,
                                                      args=thread_args)
                 gdb_upload_thread.start()
 
     def get_out_dir_path(self, time_gps):
         """Compose and return the path to a directory to store files associated
         with times in a given day (specified via a GPS time).
@@ -861,17 +819,14 @@
                     help='Upload single ifo events to GraceDB')
 parser.add_argument('--gracedb-server', metavar='URL',
                     help='URL of GraceDB server API for uploading events. '
                          'If not provided, the default URL is used.')
 parser.add_argument('--gracedb-search', type=str, default='AllSky',
                     help='String going into the "search" field of the GraceDB '
                          'events')
-parser.add_argument('--gracedb-labels', metavar='LABEL', nargs='+',
-                    help='Apply the given list of labels to events uploaded '
-                         'to GraceDB.')
 parser.add_argument('--ifar-upload-threshold', type=float, required=True,
                     help='Inverse-FAR threshold for uploading candidate '
                          'triggers to GraceDB, in years.')
 parser.add_argument('--file-prefix', default='Live')
 
 parser.add_argument('--round-start-time', type=int, metavar='X',
                     help="Round up the start time to the nearest multiple of X"
@@ -884,25 +839,15 @@
                     help="Time in seconds to allow for a plan to be created")
 parser.add_argument('--run-snr-optimization', action='store_true',
                     default=False,
                     help='Run spawned followup processes to maximize SNR for '
                          'any trigger uploaded to GraceDB')
 parser.add_argument('--snr-opt-timeout', type=int, default=400, metavar='SECONDS',
                     help='Maximum allowed duration of followup process to maximize SNR')
-parser.add_argument('--snr-opt-label', type=str, default='SNR_OPTIMIZED',
-                    help='Label to apply to snr-optimized GraceDB uploads')
-
 
-parser.add_argument('--enable-embright-has-massgap', action='store_true', default=False,
-                    help='Estimate HasMassGap probability for EMBright info. Lower limit '
-                         'of the mass gap is equal to the maximum NS mass used for '
-                         'the source classification.')
-parser.add_argument('--embright-massgap-max', type=float, default=5.0, metavar='SOLAR MASSES',
-                    help='Upper limit of the mass gap, used for estimating '
-                         'HasMassGap probability.')
 
 scheme.insert_processing_option_group(parser)
 LiveSingle.insert_args(parser)
 fft.insert_fft_option_group(parser)
 Coincer.insert_args(parser)
 SingleDetSGChisq.insert_option_group(parser)
 mchirp_area.insert_args(parser)
```

### Comparing `PyCBC-2.1.2/bin/pycbc_live_nagios_monitor` & `PyCBC-2.2.0/bin/pycbc_live_nagios_monitor`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_losc_segment_query` & `PyCBC-2.2.0/bin/pycbc_losc_segment_query`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_make_banksim` & `PyCBC-2.2.0/bin/pycbc_make_banksim`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_make_faithsim` & `PyCBC-2.2.0/bin/pycbc_make_faithsim`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_make_html_page` & `PyCBC-2.2.0/bin/pycbc_make_html_page`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_make_skymap` & `PyCBC-2.2.0/bin/pycbc_make_skymap`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_merge_inj_hdf` & `PyCBC-2.2.0/bin/pycbc_merge_inj_hdf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_multi_inspiral` & `PyCBC-2.2.0/bin/pycbc_multi_inspiral`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_optimal_snr` & `PyCBC-2.2.0/bin/pycbc_optimal_snr`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_optimize_snr` & `PyCBC-2.2.0/bin/pycbc_optimize_snr`

 * *Files 1% similar despite different names*

```diff
@@ -226,17 +226,14 @@
                          'consider it part of the coincidence. Not implemented')
 parser.add_argument('--gracedb-server', metavar='URL',
                     help='URL of GraceDB server API for uploading events. '
                          'If not provided, the default URL is used.')
 parser.add_argument('--gracedb-search', type=str, default='AllSky',
                     help='String going into the "search" field of the GraceDB '
                          'events')
-parser.add_argument('--gracedb-labels', metavar='LABEL', nargs='+',
-                    help='Apply the given list of labels to events uploaded '
-                         'to GraceDB.')
 parser.add_argument('--production', action='store_true',
                     help='Upload a production event rather than a test event')
 parser.add_argument('--enable-gracedb-upload', action='store_true', default=False,
                     help='Upload triggers to GraceDB')
 parser.add_argument('--output-path', required=True,
                     help='Path to a directory to store results in')
 parser.add_argument('--cores', type=int,
@@ -510,15 +507,15 @@
                'parameters that maximize the SNR. The FAR of this trigger is '
                'copied from {0} and does not reflect this trigger\'s template '
                'parameters.')
     comment = comment.format(original_gid)
 
     gid = doc.upload(xml_path, gracedb_server=args.gracedb_server,
                      testing=(not args.production), extra_strings=[comment],
-                     search=args.gracedb_search, labels=args.gracedb_labels)
+                     search=args.gracedb_search)
     if gid is not None:
         logging.info('Event uploaded as %s', gid)
 
         # add a note to the original G event pointing to the optimized one
         from ligo.gracedb.rest import GraceDb
 
         gracedb = GraceDb(args.gracedb_server) \
```

### Comparing `PyCBC-2.1.2/bin/pycbc_process_sngls` & `PyCBC-2.2.0/bin/pycbc_process_sngls`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_randomize_inj_dist_by_optsnr` & `PyCBC-2.2.0/bin/pycbc_randomize_inj_dist_by_optsnr`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_single_template` & `PyCBC-2.2.0/bin/pycbc_single_template`

 * *Files 0% similar despite different names*

```diff
@@ -283,16 +283,16 @@
         else:
             ra, dec, time = inj.longitude, inj.latitude, inj.time_geocent
         ltt = detector.time_delay_from_earth_center(ra, dec, time)
         td_template._epoch -= time + ltt
         # Check if waveform is too long
         tlen = (flen-1) * 2
         # FIXME: Hardcoded 7./8. factor here, but I'm not too bothered by this.
-        if len(td_template) > (7 * tlen /8):
-            new_start_idx = len(td_template) - (7 * tlen /8)
+        if len(td_template) > (7 * tlen // 8):
+            new_start_idx = len(td_template) - (7 * tlen // 8)
             td_template = td_template[new_start_idx:]
             taper_func = pycbc.waveform.utils.taper_timeseries
             td_template = taper_func(td_template, tapermethod='TAPER_START')
         if hasattr(inj, 'waveform'):
             approximant = inj.waveform
         else:
             approximant = inj.approximant
```

### Comparing `PyCBC-2.1.2/bin/pycbc_source_probability_offline` & `PyCBC-2.2.0/bin/pycbc_source_probability_offline`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_split_inspinj` & `PyCBC-2.2.0/bin/pycbc_split_inspinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_splitbank` & `PyCBC-2.2.0/bin/pycbc_splitbank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_stageout_failed_workflow` & `PyCBC-2.2.0/bin/pycbc_stageout_failed_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_submit_dax` & `PyCBC-2.2.0/bin/pycbc_submit_dax`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pycbc_upload_xml_to_gracedb` & `PyCBC-2.2.0/bin/pycbc_upload_xml_to_gracedb`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_grb_inj_combiner` & `PyCBC-2.2.0/bin/pygrb/pycbc_grb_inj_combiner`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_grb_inj_finder` & `PyCBC-2.2.0/bin/pygrb/pycbc_grb_inj_finder`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_grb_trig_cluster` & `PyCBC-2.2.0/bin/pygrb/pycbc_grb_trig_cluster`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_grb_trig_combiner` & `PyCBC-2.2.0/bin/pygrb/pycbc_grb_trig_combiner`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_make_offline_grb_workflow` & `PyCBC-2.2.0/bin/pygrb/pycbc_make_offline_grb_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_efficiency` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_efficiency`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_grb_info_table` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_grb_info_table`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_minifollowups` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_minifollowups`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_page_tables` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_page_tables`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_chisq_veto` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_chisq_veto`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_coh_ifosnr` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_coh_ifosnr`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_injs_results` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_injs_results`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_null_stats` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_null_stats`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_skygrid` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_skygrid`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_snr_timeseries` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_snr_timeseries`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_plot_stats_distribution` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_plot_stats_distribution`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/pygrb/pycbc_pygrb_pp_workflow` & `PyCBC-2.2.0/bin/pygrb/pycbc_pygrb_pp_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_combine_injection_comparisons` & `PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_combine_injection_comparisons`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_injection_set_comparison` & `PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_injection_set_comparison`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_plot_injections_found_both_workflows` & `PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_plot_injections_found_both_workflows`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_plot_injections_missed_one_workflow` & `PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_plot_injections_missed_one_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflow_comparisons/offline_search/pycbc_plot_vt_ratio_vs_ifar` & `PyCBC-2.2.0/bin/workflow_comparisons/offline_search/pycbc_plot_vt_ratio_vs_ifar`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflows/pycbc_make_bank_verifier_workflow` & `PyCBC-2.2.0/bin/workflows/pycbc_make_bank_verifier_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflows/pycbc_make_coinc_search_workflow` & `PyCBC-2.2.0/bin/workflows/pycbc_make_coinc_search_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflows/pycbc_make_faithsim_workflow` & `PyCBC-2.2.0/bin/workflows/pycbc_make_faithsim_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflows/pycbc_make_inference_inj_workflow` & `PyCBC-2.2.0/bin/workflows/pycbc_make_inference_inj_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflows/pycbc_make_inference_plots_workflow` & `PyCBC-2.2.0/bin/workflows/pycbc_make_inference_plots_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflows/pycbc_make_inference_workflow` & `PyCBC-2.2.0/bin/workflows/pycbc_make_inference_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflows/pycbc_make_psd_estimation_workflow` & `PyCBC-2.2.0/bin/workflows/pycbc_make_psd_estimation_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflows/pycbc_make_sbank_workflow` & `PyCBC-2.2.0/bin/workflows/pycbc_make_sbank_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/bin/workflows/pycbc_make_uberbank_workflow` & `PyCBC-2.2.0/bin/workflows/pycbc_make_uberbank_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/banksim/injection0.xml` & `PyCBC-2.2.0/examples/banksim/injection0.xml`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/cal/foton_filter_esd_saturation/pycbc_check_esd_saturation.sh` & `PyCBC-2.2.0/examples/cal/foton_filter_esd_saturation/pycbc_check_esd_saturation.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/cal/foton_filter_esd_saturation/pycbc_check_pcal_saturation.sh` & `PyCBC-2.2.0/examples/cal/foton_filter_esd_saturation/pycbc_check_pcal_saturation.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/cal/foton_filter_esd_saturation/run_pcal_saturation_example.sh` & `PyCBC-2.2.0/examples/cal/foton_filter_esd_saturation/run_pcal_saturation_example.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/catalog/data.py` & `PyCBC-2.2.0/examples/catalog/data.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/dataquality/on.py` & `PyCBC-2.2.0/examples/dataquality/on.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/detector/ant.py` & `PyCBC-2.2.0/examples/detector/ant.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/detector/delay.py` & `PyCBC-2.2.0/examples/detector/delay.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/detector/loc.py` & `PyCBC-2.2.0/examples/detector/loc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/distributions/mass_examples.py` & `PyCBC-2.2.0/examples/distributions/mass_examples.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/distributions/mchirp_q_from_uniform_m1m2_example.py` & `PyCBC-2.2.0/examples/distributions/mchirp_q_from_uniform_m1m2_example.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/distributions/sampling_from_config_example.py` & `PyCBC-2.2.0/examples/distributions/sampling_from_config_example.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/distributions/spin_examples.py` & `PyCBC-2.2.0/examples/distributions/spin_examples.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/distributions/spin_spatial_distr_example.py` & `PyCBC-2.2.0/examples/distributions/spin_spatial_distr_example.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/faith/injection0.xml` & `PyCBC-2.2.0/examples/faith/injection0.xml`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/filter/chisq.py` & `PyCBC-2.2.0/examples/filter/chisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/filter/fir.py` & `PyCBC-2.2.0/examples/filter/fir.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/filter/pass.py` & `PyCBC-2.2.0/examples/filter/pass.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/filter/snr.py` & `PyCBC-2.2.0/examples/filter/snr.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/gw150914/audio.py` & `PyCBC-2.2.0/examples/gw150914/audio.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/gw150914/gw150914_h1_snr.py` & `PyCBC-2.2.0/examples/gw150914/gw150914_h1_snr.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/gw150914/gw150914_shape.py` & `PyCBC-2.2.0/examples/gw150914/gw150914_shape.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/bbh-injection/run.sh` & `PyCBC-2.2.0/examples/inference/bbh-injection/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/bbh-injection/run_test.sh` & `PyCBC-2.2.0/examples/inference/bbh-injection/run_test.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/gw150914/plot.sh` & `PyCBC-2.2.0/examples/inference/gw150914/plot.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/gw150914/run.sh` & `PyCBC-2.2.0/examples/inference/gw150914/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/gw150914/run_test.sh` & `PyCBC-2.2.0/examples/inference/gw150914/run_test.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/hierarchical/run_test.sh` & `PyCBC-2.2.0/examples/inference/hierarchical/run_test.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/lisa_smbhb/advanced_plot.py` & `PyCBC-2.2.0/examples/inference/lisa_smbhb/advanced_plot.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/lisa_smbhb/get.sh` & `PyCBC-2.2.0/examples/inference/lisa_smbhb/get.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/margtime/run.sh` & `PyCBC-2.2.0/examples/inference/margtime/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/margtime/run_inj.sh` & `PyCBC-2.2.0/examples/inference/margtime/run_inj.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/samplers/run.sh` & `PyCBC-2.2.0/examples/inference/samplers/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inference/single/run_marg.sh` & `PyCBC-2.2.0/examples/inference/single/run_marg.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inspiral/check_GW150914_detection.py` & `PyCBC-2.2.0/examples/inspiral/check_GW150914_detection.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/inspiral/run.sh` & `PyCBC-2.2.0/examples/inspiral/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/live/check_results.py` & `PyCBC-2.2.0/examples/live/check_results.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/live/generate_injections.py` & `PyCBC-2.2.0/examples/live/generate_injections.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/live/make_singles_fits_file.py` & `PyCBC-2.2.0/examples/live/make_singles_fits_file.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/live/run.sh` & `PyCBC-2.2.0/examples/live/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/make_skymap/GW170817.sh` & `PyCBC-2.2.0/examples/make_skymap/GW170817.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/make_skymap/simulated_data.sh` & `PyCBC-2.2.0/examples/make_skymap/simulated_data.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/multi_inspiral/check_faceon_faceaway_trigs.py` & `PyCBC-2.2.0/examples/multi_inspiral/check_faceon_faceaway_trigs.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/multi_inspiral/check_gw170817_trigs.py` & `PyCBC-2.2.0/examples/multi_inspiral/check_gw170817_trigs.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/multi_inspiral/faceon_faceaway.sh` & `PyCBC-2.2.0/examples/multi_inspiral/faceon_faceaway.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/multi_inspiral/run.sh` & `PyCBC-2.2.0/examples/multi_inspiral/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/noise/frequency.py` & `PyCBC-2.2.0/examples/noise/frequency.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/overlap.py` & `PyCBC-2.2.0/examples/overlap.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/psd/analytic.py` & `PyCBC-2.2.0/examples/psd/analytic.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/psd/estimate.py` & `PyCBC-2.2.0/examples/psd/estimate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/psd/read.py` & `PyCBC-2.2.0/examples/psd/read.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/search/check_job.py` & `PyCBC-2.2.0/examples/search/check_job.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/search/stats.sh` & `PyCBC-2.2.0/examples/search/stats.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/tmpltbank/testAligned.sh` & `PyCBC-2.2.0/examples/tmpltbank/testAligned.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/tmpltbank/testAligned2.sh` & `PyCBC-2.2.0/examples/tmpltbank/testAligned2.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/tmpltbank/testAligned3.sh` & `PyCBC-2.2.0/examples/tmpltbank/testAligned3.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/tmpltbank/testNonspin.sh` & `PyCBC-2.2.0/examples/tmpltbank/testNonspin.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/tmpltbank/testStoch.sh` & `PyCBC-2.2.0/examples/tmpltbank/testStoch.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/tmpltbank/testStoch4.sh` & `PyCBC-2.2.0/examples/tmpltbank/testStoch4.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/waveform/add_waveform.py` & `PyCBC-2.2.0/examples/waveform/add_waveform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/waveform/match_waveform.py` & `PyCBC-2.2.0/examples/waveform/match_waveform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/waveform/plot_detwaveform.py` & `PyCBC-2.2.0/examples/waveform/plot_detwaveform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/waveform/plot_fd_td.py` & `PyCBC-2.2.0/examples/waveform/plot_fd_td.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/waveform/plot_freq.py` & `PyCBC-2.2.0/examples/waveform/plot_freq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/waveform/plot_phase.py` & `PyCBC-2.2.0/examples/waveform/plot_phase.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/data_checker/daily_test.py` & `PyCBC-2.2.0/examples/workflow/data_checker/daily_test.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/data_checker/get_data_example.py` & `PyCBC-2.2.0/examples/workflow/data_checker/get_data_example.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/dayhopecheck/dayhopecheck.py` & `PyCBC-2.2.0/examples/workflow/dayhopecheck/dayhopecheck.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/generic/multilevel_subworkflow_data/simple.py` & `PyCBC-2.2.0/examples/workflow/generic/multilevel_subworkflow_data/simple.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/generic/simple_subworkflow_data/simple.py` & `PyCBC-2.2.0/examples/workflow/generic/simple_subworkflow_data/simple.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/inference/bbh_inj-dynesty/create_inj_workflow.sh` & `PyCBC-2.2.0/examples/workflow/inference/bbh_inj-dynesty/create_inj_workflow.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/pygrb/ER7/run_er7_pygrb_offline.sh` & `PyCBC-2.2.0/examples/workflow/pygrb/ER7/run_er7_pygrb_offline.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/pygrb/ER8/run_er8_pygrb_offline.sh` & `PyCBC-2.2.0/examples/workflow/pygrb/ER8/run_er8_pygrb_offline.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/pygrb/ER8/run_er8_pygrb_online.sh` & `PyCBC-2.2.0/examples/workflow/pygrb/ER8/run_er8_pygrb_online.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/examples/workflow/pygrb/S6/run_s6_pygrb.sh` & `PyCBC-2.2.0/examples/workflow/pygrb/S6/run_s6_pygrb.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/__init__.py` & `PyCBC-2.2.0/pycbc/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/_version.py` & `PyCBC-2.2.0/pycbc/_version.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/_version_helper.py` & `PyCBC-2.2.0/pycbc/_version_helper.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/bin_utils.py` & `PyCBC-2.2.0/pycbc/bin_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/boundaries.py` & `PyCBC-2.2.0/pycbc/boundaries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/catalog/__init__.py` & `PyCBC-2.2.0/pycbc/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/catalog/catalog.py` & `PyCBC-2.2.0/pycbc/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/conversions.py` & `PyCBC-2.2.0/pycbc/conversions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/coordinates.py` & `PyCBC-2.2.0/pycbc/coordinates.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/cosmology.py` & `PyCBC-2.2.0/pycbc/cosmology.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/detector.py` & `PyCBC-2.2.0/pycbc/detector.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/__init__.py` & `PyCBC-2.2.0/pycbc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/angular.py` & `PyCBC-2.2.0/pycbc/distributions/angular.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/arbitrary.py` & `PyCBC-2.2.0/pycbc/distributions/arbitrary.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/bounded.py` & `PyCBC-2.2.0/pycbc/distributions/bounded.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/constraints.py` & `PyCBC-2.2.0/pycbc/distributions/constraints.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/external.py` & `PyCBC-2.2.0/pycbc/distributions/external.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/fixedsamples.py` & `PyCBC-2.2.0/pycbc/distributions/fixedsamples.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/gaussian.py` & `PyCBC-2.2.0/pycbc/distributions/gaussian.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/joint.py` & `PyCBC-2.2.0/pycbc/distributions/joint.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/mass.py` & `PyCBC-2.2.0/pycbc/distributions/mass.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/power_law.py` & `PyCBC-2.2.0/pycbc/distributions/power_law.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/qnm.py` & `PyCBC-2.2.0/pycbc/distributions/qnm.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/sky_location.py` & `PyCBC-2.2.0/pycbc/distributions/sky_location.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/spins.py` & `PyCBC-2.2.0/pycbc/distributions/spins.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/uniform.py` & `PyCBC-2.2.0/pycbc/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/uniform_log.py` & `PyCBC-2.2.0/pycbc/distributions/uniform_log.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/distributions/utils.py` & `PyCBC-2.2.0/pycbc/distributions/utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/dq.py` & `PyCBC-2.2.0/pycbc/dq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/coherent.py` & `PyCBC-2.2.0/pycbc/events/coherent.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/coinc.py` & `PyCBC-2.2.0/pycbc/events/coinc.py`

 * *Files 1% similar despite different names*

```diff
@@ -993,33 +993,18 @@
     @staticmethod
     def restore_state(filename):
         """Restore state of the background buffers from a file"""
         import pickle
         return pickle.load(filename)
 
     def ifar(self, coinc_stat):
-        """Map a given value of the coincident ranking statistic to an inverse
-        false-alarm rate (IFAR) using the interally stored background sample.
-
-        Parameters
-        ----------
-        coinc_stat: float
-            Value of the coincident ranking statistic to be converted.
-
-        Returns
-        -------
-        ifar: float
-            Inverse false-alarm rate in unit of years.
-        ifar_saturated: bool
-            True if `coinc_stat` is larger than all the available background,
-            in which case `ifar` is to be considered an upper limit.
+        """Return the far that would be associated with the coincident given.
         """
         n = self.coincs.num_greater(coinc_stat)
-        ifar = self.background_time / lal.YRJUL_SI / (n + 1)
-        return ifar, n == 0
+        return self.background_time / lal.YRJUL_SI / (n + 1)
 
     def set_singles_buffer(self, results):
         """Create the singles buffer
 
         This creates the singles buffer for each ifo. The dtype is determined
         by a representative sample of the single triggers in the results.
 
@@ -1245,15 +1230,15 @@
         if len(cstat) > 0:
             offsets = numpy.concatenate(offsets)
             ctime0 = numpy.concatenate(ctimes[self.ifos[0]]).astype(numpy.float64)
             ctime1 = numpy.concatenate(ctimes[self.ifos[1]]).astype(numpy.float64)
             logging.info("Clustering %s coincs", ppdets(self.ifos, "-"))
             cidx = cluster_coincs(cstat, ctime0, ctime1, offsets,
                                   self.timeslide_interval,
-                                  self.analysis_block + 2*self.time_window,
+                                  self.analysis_block,
                                   method='cython')
             offsets = offsets[cidx]
             zerolag_idx = (offsets == 0)
             bkg_idx = (offsets != 0)
 
             for ifo in self.ifos:
                 single_expire[ifo] = numpy.concatenate(single_expire[ifo])
@@ -1265,30 +1250,29 @@
         elif len(valid_ifos) > 0:
             self.coincs.increment(valid_ifos)
 
         # Collect coinc results for saving
         coinc_results = {}
         # Save information about zerolag triggers
         if num_zerolag > 0:
+            zerolag_results = {}
             idx = cidx[zerolag_idx][0]
             zerolag_cstat = cstat[cidx][zerolag_idx]
-            ifar, ifar_sat = self.ifar(zerolag_cstat)
-            zerolag_results = {
-                'foreground/ifar': ifar,
-                'foreground/ifar_saturated': ifar_sat,
-                'foreground/stat': zerolag_cstat,
-                'foreground/type': '-'.join(self.ifos)
-            }
+            zerolag_results['foreground/ifar'] = self.ifar(zerolag_cstat)
+            zerolag_results['foreground/stat'] = zerolag_cstat
             template = template_ids[idx]
             for ifo in self.ifos:
                 trig_id = trigger_ids[ifo][idx]
                 single_data = self.singles[ifo].data(template)[trig_id]
                 for key in single_data.dtype.names:
-                    path = f'foreground/{ifo}/{key}'
+                    path = 'foreground/%s/%s' % (ifo, key)
                     zerolag_results[path] = single_data[key]
+
+            zerolag_results['foreground/type'] = '-'.join(self.ifos)
+
             coinc_results.update(zerolag_results)
 
         # Save some summary statistics about the background
         coinc_results['background/time'] = numpy.array([self.background_time])
         coinc_results['background/count'] = len(self.coincs.data)
 
         # Save all the background triggers
```

### Comparing `PyCBC-2.1.2/pycbc/events/coinc_rate.py` & `PyCBC-2.2.0/pycbc/events/coinc_rate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/cuts.py` & `PyCBC-2.2.0/pycbc/events/cuts.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/eventmgr.py` & `PyCBC-2.2.0/pycbc/events/eventmgr.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/eventmgr_cython.pyx` & `PyCBC-2.2.0/pycbc/events/eventmgr_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/ranking.py` & `PyCBC-2.2.0/pycbc/events/ranking.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/significance.py` & `PyCBC-2.2.0/pycbc/events/significance.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/simd_threshold_ccode.cpp` & `PyCBC-2.2.0/pycbc/events/simd_threshold_ccode.cpp`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/simd_threshold_cython.pyx` & `PyCBC-2.2.0/pycbc/events/simd_threshold_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/single.py` & `PyCBC-2.2.0/pycbc/events/single.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/stat.py` & `PyCBC-2.2.0/pycbc/events/stat.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/threshold_cpu.py` & `PyCBC-2.2.0/pycbc/events/threshold_cpu.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/threshold_cuda.py` & `PyCBC-2.2.0/pycbc/events/threshold_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/trigger_fits.py` & `PyCBC-2.2.0/pycbc/events/trigger_fits.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/triggers.py` & `PyCBC-2.2.0/pycbc/events/triggers.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/events/veto.py` & `PyCBC-2.2.0/pycbc/events/veto.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/__init__.py` & `PyCBC-2.2.0/pycbc/fft/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/backend_cpu.py` & `PyCBC-2.2.0/pycbc/fft/backend_cpu.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/backend_cuda.py` & `PyCBC-2.2.0/pycbc/fft/backend_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/backend_mkl.py` & `PyCBC-2.2.0/pycbc/fft/backend_mkl.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/backend_support.py` & `PyCBC-2.2.0/pycbc/fft/backend_support.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/class_api.py` & `PyCBC-2.2.0/pycbc/fft/class_api.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/core.py` & `PyCBC-2.2.0/pycbc/fft/core.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/cuda_pyfft.py` & `PyCBC-2.2.0/pycbc/fft/cuda_pyfft.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/cufft.py` & `PyCBC-2.2.0/pycbc/fft/cufft.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/fft_callback.py` & `PyCBC-2.2.0/pycbc/fft/fft_callback.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/fftw.py` & `PyCBC-2.2.0/pycbc/fft/fftw.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/fftw_pruned.py` & `PyCBC-2.2.0/pycbc/fft/fftw_pruned.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/fftw_pruned_cython.pyx` & `PyCBC-2.2.0/pycbc/fft/fftw_pruned_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/func_api.py` & `PyCBC-2.2.0/pycbc/fft/func_api.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/mkl.py` & `PyCBC-2.2.0/pycbc/fft/mkl.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/npfft.py` & `PyCBC-2.2.0/pycbc/fft/npfft.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/fft/parser_support.py` & `PyCBC-2.2.0/pycbc/fft/parser_support.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/autocorrelation.py` & `PyCBC-2.2.0/pycbc/filter/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/fotonfilter.py` & `PyCBC-2.2.0/pycbc/filter/fotonfilter.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/matchedfilter.py` & `PyCBC-2.2.0/pycbc/filter/matchedfilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1795,35 +1795,30 @@
 
         return result, veto_info
 
 def followup_event_significance(ifo, data_reader, bank,
                                 template_id, coinc_times,
                                 coinc_threshold=0.005,
                                 lookback=150, duration=0.095):
-    """Given a detector, a template waveform and a set of candidate event
-    times in different detectors, perform an on-source/off-source analysis
-    to determine if the SNR in the first detector has a significant peak
-    in the on-source window. The significance is given in terms of a
-    p-value. See Dal Canton et al. 2021 (https://arxiv.org/abs/2008.07494)
-    for details.
+    """ Followup an event in another detector and determine its significance
     """
     from pycbc.waveform import get_waveform_filter_length_in_time
     tmplt = bank.table[template_id]
     length_in_time = get_waveform_filter_length_in_time(tmplt['approximant'],
                                                         tmplt)
 
     # calculate onsource time range
     from pycbc.detector import Detector
     onsource_start = -numpy.inf
     onsource_end = numpy.inf
     fdet = Detector(ifo)
 
     for cifo in coinc_times:
         time = coinc_times[cifo]
-        dtravel = Detector(cifo).light_travel_time_to_detector(fdet)
+        dtravel =  Detector(cifo).light_travel_time_to_detector(fdet)
         if time - dtravel > onsource_start:
             onsource_start = time - dtravel
         if time + dtravel < onsource_end:
             onsource_end = time + dtravel
 
     # Source must be within this time window to be considered a possible
     # coincidence
@@ -1837,23 +1832,23 @@
         bdur = data_reader.strain.duration * .75
 
     # Require all strain be valid within lookback time
     if data_reader.state is not None:
         state_start_time = data_reader.strain.end_time \
                 - data_reader.reduced_pad * data_reader.strain.delta_t - bdur
         if not data_reader.state.is_extent_valid(state_start_time, bdur):
-            return None
+            return None, None, None, None
 
     # We won't require that all DQ checks be valid for now, except at
     # onsource time.
     if data_reader.dq is not None:
         dq_start_time = onsource_start - duration / 2.0
         dq_duration = onsource_end - onsource_start + duration
         if not data_reader.dq.is_extent_valid(dq_start_time, dq_duration):
-            return None
+            return None, None, None, None
 
     # Calculate SNR time series for this duration
     htilde = bank.get_template(template_id, min_buffer=bdur)
     stilde = data_reader.overwhitened_data(htilde.delta_f)
 
     sigma2 = htilde.sigmasq(stilde.psd)
     snr, _, norm = matched_filter_core(htilde, stilde, h_norm=sigma2)
@@ -1867,35 +1862,27 @@
     bstart = float(snr.start_time) + length_in_time + trim_pad
     bkg = abs(snr.time_slice(bstart, onsource_start)).numpy()
 
     window = int((onsource_end - onsource_start) * snr.sample_rate)
     nsamples = int(len(bkg) / window)
 
     peaks = bkg[:nsamples*window].reshape(nsamples, window).max(axis=1)
-    num_louder_bg = (peaks >= peak_value).sum()
-    pvalue = (1 + num_louder_bg) / float(1 + nsamples)
-    pvalue_saturated = num_louder_bg == 0
+    pvalue = (1 + (peaks >= peak_value).sum()) / float(1 + nsamples)
 
     # Return recentered source SNR for bayestar, along with p-value, and trig
     peak_full = int((peak_time - snr.start_time) / snr.delta_t)
     half_dur_samples = int(snr.sample_rate * duration / 2)
     snr_slice = slice(peak_full - half_dur_samples,
                       peak_full + half_dur_samples + 1)
     baysnr = snr[snr_slice]
 
     logging.info('Adding %s to candidate, pvalue %s, %s samples', ifo,
                  pvalue, nsamples)
 
-    return {
-        'snr_series': baysnr * norm,
-        'peak_time': peak_time,
-        'pvalue': pvalue,
-        'pvalue_saturated': pvalue_saturated,
-        'sigma2': sigma2
-    }
+    return baysnr * norm, peak_time, pvalue, sigma2
 
 def compute_followup_snr_series(data_reader, htilde, trig_time,
                                 duration=0.095, check_state=True,
                                 coinc_window=0.05):
     """Given a StrainBuffer, a template frequency series and a trigger time,
     compute a portion of the SNR time series centered on the trigger for its
     rapid sky localization and followup.
```

### Comparing `PyCBC-2.1.2/pycbc/filter/matchedfilter_cpu.pyx` & `PyCBC-2.2.0/pycbc/filter/matchedfilter_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/matchedfilter_cuda.py` & `PyCBC-2.2.0/pycbc/filter/matchedfilter_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/matchedfilter_numpy.py` & `PyCBC-2.2.0/pycbc/filter/matchedfilter_numpy.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/qtransform.py` & `PyCBC-2.2.0/pycbc/filter/qtransform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/resample.py` & `PyCBC-2.2.0/pycbc/filter/resample.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/simd_correlate.py` & `PyCBC-2.2.0/pycbc/filter/simd_correlate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/simd_correlate_ccode.cpp` & `PyCBC-2.2.0/pycbc/filter/simd_correlate_ccode.cpp`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/simd_correlate_cython.pyx` & `PyCBC-2.2.0/pycbc/filter/simd_correlate_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/filter/zpk.py` & `PyCBC-2.2.0/pycbc/filter/zpk.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/frame/__init__.py` & `PyCBC-2.2.0/pycbc/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/frame/frame.py` & `PyCBC-2.2.0/pycbc/frame/frame.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/frame/losc.py` & `PyCBC-2.2.0/pycbc/frame/losc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/frame/store.py` & `PyCBC-2.2.0/pycbc/frame/store.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/burn_in.py` & `PyCBC-2.2.0/pycbc/inference/burn_in.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/entropy.py` & `PyCBC-2.2.0/pycbc/inference/entropy.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/evidence.py` & `PyCBC-2.2.0/pycbc/inference/evidence.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/gelman_rubin.py` & `PyCBC-2.2.0/pycbc/inference/gelman_rubin.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/geweke.py` & `PyCBC-2.2.0/pycbc/inference/geweke.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/__init__.py` & `PyCBC-2.2.0/pycbc/inference/io/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/base_hdf.py` & `PyCBC-2.2.0/pycbc/inference/io/base_hdf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/base_mcmc.py` & `PyCBC-2.2.0/pycbc/inference/io/base_mcmc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/base_multitemper.py` & `PyCBC-2.2.0/pycbc/inference/io/base_multitemper.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/base_nested_sampler.py` & `PyCBC-2.2.0/pycbc/inference/io/base_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/base_sampler.py` & `PyCBC-2.2.0/pycbc/inference/io/base_sampler.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/cpnest.py` & `PyCBC-2.2.0/pycbc/inference/io/cpnest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/dynesty.py` & `PyCBC-2.2.0/pycbc/inference/io/dynesty.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/emcee.py` & `PyCBC-2.2.0/pycbc/inference/io/emcee.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/emcee_pt.py` & `PyCBC-2.2.0/pycbc/inference/io/emcee_pt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/epsie.py` & `PyCBC-2.2.0/pycbc/inference/io/epsie.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/multinest.py` & `PyCBC-2.2.0/pycbc/inference/io/multinest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/posterior.py` & `PyCBC-2.2.0/pycbc/inference/io/posterior.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/ptemcee.py` & `PyCBC-2.2.0/pycbc/inference/io/ptemcee.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/txt.py` & `PyCBC-2.2.0/pycbc/inference/io/txt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/io/ultranest.py` & `PyCBC-2.2.0/pycbc/inference/io/ultranest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/jump/__init__.py` & `PyCBC-2.2.0/pycbc/inference/jump/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/jump/angular.py` & `PyCBC-2.2.0/pycbc/inference/jump/angular.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/jump/bounded_normal.py` & `PyCBC-2.2.0/pycbc/inference/jump/bounded_normal.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/jump/discrete.py` & `PyCBC-2.2.0/pycbc/inference/jump/discrete.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/jump/normal.py` & `PyCBC-2.2.0/pycbc/inference/jump/normal.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/__init__.py` & `PyCBC-2.2.0/pycbc/inference/models/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/analytic.py` & `PyCBC-2.2.0/pycbc/inference/models/analytic.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/base.py` & `PyCBC-2.2.0/pycbc/inference/models/base.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/base_data.py` & `PyCBC-2.2.0/pycbc/inference/models/base_data.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/brute_marg.py` & `PyCBC-2.2.0/pycbc/inference/models/brute_marg.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/data_utils.py` & `PyCBC-2.2.0/pycbc/inference/models/data_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/gated_gaussian_noise.py` & `PyCBC-2.2.0/pycbc/inference/models/gated_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/gaussian_noise.py` & `PyCBC-2.2.0/pycbc/inference/models/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/hierarchical.py` & `PyCBC-2.2.0/pycbc/inference/models/hierarchical.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/marginalized_gaussian_noise.py` & `PyCBC-2.2.0/pycbc/inference/models/marginalized_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/relbin.py` & `PyCBC-2.2.0/pycbc/inference/models/relbin.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/relbin_cpu.pyx` & `PyCBC-2.2.0/pycbc/inference/models/relbin_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/single_template.py` & `PyCBC-2.2.0/pycbc/inference/models/single_template.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/models/tools.py` & `PyCBC-2.2.0/pycbc/inference/models/tools.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/option_utils.py` & `PyCBC-2.2.0/pycbc/inference/option_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/__init__.py` & `PyCBC-2.2.0/pycbc/inference/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/base.py` & `PyCBC-2.2.0/pycbc/inference/sampler/base.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/base_cube.py` & `PyCBC-2.2.0/pycbc/inference/sampler/base_cube.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/base_mcmc.py` & `PyCBC-2.2.0/pycbc/inference/sampler/base_mcmc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/base_multitemper.py` & `PyCBC-2.2.0/pycbc/inference/sampler/base_multitemper.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/cpnest.py` & `PyCBC-2.2.0/pycbc/inference/sampler/cpnest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/dummy.py` & `PyCBC-2.2.0/pycbc/inference/sampler/dummy.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/dynesty.py` & `PyCBC-2.2.0/pycbc/inference/sampler/dynesty.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/emcee.py` & `PyCBC-2.2.0/pycbc/inference/sampler/emcee.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/emcee_pt.py` & `PyCBC-2.2.0/pycbc/inference/sampler/emcee_pt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/epsie.py` & `PyCBC-2.2.0/pycbc/inference/sampler/epsie.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/multinest.py` & `PyCBC-2.2.0/pycbc/inference/sampler/multinest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/ptemcee.py` & `PyCBC-2.2.0/pycbc/inference/sampler/ptemcee.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inference/sampler/ultranest.py` & `PyCBC-2.2.0/pycbc/inference/sampler/ultranest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inject/inject.py` & `PyCBC-2.2.0/pycbc/inject/inject.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/inject/injfilterrejector.py` & `PyCBC-2.2.0/pycbc/inject/injfilterrejector.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/io/__init__.py` & `PyCBC-2.2.0/pycbc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/io/hdf.py` & `PyCBC-2.2.0/pycbc/io/hdf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/io/ligolw.py` & `PyCBC-2.2.0/pycbc/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/io/live.py` & `PyCBC-2.2.0/pycbc/io/live.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,32 +257,32 @@
                 kwargs['padata'].do_pastro_calc(trigger_data, horizons)
         elif 'p_terr' in kwargs:
             self.p_astro, self.p_terr = 1 - kwargs['p_terr'], kwargs['p_terr']
         else:
             self.p_astro, self.p_terr = None, None
 
         # Source probabilities and hasmassgap estimation
-        self.probabilities = None
-        self.hasmassgap = None
         if 'mc_area_args' in kwargs:
             eff_distances = [sngl.eff_distance for sngl in sngl_inspiral_table]
             self.probabilities = calc_probabilities(coinc_inspiral_row.mchirp,
                                                     coinc_inspiral_row.snr,
                                                     min(eff_distances),
                                                     kwargs['mc_area_args'])
-            if 'embright_mg_max' in kwargs['mc_area_args']:
-                hasmg_args = copy.deepcopy(kwargs['mc_area_args'])
-                hasmg_args['mass_gap'] = True
-                hasmg_args['mass_bdary']['gap_max'] = \
-                    kwargs['mc_area_args']['embright_mg_max']
-                self.hasmassgap = calc_probabilities(
-                                      coinc_inspiral_row.mchirp,
-                                      coinc_inspiral_row.snr,
-                                      min(eff_distances),
-                                      hasmg_args)['Mass Gap']
+            kwargs['hasmassgap_args'] = copy.deepcopy(kwargs['mc_area_args'])
+            kwargs['hasmassgap_args']['mass_gap'] = True
+            kwargs['hasmassgap_args']['mass_bdary']['ns_max'] = 3.0
+            kwargs['hasmassgap_args']['mass_bdary']['gap_max'] = 5.0
+            self.hasmassgap = calc_probabilities(
+                                  coinc_inspiral_row.mchirp,
+                                  coinc_inspiral_row.snr,
+                                  min(eff_distances),
+                                  kwargs['hasmassgap_args'])['Mass Gap']
+        else:
+            self.probabilities = None
+            self.hasmassgap = None
 
         # Combine p astro and source probs
         if self.p_astro is not None and self.probabilities is not None:
             self.astro_probs = {cl: pr * self.p_astro for
                                 cl, pr in self.probabilities.items()}
             self.astro_probs['Terrestrial'] = self.p_terr
         else:
@@ -336,15 +336,15 @@
             self.pastro_file = os.path.join(save_dir, 'pa_pterr.json')
             with open(self.pastro_file, 'w') as pastrof:
                 json.dump({'p_astro': self.p_astro, 'p_terr': self.p_terr},
                           pastrof)
             logging.info('P_astro file saved as %s', self.pastro_file)
 
     def upload(self, fname, gracedb_server=None, testing=True,
-               extra_strings=None, search='AllSky', labels=None):
+               extra_strings=None, search='AllSky'):
         """Upload this candidate to GraceDB, and annotate it with a few useful
         plots and comments.
 
         Parameters
         ----------
         fname: str
             The name to give the xml file associated with this trigger
@@ -352,16 +352,14 @@
             URL to the GraceDB web API service for uploading the event.
             If omitted, the default will be used.
         testing: bool
             Switch to determine if the upload should be sent to gracedb as a
             test trigger (True) or a production trigger (False).
         search: str
             String going into the "search" field of the GraceDB event.
-        labels: list
-            Optional list of labels to tag the new event with.
         """
         import matplotlib
         matplotlib.use('Agg')
         import pylab as pl
 
         if fname.endswith('.xml.gz'):
             self.basename = fname.replace('.xml.gz', '')
@@ -371,82 +369,67 @@
             raise ValueError("Upload filename must end in .xml or .xml.gz, got"
                              " %s" % fname)
 
         # First make sure the event is saved on disk
         # as GraceDB operations can fail later
         self.save(fname)
 
-        # hardware injections need to be maked with the INJ tag
-        if self.is_hardware_injection:
-            labels = (labels or []) + ['INJ']
-
-        # connect to GraceDB if we are not reusing a connection
-        if not hasattr(self, 'gracedb'):
-            logging.info('Connecting to GraceDB')
-            gdbargs = {'reload_certificate': True, 'reload_buffer': 300}
-            if gracedb_server:
-                gdbargs['service_url'] = gracedb_server
-            try:
-                from ligo.gracedb.rest import GraceDb
-                self.gracedb = GraceDb(**gdbargs)
-            except Exception as exc:
-                logging.error('Failed to create GraceDB client')
-                logging.error(exc)
-
-        # create GraceDB event
-        logging.info('Uploading %s to GraceDB', fname)
-        group = 'Test' if testing else 'CBC'
         gid = None
         try:
-            response = self.gracedb.create_event(
-                group,
-                "pycbc",
-                fname,
-                search=search,
-                labels=labels
-            )
-            gid = response.json()["graceid"]
+            if not hasattr(self, 'gracedb'):
+                from ligo.gracedb.rest import GraceDb
+                gdbargs = {'reload_certificate': True, 'reload_buffer': 300}
+                self.gracedb = GraceDb(gracedb_server, **gdbargs) \
+                    if gracedb_server else GraceDb(**gdbargs)
+            # create GraceDB event
+            group = 'Test' if testing else 'CBC'
+            r = self.gracedb.create_event(group, "pycbc", fname, search).json()
+            gid = r["graceid"]
             logging.info("Uploaded event %s", gid)
+
+            if self.is_hardware_injection:
+                self.gracedb.write_label(gid, 'INJ')
+                logging.info("Tagging event %s as an injection", gid)
+
         except Exception as exc:
-            logging.error('Failed to create GraceDB event')
+            logging.error('Something failed during the upload of event %s on '
+                          'GraceDB. The event may not have been uploaded!',
+                          fname)
             logging.error(str(exc))
 
         # Upload em_bright properties JSON
-        if self.hasmassgap is not None and gid is not None:
+        if self.hasmassgap is not None:
             try:
                 self.gracedb.write_log(
                     gid, 'EM Bright properties JSON file upload',
                     filename=self.embright_file,
                     tag_name=['em_bright']
                 )
                 logging.info('Uploaded em_bright properties for %s', gid)
             except Exception as exc:
                 logging.error('Failed to upload em_bright properties file '
                               'for %s', gid)
                 logging.error(str(exc))
 
         # Upload multi-cpt p_astro JSON
-        if self.astro_probs is not None and gid is not None:
+        if self.astro_probs is not None:
             try:
                 self.gracedb.write_log(
                     gid, 'Multi-component p_astro JSON file upload',
                     filename=self.multipa_file,
                     tag_name=['p_astro'],
                     label='PASTRO_READY'
                 )
                 logging.info('Uploaded multi p_astro for %s', gid)
             except Exception as exc:
-                logging.error(
-                    'Failed to upload multi p_astro file for %s',
-                    gid
-                )
+                logging.error('Failed to upload multi p_astro file for %s', gid)
                 logging.error(str(exc))
 
         # If there is p_astro but no probabilities, upload p_astro JSON
-        if hasattr(self, 'pastro_file') and gid is not None:
+        if hasattr(self, 'pastro_file'):
             try:
                 self.gracedb.write_log(
                     gid, '2-component p_astro JSON file upload',
                     filename=self.pastro_file,
                     tag_name=['sig_info']
                 )
                 logging.info('Uploaded p_astro for %s', gid)
@@ -486,15 +469,15 @@
             for ifo in sorted(self.psds):
                 # Undo dynamic range factor
                 curr_psd = self.psds[ifo].astype(numpy.float64)
                 curr_psd /= pycbc.DYN_RANGE_FAC ** 2.0
                 curr_psd.save(snr_series_fname, group='%s/psd' % ifo)
 
         # Upload SNR series in HDF format and plots
-        if self.snr_series is not None and gid is not None:
+        if self.snr_series is not None:
             try:
                 self.gracedb.write_log(
                     gid, 'SNR timeseries HDF file upload',
                     filename=snr_series_fname
                 )
                 self.gracedb.write_log(
                     gid, 'SNR timeseries plot upload',
@@ -524,39 +507,32 @@
             colors = [source_color(label) for label in labels]
             fig, ax = pl.subplots()
             ax.pie(sizes, labels=labels, colors=colors, autopct='%1.1f%%',
                    textprops={'fontsize': 15})
             ax.axis('equal')
             fig.savefig(self.prob_plotf)
             pl.close()
-            if gid is not None:
-                try:
-                    self.gracedb.write_log(
-                        gid,
-                        'Source probabilities JSON file upload',
-                        filename=self.prob_file,
-                        tag_name=['pe']
-                    )
-                    logging.info('Uploaded source probabilities for %s', gid)
-                    self.gracedb.write_log(
-                        gid,
-                        'Source probabilities plot upload',
-                        filename=self.prob_plotf,
-                        tag_name=['pe']
-                    )
-                    logging.info(
-                        'Uploaded source probabilities pie chart for %s',
-                        gid
-                    )
-                except Exception as exc:
-                    logging.error(
-                        'Failed to upload source probability results for %s',
-                        gid
-                    )
-                    logging.error(str(exc))
+            try:
+                self.gracedb.write_log(
+                    gid, 'Source probabilities JSON file upload',
+                    filename=self.prob_file,
+                    tag_name=['pe']
+                )
+                logging.info('Uploaded source probabilities for %s', gid)
+                self.gracedb.write_log(
+                    gid, 'Source probabilities plot upload',
+                    filename=self.prob_plotf,
+                    tag_name=['pe']
+                )
+                logging.info('Uploaded source probabilities pie chart for %s',
+                             gid)
+            except Exception as exc:
+                logging.error(
+                    'Failed to upload source probability results for %s', gid)
+                logging.error(str(exc))
 
         if gid is not None:
             try:
                 # Add code version info
                 gracedb_tag_with_version(self.gracedb, gid)
                 # Add any annotations to the event log
                 for text in (extra_strings or []):
```

### Comparing `PyCBC-2.1.2/pycbc/io/record.py` & `PyCBC-2.2.0/pycbc/io/record.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/libutils.py` & `PyCBC-2.2.0/pycbc/libutils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/mchirp_area.py` & `PyCBC-2.2.0/pycbc/mchirp_area.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/neutron_stars/eos_utils.py` & `PyCBC-2.2.0/pycbc/neutron_stars/eos_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/neutron_stars/ns_data/equil_2H.dat` & `PyCBC-2.2.0/pycbc/neutron_stars/ns_data/equil_2H.dat`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/neutron_stars/pg_isso_solver.py` & `PyCBC-2.2.0/pycbc/neutron_stars/pg_isso_solver.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/noise/gaussian.py` & `PyCBC-2.2.0/pycbc/noise/gaussian.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/noise/reproduceable.py` & `PyCBC-2.2.0/pycbc/noise/reproduceable.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/opt.py` & `PyCBC-2.2.0/pycbc/opt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/pnutils.py` & `PyCBC-2.2.0/pycbc/pnutils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/pool.py` & `PyCBC-2.2.0/pycbc/pool.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/population/fgmc_functions.py` & `PyCBC-2.2.0/pycbc/population/fgmc_functions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/population/fgmc_laguerre.py` & `PyCBC-2.2.0/pycbc/population/fgmc_laguerre.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/population/fgmc_plots.py` & `PyCBC-2.2.0/pycbc/population/fgmc_plots.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/population/live_pastro.py` & `PyCBC-2.2.0/pycbc/population/live_pastro.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,35 +27,14 @@
            len(spec_json['sig_per_yr_binned']) + 1
     assert 'ref_bns_horizon' in spec_json  # float
     assert 'netsnr_thresh' in spec_json  # float
 
     return spec_json
 
 
-def check_template_param_bin_farlim_data(spec_json):
-    """
-    Parameters
-    ----------
-    spec_json: JSON dictionary-like object
-        Result of parsing json file containing static data
-
-    Returns
-    -------
-    spec_json: dictionary
-    """
-    # Standard template param bin checks
-    check_template_param_bin_data(spec_json)
-
-    # In addition, need limiting FAR and SNR values
-    assert 'limit_far' in spec_json
-    assert 'limit_snr' in spec_json
-
-    return spec_json
-
-
 def read_template_bank_param(spec_d, bankf):
     """
     Parameters
     ----------
     spec_d: dictionary
         Prerequisite data for p astro calc
     bankf: string
@@ -223,15 +202,15 @@
 
     # Get noise rate density
     if 'bg_fac' not in padata.spec:
         expfac = 6.
     else:
         expfac = padata.spec['bg_fac']
 
-    # List of ifos over trigger threshold
+    # Ifos over trigger threshold
     tr_ifos = trdata['triggered']
 
     # FAR is in Hz, therefore convert to rate per year (per SNR)
     dnoise = noise_density_from_far(trdata['far'], expfac) * lal_s_per_yr
     logging.debug('FAR %.3g, noise density per yr per SNR %.3g',
                   trdata['far'], dnoise)
     # Scale by fraction of templates in bin
@@ -255,41 +234,17 @@
     logging.debug('After triggered ifo rate rescaling %.3g', dsig)
 
     p_astro = dsig / (dsig + dnoise)
     logging.debug('p_astro %.4g', p_astro)
     return p_astro, 1 - p_astro
 
 
-def template_param_bin_types_farlim_pa(padata, trdata, horizons):
-    """
-    Parameters
-    ----------
-    padata: PAstroData instance
-        Static information on p astro calculation
-    trdata: dictionary
-        Trigger properties
-    horizons: dictionary
-        BNS horizon distances keyed on ifo
-
-    Returns
-    -------
-    p_astro, p_terr: tuple of floats
-    """
-    # If the network SNR and FAR indicate saturation of the FAR estimate,
-    # set them to specified fixed values
-    trdata = padata.apply_significance_limits(trdata)
-
-    # Now perform standard calculation with event types
-    return template_param_bin_types_pa(padata, trdata, horizons)
-
-
 __all__ = [
     "check_template_param_bin_data",
     "read_template_bank_param",
     "noise_density_from_far",
     "signal_pdf_from_snr",
     "signal_rate_rescale",
     "signal_rate_trig_type",
     "template_param_bin_pa",
     "template_param_bin_types_pa",
-    "template_param_bin_types_farlim_pa",
 ]
```

### Comparing `PyCBC-2.1.2/pycbc/population/live_pastro_utils.py` & `PyCBC-2.2.0/pycbc/population/live_pastro_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,31 +23,26 @@
                                    'up p_astro calculation')
 
     return live_pastro_group
 
 
 # Choices of p astro calc method
 _check_spec = {
-    'template_param_bins': livepa.check_template_param_bin_data,
-    'template_param_bins_types': livepa.check_template_param_bin_data,
-    'template_param_bins_types_farlim':
-        livepa.check_template_param_bin_farlim_data
+      'template_param_bins': livepa.check_template_param_bin_data,
+      'template_param_bins_types': livepa.check_template_param_bin_data
 }
 
 _read_bank = {
-    'template_param_bins': livepa.read_template_bank_param,
-    'template_param_bins_types': livepa.read_template_bank_param,
-    'template_param_bins_types_farlim': livepa.read_template_bank_param
+      'template_param_bins': livepa.read_template_bank_param,
+      'template_param_bins_types': livepa.read_template_bank_param
 }
 
 _do_calc = {
-    'template_param_bins': livepa.template_param_bin_pa,
-    'template_param_bins_types': livepa.template_param_bin_types_pa,
-    'template_param_bins_types_farlim':
-        livepa.template_param_bin_types_farlim_pa
+      'template_param_bins': livepa.template_param_bin_pa,
+      'template_param_bins_types': livepa.template_param_bin_types_pa
 }
 
 
 class PAstroData():
     """ Class for managing live p_astro calculation persistent info """
     def __init__(self, specfile, bank):
         """
@@ -72,40 +67,14 @@
             except KeyError as ke:
                 raise ValueError("Can't find 'method' in p_astro spec file!") \
                     from ke
             logging.info('Setting up p_astro data with method %s', self.method)
             self.spec = _check_spec[self.method](self.spec_json)
             self.bank = _read_bank[self.method](self.spec, bank)
 
-    def apply_significance_limits(self, trigger_data):
-        """
-        If the network SNR and FAR indicate saturation of the FAR estimate,
-        set them to the fixed values given in the specification.
-        """
-        # This only happens for double or triple events
-        if len(trigger_data['triggered']) == 1:
-            return trigger_data
-
-        if len(trigger_data['triggered']) > 1:
-            farlim = self.spec['limit_far']
-            snrlim = self.spec['limit_snr']
-            # Only do anything if FAR and SNR are beyond given limits
-            if trigger_data['far'] > farlim or \
-                    trigger_data['network_snr'] < snrlim:
-                return trigger_data
-
-            logging.debug('Truncating FAR and SNR from %f, %f to %f, %f',
-                          trigger_data['far'], trigger_data['network_snr'],
-                          farlim, snrlim)
-            trigger_data['network_snr'] = snrlim
-            trigger_data['far'] = farlim
-            return trigger_data
-
-        raise RuntimeError('Number of triggered ifos must be >0 !')
-
     def do_pastro_calc(self, trigger_data, horizons):
         """ No-op, or call the despatch dictionary to evaluate p_astro """
         if not self.do:
             return None, None
 
         logging.info('Computing p_astro')
         p_astro, p_terr = _do_calc[self.method](self, trigger_data, horizons)
```

### Comparing `PyCBC-2.1.2/pycbc/population/population_models.py` & `PyCBC-2.2.0/pycbc/population/population_models.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/population/rates_functions.py` & `PyCBC-2.2.0/pycbc/population/rates_functions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/population/scale_injections.py` & `PyCBC-2.2.0/pycbc/population/scale_injections.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/psd/__init__.py` & `PyCBC-2.2.0/pycbc/psd/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/psd/analytical.py` & `PyCBC-2.2.0/pycbc/psd/analytical.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/psd/analytical_space.py` & `PyCBC-2.2.0/pycbc/psd/analytical_space.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/psd/estimate.py` & `PyCBC-2.2.0/pycbc/psd/estimate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/psd/read.py` & `PyCBC-2.2.0/pycbc/psd/read.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/psd/variation.py` & `PyCBC-2.2.0/pycbc/psd/variation.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/rate.py` & `PyCBC-2.2.0/pycbc/rate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/color.py` & `PyCBC-2.2.0/pycbc/results/color.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/dq.py` & `PyCBC-2.2.0/pycbc/results/dq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/followup.py` & `PyCBC-2.2.0/pycbc/results/followup.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/layout.py` & `PyCBC-2.2.0/pycbc/results/layout.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/legacy_grb.py` & `PyCBC-2.2.0/pycbc/results/legacy_grb.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/metadata.py` & `PyCBC-2.2.0/pycbc/results/metadata.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/mpld3_utils.py` & `PyCBC-2.2.0/pycbc/results/mpld3_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/plot.py` & `PyCBC-2.2.0/pycbc/results/plot.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/psd.py` & `PyCBC-2.2.0/pycbc/results/psd.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/pygrb_plotting_utils.py` & `PyCBC-2.2.0/pycbc/results/pygrb_plotting_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/pygrb_postprocessing_utils.py` & `PyCBC-2.2.0/pycbc/results/pygrb_postprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/render.py` & `PyCBC-2.2.0/pycbc/results/render.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/scatter_histograms.py` & `PyCBC-2.2.0/pycbc/results/scatter_histograms.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/css/bootstrap/3.3.2/bootstrap.min.css` & `PyCBC-2.2.0/pycbc/results/static/css/bootstrap/3.3.2/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/css/bootstrap.min.css` & `PyCBC-2.2.0/pycbc/results/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/css/fancybox/2.1.5/jquery.fancybox.css` & `PyCBC-2.2.0/pycbc/results/static/css/fancybox/2.1.5/jquery.fancybox.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/css/pycbc/orange.css` & `PyCBC-2.2.0/pycbc/results/static/css/pycbc/orange.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/css/pycbc/red.css` & `PyCBC-2.2.0/pycbc/results/static/css/pycbc/red.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Light.eot` & `PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Light.eot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Light.html` & `PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Light.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Light.ttf` & `PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Light.woff` & `PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Light.woff`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Semibold.eot` & `PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Semibold.eot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Semibold.html` & `PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Semibold.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Semibold.ttf` & `PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/fonts/Lato-Semibold.woff` & `PyCBC-2.2.0/pycbc/results/static/fonts/Lato-Semibold.woff`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/js/bootstrap/3.3.2/bootstrap.min.js` & `PyCBC-2.2.0/pycbc/results/static/js/bootstrap/3.3.2/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/js/bootstrap.min.js` & `PyCBC-2.2.0/pycbc/results/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/js/fancybox/2.1.5/fancybox-orange.js` & `PyCBC-2.2.0/pycbc/results/static/js/fancybox/2.1.5/fancybox-orange.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.js` & `PyCBC-2.2.0/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.pack.js` & `PyCBC-2.2.0/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.pack.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/js/jquery/1.10.2/jquery-1.10.2.min.js` & `PyCBC-2.2.0/pycbc/results/static/js/jquery/1.10.2/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/js/jquery/1.10.2/jquery.mousewheel-3.0.6.pack.js` & `PyCBC-2.2.0/pycbc/results/static/js/jquery/1.10.2/jquery.mousewheel-3.0.6.pack.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/static/js/jquery.min.js` & `PyCBC-2.2.0/pycbc/results/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/str_utils.py` & `PyCBC-2.2.0/pycbc/results/str_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/table_utils.py` & `PyCBC-2.2.0/pycbc/results/table_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/templates/files/file_default.html` & `PyCBC-2.2.0/pycbc/results/templates/files/file_default.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/templates/files/file_glitchgram.html` & `PyCBC-2.2.0/pycbc/results/templates/files/file_glitchgram.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/templates/files/file_pre.html` & `PyCBC-2.2.0/pycbc/results/templates/files/file_pre.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/templates/files/file_tmplt.html` & `PyCBC-2.2.0/pycbc/results/templates/files/file_tmplt.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/templates/orange.html` & `PyCBC-2.2.0/pycbc/results/templates/orange.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/templates/red.html` & `PyCBC-2.2.0/pycbc/results/templates/red.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/templates/wells/two_column.html` & `PyCBC-2.2.0/pycbc/results/templates/wells/two_column.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/results/versioning.py` & `PyCBC-2.2.0/pycbc/results/versioning.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/scheme.py` & `PyCBC-2.2.0/pycbc/scheme.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/sensitivity.py` & `PyCBC-2.2.0/pycbc/sensitivity.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/strain/__init__.py` & `PyCBC-2.2.0/pycbc/strain/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/strain/calibration.py` & `PyCBC-2.2.0/pycbc/strain/calibration.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/strain/gate.py` & `PyCBC-2.2.0/pycbc/strain/gate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/strain/lines.py` & `PyCBC-2.2.0/pycbc/strain/lines.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/strain/recalibrate.py` & `PyCBC-2.2.0/pycbc/strain/recalibrate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/strain/strain.py` & `PyCBC-2.2.0/pycbc/strain/strain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1561,19 +1561,16 @@
                     and self.data_quality_flags[0] == 'veto_nonzero':
                 sb_kwargs['valid_on_zero'] = True
                 logging.info('DQ channel %s interpreted as zero = good',
                              data_quality_channel)
             else:
                 sb_kwargs['valid_mask'] = pycbc.frame.flag_names_to_bitmask(
                         self.data_quality_flags)
-                logging.info(
-                    'DQ channel %s interpreted as bitmask %s = good',
-                    data_quality_channel,
-                    bin(sb_kwargs['valid_mask'])
-                )
+                logging.info('DQ channel %s interpreted as bitmask %s = good',
+                             data_quality_channel, bin(valid_mask))
             self.dq = pycbc.frame.StatusBuffer(frame_src, data_quality_channel,
                                                start_time, **sb_kwargs)
 
         if idq_channel is not None:
             if idq_state_channel is None:
                 raise ValueError(
                     'Each detector with an iDQ channel requires an iDQ state channel as well')
```

### Comparing `PyCBC-2.1.2/pycbc/tmpltbank/bank_conversions.py` & `PyCBC-2.2.0/pycbc/tmpltbank/bank_conversions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/tmpltbank/bank_output_utils.py` & `PyCBC-2.2.0/pycbc/tmpltbank/bank_output_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/tmpltbank/brute_force_methods.py` & `PyCBC-2.2.0/pycbc/tmpltbank/brute_force_methods.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/tmpltbank/calc_moments.py` & `PyCBC-2.2.0/pycbc/tmpltbank/calc_moments.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/tmpltbank/coord_utils.py` & `PyCBC-2.2.0/pycbc/tmpltbank/coord_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/tmpltbank/lambda_mapping.py` & `PyCBC-2.2.0/pycbc/tmpltbank/lambda_mapping.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/tmpltbank/lattice_utils.py` & `PyCBC-2.2.0/pycbc/tmpltbank/lattice_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/tmpltbank/option_utils.py` & `PyCBC-2.2.0/pycbc/tmpltbank/option_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/tmpltbank/partitioned_bank.py` & `PyCBC-2.2.0/pycbc/tmpltbank/partitioned_bank.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/transforms.py` & `PyCBC-2.2.0/pycbc/transforms.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/types/aligned.py` & `PyCBC-2.2.0/pycbc/types/aligned.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/types/array.py` & `PyCBC-2.2.0/pycbc/types/array.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/types/array_cpu.pyx` & `PyCBC-2.2.0/pycbc/types/array_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/types/array_cuda.py` & `PyCBC-2.2.0/pycbc/types/array_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/types/config.py` & `PyCBC-2.2.0/pycbc/types/config.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/types/frequencyseries.py` & `PyCBC-2.2.0/pycbc/types/frequencyseries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/types/optparse.py` & `PyCBC-2.2.0/pycbc/types/optparse.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/types/timeseries.py` & `PyCBC-2.2.0/pycbc/types/timeseries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/vetoes/autochisq.py` & `PyCBC-2.2.0/pycbc/vetoes/autochisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/vetoes/bank_chisq.py` & `PyCBC-2.2.0/pycbc/vetoes/bank_chisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/vetoes/chisq.py` & `PyCBC-2.2.0/pycbc/vetoes/chisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/vetoes/chisq_cpu.pyx` & `PyCBC-2.2.0/pycbc/vetoes/chisq_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/vetoes/chisq_cuda.py` & `PyCBC-2.2.0/pycbc/vetoes/chisq_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/vetoes/sgchisq.py` & `PyCBC-2.2.0/pycbc/vetoes/sgchisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/SpinTaylorF2.py` & `PyCBC-2.2.0/pycbc/waveform/SpinTaylorF2.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/__init__.py` & `PyCBC-2.2.0/pycbc/waveform/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/bank.py` & `PyCBC-2.2.0/pycbc/waveform/bank.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/compress.py` & `PyCBC-2.2.0/pycbc/waveform/compress.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/decompress_cpu.py` & `PyCBC-2.2.0/pycbc/waveform/decompress_cpu.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/decompress_cpu_ccode.cpp` & `PyCBC-2.2.0/pycbc/waveform/decompress_cpu_ccode.cpp`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/decompress_cpu_cython.pyx` & `PyCBC-2.2.0/pycbc/waveform/decompress_cpu_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/decompress_cuda.py` & `PyCBC-2.2.0/pycbc/waveform/decompress_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/generator.py` & `PyCBC-2.2.0/pycbc/waveform/generator.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/multiband.py` & `PyCBC-2.2.0/pycbc/waveform/multiband.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/nltides.py` & `PyCBC-2.2.0/pycbc/waveform/nltides.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/parameters.py` & `PyCBC-2.2.0/pycbc/waveform/parameters.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/plugin.py` & `PyCBC-2.2.0/pycbc/waveform/plugin.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/premerger.py` & `PyCBC-2.2.0/pycbc/waveform/premerger.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/pycbc_phenomC_tmplt.py` & `PyCBC-2.2.0/pycbc/waveform/pycbc_phenomC_tmplt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/ringdown.py` & `PyCBC-2.2.0/pycbc/waveform/ringdown.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/sinegauss.py` & `PyCBC-2.2.0/pycbc/waveform/sinegauss.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/spa_tmplt.py` & `PyCBC-2.2.0/pycbc/waveform/spa_tmplt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/spa_tmplt_cpu.pyx` & `PyCBC-2.2.0/pycbc/waveform/spa_tmplt_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/spa_tmplt_cuda.py` & `PyCBC-2.2.0/pycbc/waveform/spa_tmplt_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/supernovae.py` & `PyCBC-2.2.0/pycbc/waveform/supernovae.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/utils.py` & `PyCBC-2.2.0/pycbc/waveform/utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/utils_cpu.pyx` & `PyCBC-2.2.0/pycbc/waveform/utils_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/utils_cuda.py` & `PyCBC-2.2.0/pycbc/waveform/utils_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/waveform.py` & `PyCBC-2.2.0/pycbc/waveform/waveform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/waveform/waveform_modes.py` & `PyCBC-2.2.0/pycbc/waveform/waveform_modes.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/__init__.py` & `PyCBC-2.2.0/pycbc/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/coincidence.py` & `PyCBC-2.2.0/pycbc/workflow/coincidence.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/configparser_test.py` & `PyCBC-2.2.0/pycbc/workflow/configparser_test.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/configuration.py` & `PyCBC-2.2.0/pycbc/workflow/configuration.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/core.py` & `PyCBC-2.2.0/pycbc/workflow/core.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/datafind.py` & `PyCBC-2.2.0/pycbc/workflow/datafind.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/dq.py` & `PyCBC-2.2.0/pycbc/workflow/dq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/grb_utils.py` & `PyCBC-2.2.0/pycbc/workflow/grb_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/inference_followups.py` & `PyCBC-2.2.0/pycbc/workflow/inference_followups.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/injection.py` & `PyCBC-2.2.0/pycbc/workflow/injection.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/jobsetup.py` & `PyCBC-2.2.0/pycbc/workflow/jobsetup.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/matched_filter.py` & `PyCBC-2.2.0/pycbc/workflow/matched_filter.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/minifollowups.py` & `PyCBC-2.2.0/pycbc/workflow/minifollowups.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/pegasus_files/pegasus-properties.conf` & `PyCBC-2.2.0/pycbc/workflow/pegasus_files/pegasus-properties.conf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/pegasus_sites.py` & `PyCBC-2.2.0/pycbc/workflow/pegasus_sites.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/pegasus_workflow.py` & `PyCBC-2.2.0/pycbc/workflow/pegasus_workflow.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/plotting.py` & `PyCBC-2.2.0/pycbc/workflow/plotting.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/psd.py` & `PyCBC-2.2.0/pycbc/workflow/psd.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/psdfiles.py` & `PyCBC-2.2.0/pycbc/workflow/psdfiles.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/segment.py` & `PyCBC-2.2.0/pycbc/workflow/segment.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/splittable.py` & `PyCBC-2.2.0/pycbc/workflow/splittable.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pycbc/workflow/tmpltbank.py` & `PyCBC-2.2.0/pycbc/workflow/tmpltbank.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/pyproject.toml` & `PyCBC-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/setup.py` & `PyCBC-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             return ''
 
     # If this is a pycbc git repo always populate version information using GIT
     try:
         vinfo = _version_helper.generate_git_version_info()
     except:
         vinfo = vdummy()
-        vinfo.version = '2.1.2'
+        vinfo.version = '2.2.0'
         vinfo.release = 'True'
 
     with open('pycbc/version.py', 'wb') as f:
         f.write("# coding: utf-8\n".encode('utf-8'))
         f.write(("# Generated by setup.py for PyCBC on %s.\n\n"
                 % vinfo.build_date).encode('utf-8'))
```

### Comparing `PyCBC-2.1.2/test/bankvetotest.py` & `PyCBC-2.2.0/test/bankvetotest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/fft_base.py` & `PyCBC-2.2.0/test/fft_base.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/lalsim.py` & `PyCBC-2.2.0/test/lalsim.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_array.py` & `PyCBC-2.2.0/test/test_array.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_array_lal.py` & `PyCBC-2.2.0/test/test_array_lal.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_autochisq.py` & `PyCBC-2.2.0/test/test_autochisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_calibration.py` & `PyCBC-2.2.0/test/test_calibration.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_chisq.py` & `PyCBC-2.2.0/test/test_chisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_coinc_stat.py` & `PyCBC-2.2.0/test/test_coinc_stat.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_conversions.py` & `PyCBC-2.2.0/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_correlate.py` & `PyCBC-2.2.0/test/test_correlate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_cuts.py` & `PyCBC-2.2.0/test/test_cuts.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_detector.py` & `PyCBC-2.2.0/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_distributions.py` & `PyCBC-2.2.0/test/test_distributions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_dq.py` & `PyCBC-2.2.0/test/test_dq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_fft_mkl_threaded.py` & `PyCBC-2.2.0/test/test_fft_mkl_threaded.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_fft_unthreaded.py` & `PyCBC-2.2.0/test/test_fft_unthreaded.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_fftw_openmp.py` & `PyCBC-2.2.0/test/test_fftw_openmp.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_fftw_pthreads.py` & `PyCBC-2.2.0/test/test_fftw_pthreads.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_frame.py` & `PyCBC-2.2.0/test/test_frame.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_frequencyseries.py` & `PyCBC-2.2.0/test/test_frequencyseries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_infmodel.py` & `PyCBC-2.2.0/test/test_infmodel.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_injection.py` & `PyCBC-2.2.0/test/test_injection.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_io_live.py` & `PyCBC-2.2.0/test/test_io_live.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_live_coinc_compare.py` & `PyCBC-2.2.0/test/test_live_coinc_compare.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_matchedfilter.py` & `PyCBC-2.2.0/test/test_matchedfilter.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_noise.py` & `PyCBC-2.2.0/test/test_noise.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_pnutils.py` & `PyCBC-2.2.0/test/test_pnutils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_psd.py` & `PyCBC-2.2.0/test/test_psd.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_resample.py` & `PyCBC-2.2.0/test/test_resample.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_schemes.py` & `PyCBC-2.2.0/test/test_schemes.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_significance_module.py` & `PyCBC-2.2.0/test/test_significance_module.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_skymax.py` & `PyCBC-2.2.0/test/test_skymax.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_spatmplt.py` & `PyCBC-2.2.0/test/test_spatmplt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_threshold.py` & `PyCBC-2.2.0/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_timeseries.py` & `PyCBC-2.2.0/test/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_tmpltbank.py` & `PyCBC-2.2.0/test/test_tmpltbank.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_transforms.py` & `PyCBC-2.2.0/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_waveform.py` & `PyCBC-2.2.0/test/test_waveform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/test_waveform_utils.py` & `PyCBC-2.2.0/test/test_waveform_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/test/utils.py` & `PyCBC-2.2.0/test/utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/benchmarking/absolute_times.py` & `PyCBC-2.2.0/tools/benchmarking/absolute_times.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/einsteinathome/check_GW150914_detection.py` & `PyCBC-2.2.0/tools/einsteinathome/check_GW150914_detection.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/static/hooks/hook-pycbc.py` & `PyCBC-2.2.0/tools/static/hooks/hook-pycbc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/static/runtime-scipy.py` & `PyCBC-2.2.0/tools/static/runtime-scipy.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/timing/arr_perf.py` & `PyCBC-2.2.0/tools/timing/arr_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/timing/banksim/banksim.py` & `PyCBC-2.2.0/tools/timing/banksim/banksim.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/timing/correlate_perf.py` & `PyCBC-2.2.0/tools/timing/correlate_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/timing/fft_perf.py` & `PyCBC-2.2.0/tools/timing/fft_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/timing/match_perf.py` & `PyCBC-2.2.0/tools/timing/match_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tools/timing/wav_perf.py` & `PyCBC-2.2.0/tools/timing/wav_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.1.2/tox.ini` & `PyCBC-2.2.0/tox.ini`

 * *Files identical despite different names*

