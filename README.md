# Appointment cancellation detector

This is a simple script that trains a `sklearn` algorithm to detect future cancellations of doctor's appointments. You can use this repo to do your exercise *Package your algorithm training* in [Jedha's fullstack program](https://app.jedha.co).

To use this repo, simply run:

`git clone https://github.com/JedhaBootcamp/appointment_cancellation_detector`

### Run script using Docker container

If you want to run `train.py` script at once, you can use `run.sh` file. Simply run:

`bash run.sh`

### Open a notebook 

If you prefer to open up a Jupyter notebook, you can use `openJupyter.sh` simply run:

`bash openJupyter.sh` 


## Troubleshooting 

👋 **Make sure that you exported your personal environment variables on your local terminal**. Especially, you need:

* `MLFLOW_EXPERIMENT_ID`
* `MLFLOW_TRACKING_URI`
* `AWS_ACCESS_KEY_ID`
* `AWS_SECRET_ACCESS_KEY`
* `BACKEND_STORE_URI`
* `ARTIFACT_ROOT`

Our advice is to create a `secrets.sh` file containing:

```bash
export MLFLOW_EXPERIMENT_ID="REPLACE_WITH_YOUR_MLFLOW_EXPERIMENT_ID"
export MLFLOW_TRACKING_URI="REPLACE_WITH_YOUR_MLFLOW_TRACKING_URI";
export AWS_ACCESS_KEY_ID="REPLACE_WITH_YOUR_AWS_ACCESS_KEY_ID";
export AWS_SECRET_ACCESS_KEY="REPLACE_WITH_YOUR_AWS_SECRET_ACCESS_KEY";
export BACKEND_STORE_URI="REPLACE_WITH_YOUR_BACKEND_STORE_URI";
export ARTIFACT_ROOT="REPLACE_WITH_YOUR_ARTIFACT_ROOT";
```

You can then simply run `source secrets.sh` to export all your environmnet variables at once. 

Happy coding! 👩‍💻



##
```
[ec2-user@ip-172-31-14-86 ~]$ mlflow run . --build-image --experiment-name mlflow-demo
2026/06/29 14:11:07 INFO mlflow.projects.docker: === Building docker image californian_housing_market:2b6c086 ===
2026/06/29 14:12:52 INFO mlflow.projects.utils: === Created directory /tmp/tmpyqk2uxez for downloading remote URIs passed to arguments of type 'path' ===

bash: line 1: -e: command not found
"docker run" requires at least 1 argument.
See 'docker run --help'.

Usage:  docker run [OPTIONS] IMAGE [COMMAND] [ARG...]

Create and run a new container from an image
🏃 View run unleashed-mink-754 at: https://franckidda-my-mlflow-tracker.hf.space/#/experiments/3/runs/3582836ebea942aaadfd12453e3248c4
🧪 View experiment at: https://franckidda-my-mlflow-tracker.hf.space/#/experiments/3
2026/06/29 14:12:58 ERROR mlflow.cli: === Run (ID '3582836ebea942aaadfd12453e3248c4') failed ===
```