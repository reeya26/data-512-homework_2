#  Homework 2: Considering Bias in Data
The goal of this project is to explore the concept of bias in data using Wikipedia articles. We will consider articles on political figures from different countries.

This repository contains the data files, code and results of Homework 2, for the course Data 512: Human Centered Data Science.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/reeya26/data-512-homework_1/blob/main/LICENSE) ![Language](https://img.shields.io/badge/language-python-blue.svg)

## Resources Used
- Editor used: Jupyter Notebook
- Python version: 3.9.4
- Packages used: json, time, requests, urllib, pandas, numpy


## Data 

Source Files:

- [Politicians](https://github.com/reeya26/data-512-homework_2/blob/main/data/politicians_by_country_SEPT.2022.csv%20-%20politicians_international_SEPT.2022.csv)
This dataset contains the List of Politicians with Wikipedia articles along with website links
- [Population](https://github.com/reeya26/data-512-homework_2/blob/main/data/population_by_country_2022.csv%20-%20population_by_country_2022.csv) 
This dataset contains the list of all Countries in the world with their Population in millions.

Intermediary Files:

- [wp_countries-no_match.txt](https://github.com/reeya26/data-512-homework_2/blob/main/intermediary_files/wp_countries-no_match.txt)
List of countries which did not have any API return for a Revision ID
- [wp_politicians_by_country.csv](https://github.com/reeya26/data-512-homework_2/blob/main/intermediary_files/wp_politicians_by_country.csv)
List of all politicians whose Wikipedia article returned a Revision ID and ORES Result 

## Project Organization

This package has the following structure.

```
data-512-homework_2/
  |- license
  |- readme.md
  |- Considering Bias in Data.ipynb
  |- data/
    |- politicians
    |- population
  |- intermediary_files/
    |- wp_countries-no_match.txt
    |- wp_politicians_by_country.csv
    
```




## Research Implications

We obtain two results from this analysis.


#### 1. List of Dictionaries saved as Json files


- [Monthly desktop access](https://github.com/reeya26/data-512-homework_1/blob/main/json/dino_monthly_desktop_201501_202209.json) : Monthly desktop page traffic is based on one single request.
- [Monthly mobile access](https://github.com/reeya26/data-512-homework_1/blob/main/json/dino_monthly_mobile_201501_202209.json) : The API separates mobile access types into two separate requests, summing these to make one count for all mobile pageviews.
- [Monthly cumulative](https://github.com/reeya26/data-512-homework_1/blob/main/json/dino_monthly_cumulative_201501_202209.json) : Monthly cumulative data is the sum of all mobile, and all desktop traffic per article.

#### 2. Visualizations based on the analysis

 
 - Top 10 Peak Page Views Maximum Average and Minimum Average
 
![Result 1](https://github.com/reeya26/data-512-homework_1/blob/main/results/Q1-%20Maximum%20Average%20and%20Minimum%20Average.png "Result 1")



