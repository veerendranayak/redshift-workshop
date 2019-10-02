# Redshift Immersion Day Labs
This GitHub project provides a series of lab exercises which help users get started using the Redshift platform.

## Goals
Amazon Redshift is a fast, fully managed, petabyte-scale data warehouse solution that uses columnar storage to minimise IO, provides high data compression rates, and offers fast performance. This GitHub project provides a series of lab exercises which help users get started using the Redshift platform.  It also helps demonstrate the many features built into the platform.

As part of Lab Setup, we have created Redshift cluster in each of the accounts. So we will start with configuring JDBC connectivity to Redshift in Lab1.

## Labs
|# |Lab Name |Lab Description |
|---- |---- | ----|
|1 |[Configuring JDBC connectivity](lab1-redshiftconnectivity/README.md) | connectivity with SQL Workbench/J |
|2 |[Data Loading](lab2/README.md) |Table creation, data load, and table maintenance |
|3 |[Table Design & Query Tuning](lab3/README.md) |Setting distribution and sort keys, deep copy, explain plans, system table queries |
|4 |[Modernize Your Data Warehouse with Amazon Redshift Spectrum](lab4/README.md) |Query petabytes of data in your data warehouse and exabytes of data in your S3 data lake, using Redshift Spectrum |
|5 |[Amazon Redshift Spectrum Query Tuning](lab5/README.md) | Diagnose Redshift Spectrum query performance and optimize by leveraging partitions, optimizing storage, and predicate pushdown.|
|6 | [Amazon Redshift Operations](lab6/README.md) | Step through some common operations a Redshift Administrator may have to do to maintain their Redhshift environment including Event Subscriptions, Cluster Encryption, Cross Region Snapshots, and Elastic Resize |
|7 | [Querying Nested JSON](lab7/README.md) | Query Nested JSON datatypes (array, struct, map) and load nested data types into flattened structures.|
