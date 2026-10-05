# Weather comparison between Seattle and Burlington

> We will use the data science methodology to investigate whether it rains more in Seattle, WA or Burlington, VT

---

## Project Overview

- **Objective:** Learn if it rains more in Seattle, WA or Burlington, VT
- **Domain:** Weather
- **Key Techniques:** Data cleaning, Exploratory data analysis, T tests and Z tests

---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

- **Source:** National Oceanic and Atmospheric Administration https://www.ncei.noaa.gov/cdo-web/search?datasetid=GHCND
- **Description:** Data from 01-01-2018 to 12-31-2022. Data from Seattle, WA contains 1658 rows and 10 columns including STATION, NAME, DATE, DAPR, MDPR, PRCP, SNOW, SNWD, WESD, and WESF. Data from Burlington, VT contains 1826 rows and 6 columns including STATION, NAME, DATE, PRCP, SNOW, and SNWD. We are interested in the columns DATE and PRCP.   

---

## Analysis

JupyterLab was used to preform the analysis. The file is called Weather_Data.ipynb and the code should be run in the order it appears. The file explores and cleans the data into the file clean_seattle_burlington_weather.csv, preforms exploratory data analysis, then preforms T and Z tests to compare the mean precipitation and the proportion of days with precipitation.

---

## Results

T tests for difference in mean precipitation:
- No significant difference was found in the mean precipitation in the two cities. 
- A significant difference in mean precipitation by month was found in Jan, Feb, Jun, Jul, Aug, Sep, Nov, and Dec. Mean precipitation is greater in Seattle in Jan, Feb, Nov, and Dec. It is greater in Burlington in Jun, Jul, Aug, and Sep.
- A significant difference in mean precipitation by season was found in Winter and Summer. Mean precipitation is greater in Seattle in Winter and in Burlington in Summer.

Z tests for difference in the proportion of days with precipitation
- A significant difference was found in the proportion of days with precipitation. Seattle has a greater proportion of days with precipitation.
- A significant difference in the proportion of days with precipitation by month was found in Jan, Feb, Apr, Jul, Oct, Nov, and Dec. The proportion of days with precipitation is greater in Seattle in Jan, Feb, Apr, Oct, Nov, and Dec. Burlington has no months with a greater proportion of days with precipitation.
- A significant difference in the proportion of days with precipitation by season was found in all seasons. The proportion of days with precipitation is greater in Seattle in Winter, Spring, and Fall. It is greater in Burlington in Summer.

Full results can be found in results.pdf in the reports folder.
---

## Authors

- Joey Matte - [@mattejoey](https://github.com/mattejoey)

---

## License

This project is licensed under the MIT License.

---

## Acknowledgements

- Tools/libraries used: numpy, pandas, matplotlib, seaborn, scipy, statsmodels, calendar, jupyter, notebook, ipython
- Courses referenced: Seattle University MSDS DATA 5100 Foundations of Data Science
- Inspiration: Dr. Xiaoxi Zhang
