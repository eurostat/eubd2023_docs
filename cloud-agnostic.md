# Cloud agnostic datalab

Web service to easily deploy and use containerized data science services (JupyterLab, Rstudio, Spark, Superset, PostgreSQL)
Main service for the Hackathon

![Agnostic overview](img/agnostic_overview.png)

***Usecase***

Your team needs to read the data from S3 (with programmatic access) with Spark to do some processing. 
Your team needs  to create a specific data view, push it to PostgreSQL and create a custom dashboard on Superset.


## Login

## Home

## My Account

## Service Catalog

## My Services


## My Data

## Limitations

 - Deployment configuration cannot be changed after its launch
 - Manually updating a secret automatically generated at the instance deployment
 - Each service is provided with a specific service’s version
 - Don’t update services’ version manually/from the UI
 - No root access for JupyterLab and R-Studio
 - Some libraries will need to be installed by the user
 - Simultaneous access to shared services is limited
 - The storage quota of the DSL is not validated against its limits
