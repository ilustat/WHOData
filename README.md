# WHOData
WHO Mortality Data

In this document, the steps to *tidy* the [World Health Organisation's (WHO)](www.who.int) mortality data for use in R are documented. The following steps are presented.

* Data source: <http://www.who.int/healthinfo/mortality_data/en/>
  + It is assumed that data has been downloaded
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
  
