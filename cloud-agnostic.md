# Cloud agnostic datalab

The Cloud Agnostic Datalab is a web service to easily deploy and use containerized data science services like JupyterLab, Rstudio, Spark, Superset and PostgreSQL. It is the main service provided for the hackathon.

![Agnostic overview](img/agnostic_overview.png)

***Typical use case***

It can be used if you want to read data from S3 buckets (with programmatic access) and do some data processing with R/Python/Spark and finally you can create a specific data view, push it to PostgreSQL database and create a custom dashboard with Superset.

The The Cloud Agnostic Datalab is available under this address: [The address will be provided here on 2nd March](cloud-agnostic.md)

## Login

For access to the service you have to click on the EC DataPlatform Azure AD.

![Login screen](img/cag_login_highlighted.png)

There you have to use the provided Azure AD login credentials which you received previously and activated with MFA.

![Azure AD login](img/azure_ad.png)


## Home

After successful login you arrive at the home screen of the Cloud Agnostic Datalab.

![Home](img/cag_home.png)

Here you can find a link to this documentation and the terms of use of these services. ***Please read it at least once,*** because by using these services you agree those terms. 


## My Account

Under the **My Account** you find your Azure AD identifier, your name, your email which is used in the MS Teams group and where you receive the information about your Azure AD account activation. In addition, you will find here the use of resources for your Data Science Lab (DSL) available for your group. 

![Account](img/cag_account.png)

## Service Catalog

Under the **Service Catalog** you find the available services you can launch. 

![Catalogue](img/cag_catalogue.png)

You can choose from the following services:

```{dropdown} Apache Airflow v1.6.0

For the Airflow configuration you have to provide:
 - the name
 - if it is shared or private
 - the DSL of your group - there is only one possibility for your group
 - you have to select the configuration - the **Default** gives you predefined resources, for the **Custom** you can change some of them if the default does not work for you
 - you can change the provided username
 - you have to select the storage (NFS PVC name) - there is only one possibility for your group 
```


```{dropdown} Apache Superset v1.0

For the Airflow configuration you have to provide:
 - the name
 - if it is shared or private
 - the DSL of your group - there is only one possibility for your group
 - you have to select the configuration - the **Micro** gives you predefined resources, for the **Custom** you can change some of them if the default does not work for you
 - you have to provide an admin username 
 - you have to provide an admin email, first name and last name 
```
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
