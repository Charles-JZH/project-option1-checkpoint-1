# project-option1-checkpoint
The code of driver written in vue.js is in the driver folder. In my implementation, only the driver has the dockerfile, so in the dockerfle folder there is only one Dockerfile for driver.  
The display of driver:
![image](https://github.com/Charles-JZH/project-option1-checkpoint/blob/main/driver/display-image.png)

## All docker images dockerhub addresses:  
https://hub.docker.com/repository/docker/charlesjiang1997/driver  
https://hub.docker.com/repository/docker/charlesjiang1997/hadoop  
https://hub.docker.com/repository/docker/charlesjiang1997/jupyter  
https://hub.docker.com/repository/docker/charlesjiang1997/sonarqube  
https://hub.docker.com/repository/docker/charlesjiang1997/spark  

## The steps to run all Docker images on Kubernetes:
1. Push all usable Docker images to my personal dockerhub.  
2. Write deployment configuration files (namely xxx-deployment.yaml) for all Docker images, using their corresponding dockerhub addresses.  
3. Write service configuration files (namely xxx-service.yaml) for all Docker images.  
4. Using "kubectl apply -f xxx-deployment.yaml" command to deploy all Docker images to Kubernetes.  
5. Using "kubectl apply -f xxx-service.yaml" command to deploy all Docker image services to Kubernetes.  
6. Using "kubectl get pods" and "kubectl get svc" to see all running pods and services, as my uploaded picture shows.
