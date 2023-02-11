# Week 0 — Billing and Architecture / Bootcamp Overview and Introduction to Cloud Spend
## Technical Tasks
In the class, we are going to lay out the foundation for the entire bootcamp by:
```
👉 Discussing the format of the bootcamp
👉 Going over the business use-case of our project
👉 Looking at an architectural diagram of what we plan to build
👉 Showcase how to use Lucid Charts to build architectures
👉 Talk about C4 Models
👉 Running through the cloud services we will utilize
👉 Testing that we can access our AWS accounts
👉 Settings up AWS free-tier and understand how to track spend in AWS --> eg . AWS Budgets, AWS Cost Explorer, Billing Alarms
👉 Understanding how to look at monthly billing reports
👉 Launching AWS CloudShell and looking at AWS CLI
👉 Generating AWS credentials
```
## Business Scenario
```
Your company has asked to put together a technical presentation on the proposed architecture that will be implemented so it can be reviewed by the fractional CTO.

Your presentation must include a technical architectural diagram and breakdown of possible services used along with their justification.

The company also wants to generally know what spend we expect to encounter and how we will ensure we keep our spending low.
```
## Weekly Outcome
```
✅ Gain confidence when working meter-billing with a Cloud Service Provider (CSP)
✅ To understand how to build useful architecture diagrams
✅ To gain a general idea of the cost of common cloud services
✅ To ensure we have a working AWS account
```
## [Possible Spend Considerations](https://docs.google.com/document/d/10Hec7Or1ZUedl0ye-05mVPhYFR5-ySh2K8ZbFqTxu1w/edit#bookmark=id.n67i8zg8ikxc)
```
👉 You need a credit card to activate your AWS Account
👉 If your AWS account is older than a year, you will not be eligible for some free-tier services.
```
## Alternatives and Considerations
```
TBD
```

## Security Considerations
```
TBD
```

## Homework Challenges 

✅ [Destroy your root account](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user.html#id_root-user_manage_delete-key), [Set MFA](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_mfa_enable_virtual.html), IAM role

![MFA, Root user](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0%20-%20IAM%20Root%20MFA.png)

![MFA, IAM user](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-%20IAM%20Logged%20in.png)

![IAM user logging in](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-%20IAM%20Login.png)

✅ [Set a billing alarm](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/monitor_estimated_charges_with_cloudwatch.html#turning_on_billing_metrics), [Set a AWS Budget](https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-create.html)

![Billing Alert](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-Billing%20Alerts.png)

![Budget](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-Budget.png)

✅ Use EventBridge to hookup Health Dashboard to SNS and send notification when there is a service health issue.
✅ Review all the questions of each pillars in the [Well Architected](https://aws.amazon.com/architecture/well-architected/) Tool (No specialized lens)
✅ Research the technical and [service limits](https://docs.aws.amazon.com/general/latest/gr/aws_service_limits.html) of specific services and how they could impact the technical path for technical flexibility. 
✅ Open a support ticket and request a service limit
✅ Create an architectural diagram (to the best of your ability) the CI/CD logical pipeline in Lucid Charts
 ([HighLevel Architecture Flow](https://lucid.app/lucidchart/8dd4bb31-a6b9-480b-986f-65f8256dc229/edit?invitationId=inv_743505e2-23ee-42d6-84dc-aabcde24a6d3))
-----
## Highlevel Architecture Considerations (Well Architecture Inspired):

To architect a Twitter Clone/Similar Microservice Application on AWS, the following steps should be considered:

👉 Define the requirements and scope of the application: To start with, need to finalize on defines requirements of your application, such as how many users to handle, how many posts per second, handling followers and followees etc. This will help you determine the right components and services to use in your architecture

👉 Choose a load balancer: To handle/distribute the incoming traffic (may be evenly) to your application, could use an Amazon ELB or Amazon ALB to balance the load between multiple instances of microservices

👉 Content Delivery Network (CDN): To serve media files, such as images and videos, could use Amazon CloudFront to distribute the content closer to the end-user for faster delivery

👉 Cache: To improve the performance of your application, you can use Amazon ElastiCache for in-memory caching

👉 Decide on a database: Could choose to use a relational database like Amazon RDS or a NoSQL database like Amazon DynamoDB depending on use case and requirements to store user information and posts. If large amounts of data, may want to consider using Amazon S3 or Amazon Glacier for long-term data storage

👉 Monitor and scale the application: Could use Amazon CloudWatch and Amazon Auto Scaling to monitor application and scale it as needed to handle changing traffic patterns. Also could use Amazon ECS or EKS to monitor and manage the performance of your application. This will help identify and resolve issues quickly, ensuring the reliability and availability of the application.

👉 Application instances: To handle incoming requests, can have multiple instances of application running in Amazon EC2 or Amazon ECS depending on budget/requirements

👉 Data model: Design the data model: Create a data model that defines the data that needs to be stored in each microservice, as well as the relationships between the data. This will help you determine the appropriate storage options and help you with data consistency.


👉 App refactor aka create microservices: Write the code for each microservice, using the appropriate programming languages and frameworks for each. Make sure to follow best practices for writing scalable and secure microservices. Create multiple microservices for application, such as a user management service, a post management service, and a notifications service. Each service can be deployed in its own Amazon EC2 instance or using Amazon ECS or Amazon Fargate, depending on overall budget/needs.

👉  MVP: Deploy and test the microservices: Deploy the microservices to the AWS environment and test them to make sure they work as expected. This will help you identify and resolve any issues before your application goes live.

👉 Use Amazon SNS for notifications: To send notifications to users, use Amazon SNS to publish messages to multiple subscribers, such as email, SMS, and mobile push notifications