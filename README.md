# WIP

## Step 1: create conda environment

conda create -n mlflow_tracking-env python=3.9

conda activate mlflow_tracking-env

## Step 2: install requirements

pip install -r requirements

## Step 3: launch MLFlow UI (in terminal)

*Option 1*: without using tracking server

```sh
cd /notebooks #mlflow should be always launched from the folder with notebooks/scripts
mlflow ui
```

Go to http://127.0.0.1:5000 which will open UI for tracked experiments.

*Option 2*: with local tracking server

```sh
cd /notebooks #mlflow should be always launched from the folder with notebooks/scripts
mlflow server --backend-store-uri sqlite:///backend.db --default-artifact-root ./artifacts_local
```

## Step 4: run notebook

## Sources for mlflow setups:

[MLOps Zoomcamp 2.2](https://youtu.be/cESCQE9J3ZE)
[MLOps Zoomcamp 2.6](https://youtu.be/1ykg4YmbFVA)





