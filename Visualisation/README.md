
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
1. 	R and Microsoft Excel - For Data Wrangling to generate clean final master dataset (uploaded on github separately)
2.	Power BI – For Data exploration using visualisation


### IV. DATA EXPLORATION

#### 1. Average Per Capita Economic Growth and Energy Consumption in each Australian State

<img width="614" alt="1" src="https://user-images.githubusercontent.com/64317646/133422713-804b86df-6157-459a-ae96-626666c1dfdd.png">

- we need to find whether different Australian states are contributing towards economic growth in each Australian state. 
- Map of Australia on LHS shows average GDP ($/person) whereas map on RHS shows per capita energy consumption in each state and territory in Australia. 
- Here, we have avoided using aggregate energy consumption figures as it may mislead the analysis by focusing of regions with higher population and hence relatively higher aggregate energy consumption. Per capita measures energy consumption on per individual basis hence removes the bias introduced due to population. 
- NSW has the lowest per capita energy consumption (206 GJ/person) but has relatively better per capita GDP (501,798 AUD MN) compared to other Australian states.

#### 2. Clean energy production initiatives over the past decade

<img width="564" alt="2" src="https://user-images.githubusercontent.com/64317646/133423291-7c82f69d-3589-4dfe-8452-79c136f88ffb.png">

- To analyse clean energy production initiatives undertaken by the Australian states, I plotted energy generation using renewable and non-renewable fuels for different states over the last decade. 
- For Tasmania (TAS), renewable energy generation is more than non-renewable energy generation with the biggest gap in renewable (12,995 GWh) and non-renewable (1,005 GWh) energy generation in 2014. 
- In all other states, non-renewable energy generation is higher than renewable energy generation. But it is worth noticing that gap between non-renewable energy generation and renewable energy generation is becoming narrower over the decade indicating sustainable growth with a focus on renewable energy generation.

#### 3. Australia's Preparadeness to fight climate change in terms of energy productivity

<img width="377" alt="3" src="https://user-images.githubusercontent.com/64317646/133424686-a6a809bf-97f7-4dda-b4b7-4af66e2b37af.png">

- Energy Productivity = GDP (AUD MN) / Energy Consumption (PJ)
- Since fossil fuels dominate Australia’s Energy Consumption, less Energy Consumption for the same GDP indicates better preparedness of the state to tackle climate change.
- Hence, we can inverse proportion between Energy Productivity and Energy Consumption in the above figure


### V. Final Dashboard

Final dashboard with all visualisations and key findings.

<img width="1171" alt="4" src="https://user-images.githubusercontent.com/64317646/133425493-f34799db-d88a-42a8-befd-f33106399bfa.png">


#### 1. Interactivity

I selected NSW region in one of the maps, automatically values in all visualisations changed to reflect only NSW region

<img width="1171" alt="5" src="https://user-images.githubusercontent.com/64317646/133425664-317abe5b-72c4-45c1-b7f3-cbd4de08b677.png">


#### 2. Dashboard Link

**[Power BI Dashboard Link](https://app.powerbi.com/groups/me/reports/dfbe221f-6433-481b-9fe8-3aa3931152ee?ctid=ef7a487a-77ca-410a-803d-e426b62a587f&pbi_source=linkShare "Power BI Dashboard Link")**

(p.s. Not sure whether link is accessible since I am using a free version of Power BI.)





