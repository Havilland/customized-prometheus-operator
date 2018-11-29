# customized-prometheus-operator

## DISCLAIMER

The changes this template makes to the operator haven't been tested thoroughly yet. 

Use this at your own risk. 

Further documentation will be added as soon as more testing has been done.

So far it works in the following setup:

### Working setup

CDK with version 3.11.43 deployed  
Kubernetes Master: v1.11.0+d4cacc0  
OpenShift Web Console: v3.11.43  
prometheus-operator v0.25.0 

## Usage

The template in this repo will deploy a customized prometheus operator. You can change the apiGroup of the operator to deploy it alongside the current cluster-monitoring-operator of openshift.

## Variables

* API_GROUP 
* OPERATOR_VERSION 
* ROLE_NAME

You will have to change the namespace of the clusterrolebinding in the template. It is still hardcoded into the template as of now I haven't found a way to automate this.

    namespace: custom-prometheus-operator
