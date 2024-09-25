# Project Template

This template provides a basic structure for data engineering or data science projects. It serves as a starting point to organize code, data, and models clearly and modularly.

## Directory Structure

```
├── LICENSE                    <- Open-source license if applicable
├── README.md                  <- The top-level README for developers using this project
├── data
│   ├── external               <- Data from third-party sources
│   ├── raw                    <- Original, immutable data dump
│   ├── staging                <- Data staged for transformation (cleaning, deduplication, etc.)
│   └── processed              <- The final, processed data sets ready for consumption
│
├── notebooks                  <- Jupyter notebooks for exploration, prototyping, or validation
│
├── reports                    <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures                <- Generated graphics and figures for reporting
│
├── references                 <- Data dictionaries, manuals, and all other explanatory materials
│
├── src                        <- Source code for this project
│   ├── __init__.py            <- Makes `src` a Python module
│   ├── utils.py               <- Helper functions for common tasks (logging, retry logic, etc.)
│   ├── config.py              <- Load and parse configuration settings
│
├── pipelines                  <- Scripts for data pipelines (ingestion, transformation, loading)
│   ├── __init__.py            <- Makes `pipelines` a Python module
│   ├── extract.py             <- Script for ingesting data
│   ├── transform.py           <- Script for transforming and cleaning data
│   └── load.py                <- Script for loading data into a target system
│
├── tests                      <- Unit tests and integration tests
│   ├── __init__.py            <- Makes `tests` a Python module
│   ├── test_ingest.py         <- Unit test for ingestion process
│   ├── test_transform.py      <- Unit test for transformation scripts
│   └── test_load.py           <- Unit test for loading data
│
├── requirements.txt           <- The requirements file for reproducing the environment
```
## Adjusting .gitignore

Ensure to adjust the `.gitignore` file according to your project needs. For example, since this is a template, the `/data/` folder is commented out and data will not be exlucded from source control:

```plaintext
# exclude data from source control by default
# /data/
```

Typically, its convenient to exclude this folder if it contains either sensitive data that shouldn't be added to version control or large files.
