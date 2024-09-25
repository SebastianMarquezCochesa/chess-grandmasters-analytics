# Project Template

This template provides a basic structure for data engineering or data science projects. It serves as a starting point to organize code, data, and models clearly and modularly.

## Directory Structure

```
├── LICENSE            <- Open-source license if one is chosen
├── README.md          <- The top-level README for developers using this project
│
├── data               <- Directory for all project data
│   ├── external       <- Data from third-party sources
│   ├── raw            <- Original, immutable data dump
│   ├── staging        <- Data staged for transformation (cleaning, deduplication, etc.)
│   └── processed      <- Final, processed data sets ready for consumption
│
├── notebooks          <- Jupyter notebooks for exploration, prototyping, or validation
│
├── reports            <- Generated analysis as HTML, PDF, etc.
│   └── figures        <- Generated graphics and figures for reporting
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials
│
├── src                <- Source code for this project
│   ├── __init__.py    <- Makes `src` a Python module
│   ├── utils.py       <- Helper functions for common tasks
│   └── config.py      <- Configuration settings loader
│
├── pipelines          <- Scripts for data pipelines (ingestion, transformation, loading)
│   ├── __init__.py    <- Makes `pipelines` a Python module
│   ├── extract.py     <- Script for extracting data from external sources
│   ├── transform.py   <- Script for cleaning and transforming data
│   └── load.py        <- Script for loading data into the target system
│
├── tests              <- Unit tests and integration tests
│   ├── __init__.py    <- Makes `tests` a Python module
│   ├── test_extract.py   <- Unit test for the data extraction process
│   ├── test_transform.py <- Unit test for the data transformation process
│   └── test_load.py      <- Unit test for the data loading process
│
├── requirements.txt   <- The requirements file for reproducing the environment
```
## Adjusting .gitignore

Ensure to adjust the `.gitignore` file according to your project needs. For example, since this is a template, the `/data/` folder is commented out and data will not be exlucded from source control:

```plaintext
# exclude data from source control by default
# /data/
```

Typically, its convenient to exclude this folder if it contains either sensitive data that shouldn't be added to version control or large files.