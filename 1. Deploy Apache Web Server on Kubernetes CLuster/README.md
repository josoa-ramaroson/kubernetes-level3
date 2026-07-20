Task description : 
```text
There is an application that needs to be deployed on Kubernetes cluster under Apache web server. The Nautilus application development team has asked the DevOps team to deploy it. We need to develop a template as per requirements mentioned below:

    1. Create a namespace named as httpd-namespace-xfusion.

    2. Create a deployment named as httpd-deployment-xfusion under newly created namespace. For the deployment use httpd image with latest tag only and remember to mention the tag i.e httpd:latest, and make sure replica counts are 2.

    3. Create a service named as httpd-service-xfusion under same namespace to expose the deployment, nodePort should be 30004.
```

To execute these tasks, I created three YAML files: namespace.yaml, deployment.yaml, and service.yaml. Then apply them consecutively with:
```shell
    kubectl apply -f namespace.yaml
    kubectl apply -f deployment.yaml
    kubectl apply -f service.yaml
```
