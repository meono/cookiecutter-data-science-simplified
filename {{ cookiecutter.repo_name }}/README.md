{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Project Organization
------------
    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── TODO.md            <- A helpful TODO list for project related tasks.
    ├── .env               <- contains usernames/passwords to access database, etc (file is ignored with .gitignore)
    ├── .env_template      <- template to make your own .env file
    ├── certificates       <- eg. ssl certificate needed for sql access (contents ignored with .gitignore)
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         and a short `_` delimited description, e.g.
    │                         `01_initial_data_exploration`.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── environment.yml    <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `conda env export --no-builds -n {{cookiecutter.project_name}} > environment.yml`
    │
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   ├── data           <- Scripts to download or generate data
    │   ├── utilities      <- Scripts or modules for miscellaneous functions
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │
    └── Anything else?
--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
