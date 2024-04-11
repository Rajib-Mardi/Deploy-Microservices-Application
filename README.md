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

---------------------------------------------------------------------------------------

<img src="https://github.com/Rajib-Mardi/Deploy-Microservices-Application/assets/96679708/639fc5ea-c3bd-48cd-8949-cbf32439183a" width="700">






------------------------------------------------------------

### Project: 
* Deploy Microservices application in Kubernetes with Production & Security Best Practices
### Technologiesused: 
* Kubernetes, Redis, Linux, DigitalOcean

### Project Description

### The application is a web-based e-commerce app where users can browse items, add them to the cart, and purchase them.

#### Microservices Deployed:

* Frontend Service: Acts as the entry point for user requests. It receives requests from the browser and forwards them to other microservices.
Cart Service: Stores shopping cart information. Utilizes Redis as an in-memory database.
* Other Microservices: Include Currency, Product Catalog, Payment, Shipping, Email, Checkout, and Recommendation services.

#### Interconnection of Microservices:

* The frontend service is the entry point, receiving requests from the browser and routing them to other microservices as needed.
* The cart service stores shopping cart data in Redis, acting as a central repository for cart information.
* Microservices communicate with each other as required by the application logic to facilitate browsing, purchasing, and other functionalities.

#### External Accessibility and Entry Point:

* The frontend service is accessible externally and serves as the entry point for user requests. It is exposed as a LoadBalancer service to access from the internet.
All other microservices are accessible internally within the Kubernetes cluster and are not exposed externally. They are accessed through ClusterIP services.

#### Deployment Configuration:

* Deployment configurations are created for each microservice specifying details such as image versions, ports, environment variables, and other settings.
Services are defined for each microservice to enable communication between them within the Kubernetes cluster.

#### Production & Security Best Practices:

* Each container is configured with specific image versions, liveness and readiness probes, resource requests, and limits to ensure reliability and scalability.
* LoadBalancer or Ingress is used to securely expose the frontend service to the internet.
* Multiple replicas are deployed for high availability, and labels are applied to all resources for easy identification and management.
* Namespaces are utilized to isolate resources and manage access control.
* Regular updates ensure Kubernetes nodes run the latest versions for security and performance enhancements.
* Containers are configured to run without root access to enhance security.
* Images are scanned for vulnerabilities to ensure they are free of security risks.

#### Deployment Process:

* Create a K8s cluster with 3 Worker Nodes on DigitalOcean (or any other cloud platform).
* Connectto the cluster
* Create a Namespace and deployed all the micro services into it
* create a nginx-ingress controller to act as the load balancer for access in the browser.

* The microservices are deployed to the Kubernetes cluster using the defined deployment configurations and services.
