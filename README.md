<!-- # ds-modeling-pipeline
Skeleton project for building a simple model in python script
This is the simplest way to do it. We train a simple model in the jupyter notebook, where we select only some features and do minimal cleaning. The output is then stored in simple python scripts. -->

# Psychology vs. Drug Use Machine Learning Project
Data used is the  [Psychology vs Drug Use Data Set](https://archive.ics.uci.edu/ml/datasets/Drug+consumption+%28quantified%29).

##
Requirements:
- pyenv with Python: 3.9.4

### Environment

Same procedure as last time...

Use the requirements file in this repo to create a new environment.

```BASH
make setup 

#or 

pyenv local 3.9.4
python -m venv .venv
pip install --upgrade pip
pip install -r requirements.txt
```

If You encounter errors related to statsmodels, try:

```BASH
OPENBLAS="$(brew --prefix openblas)" pip install numpy statsmodels
```

<!-- ## Usage

In order to train the model and store test data in the data folder and the model in models run:

```bash
#activate env
source .venv/bin/activate

python train.py  
```

In order to test that predict works on a test set you created run:

```bash
python predict.py models/linear_regression_model.sav data/X_test.csv data/y_test.csv
``` -->

## Limitations

development libraries are part of the production environment, normally these would be separate as the production code should be as slim as possible

## Contents

1. The [Clean Data](clean_data.ipynb) notebook imports the original data and exports a clean version of it 
2. The [Modeling](modeling.ipynb) notebook contains the code for evaluation different models and tuning the best performing one
