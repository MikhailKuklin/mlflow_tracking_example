# Example of usage of MLFlow tracking
Repo contains two notebooks which demonstrate functionality of MLFlow tracking:

*/notebooks/exp_mlflow_local_autolog.ipynb*: basic use with [autlog()](https://www.mlflow.org/docs/latest/tracking.html#automatic-logging) from MLflow

*/notebooks/exp_mlflow_serve_custom.ipynb*: custom configuration of tracking parameters

More detailed information about model can be found in this [repo](https://github.com/MikhailKuklin/Logistic_regression_from_scratch) and [blog post](https://wordpress.com/view/mikhailkuklin.wordpress.com) 

## Step 1: create conda environment

```sh
conda create -n mlflow_tracking-env python=3.9

conda activate mlflow_tracking-env
```

## Step 2: install requirements

```sh
pip install -r requirements.txt
```

## Step 3: launch MLFlow UI

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

## Sources for MLflow setups:

[MLOps Zoomcamp 2.2](https://youtu.be/cESCQE9J3ZE)

[MLOps Zoomcamp 2.6](https://youtu.be/1ykg4YmbFVA)





