# Introduction

Hi there!

My name is Nigel McKernan and I am an aspiring Data Scientist from Winnipeg, Manitoba, currently based in Vancouver, British Columbia.

Here you can find my portfolio of projects that I've undertaken on my personal time.

# Projects

## Master's Thesis

My Master's Thesis examined the **endogenous** link between house prices and air pollution in the Canadian real estate market, and to resolve said endogeneity via meteorological data via a 2SLS Panel-Data regression model and temporal disaggregation of certain data.

You can find an HTML-rendered RMarkdown document [here](https://nigelmckernan.ca/media/ma_paper). I will be uploading the R code to this repository at a later date.


## [Vancouver 311 Requests Data Engineering Project](https://github.com/nigeljmckernan/van_311_requests_de)


A project showcasing my Data Engineering skillset leveraging various technologies.

The overall goal was to ingest structured data from the City of Vancouver's 311 Requests data from its Open Data portal into a data lake on AWS S3, and from there deploy transformations of that source data across Bronze, Silver, and Gold medallion layers onto Snowflake.

Ingestion of the source data was mainly handled via modular Python scripts mainly leveraging `requests` and `pandas`.

`dbt` handled all of the transformation logic across both `dev` and `prd` schemas onto Snowflake.

Apache Airflow handled all orchestration of ingest from the API to S3, and subsequently the transformations on Snowflake.

## [Faker Electronics Retailer Data Engineering Project](https://github.com/nigeljmckernan/faker-electronics-retailer-de)

This project was to also showcase my Data Enginering skillset, this time however, using synthetic data generated from a combination of the `faker` and `random` libraries in Python.

I wanted to generate synthetic data of a fictitious electronics retailer to use data from a domain I had 7+ years of experience with: retail & CPG.

Similar set of technologies used compared to [this project](#vancouver-311-requests-data-engineering-project), however this time I swapped standard Airflow for Astronomer Cosmos, due to its native integration of `dbt` DAG's and other conveniences.

I likely wouldn't return to a portfolio project where I needed to generate synthetic data with a certain degree of realism needing to be achieved, as this took quite a significant amount of time (even using AI to assist me with the data generation UDF's) for a part of the project where this was _not_ the main focus or goal.


## [Water Point Data Exchange Project](https://github.com/nigeljmckernan/WPDXMLStack)

**NOTE**: This is somewhat of an older project that I undertook a few years ago, and is _not_ representative of my data science and machine learning skills at present. I have included it for posterity 

A project utilizing the Water Point Data Exchange TidyTuesday dataset to fit various machine learning mdoels via the `tidymodels` ecosystem, and also performing ensemble model stacking with the `stacks` package.

This dataset contains data over many years of various water pumps in various countries.

The dataset's completenesss rate of most of the fields are satisfactory, with opportunity to extract many features for fitting ML models.
