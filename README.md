[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Eenrics/Udacity-ML-app/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Eenrics/Udacity-ML-app/tree/main)

## Project Summary

This project is operationalized Machine Learning Microservice API. 

This app is pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project is to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

---

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m pip install --user virtualenv
# You should have Python 3.7 available in your host. 
# Check the Python path using `which python3`
# Use a command similar to this one:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
```
* Run `make install` to install the necessary dependencies
* Run `make lint` to lint the dockerfile and python code scripts

### How to run the python script and web app

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`
4. Run `make install` to install the necessary dependencies
5. Run `make lint` to lint the dockerfile and python code scripts

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl

### explanation of the files in the repository
* `app.py`, `model_data/`, `output_txt_files/` ---  These are the heart of the application
* `Dockerfile`, `Makefile`  ---   Makefile and Docker file of the project
* `README.md`  ---   Instruction of the application
* `docker_out.txt`, `kubernetes.out.txt`  ---   log output of the application
* `make_prediction.sh`  ---  simple test script that tests if the application works
* `run_docker.sh`, `run_kubernetes.sh`, `upload_docker.sh`  ---   Sets up the docker and kubernetes cluster
* `requirements.txt`  ---   Dependencies for the application to run

### DevOps Engineer
> Both GitHub accounts are mine.  `EbenGitHub`   &   `Eenrics`
>  Abenezer Eshetie  (ebenezeresh525@gmail.com)
