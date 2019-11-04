[![CircleCI](https://circleci.com/gh/sagar437/project-ml-microservice-kubernetes/tree/master.svg?style=svg)](https://circleci.com/gh/sagar437/project-ml-microservice-kubernetes/tree/master)


This project operationalizes a Python flask app—in a provided file, `app.py`that serves out predictions  about housing prices through API calls `sklearn` model that has been trained to predict housing prices in Boston. 

This project operationalizes the working, machine learning microservice using Kubernetes and Docker which is an open-source system for automating the management of containerized applications. The following things were done in this project.

1. Project code was tested using linting
2. Docker was used to containerize this application
3. Deployed the containerized application and made a prediction
4. Improved the log statements in the source code for this application
5. Configured Kubernetes and create a Kubernetes cluster using minikube
6. Deployed a container using Kubernetes and make a prediction
7. Upload a complete Github repo with CircleCI to indicate that your code has been tested

## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
