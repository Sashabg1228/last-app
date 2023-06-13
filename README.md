# last-app
## Project Description
The main goal of this project was to gain a deeper understanding of AWS lambda functions and their potential use cases. After some research the AWS SAM was chosen for the deployment of th serverless Python application on AWS. AWS SAM simplifies the process of deploying these applications as serverless functions, making it easy to manage and scale the infrastructure.

## About SAM
AWS SAM (Serverless Application Model) is an open-source framework developed by Amazon Web Services (AWS) that simplifies the deployment and management of serverless applications on AWS. SAM provides a simplified syntax for defining serverless resources such as functions, APIs, and event triggers, and it leverages AWS CloudFormation for infrastructure provisioning and deployment.

## How AWS SAM works

1. Initialization 
The command sam init is run in the terminal. It results in the creation of the whole project. The source code of the AWS lambda function is in the hello_world subdirectory.

2. Building 
After the command sam build is run in the main directory of the project, the new subdirectory .aws-sam is created. there is stored the build. 
IMPORTANT: It is necessary for the application to be build the python version to be the same as the version writen in the template.yaml file. If the version is not the same you have to create one that matches the requirements.

3. Deployment
After the application is built successfully the command sam deploy is run. This command updates the deployed application in the AWS environment while maintaining the originally assigned API Gateway URL.

4. Enjoy
