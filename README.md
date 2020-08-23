# Data_Wrangling_and_Exploratory_Analysis_on_WHO_Child_Deaths_Data

My prime interest to work on this project is the Untidiness of the data. The challenge here is to create a more meaningful and easily understanding data from raw excel files.

Data source location:
Global Health Observatory data repository:
http://apps.who.int/gho/data/node.home >> By Category>> Child Health>> Child mortality and CAUSE OF DEATHS>> Cause of Child Death>> Number of Deaths by Cause>> Number of Deaths by Country>>Diseases
Upon clicking on each cause of death I was able to download dataset by clicking CSV table.
There are 13 CSV files one each for each cause of death.
Each csv file has 198 rows(each country) and 54 columns(columns separated with age-group(3) and year(2000-2017)) and average file size is 0.055MB.
Combined datasets have more than 10476 rows and 16 columns.

Context of Data:
This datasets are about number of deaths between 0-4 years age group from 2000-2017 in all countries around the world.

Modules:
Requests module to get data from the URL.
Melt function in pandas to reframe year wise columns to rows and creating death count column. Applying this on each of 13 csv files and creating a disease column for each csv.
Plotly module to plot the countries and continent wise deaths of childs to know which country is suffers most for each cause of death.
PyCountry converter, as we only have country coulmn this module helps to group all the countries in each continent and create a new continent column.

- It's  good finding that there is annual drop in deaths across the years.
- South America registers most number of deaths because of Respiratory infections in chils of 0-4 age group.
