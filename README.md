# Overview
Deploy a pre-trained ML app using CI/CD with github action and azure devops.


## Project Plan


* https://trello.com/invite/b/KpzguGUS/ATTIaa1c9707691471b68e9c4c3f82476c5e412A3089/untitled-board 
* https://docs.google.com/spreadsheets/d/1s-Cb83qRh870S7P5DGP6j4qKz714c_LwSNWEecOZmRE/edit?usp=sharing

## Instructions

<TODO:  
* Architectural Diagram (Shows how key parts of the system work)>

<TODO:  Instructions for running the Python project.  How could a user with no context run this project without asking you for any help.  Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

* Project running on Azure App Service
![image](https://user-images.githubusercontent.com/47712278/228059139-909f0eea-5b04-4b28-8a19-4c8cee214f3b.png)

![image](https://user-images.githubusercontent.com/47712278/228059180-78d8d0e8-1d5d-4c0b-bad0-5aef77385f05.png)


* Project cloned into Azure Cloud Shell
![image](https://user-images.githubusercontent.com/47712278/228059299-6273a9a3-8ea5-4d73-a815-a77cf13df778.png)


* Passing tests that are displayed after running the `make all` command from the `Makefile`
![image](https://user-images.githubusercontent.com/47712278/228059739-0143af35-95c4-40de-a4a7-f458099a6e40.png)

* Output of a test run

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).
![image](https://user-images.githubusercontent.com/47712278/228060088-7ffe8ef4-c9ad-4bda-a54b-2e882d6e1972.png)

* Running Azure App Service from Azure Pipelines automatic deployment
![image](https://user-images.githubusercontent.com/47712278/228060398-a186655c-0f34-411e-b3ba-cb127411c2b6.png)


* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

```bash
ahmed [ ~/Azure-ML-flask-app ]$ ./make_predict_azure_app.sh 
Port: 443
{"prediction":[48976299843.46421]}
```

* Output of streamed log files from deployed application

> 023-03-27T20:13:58.839Z INFO  - Initiating warmup request to container joyontest_6_bc50f6da for site joyontest

2023-03-27T20:14:11.705Z INFO  - Container joyontest_6_bc50f6da for site joyontest initialized successfully and is ready to serve requests.

2023-03-27T20:14:11.726Z INFO  - Recycling container because of AppSettingsChange and isMainSite = True

2023-03-27T20:14:12.023Z INFO  - 3.10_20230116.1.tuxprod Pulling from appsvc/python

2023-03-27T20:14:12.025Z INFO  -  Digest: sha256:4a5961876e6504cb2deae9f334456274b4c64bd5d3cb0c5683448e2c935d6063

2023-03-27T20:14:12.026Z INFO  -  Status: Image is up to date for mcr.microsoft.com/appsvc/python:3.10_20230116.1.tuxprod

2023-03-27T20:14:12.030Z INFO  - Pull Image successful, Time taken: 0 Minutes and 0 Seconds

2023-03-27T20:14:12.090Z INFO  - Starting container for site

2023-03-27T20:14:12.090Z INFO  - docker run -d --expose=8000 --name joyontest_7_18ba39c1 -e WEBSITE_SITE_NAME=joyontest -e WEBSITE_AUTH_ENABLED=False -e WEBSITE_ROLE_INSTANCE_ID=0 -e WEBSITE_HOSTNAME=joyontest.azurewebsites.net -e WEBSITE_INSTANCE_ID=b56fddc3589a27a6c59d63031ce71b3c56ab18251f4ee91992cd3a612bef33bb -e HTTP_LOGGING_ENABLED=1 -e WEBSITE_USE_DIAGNOSTIC_SERVER=True appsvc/python:3.10_20230116.1.tuxprod  



2023-03-27T20:14:13.307Z INFO  - Initiating warmup request to container joyontest_7_18ba39c1 for site joyontest

2023-03-27T20:14:25.282Z INFO  - Container joyontest_7_18ba39c1 for site joyontest initialized successfully and is ready to serve requests.

## Enhancements

<TODO: A short description of how to improve the project in the future>

## Demo 

https://youtu.be/3luSYFG14U8


