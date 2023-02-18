# Cloud accelerated datalab

The Cloud Accelerated Datalab is web service to easily manage the cloud-based resources provided to each team like the S3 buckets, EC2 machines and IAM credentials. It is a secondary service for the hackathon

![Accelerated overview](img/accelerated_overview.png)

***Typical use case***

It can be used if the services in the Cloud Agnostic Datalab does not fulfill your needs. For example, you need to leverage GPU power to run computationally expensive data processing/ML tasks or you need root access to install a specific tool/software. Also this is the place where you can get temporary AWS access credentials to have programmatic access to the S3 Buckets of the hackathon.


The The Cloud Accelerated Datalab is available under this address: [The address will be provided here on 2nd March 2023](cloud-accelerated.md)

## Login

To access the Login page you have click on the **Log In** button

![landing](img/cac_landing.png)

For access to the service you have to click on the EC DataPlatform Azure AD.

![Login screen](img/cac_login_highlighted.png)

There you have to use the provided Azure AD login credentials which you received previously and activated with MFA.

![Azure AD login](img/azure_ad.png)

## Home

After successful login you arrive at the home screen of the Cloud Accelerated Datalab.

![Home](img/cac_home.png)

Here you can find a link to this documentation and the terms of use of these services. ***Please read it at least once,*** because by using these services you agree those terms. 

## My Account

Under the **My Account** you find your Azure AD identifier, your name, your email which is used in the MS Teams group and where you receive the information about your Azure AD account activation. In addition, you will find here the of your group.

The sub menu *Cost Reports* is not used during the hackathon.

![Account](img/cac_account.png)

## Services 

Under the **Services** you find the list of AWS services you can manage from the Cloud Accelerated Portal. 

### Amazon EC2

Under the **Amazon EC2** you can start and stop a Linux server or a Windows server with admin rights.

![EC2](img/cac_ec2.png)

```{dropdown} Linux server

It is a Linux server with a data science image on it. It is a [g5.4xlarge](https://instances.vantage.sh/aws/ec2/g5.4xlarge) instance with 16 cores, 64 GB RAM and with an NVIDIA A10G GPU. 


```

```{dropdown} Windows server

It is a Windows server without any pre-installed software. It is a [r5.8xlarge](https://instances.vantage.sh/aws/ec2/r5.8xlarge) instance with 32 cores and 256 GB RAM. 
```



### Amazon S3

### Amazon IAM

### Amazon RDS

It is not used for the hackathon.

## Limitations

 - Don’t update services’ version manually/from the UI
 - This does not apply to second level software packages such as libraries etc.
 - Users are limited when accessing AWS Management Console (only S3 Access)
 - The user cannot launch an EC2 instance (or an RDS instance) directly from the portal. Only Start/Stop and access the applications running on the instances

