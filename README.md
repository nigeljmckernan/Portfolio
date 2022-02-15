# Introduction

Hi there!

My name is Nigel McKernan and I am an aspiring Data Scientist from Winnipeg, Manitoba.

Here you can find my portfolio of projects that I've undertaken on my personal time.

If you would like to see my personal website which includes my CV and Master's Thesis and its corresponding code, please go [here](https://nigelmckernan.ca).

I prefer to work in R, though I am learning Python from  a data science perspective.

Here are my current projects with links to their respective code and documentation in this repository.

# R

## Master's Thesis

My Master's Thesis examined the **endogenous** link between house prices and air pollution in the Canadian real estate market, and to resolve said endogeneity via meteorological data via a 2SLS Panel-Data regression model and temporal disaggregation of certain data.

You can find an HTML-rendered RMarkdown document [here](https://nigelmckernan.ca/media/ma_paper). I will be uploading the R code to this repository at a later date.

## [TransLoc API Dashboard](https://github.com/nigeljmckernan/TransLocShinyDashboard)

A simple [Shiny](https://shiny.rstudio.com) dashboard that pulls data from TransLoc's OpenAPI endpoints via the `httr` package. 

My intentions behind this projecy were to gain experience in the world of `HTTP` requests, specifically using the `httr` package to facilitate the ease of `GET` requests to pull data from API's, and perform further unnesting of the underlying JSON data with the `jsonlite` package.

The API contains real-time data about public transportation vehicles and their routes throughout various jurisdictions and municipalities across the United States.

My initial intention with this dashboard was to fit various machine learning models (via the `tidymodels` and `modeltime` ecosystems) for forecasting arrival delays of vehicles. Also to perform K-means clustering on the vehicles for identifying abstract groups of vehicles per their features.

Via an initial EDA, the data completeness of many columns across the different tables/endpoints tends to be very low, with little information to help impute missing observations.

As such, I've left it as a simple dashboard to pull data on specific transportation agenices, and to plot these agency locations, their jurisdiction bounds, as well as the current locations of their vehicles on [Leaflet](https://rstudio.github.io/leaflet/) maps.

You can find the app [here](https://nigeljmckernan.shinyapps.io/TransportationDashboard/).

## [Water Point Data Exchange Project](https://github.com/nigeljmckernan/WPDXMLStack)

A project utilizing the Water Point Data Exchange TidyTuesday dataset to fit various machine learning mdoels via the `tidymodels` ecosystem, and also performing ensemble model stacking with the `stacks` package.

This dataset contains data over many years of various water pumps in various countries.

The dataset's completenesss rate of most of the fields are satisfactory, with opportunity to extract many features for fitting ML models.
