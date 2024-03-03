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
