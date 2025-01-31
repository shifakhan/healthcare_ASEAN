healthcare_ASEAN
==============================

Open data project on exploration of healthcare data for the ASEAN region, currently focusing on Malaria and Dengue. 

For more information on the project's background, impact and how to set up the project please go through [docs](https://github.com/shifakhan/healthcare_ASEAN/tree/master/docs/README).

Trello board: https://trello.com/b/NtM7qDC5/project-healthcare-asean  
Slack Channel on DataKindSG team: #healthcare_asean  

The data folder is currently not uploaded to the github repo (see .gitignore)  
For new repositories, run: `python download.py` from `.\src\data\`  
To get latest data, run: `python .\src\data\download_lastmonth_data.py`  

Previously collected data is available in the Project Google drive folder.  

Granularity
------------
 * weekly data
 * location: state/province level 

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data
    │   │   ├── download   <- Scripts for downloading from each raw data source
    │   │   │   └── logconf.ini <- setup for logging configuration for scripts in download/
    │   │   ├── download.py <- Script to download raw data using modules in `download/`
    │   │   │
    │   │   ├── clean      <- Scripts to clean raw data
    │   │   ├── clean.py   <- Script to clean raw data using modules in 'clean/'
    │   │   │
    │   │   └── logconf.ini <- setup for logging configuration for scripts in data/
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    ├── test               <- Directory for souce codes testing
    │   ├── func           <- Directory for souce codes functional testing
    │   │   ├── data
    │   │   ├── features
    │   │   └── models
    │   ├── unit           <- Directory for souce codes unit testing
    │   │   ├── data
    │   │   ├── features
    │   │   └── models
    └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org
