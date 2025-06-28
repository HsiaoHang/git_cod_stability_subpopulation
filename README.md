# git_cod_stability_subpopulation

This repository contains three folders: data, script, and output, to reproduce all the results of the paper 'Dynamical stability and drivers of Atlantic cod subpopulations in the North Sea and adjacent waters'. 

a. The data folder contains 

1. [subpopulation_data.xlsx] This is the abundance data by age and subpopulation.

2. [temp.ctd.csv] and [fishing_mortality_sub.xlsx] These are temperature and fishing mortality data.


b. The script folder contains five R scripts:

1. [Demo_MDR_function.R] 
This script is from Chang et al. 2021 https://onlinelibrary.wiley.com/doi/10.1111/ele.13897. It provides functions to run MDR-Smap.

2. [Demo_MDR_Smap_20210625.R] 
This script is from Chang et al. 2021 https://onlinelibrary.wiley.com/doi/10.1111/ele.13897. This script provides demonstration on running the functions in [Demo_MDR_function.R]. 
  
To reproduce the results of this paper, run the following three scripts subsequently: 


1. [smap_sub.Rmd] runs MDR S-map to obtain the jacobian matrices of age groups for each subpopulation.

2. [stability_sub.Rmd] derives population stability and sensitivity of age groups from the jacobian matrices.

3. [ccm.sub.Rmd] runs ccm to test causal links between abundance/dynamical stability and temperature/fishing mortality.


c. The output folder contains the outputs from each step of MDR S-map and ccm.


Note: use rEDM package version 1.2.3 for reproducibility; other versions may generate different results.


