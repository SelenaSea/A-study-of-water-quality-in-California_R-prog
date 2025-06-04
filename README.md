# A study of water quality in a particular Placer County, California.

I wanted to study how, based on chemical analyses of water, it is possible, for example, to identify areas of surface water pollution with precise geodata. In the future, based on the available data, it is possible to conduct a sanitary and environmental inspection of these areas.

This project is based on open sources https://data.cnra.ca.gov/dataset/water-quality-data

## Special thanks to the California Department of Water Resources
(https://data.cnra.ca.gov/organization/dwr/portal/home) for updating this database periodically.

Several stages of analysis were worked out using the R language:

Loading and cleaning data
Identifying outliers
Analysis of the distribution of different chemical elements in water
Visualization on the map
Comparison with standards
When cleaning and preparing data for analysis, several erroneous indicators in geographic coordinates were identified (there are some coordinates of water intake far beyond California, on the eastern side of the United States in the Atlantic Ocean :) )

Also, the recorded pH indicators of water were checked, which have too large deviations from the standard corridor of this indicator.

## The project consists of two parts. 

Part 1, I clean, prepare the database and form new tables for the upcoming analysis.

Part 2, is the analysis itself, where I identify certain trends in the behavior of the chemical composition of water over a certain period using pH as an example. 

Thus, for example, it is clear how the accuracy of measurements has increased over the years with the advent of more sensitive analysis tools. 

I compare the accuracy of measurements in the laboratory and in the field, which also revealed an interesting trend and confirmed my theory of the importance of correctly collecting water for analysis. 

Thus, when studying in the field, directly at the site of water sampling, the indicators, for example, pH are higher than when the water "reaches" the laboratory over some time.
