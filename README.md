### Project: 
* Deploy Microservices application in Kubernetes with Production & Security Best Practices
### Technologiesused: 
* Kubernetes, Redis, Linux, DigitalOcean

### Project Description

* Created YAML file with 11 Deployment and corresponding Service manifests for all microservices of an online shop application.
* All the  Services  Components are Internal Services, except the Frontend Service, which needs to be accessed from browser.
*   Added version , Configured Liveness Probe for each container
*  Configured Readiness Probe for each container
* Configured Resource Requests
*  Configured Resource Limits
*  Configure more than 1 Replica for each Deployment
* Created a K8s cluster with 3 Worker Nodes on DigitalOcean (or any other cloud platform).
* Connected to the cluster
* Created a Namespace and deployed all the micro services into it
*  Accessed Online Shop with Browser

