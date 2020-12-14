# country_data.csv
Outline of SARS-CoV-2 statistics (i.e. percent positivity, sequencing rate, seroprevalence) obtained in each country around the world. The data is grouped by month for each country. 

# Motivation
With disproportion sequencing rates around different countries in the world, it is increasingly important to minimize unrepresentative sampling during phylogenetic analyses. This data is intended to help researchers conduct SARS-CoV-2 sequence sampling with as little sampling bias as possible. 

# Columns
The representation of the columns are as follows:

## date
The date (year-month) to which the data pertains to.

## location
The location (country) to which the data pertains to.

## cases
The number of confirmed cases in each country in the corresponding month. The data was obtained from https://worldometer.info/coronavirus/

## deaths
The number of confirmed deaths in each country in the corresponding month. The data was obtained from https://worldometer.info/coronavirus/

## tests
The number of confirmed tests performed in each country in the corresponding month. The data was obtained from https://worldometer.info/coronavirus/

## percent_positivity
The percent positivity was defined as the number of cases divided by the number of tests for each country in each month.

## CFR
The case fatality rate (CFR) was defined as the number of deaths divided by the number of cases for each country in each month.

## sequences
The number of SARS-CoV-2 genome sequences obtained for each country in each month. All sequences were collected from GISAID, and redundant sequences were removed with Nybbler.  

## sequencing_rate
The sequencing rate was defined as the number of genome sequences divided by the number of cases for each country in each month.

## sero_study_participants
The sero_study_participants was defined as the sum of participants in all seroprevalence studies for each country in each month. The number of seroprevalence participants were obtained from https://serotracker.com/ and the date of the seroprevalence studies were defined as the midpoint between the study start and end date. If either the start or end date was missing, the date that was available was used as the study date. 

## avg_seroprevalence
The weighted seroprevalence average from all seroprevalence studies for each country in each month. Seroprevalence estimates were weighted by the number of participants involved in each study. Seroprevalence estimates were obtained from https://serotracker.com/   

## ICL_estimate_mean
The estimated number of new cases for each country in each month according to the Imperial College London's (ICL) model. The number of cases was calculated by summing the number of estimated new cases (mean) in each day for every month. The ICL model was obtained from https://github.com/mrc-ide/global-lmic-reports/tree/master/data

## IHME_estimate_mean
The estimated number of new cases for each country in each month according to the Institute for Health Metrics and Evaluation's (IHME) model. The number of cases was calculated by summing the number of estimated new cases (mean) in each day for every month. The IHME model was obtained from http://www.healthdata.org/covid/data-downloads

## LSHTM_estimate_median
The estimated number of new cases for each country in each month according to the London School of Hygiene and Tropical Medicine's (LSHTM) model. The number of cases was calculated by summing the number of estimated new cases (median) in each day for every month. The LSHTM model was obtained from https://cmmid.github.io/topics/covid19/global_cfr_estimates.html

## YYG_estimate_mean
The estimated number of new cases for each country in each month according to Youyang Gu's (YYG) model. The number of cases was calculated by summing the number of estimated new cases (mean) in each day for every month. The YYG model was obtained from https://github.com/youyanggu/covid19_projections/tree/master/projections