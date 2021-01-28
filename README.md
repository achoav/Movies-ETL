# Movies-ETL
This week's modules went through the ETL process to prepare for a hackathon for a fictitious streaming service. Data was provided in the form of 2 .csv files (source: Kaggle, and files were named 'movies_metadata' & 'ratings'), due to the size the CSV files were not uploaded to Github.  Data was provided also on a .json file (source: Wiki data, and file wikipedia-movies.json). Data is gathered from both Wikipedia and Kaggle, combined, and saved into a SQL database so that the hackathon participants have a nice, clean dataset to use.

In this challenge, a Python script was written that performs all three ETL steps on the Wikipedia and Kaggle data.
Utilizing python and SQL to build-out ETL pipelines that clean, transform, and load datasets into a database. 

##  Resources 
- Python 3.7.6, JupyterLab 2.26, Jupyter Core 4.6.3
- [PostgreSQL 11.10](https://www.postgresql.org/), [Pgadmin 4.20](https://www.pgadmin.org/) 
- Movie Data sourced from [IMDB](https://developer.imdb.com/?ref=ft_ds), [Kaggle](https://www.kaggle.com/) <small><i>(note: due to size of the raw data files, they are not included within this repo) </i></small>

## Overview 
The purpose of this project is to create a program that helps automate processing large sets of data. 

## Primary steps & stages of the pipeline 

- <b>Extract</b><br>
This stage involves the initial retrieval and reading of data in various formats (csv, json) by using a python environment that can interpret the data. 

- <b>Transform</b><br>
This stage involves several more granular step including but not limited to: 
  - Cleaning data: assessing missing values and any corrupt data, formating   
  - Transforming: filtering , formatting, classifying (data type is redefined/changed to better suit analysis interpretation), merging data
 
- <b>Load</b><br>
This stage involves connecting to a database/server from the python environment and loading the data into the appropriate tables/schemas.  Two tables were created , called movies and ratings. On the Resources tab, the user can see a movies_query.png and a ratings_query.png files generated from PgAdmin 2.


