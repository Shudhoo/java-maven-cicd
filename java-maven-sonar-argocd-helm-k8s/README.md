# This is my Readme and Post Defination of this particular Project

Today I worked on this Java Based application which is build using maven and have a CICD Pipeline follwoing DevSecOps Pratices !
The Ultimate Pipeline has phases like ( GitHub-Webhook ) -> ( Maven ) -> ( SonarQube ) -> ( Unit Tests ) -> ( Docker Build and Push ) = Continuous Integration
The Aother part which is Continious Develivery is done using ArgoCD ( Docker Hub ) <- ( ArgoCD Controller ) -> ( Kubernetes Manifests )

This is the flow of my Jenkins Pipeline .

### Password Jenkins --> java-maven-project  ###
###  -->   ###

Jenkins Dashboard 
![alt text](<Screenshot from 2025-07-29 23-35-38.png>)

### Step 1. Have you ever think that running jenkins pipeline and agents of different diffrent OS will be usefull but they are running even when there is no pipeilne running these causes wasteage of resources and well the most is increasing . To use resources and save the cost we can use the Jenkins Docker Agents
In my this project I am going to use docker as a jenkins agent and will build my application using maven and unit for test there is a image already there on Docker Hug i ahve configured that .

### Step 2. I have used execute shell method to update the manifest repo with the build number and later this repo will be wtached by the ArgoCD Controller in K8s-Cluster to update the image/version of the application 

### Step 3. 
For this particular Project of Java and Maven I am using Minikube for my Deployemnt of Application i have installed argocd form operatorshub.io .

