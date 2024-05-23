
**OEC Assignment**

## **Overview**

This project is a simple architecture with a front-end project that communicates with a backend payments API. The goal is to containerize both applications, deploy them using Helm charts on a local Minikube cluster, and demonstrate the functionality by port forwarding into the front-end service.

## **Project Structure**

- **frontend/**: Contains the front-end application.
    - Dockerfile
- **payments-api/**: Contains the backend payments API.
    - Dockerfile
- **helm/**: Contains the helm files of both front end and backend.

## **Prerequisites**

- Docker
- Minikube
- Helm
- Kubectl


Built docker images directly on the minikube cluster

Front End Docker Image: docker.io/library/front-end-image:latest

Backend Image: docker.io/library/payments-api-image:latest

![image](https://github.com/vishalr127/oecassignment/assets/146502410/07a6a2df-461f-471b-b705-ff8a5eb22445)

Deployed the application onto the minikube through Helm Chart

![image](https://github.com/vishalr127/oecassignment/assets/146502410/7e619d44-158e-4671-a45d-d0858efd6b5a)




