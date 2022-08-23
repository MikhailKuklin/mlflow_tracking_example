# WIP

## Step 1: create conda environment

conda create -n mlflow_tracking-env python=3.9

conda activate mlflow_tacking-env

## Step 2: install requirements

pip install -r requirements

## Step 3: launch MLFlow UI (in terminal)

mlflow ui --backend-store-uri sqlite:///mlflow.db

Go to http://127.0.0.1:5000 which will open UI for tracked experiments.





