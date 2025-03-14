
Module 11 Challenge

Module 11 Challenge

# Mars News and Weather Data Scrapping & Analysis

## Project Overview

This project involves web scraping and data analysis to extract and analyze Mars news articles znd Mars weather data. It leverages Splinter for automated browsing and BeautifulSoup got HTML psrsing. The extracted data is structured using Pandas and visualized using Matplotlib.

## Technologies Used

* Python
* Splinter (for automated browsing)
* Pandas
* Matplotlib (for data visulaiztion)
* Jupyter Notebook (for executing the project)

## Deliverables

### Scrape Titles and Preview Text from Mars News
* Automated the browsing of the [Mars News Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html)
* Identify and extract:
* Store extracted data in a Python dictionary format:
```
 {'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm",
'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
```
* Store multiple articles in a list and optionally export to JSON.

### Automated the browsing of the Mars temperature Data Site at [Mars Temperature Data](https://static.bc-edx.com/data/web/mars_facts/temperature.html)
* Scrape weather data using BeautifulSoup.
* Extract the following fields:
    * id: Transmission ID
    * terrestrial_data: Earth data
    * sol: Martian day count since Curiosity lasned
    * ls: Solar longitude
    * month: Martian month
    * min_temp: Minimum daily temperature (°C)
    * pressure: Atmosheric pressure (Pa)

### Datea Processing & Analysis
* Convert data types (datetime, int, float).
* Analyze Mars weather patterns:
    
    * Number of months on Mars
    * Numbr of Martian days in dataset
    * Coldest and warmest months

    ![Temperature Bar Chart](Images/Temperature_Bar_Chart.png)



* Month with lowest & highest atmospheric pressure

    ![Pressure Bar Chart](Images/Pressure_Bar_Chart.png)

* Estimating the length of a Martian year.
    * Plot minimum daily temperature to observe cyclic patterns.
    * Visually estimate how many Earth days equal one Martian year (~687 Earth days).
* Export the DataFrame to a CSV file for further analysis.

### Instructions

### Part 1: Scrape Mars News
1. Open part_1_mars_news.ipynb in Jupyter Nptebook.
2. Run the script to:
    * Visit the Mars news website.
    * Extract titles and preview text.
    * Store data in a list of dictionaries.
    * Save as a Json file.
    
### Part 2; Scrape and Analyze Mars Weather Data
1. Open part_2_mars_news.ipynb in Jupyter Notebook.
2. Run the script:
    * Scrape the Mars temperature table.
    * Convert the data into a Pandas DataFrame.
    * Analyze seasonal temperature and pressure trends.
    * Estimate the length of a Martian year by plotting temperature trends.
    * Save results to a CSV file.

### Results & Insights
* Mars has 12 months, eash experiencing different temperature and pressure variations.
* The coldest months and warmest months were identified using average minimum temperatures.
* Atmospheric pressure flucuates with the seasons, with lowest and highest pressure months visualzed.
* By analyzing minimum temperature cycles, we estimated a Martian year to be about 687 Earth days.

### Conclusion 

Tis project enhances web scraping, data structuring, and visualization skills while uncovering seasonal patterns on Mars. The insights gained help us understand Martian climate cycles, which is essential for future missions to the red Planet.




