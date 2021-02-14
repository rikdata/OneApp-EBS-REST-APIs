# OneApp-EBS-REST-APIs
RikData OneApp is a mobile application for creating, viewing, and updating various business-related documents and transactions in different ERP systems(Oracle Cloud Application, Oracle EBS R12, SAP HANA S/4). 

The primary difference between OneApp EBS and Oracle Cloud Application is the REST APIs used on the server-side. As Oracle Cloud provides well defined REST APIs for Cloud application, OneApp uses all the REST APIs created by Oracle. However, REST APIs available in Oracle EBS is very limited and not that well structured. Though some APIs are available as part of Integrated SOA Gateway (ISG), the APIs are available only for few entities and not well defined as in Oracle Cloud. Thus, OneApp uses a separate application (RikData OneApp REST APIs for EBS).

RikData OneApp REST APIs for EBS is a Spring-based application that uses Java in the backend and Dart/Flutter/JavaScript in the frontend. OneApp EBS exposes all EBS entities (Tables) through REST API. Using RikData OneApp REST APIs for EBS, you can view data available in all EBS R12 tables (15000 + tables). Using OneApp EBS, you can also create/update/delete records in all interface tables.


## How to use
Download the application. 
Unzip all the files.
Change your EBS Database details in application.properties file

spring.datasource2.url=jdbc:oracle:thin:@//localhost:1521/ebsdb

spring.datasource2.username=username

spring.datasource2.password=password

Start the application using Java

java -jar oneapp-0.0.1-RELEASE.war

Update the EBS_PROD instance of your client application (Desktop/Mobile).

Log in to the application using default username and password: admin/admin.

Read the documentation @ http://docs.rikdata.com and JavaDocs @ https://docs.rikdata.com/docs/javadocs/

