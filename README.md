# Udacity Cloud DevOps Capstone Project

This is final project of Udacity Cloud DevOps Engineer Nanodegree Program.

## Project Overview

In this project I have implemented all the knowledge that I have learnt from the Udacity Cloud DevOps Engineer Nanodegree program. In this project I have

-   Created Jenkins server using the AWS CloudFormation.
-   Installed all the needed tools in Jenkins master server using the Launch Configuration.
-   Created a infrastructure pipeline using Jenkins that creates one EKS cluster in AWS.
-   Created one application deployment pipeline that deploys the application docker container in the kubernetes cluster.
-   Used blue/green deployment strategy to deploy the application.

## Project Files

#### infrastructure

This folder all the files related to infrastructure deployment.

-   `jenkins-server-parameters.json`: Parameters file for cloud formation stack.
-   `jenkins-server.yml`: CloudFormation template for creating jenkins server.
-   `Jenkinsfile`: Jenkinsfile for creating EKS cluster and configuring kubectl.

#### kubernetes-resources

This folder contains all template files for Kubernetes resources.

-   `blue-replication-controller.yml`: A replication controller template that creates pods with label as `app=blue`.
-   `blue-service.yml`: A service template that selects all the pods with label as `app=blue`.
-   `green-replication-controller.yml`: A replication controller template that creates pods with label as `app=green`.
-   `green-service.yml`: A service template that selects all the pods with label as `app=green`.

#### screenshots

This folder contains all screenshots taken during creation of this project.

#### scripts

This folder contains script to create, delete and update CloudFormation stack.

#### Dockerfile

This is Dockerfile of application.

#### index.html

This is main html file of application.

#### Jenkinsfile

This file contains the steps of CICD pipeline of application.

