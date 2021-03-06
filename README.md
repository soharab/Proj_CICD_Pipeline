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


## Instructions


* Architectural Diagram (Shows how key parts of the system work)

https://pasteboard.co/JQaH2mg.png

Instructions

-clone the github repository into your local Azure Cloud shell.

-Create a new python virtual environment and enter in to the virtual environment.

-Create a Makefile with the make Instructions for Install ,lint ,Test targets.

- Build the Project locally,using the make all command
- 
-Once the Build is successful,we should deploy the application using The Azure App service using the command
az webapp up -n <name of the application>.
 
-Once the deployment is succesful,The website can be accessed ,in the Browser using the URL
 http://<name of the application>.azurewebsites.net
 
 -Once the Build is Successfully deployed using Azure App service,we can go ahead and configure it for automatic build and deployment using Azure Pipelines.
 
 -Login to Azure Devops and Create a new project for this purpose and Go to project settings and Create a new pipelines.
 
 -Connect this pipelines to utizile the GitHub repository and Then Connect to the Deployment Azure App service.



* Project running on Azure App Service
https://cicdprojectdemo.azurewebsites.net/

* Project cloned into Azure Cloud Shell

https://pasteboard.co/JQaD3lo.png

* Passing tests that are displayed after running the `make all` command from the `Makefile

https://pasteboard.co/JQaByF8.png

* Output of a test run
 
https://pasteboard.co/JQv2j8l.png

*GitHub actions Badge

[![Python application test with Github Actions](https://github.com/soharab/Proj_CICD_Pipeline/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/soharab/Proj_CICD_Pipeline/actions/workflows/pythonapp.yml)

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).

https://pasteboard.co/JQaEkio.png

https://pasteboard.co/JQv6FBv.png

* Running Azure App Service from Azure Pipelines automatic deployment

https://pasteboard.co/JQaF4bz.png

* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:


* Output of streamed log files from deployed application

https://pasteboard.co/JQaF4bz.png

* Locust Load Testing Screenshot

https://pasteboard.co/JQv7M0T.png

## Enhancements

 This project can be improved by adding more tests and more linting profiles.

## Demo 

Demo video is available at the link

https://www.youtube.com/watch?v=pmBYlalSTs0



