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
![Снимок экрана 2025-03-17 181747](https://github.com/user-attachments/assets/9447696d-9907-4824-8f3e-5f4fb301a6ba)


Also, the recorded pH indicators of water were checked, which have too large deviations from the standard corridor of this indicator.

## The project consists of two parts. 

Part 1, I clean, prepare the database and form new tables for the upcoming analysis.

Part 2, is the analysis itself, where I identify certain trends in the behavior of the chemical composition of water over a certain period using pH as an example. 

Thus, for example, it is clear how the accuracy of measurements has increased over the years with the advent of more sensitive analysis tools. 
![Снимок экрана 2025-06-04 112712](https://github.com/user-attachments/assets/07f51ece-24b5-4b51-94dd-22904fca020d)


By the end of the last century, after 1995, it is visible on the graph that surface water sources sharply reduced water research in laboratory conditions, and then in some years until 2005, 
it was almost zero, and water quality monitoring was only carried out in field conditions. 
From 2005 to 2015, there is a small stage of laboratory research, and then observations are almost absent again until 2021.


I compare the accuracy of measurements in the laboratory and in the field, which also revealed an interesting trend and confirmed my theory of the importance of correctly collecting water for analysis. 

Thus, when studying in the field, directly at the site of water sampling, the indicators, for example, pH are higher than when the water "reaches" the laboratory over some time.
![Снимок экрана 2025-06-04 112923](https://github.com/user-attachments/assets/5c76307f-8f26-4d43-a2dd-61947b9e41b0)

Here you can clearly see that field water samples show high pH levels, while such high levels are not found in lab samples. I assume this may be due to the time it takes to deliver water to the lab, changes in water composition due to air exposure in the container (non-compliance with water sampling protocols), prolonged storage of the water sample before reaching the lab, and other factors. This is a reason for an in-depth analysis of the delta between pH 10 and above between Field and Lab. Also, the presence of zero values only in field conditions. Visualization clearly shows the difference in how pH levels depend on the method of water analysis.
