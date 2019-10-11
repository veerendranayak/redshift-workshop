# LAB 1 - Setup JDBC connectivity
In this lab you will install JDBC tool and setup connectivity .

## Contents
* [Download and Install Client Tool](#Download-and-Install-Client-Tool)
* [Configure Client Tool](#configure-client-tool)
* [Run Sample Query](#run-sample-query)


## Download and Install Client Tool
* While Amazon Redshift does provide a web-based [Query editor](https://console.aws.amazon.com/redshift/home?#query:) for executing simple queries, for these labs, it is recommended you install a third-party tool. We will use SQL Workbench/J

* Download SQL Workbench from link --> [SQL Workbench/J](http://www.sql-workbench.eu/downloads.html). Select "Generic package for all systems including all optional libraries"

* Once you download SQL Workbench, you will need JDBC or ODBC driver. In this exercise we will use JDBC driver that can be downloaded from [RedShift JDBC Documentation] (https://s3.amazonaws.com/redshift-downloads/drivers/jdbc/1.2.34.1058/RedshiftJDBC42-no-awssdk-1.2.34.1058.jar)

## Configure Client Tool

* Launch SQL Workbench/J (go to downloaded folder and open sqlworkbench.jar). Navigate to [File | Manage Drivers].
* Select "Amazon Redshift" and set the driver Library location to where you downloaded the Redshift JDBC Driver. Click Ok.
![](../images/Library.png)
* Navigate to [File | Connect Window] to create a new connection profile and modify the following settings and once complete click on the "Test Connection" button.
  * Name - "LabConnection"
  * Driver - Amazon Redshift (com.amazon.redshift.jdbc.Driver)
  * URL - Find this by navigating to the [Cluster List](https://console.aws.amazon.com/redshift/home?cluster-details:#cluster-list:), selecting your cluster, and copying the JDBC URL.  
  ![](../images/JDBCUrl.png)
  * Username - awsuser
  * Password - Shutterfly123
  * Autocommit - enabled
  * Alternate Delimiter /  (forward slash)

![](../images/Connection.png)

## Run Sample Query
* Run the following query to list the users within the redshift cluster.  
```
select * from pg_user
```
* If you receive the following results, you have established connectivity and this lab is complete.  
![](../images/Users.png)
