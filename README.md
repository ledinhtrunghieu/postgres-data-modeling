# Project: Data Modeling with Postgres - Udacity Data Engineer Nanodegree

## 1. Introduction

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

They'd like a data engineer to create a Postgres database with tables designed to optimize queries on song play analysis. My role is to create a database schema and ETL pipeline which transfer the data from local files to the database for this analysis.

I wanted to do this locally but my Windows crashed when installing Docker so I have to do it in Udacity's Project workspace.

## 2. Project structure explanation

```
postgres-data-modeling
│   README.md               # Project description
│
└───data                    # The dataset
|   |               
│   └───log_data             
│   |   │  ...
|   └───song_data
│       │  ...
│   
└───notebooks               # Jupyter notebooks
|   |               
│   └───etl.ipynb           # ETL test notebook
│   |   │        
|   └───test.ipynb          # Test notebook
|  
└───python_scripts
│   │  create_tables.py     # Tables creation script
|   |  etl.py               # ETL script
|   |  sql_queries.py       # Definition of all sql queries
```

## 3. Run python scripts

```
cd python_scripts
python create_tables.py
python etl.py
```