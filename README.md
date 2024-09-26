# Chess GrandMasters Analytics (In Progress...)

A project dedicated to analyzing chess grandmasters' games using data obtained from the [Chess.com API](https://www.chess.com/news/view/published-data-api). This project aims to explore various aspects of grandmaster's gameplay, including the most common openings, the number of moves per game, and overall game statistics. The goal is to provide insights and visualizations that can help chess enthusiasts and players understand the strategies employed by top players.

## Directory Structure

```
├── LICENSE                    
├── README.md                  
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

