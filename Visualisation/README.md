
## Analytics Project (using Power BI)

### I. Introduction

In recent years, most of the developed economies need economy-wide actions to facilitate decarbonization and sustainable development as the world recovers from the COVID-19 global pandemic. Developed countries have been forced to rethink their development pathways following the goals of the Paris Agreement on climate change through long-term strategies.

For sustainable growth, emissions must reduce as a country make economic growth. Such growth can be termed sustainable as it does not use fossil fuels for growth. To explore this further, I decided to focus on the Energy, Economy and Emissions parameters of Australia, one of the developed countries, and analyse its path towards sustainable development over the past decades. 

[![Visualisation](https://blueandgreentomorrow.com/wp-content/uploads/2018/10/eco-investing.jpg "Visualisation")](https://blueandgreentomorrow.com/wp-content/uploads/2018/10/eco-investing.jpg "Visualisation")


### II. Description of the Open Datasets

#### 1. Australian Energy Update 2020 - Table B 
- Tabular data (xls file, 225KB): 
- Australian population, GDP and energy consumption, by state and territory. 
- It has temporal attributes (both continuous and discrete) with duration ranging from financial year (FY) 1960-61 to FY 2018-19. This table has 9 worksheets with each having ~ 65 rows and 7 columns.	

Key attributes in the Table B dataset:
1.	Year
2.	Each worksheet for different states
3.	Population (Number)
4.	GDP / GSP (in $ million)
5.	Energy Consumption (PJ)
6.	Per capita Energy consumption (GJ/Person)
7.	Energy Intensity (GJ/$ million)
8.	Energy Productivity ($ million / PJ)

Link:https://www.energy.gov.au/publications/australian-energy-update-2020


#### 2. Australian Energy Update 2020 - Table F 
- Tabular data (xls file, 1.2MB):
- Australian energy consumption, by state and territory, by industry and fuel type, energy units. 
- It has temporal attributes (both continuous and discrete) with duration ranging from FY 1973-74 to FY 2018-19. This table has 10 worksheets with each having ~ 2,072 rows and 47 columns.

Key attributes in the Table F dataset:
1.	Year
2.	Each worksheet for different states
3.	Total Energy Consumption (PJ)
4.	Energy consumption by different industries

Link: https://www.energy.gov.au/publications/australian-energy-update-2020

	
#### 3. Australian Energy Update 2020 - Table O
- Tabular data (xls file, 126KB): 
- Australian electricity generation, by state and territory, by fuel type, physical units.
- It has temporal attributes (both continuous and discrete) with duration ranging from FY 2008-09 to FY 2018-19. This table has 14 worksheets with each having ~ 47 rows and 12 columns.

Key attributes in the Table O dataset:
1.	Year
2.	Each worksheet for different states
3.	Energy generation using non-renewable fuels
4.	Energy generation using renewable resources

Link: https://www.energy.gov.au/publications/australian-energy-update-2020


### III. Tools and Libraries Used for Analysis
1. 	R and Microsoft Excel - For Data Wrangling
2.	Power BI – For Data exploration using visualisation


### IV. DATA EXPLORATION

#### 1. Average Per Capita Economic Growth and Energy Consumption in each Australian State
<img width="614" alt="1" src="https://user-images.githubusercontent.com/64317646/133422713-804b86df-6157-459a-ae96-626666c1dfdd.png">











