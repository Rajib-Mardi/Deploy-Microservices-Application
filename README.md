### Project: 
* Deploy Microservices application in Kubernetes with Production & Security Best Practices
### Technologiesused: 
* Kubernetes, Redis, Linux, DigitalOcean

### Project Description

* Created YAML file with 11 Deployment and corresponding Service manifests for all microservices of an online shop application.
* All the  Services  Components are Internal Services, except the Frontend Service, which needs to be accessed from browser.
* Added version , Configured Liveness Probe for each container
*  Configured Readiness Probe for each container
* Configured Resource Requests
*  Configured Resource Limits
*  Configure more than 1 Replica for each Deployment
* Created a K8s cluster with 3 Worker Nodes on DigitalOcean (or any other cloud platform).
* Connected to the cluster
* Created a Namespace and deployed all the micro services into it
* created a nginx-ingress controller to act as the load balancer for access in the browser.


<img src="https://github.com/Rajib-Mardi/Deploy-Microservices-Application/assets/96679708/8a93f3ab-c65e-4262-9462-1955ed414395" width="700">

*  Accessed Online Shop with Browser

<img src="https://github.com/Rajib-Mardi/Deploy-Microservices-Application/assets/96679708/5eed310a-0006-43eb-a56f-ec4b869cdee1" width="700">



-----------------------------------------------------------------------------


### Project: 
* Create Helm Chart for Microservices
### Technologiesused: 
* Kubernetes, Helm, Helmfile


### Project Description:
* Create 1 shared Helm Chart for all microservices, to reuse common Deployment and Service configurations for the services.

* Created “microservices” Helm Chart.
* Created values.yaml files for each microservice.
* Created “redis” Helm Chart and values file for it.
* created a nginx-ingress controller to act as the load balancer for access in the browser.
* Deploy Microservices with Helm
    * Write a script file that has all these helms installed inside the script file.
    * execute the script file
      ```
      chmod u+x install.sh
      ./install.sh
      ```

<img src="https://github.com/Rajib-Mardi/Deploy-Microservices-Application/assets/96679708/ed7f308f-c6d1-4158-bfd5-4a66e7fa1857" width="700">

* Created the Helmfile
* Installed the Helmfile
* Deploy Microservices with Helmfile


<img src="https://github.com/Rajib-Mardi/Deploy-Microservices-Application/assets/96679708/6d4dced2-df91-4e20-bedb-b346290e4ad7" width="700">



<img src="(https://github.com/Rajib-Mardi/Deploy-Microservices-Application/assets/96679708/639fc5ea-c3bd-48cd-8949-cbf32439183a" width="700">


