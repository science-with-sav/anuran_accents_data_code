# anuran_accents
This github repository houses all relevant data and code to Anuran Accents, Weaver et al. 2020. <br />Citation:

## Folders
**Weaver_collected_call_data**: Selection data for each recording analyzed.<br />**range_maps**: Necessary data to create range shapefiles.<br />**data_for_analysis**: Files that are created using these scripts and saved for use in one or more later scripts.<br />**exported_figures** & **exported_tables**: Created using these scripts and exported for use in the manuscript.

## R code
**1_clean_summarize_data**: Checks that data was loaded in correctly. Exports date ranges of individuals/calls analyzed for Table 1. Calculates mean and standard deviations for each individual and species and exports for Table 1. Checks data distributions. Plots Figure 2 and range maps for Figure 1 and Supplementary Figure 1. Models call variables by temperature.<br />**2_resampling_function**: Creates and applies functions to test call variability as a function of the number of individuals sampled. <br />**3_resampling_analysis**: Transforms data and plots Figure 3. <br />**4_area_time_function**: Creates and applies functions to test call variability as a function of the geographic area covered by the individuals in a sample and the intra-annual time difference in days between the individuals in a sample. <br />**5_area_time_analysis**: Scales all data and checks distributions before and after scaling. Models call variability as a function of geographic area and intra-annual time across species and for each species individually. Plots Figures 4 and 5. Models ecological parameter estimates as a function of range size and as a function of species maximum SVL.

## Session Info
The scripts in this repository successfully run under the following session information in R:
R version 3.5.0 (2018-04-23)
Platform: x86_64-w64-mingw32/x64 (64-bit)
Running under: Windows >= 8 x64 (build 9200)

Matrix products: default

locale:
[1] LC_COLLATE=English_Australia.1252  LC_CTYPE=English_Australia.1252    LC_MONETARY=English_Australia.1252
[4] LC_NUMERIC=C                       LC_TIME=English_Australia.1252    

attached base packages:
[1] stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
 [1] rgeos_0.3-27            rnaturalearthdata_0.1.0 rnaturalearth_0.1.0     mgcv_1.8-28            
 [5] nlme_3.1-137            extrafont_0.17          patchwork_0.0.1         scales_1.0.0           
 [9] MASS_7.3-51.5           broom.mixed_0.2.6       broom_0.7.0             lmerTest_3.1-1         
[13] lme4_1.1-23             Matrix_1.2-14           forcats_0.3.0           purrr_0.3.2            
[17] tibble_3.0.0            tidyverse_1.2.1         stringr_1.4.0           lwgeom_0.1-6           
[21] lubridate_1.7.4         sf_0.9-2                ggplot2_3.3.0           tidyr_1.0.0            
[25] dplyr_0.8.3             readr_1.3.1            

loaded via a namespace (and not attached):
 [1] httr_1.4.1         numDeriv_2016.8-1  tools_3.5.0        TMB_1.7.18         backports_1.1.2    R6_2.2.2          
 [7] KernSmooth_2.23-15 DBI_1.0.0          colorspace_1.4-1   withr_2.1.2        sp_1.3-1           tidyselect_0.2.5  
[13] emmeans_1.4.5      compiler_3.5.0     extrafontdb_1.0    cli_1.0.1          rvest_0.3.2        xml2_1.2.2        
[19] sandwich_2.4-0     labeling_0.3       classInt_0.4-2     mvtnorm_1.0-7      digest_0.6.17      minqa_1.2.4       
[25] pkgconfig_2.0.2    rlang_0.4.5        readxl_1.3.1       rstudioapi_0.8     generics_0.0.2     zoo_1.8-6         
[31] jsonlite_1.6.1     magrittr_1.5       Rcpp_1.0.2         munsell_0.5.0      lifecycle_0.2.0    stringi_1.4.3     
[37] multcomp_1.4-8     yaml_2.2.1         plyr_1.8.4         grid_3.5.0         crayon_1.3.4       lattice_0.20-35   
[43] haven_2.1.0        splines_3.5.0      hms_0.4.2          knitr_1.28         pillar_1.4.3       boot_1.3-20       
[49] estimability_1.3   reshape2_1.4.3     codetools_0.2-15   glue_1.3.0         modelr_0.1.2       vctrs_0.2.4       
[55] nloptr_1.0.4       Rttf2pt1_1.3.7     cellranger_1.1.0   gtable_0.2.0       assertthat_0.2.0   xfun_0.10         
[61] xtable_1.8-2       e1071_1.7-3        coda_0.19-2        class_7.3-14       survival_2.41-3    glmmTMB_1.0.1     
[67] units_0.6-2        statmod_1.4.30     TH.data_1.0-8      ellipsis_0.3.0
