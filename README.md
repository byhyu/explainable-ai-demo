Predictive Modeling with Demo of Explainable AI using Chicago Crime Dataset
==============================

## Overview

Here is my （ @byhyu） take on the Quantiply data science challenge problem: predictive modeling for Chicago crime dataset. The original problem statement from Quantiply is attached below:

Convervative industries may take different approaches for anomaly detection and predictions from research community.  They are used to the rule based systems (https://www.casewareanalytics.com/blog/rules-based-vs-advanced-analytics-%E2%80%93-do-you-have-choose), which is easy to understand even though these systems yield high false positive rates. In addition, the end users may not have enough machine learning/AI background to comprehend the explanations that are accessible to ML practitioners. One of the major differentiators  is our explainable AI (XAI). We developed an XAI framework to help explain the decision making process of complex models like neural networks.

On a daily basis, we tackle challenging problems, from building state-of-the-art unsupervised generative models, to explaining the how and the why of the decision-making process of the models.

## XAI Frameworks
 Here are some XAI frameworks:

 . https://arxiv.org/pdf/1602.04938v1.pdf
 . http://papers.nips.cc/paper/7062-a-unified-approach-to-interpreting-model-predictions.pdf
. https://homes.cs.washington.edu/~marcotcr/aaai18.pdf
 . https://github.com/datascienceinc/Skater

In this prject, I will demonstrate the fundamental ideas of these frameworks using the Chicago Crime dataset.

## Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- Documention using Sphinx
    │
    ├── exploration          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-hyu-eda`.
    │
    ├── references         <- Data dictionaries, manuals, papers, and all other explanatory materials.
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
    │   │   └── visualize.py
    ├── tests 				     <- test driven data analysis
    ├── test_environment.py <- check if environement is set up correctly


## Dataset

For this assignment, we have picked the *Chicago Crime Dataset*. You can download and learn more about the dataset at: 

[chicago crime dataset](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-present/ijzp-q8t2)

The size of the dataset is approx. 1.6 GB.

*The target variable is `Primary Type`. It is a multi-class classification problem.*

## How to Run

First, make sure that you have [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/install.html) installed and install the project.

```shell
mkvirtualenv chicagocrime-env
pip install -e .
```

## How to Contribute

First, make sure that you have [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/install.html) installed and install the project in development mode.

```shell
mkvirtualenv chicagocrime-env
git clone https://github.com/quantiply-labs/dslab-HongYu.git
cd dslab-HongYu
pip install -r requirements.txt
pip install -e .
pip freeze | grep -v chicagocrime > requirements.txt
```

Then, create or select a GitHub branch and have fun... 
