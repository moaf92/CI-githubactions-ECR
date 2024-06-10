# CICD-githubactions-ECR
in this project we will use CI using githubactions,we will have maven to build the code sonarqube for code scanning, sonarcloud for quality gates of our code inspection, docker to build our artifact into a docker image, aws ECR to store our docker image 
# STEPS

- First we are going to pull our sourcecode in the workflow of our repo, test it and get analysis of checkstyle type

- On sonarcloud create organization and projectname after this create token to save them as github secret for our project, pass these parameters into workflow 
  after setup sonar scanner

- Crete our quality gates and attach it to our project

- Now time to build our docker image and upload it to amazon ECR, but first we have to create IAM user  with ecr and ecs polices, create ECR repo and RDS 
  database

- create database of type MYSQL and create instance to run mysql client on it and clone our sourcecode of db to run againt MYSQL database

- build our docker image mention our ecr regisrtey to store the buld image

