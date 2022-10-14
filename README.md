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


#### What (potential) sources of bias did you discover in the course of your data processing and analysis?

After making a list of countries (wp_countries-no_match.txt), which did not return any Revision ID or ORES Result after passing through the API Call functions, we observe that the following countries feature in this list:
* United States
* Canada
* United Kingdom
* Australia

These are some of the largest English-langauge speaking countries in the world, and thus not including them in the list of Wikipedia English articles is a potential source of bias. If they were included, the analysis results would look very different.

#### What biases did you expect to find in the data (before you started working with it), and why?

Considering the wide range of countries being represented, there is a high chance of disproportionate number of articles per country. Every country has its uniqueness including the main language. Considering that for many countries, English is not the main language, those countries would not have many articles displayed. 

#### How might a researcher supplement or transform this dataset to potentially correct for the limitations/biases you observed?

In order to address the concerns mentioned above, I would only include English language countries to have a fair comparison between the number of articles being published per country. Also, with certain countries have a large population, the number of educated people isn't always high. I would account for that to compare the research output.


