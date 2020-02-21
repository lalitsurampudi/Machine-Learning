# Project: Data Modeling with Postgres

## Introduction
Introduction
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The data resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app. The task is to create a database schema and ETL pipeline for this analysis.

## Schema design

The data model follows star schema with dimension tables containing songs, users, artists and time data and fact table contains songplays data.

## Scripts

**sql_queries.py**
The script contains SQL queries to CREATE, INSERT and DROP tables in the Sparkify database.

**create_tables.py**
The script successfully connects to the Sparkify database, drops any tables if they exist, and creates the tables.

**etl.py:** 
The script connects to the Sparkify database, extracts and processes the `log_data` and `song_data`, and loads data into the five tables - `songs`, `users`, `artists`, `time` and `songplays`.

**etl.ipynb**
The Jupyter notebook contains step-by-step execution of the ETL process.

**test.ipynb**
The Jupyter notebook contains SQL commands to validate the connection to the `sparkifydb` database and query the data in the tables that were created and loaded using `create_tables.py` and `etl.py` scripts.

**run_scritps.ipynb**
The Jupyter notebook contains commands to execute `create_tables.py` and `etl.py` scripts in the terminal.