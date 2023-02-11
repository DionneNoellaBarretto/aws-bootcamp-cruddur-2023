# Week 4 — Postgres and RDS

## Technical Tasks
In the class, we are going to:

👉 Have a lecture about data modelling in (3rd Normal Form) 3NF for SQL

👉 Launch Postgres locally via a container

👉 Seed our Postgres Database table with data

👉 Write a Postgres adapter

👉 Write a DDL (for creating schema)

👉 Write an SQL read query

👉 Write an SQL write query

👉 Provision an [RDS Postgres instance](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_PostgreSQL.html)

👉 Configure [VPC Security Groups](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)

👉 Configure local backend application to use production connection URL

👉 Add a caching layer using Momento Serverless Cache

👉 Propagate metrics from DDB to an RDS metrics table 

## Business Scenario
```
The CEO met with the primary investor and demoed the web-application. The CEO feels the investor was impressed with our rapid development progress thus far.

The primary investor asked us how we plan to track platform growth. The CEO said that we had already begun implementation on basic tracking growth metrics within a backend dashboard of our platform:
🗹  How many users are on the platform
🗹  How many posts are on the platform
🗹  How many new users per day for the last week
🗹  How many new posts per day for the last week

The CEO is going to meet again with the primary investor next week, and the CEO wants us to deliver on their spur-of-the-moment promise. So we need to rapidly deliver a simple dashboard with platform metrics.

To keep up with the pace of feature development, the CTO has suggested we use Postgres as a relational database. Since our backend does not require the same scale as the customer-facing part of our application.

```
## Weekly Outcome
```
✅ Be able to data model using 3rd normal forms
✅ Practical working knowledge of utilizing a Postgres database
✅ Basic knowledge of working with an Online Analytical Processing (OLAP)

```
## [Possible Spend Considerations](https://docs.google.com/document/d/10Hec7Or1ZUedl0ye-05mVPhYFR5-ySh2K8ZbFqTxu1w/edit#bookmark=id.z4yyfmaafnom)
```
👉 RDS instance
👉 RDS Snapshots
👉 Momento free-tier limit


```
## Alternatives and Considerations
```
📎 We require a Postgres service if we plan into AuthN which will rely on Postgres to store users for authentication.
📎 I want both an OnLine Transaction Processing (OLTP) and an OLAP in this project
Redshift Serverless could be used as an OLAP
📎 DDB Streams to S3 and then Athena caching to Momento could have been possible as well for our OLAP like solution

```

## Security Considerations
```
TBD
```

## Homework Challenges 
``` 
✅ 
```