Springboard DSC Mentor Example Repo
===================================

Intro
-----

This example repository is based on the
[cookiecutter](https://github.com/drivendata/cookiecutter-data-science)
design from the people at DrivenData.

To replicate this example, simply do the following at the command
prompt from within the directory where you want your project to
reside. In the example below, the user `your-username` is using macOS:

```bash
$ pip3 install cookiecutter
$ cd /Users/your-username/teaching
$ cookiecutter https://github.com/drivendata/cookiecutter-data-science

> project_name [project_name]: springboard-dsc-mentor-example
> repo_name [springboard-dsc-mentor-example]:
> author_name [Your name (or your organization/company/team)]: your-username
> description [A short description of the project.]: Example repo for mentoring in the Springboard DSC Track
> Select open_source_license:
>     1 - MIT
>     2 - BSD-3-Clause
>     3 - No license file
> Choose from 1, 2, 3 [1]: 1
> s3_bucket [[OPTIONAL] your-bucket-for-syncing-data (do not include 's3://')]:
> aws_profile [default]:
> Select python_interpreter:
>     1 - python3
>     2 - python
> Choose from 1, 2 [1]: 1

$ cd springboard-dsc-mentor-example
$ git init
$ git add .
$ git commit -m "first commit"
$ git remote add origin git@github.com:your-username/springboard-dsc-mentor-example.git
$ git push -u origin master
```

Project Organization
--------------------

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
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
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
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org

--------
