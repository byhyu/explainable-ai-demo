Predictive Modeling for Chicago Crime Dataset (*Quantiply Data Science Challenge*)
==============================

## Overview

Here is my （Hong Yu @byhongyu） take on the Quantiply data science challenge problem: predictive modeling for Chicago crime dataset. The original problem statement from Quantiply is attached below:

> At Quantiply, we develop cutting edge models to solve complex problems. Our customers, financial institutions, are conservative. They are used to the rule based systems (https://www.casewareanalytics.com/blog/rules-based-vs-advanced-analytics-%E2%80%93-do-you-have-choose), which is easy to understand even though these systems yield high false positive rates. In addition, the end users may not have enough machine learning/AI background to comprehend the explanations that are accessible to ML practitioners. One of the major differentiators of Quantiply is our explainable AI (XAI) platform. We developed an XAI framework to help explain the decision making process of complex models like neural networks.
>
> We would like to introduce the challenge to you too. We want you to live the life of a Data Scientist at Quantiply. On a daily basis, we tackle challenging problems, from building state-of-the-art unsupervised generative models, to explaining the how and the why of the decision-making process of the models.
>
> Here are some XAI frameworks for your reference:
>
> . https://arxiv.org/pdf/1602.04938v1.pdf
> . http://papers.nips.cc/paper/7062-a-unified-approach-to-interpreting-model-predictions.pdf
> . https://homes.cs.washington.edu/~marcotcr/aaai18.pdf
> . https://github.com/datascienceinc/Skater
>
> NOTE: Note, we are not satisfied with any of the methods above. We of course do not expect you to develop a new method over such a short time.
>
> ### Our expectation

> This challenge is very open ended. What we would you like to demonstrate are the following:
>
> . Research what XAI is.
> . Show how you approach this problem, let us know your thoughts.
> . Build a classification model on the provided dataset.
> . Provide explanations to your predictions.
>
> ### Deliverables
>
> - Submit a document that elaborates your thoughts on these methods, such as the basic concepts, advantages, drawbacks, etc.
>
> - Use the classification model as an opportunity to demonstrate your data science skills.
>
> - *Also, please let us know what you would like to do if you were given more time.*
>
> - You can use any programming language of your choice.
>
> - You can present your findings in any format as you deem clear.
>
> - Instructions to run your scripts.
>
>   ### Github repo
>
>   https://github.com/quantiply-labs/dslab-HongYu

Project Organization
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