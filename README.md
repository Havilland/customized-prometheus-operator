# customized-prometheus-operator

## Usage

The template in this repo will deploy a customized prometheus operator. You can change the apiGroup of the operator to deploy it alongside the current cluster-monitoring-operator of openshift.

## Variables

API_GROUP 
OPERATOR_VERSION 
ROLE_NAME

You will have to change the namespace of the clusterrolebinding in the template. It is still hardcoded into the template as of now I haven't found a way to automate this.

    namespace: custom-prometheus-operator
