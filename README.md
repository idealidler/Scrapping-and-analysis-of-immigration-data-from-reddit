# Scrapping-and-analysis-of-immigration-data-from-reddit

This project is a Python-based solution to retrieve Reddit posts between two specified dates. The project uses the pushshift API to collect data in increments of 10 days, with a maximum of 250 posts in each iteration.

## Data Collection

The data is collected by making API requests to the pushshift API and retrieving Reddit posts based on the specified dates. The dates are defined as "posted after" and "posted before", and the API requests are made in increments of 10 days to ensure that the most recent 250 posts are collected in each iteration.

## Data Preprocessing

To avoid losing data, the time interval in the while loop has been reduced to 86400 (1 day), resulting in 250 posts collected every day. To avoid duplicates, the collected data is checked for duplicates and any duplicates are removed.

## Requirements

The project was developed using Python 3.8 and the following libraries:

1. Datetime
2. Requests
3. Json
4. Pandas
5. Numpy
6. Re

## How to Run

To run the code, make sure you have the required libraries installed and run the code in a Jupyter Notebook or a Python IDE. Start running the code from the first cell, and the program will retrieve Reddit posts between the specified dates.

## Note

Please note that the increased number of iterations may result in a large amount of data being collected and processed, so please ensure that your system has the necessary resources to handle this.
