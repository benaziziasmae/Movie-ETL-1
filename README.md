# Movies-ETL

In this module, we learned how to use the Extract, Transform, Load (ETL) process to create data pipelines. A data pipeline moves data from a source to a destination, and the ETL process creates data pipelines that also transform the data along the way. Analysis is impossible without access to good data, so creating data pipelines is often the first step before any analysis can be performed. Therefore, understanding ETL is an essential skill for data analysis.

## Overview of the project 

The goal of this analysis is to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. By taking code that was previously created, we refractored the code to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.

## Resources

- Data: [wikipedia-movies](/wikipedia-movies.JSON)
- Software : PostgresSQL , Jupyter Notebook 

## Summary 

This analysis consists of four parts, where each step is building up from beginning of extracting data and function testing, through transformation and cleaning process to its final step connect and load to the database. The entire process of ETL can be executed with a single call of the function extract_transform_load in the final step ETL_create_database.ipynb. The ETL process is broken down into four jupyter notebook files:

**1- ETL_function_test.ipynb**

- Data is extracted from the website in JSON and CSV formats.
- Data is transformed into Pandas data frames.
- JSON file requires extra step – loading file first and then transforming into data frame.
