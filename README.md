# Social Capital and Disaster-Induced Eviction Filings – Code Repository

Codes to reproduce the results of the paper **“Social Capital and Disaster-Induced Eviction Filings.”**

## Overview

This repository contains the code used to run the synthetic control and regression analyses that evaluate the impact of disasters on eviction filing rates and how social capital mitigates this impact. All scripts are written in Python.

## Repository Structure

```
code/
 ├ 1_ATT_calculation.ipynb
 ├ 2_1_Fig1.ipynb
 ├ 2_2_Fig2.ipynb
 ├ 2_3_Fig3.ipynb
 ├ 2_4_Fig4.ipynb
 ├ 3_1_Robustness_check_placebo.ipynb
 ├ 3_2_Robustness_check_diff_control.ipynb
 └ 3_3_Robustness_check_LOO.ipynb

README.md
```

## Requirements

The codes were developed using Python 3.12. Main dependencies include:

* pandas
* numpy
* statsmodels
* cvxpy
* seaborn
* matplotlib

## Data

* Eviction data were obtained from the Eviction Lab website:
https://evictionlab.org/eviction-tracking/get-the-data/

* Disaster declaration data were retrieved from the Federal Emergency Management Agency (FEMA):
https://www.fema.gov/openfema-data-page/disaster-declarations-summaries-v2

* Because some datasets are reported at the ZIP code level while others are reported at the census tract level, a ZIP code–to–census tract crosswalk from the U.S. Department of Housing and Urban Development (HUD) was used:
https://www.huduser.gov/portal/datasets/usps_crosswalk.html

* FEMA disaster assistance data (used as a proxy for disaster damage) were obtained from:
https://www.fema.gov/openfema-data-page/housing-assistance-program-data-owners-v2

* Social capital data from Meta were obtained from the Social Capital Atlas:
https://data.humdata.org/dataset/social-capital-atlas
