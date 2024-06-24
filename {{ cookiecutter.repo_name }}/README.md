{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Project Organization
------------
    ├── LICENSE
    ├── README.md                 <- The top-level README for developers using this project.
    ├── TODO.md                   <- A helpful TODO list for project related tasks.
    ├── .env                      <- contains usernames/passwords to access database, etc (file is ignored with .gitignore)
    ├── .env_template             <- template to make your own .env file
    ├── certificates              <- eg. ssl certificate needed for sql access (contents ignored with .gitignore)
    ├── data
    │   ├── external              <- Data from third party sources.
    │   ├── interim               <- Intermediate data that has been transformed.
    │   ├── processed             <- The final, canonical data sets for modeling.
    │   └── raw                   <- The original, immutable data dump.
    │
    ├── notebooks                 <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                                and a short `_` delimited description, e.g.
    │                                `01_initial_data_exploration`.
    │
    ├── reports                   <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures               <- Generated graphics and figures to be used in reporting
    │
    ├── environment.yml           <- The requirements file for reproducing the analysis environment, e.g.
    │                                generated with `conda env export --no-builds -n {{cookiecutter.project_name}} > environment.yml`.
    ├── environment_simple.yml    <- A simpler version of the environment with only the packages directly 
    │                                installed. Ideally generated through `conda env export --from-history -f environment_simple.yml`.
    │
    ├── src                       <- Source code for use in this project.
    │   ├── __init__.py           <- Makes src a Python module
    │   ├── data                  <- Scripts to download or generate data
    │   ├── utilities             <- Scripts or modules for miscellaneous functions
    │   └── visualization         <- Scripts to create exploratory and results oriented visualizations
    │
    └── Anything else?
--------

# Contributing

Some guidelines should be observed consistently across all that contribute to this project, so that this simplified version of a data science structure is still viable.

* Make sure your notebook works in the repository. 

    * If you refer to files in notebooks/scripts, they have to exist in the repository - and not just your own computer. Ideally use the dotenv path system to refer to files in the repository. 
    * Your scripts will need certain libraries to run. Make sure they are listed in the `environment_simple.yml` file. Some requirements are tricky to resolve due to version conflicts. A full environment export can be put on `environment.yml`. Make sure to built up on the previously established environment and/or test/update the rest of the notebooks/scripts accordingly.

* Keep the formatting standard.
    * Use the black formatter to format your code.

* Keep data in the structure presented.
    * Raw data should always be traceable to sources.
    * Interim data need not be well-tracked.  (#TODO: Consider adding it to gitignore?)
    * Processed data should be easily regeneratable from raw data through scripts or notebooks.

# Sources of external files:

Any data processed/generated outside this repository (and prone to change) should go under `data/external`. When new data file is added to external, the source should be catalogued here.


# Requirements:

`environment_simple.yml` file lists all packages used/needed in scripts and notebooks. This environment can be created by conda using: 

```
conda env create -f environment_simple.yml 
```


<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
