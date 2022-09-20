# Shiny Dashboard of linkage between Covid-19 and socioeconomic conditions
 
![GitHub top language](https://img.shields.io/github/languages/top/raulincadet/Covid-19?style=plastic)
![GitHub repo size](https://img.shields.io/github/repo-size/raulincadet/Covid-19?color=green)
![GitHub language count](https://img.shields.io/github/languages/count/raulincadet/Covid-19?style=flat-square)
![Lines of code](https://img.shields.io/tokei/lines/github/raulincadet/Covid-19?color=orange&style=plastic)

## Goals
This project intends to verify the linkage between the rate of COVID-19 cases with socioeconomic indicators. 

## Data sources and approach
To reach the goal of the project, data are collected from two sources : World Development Bank, using the World Development Indicators (WDI); Our World in Data. A total of five files (format CSV) are used from these sources, to implement the project. The files are related to: GDP per capita; population ; tourists arrivals ; country groups, respectively in terms of geographical region and income level; daily time series related COVID-19.

The first files are provided by the WDI, whereas the time series related to COVID-19 are provided by Our World in Data. The World Health Organization (WHO) provides data about COVID-19. However, to my knowledge, this organization do not provide time series data related to COVID-19. When we compare data provided by WHO with aggregation of time series data with those of Our World in Data, they are almost the same. The slight difference may be explain by the time data are reload online by these organizations.

Data from the five files used have been imported to R. The tibbles created have been clean, then combined. To visualize the linkage between COVID-19 and socioeconomic indicators, some graphs are realized, using the following packages: ggplot; plotly; dygraph, for time series; tmap, for thematic map.

## User interface
The users of the application are allowed to choose the indicators they want to analyze. In fact, they are allowed to modify several inputs for a same graphics, to visualize the information extracted from data. They can select a country to observe the trend of a COVID-19 indicator they select.


The graphics show that richer countries tend to have higher cases rate of COVID-19. Results show also that richer countries tend to have higher cases rate of COVID-19 because their rate of people older than 65 and 70 years old tend to be higher than it is the case in low-income level countries.
