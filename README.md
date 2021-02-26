# Overview

This project is  to demonstrate the continuous integration and continuous deployment of a python based machine learning web application.
The process starts with source control management using github and integrating with Azure pipelines in the azure cloud environment.
Whenever there is a change in the source ,It will trigger a continuous integration and subsequnetly a continuosly deploy on the Azure App Service using Azure pipelines ,which is a cloud native solution for Azure Cloud Platform.

## Project Plan
 Project Plan

* A link to a Trello board for the project

https://trello.com/b/KWR72xOW/cicd-project-demo

* A link to a spreadsheet that includes the original and final project plan

https://docs.google.com/spreadsheets/d/10qPdEpRtAW_9_iTs7RSINJ0xq5AABR5MvB9fwSQ8cLo/edit?usp=sharing
s

## Instructions


* Architectural Diagram (Shows how key parts of the system work)







Instructions

-clone the github repository into your local Azure Cloud shell.
-Create a new python virtual environment and enter in to the virtual environment.
-Create a Makefile with the make Instructions for Install ,lint ,Test targets.
- Build the Project locally,using the make all command
-Once the Build is successful,we should deploy the application using The Azure App service using the command
az webapp up -n <name of the application>.
-Once the deployment is succesful,The website can be accessed ,in the Browser using the URL
 http://<name of the application>.azurewebsites.net
 -Once the Build is Successfully deployed using Azure App service,we can go ahead and configure it for automatic build and deployment using Azure Pipelines.
 -Login to Azure Devops and Create a new project for this purpose and Go to project settings and Create a new pipelines.
 -Connect this pipelines to utizile the GitHub repository and Then Connect to the Deployment Azure App service.



* Project running on Azure App Service






















* Project cloned into Azure Cloud Shell





* Passing tests that are displayed after running the `make all` command from the `Makefile`






* Output of a test run

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).






* Running Azure App Service from Azure Pipelines automatic deployment




* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

```bash
udacity@Azure:~$ ./make_predict_azure_app.sh
Port: 443
{"prediction":[20.35373177134412]}
```

* Output of streamed log files from deployed application






## Enhancements

 This project can be improved by adding more tests and more linting profiles.

## Demo 

Demo video is available at the link

(165) CICD Project Demo-Udacity - YouTube 



