![Creative Commons License](https://i.creativecommons.org/l/by-sa/3.0/88x31.png)

This work is licensed under a [Creative Commons Attribution-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-sa/3.0/)

# Austrian Covid-19 Data

This is a collection of data on Austrian Covid-19 cases. The database contains the following information in the long format:

- Region (Always Austria)
- Date (Time and Data of Data point)
- Population in Austria as provided by Worldbank
- Type: Type of Variable
- Cases: Number of cases
- Cases_proportional: Number of cases proportional to population

The following type of variables are available:
- Dead: Cumulative number of people who died and were positively tested.          
- Infected: Cumulative number of people who were positively tested.
- Recovered: Cumulative number of people who were positively tested and have recovered.      
- In_Hospital: Current number of people in hospital with Covid-19.
- Intensive_Care: Current number of people in hospital in intensive care with Covid-19.
- Nmb_Tested: Cumulative number of tests.
- Currently_Ill: Infected - Recovered - Dead


The wide format is simply the same information (without Cases_proportional), but in a wide format.

# Data source

Data source is [wikipedia](https://de.wikipedia.org/wiki/COVID-19-Pandemie_in_%C3%96sterreich). There, the different number of data sources (Sozialministerium and Gesundheitsministerium) are merged. 
The data is scraped from wikipedia with the function scrape_wikipedia_at() in the R-package [Covid-Austria](https://github.com/joph/Covid19-Austria).
It is updated once a day at around 16:00.