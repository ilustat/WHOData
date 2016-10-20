# WHOData
## World Health Origanisation's (WHO) Mortality Data

The **WHOData** project aims to **tidy** the [World Health Organisation's (WHO)](www.who.int) mortality data using R. This is a *group* exercise to help some newcomers learn about cleaning and manipulating data using the R **tidyverse** (<https://github.com/tidyverse/tidyverse>). Please install the *tidyverse* before you start.

The following steps can be used as guide to work your way through this challenge. Please use the `WHOMortalityData.Rmd` file to get started as it outlines some of the key steps.

* Data source: <http://www.who.int/healthinfo/mortality_data/en/>
  + It is assumed that data has been downloaded
* Install the **tidyverse** packages using `install.packages("tidyverse")`
* Reading in the WHO mortality data
* Reading the International Classificaion of Diseases data
* Keep the **neoplasm**, **melanoma**, **lymphoma** and **leukaemia** data for ICD10 part 1
  + Tranform the data into long format for the number of deaths
* Transform the population data in long format
* Merge the long population data to the long neoplasm data
  + Care has to be taken with respect to the format of the age groups. 
  + Combine the youngest age groups into a new 0-4 years. 
* Calculate the mortality rate per 100,000 population in a new variable
  + rate = (100000*deaths)/pop
* Write a function that will extract data based on country, cause of death, year and sex
  + If any of these are left blank then all the data is extracted
  + A data frame containing the requested data should be returned.
* Next steps will defined later
  * Sumamry graphs
  * Summary tables
 
