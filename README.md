# EDA-using-Python

### Project Overview
This project involves analyzing and visualizing a dataset using Python. I used Jupyter Notebook to explore, clean, and draw insights from the data using pandas, numpy, and matplotlib. The goal was to practice real-world data analysis techniques and storytelling through visualizations.

### Tools and Libraries Used
- Python 3.12
- Jupyter Notebook
- pandas
- numpy
- matplotlib

### Dataset: EuCitiesTemperatures
This is a comprehensive European cities dataset containing 245 cities across 41 countries. The dataset combines geographical, political, demographic, and climatic information for cities throughout Europe and some neighboring regions.

Data Fields:
1. Geographic: City name, country, latitude/longitude coordinates, coastal status
2. Political: EU membership status
3. Demographic: Country population (in millions)
4. Climatic: Average temperature in Celsius

What the Data Represents:
This dataset represents a cross-sectional snapshot of European urban centers with their key characteristics. The temperature data appears to be annual averages, providing insight into the climatic conditions across different European regions.

Key Characteristics:
- Geographic Scope: From northern Scandinavia (Kiruna, Sweden at -2.2°C) to southern Mediterranean (various Spanish and Greek cities reaching 17-18°C)
- Political Diversity: Mix of EU members (about 70% of cities) and non-EU countries
- Urban Types: Includes major capitals, regional centers, and smaller cities
- Coastal Distribution: About 60% of cities have coastal access

### Preprocessing/Analysis
- Filled in the missing latitude and longitude values by calculating the average for that country.
- Found out the subset of cities that lie between latitudes 40 to 60 (both inclusive) and longitudes 15 to 30 (both inclusive). Also found out which countries have the maximum number of cities in this geographical band.
- Filled in the missing temperature values by the average temperature value of the similar region type. A region type would be a combinaton of whether it is in EU (yes/no) and whether it has a coastline (yes/no).

### Visualization
- Made a bar chart for the number of cities belonging to each of the regions described in Preprocessing/Analysis #3 above.
- Made a scatter plot of latitude (y-axis) v/s longitude (x-axis) values to get a map-like visual of the cities under consideration.
- The population column contains values unique to each country. So two cities of the same country will show the same population value. Made a histogram of the number of countries belonging to each population group: split the population values into 5 bins.
- Made subplots (2, 2), with proper titles, one each for the region types described in Preprocessing/Analysis #3 above.
