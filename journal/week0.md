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

✅ Gain confidence when working meter-billing with a Cloud Service Provider (CSP)

✅ To understand how to build [useful architecture diagrams- Chris' Examples](https://lucid.app/lucidchart/6f80cd2d-7d18-4731-aadc-bdda9773c092/edit?invitationId=inv_c648fee2-f691-443d-8602-7e959b41a18d&page=0_0#)

✅ To gain a general idea of the cost of common cloud services

✅ To ensure we have a working AWS account

## [Possible Spend Considerations](https://docs.google.com/document/d/10Hec7Or1ZUedl0ye-05mVPhYFR5-ySh2K8ZbFqTxu1w/edit#bookmark=id.n67i8zg8ikxc)
```
👉 You need a credit card to activate your AWS Account
👉 If your AWS account is older than a year, you will not be eligible for some free-tier services.
```

👉 [Other Cost Considerations by Chirag](https://www.youtube.com/watch?v=OVw3RrlP-sI&t=851s)
## [Security Considerations by Ashish Rajan](https://www.youtube.com/watch?v=4EMWBYVggQI&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=15)

🔐 [What Cloud Security is, Why bother?](https://aws.amazon.com/free/security/?trk=9bc21f40-12f4-4d2b-8b8d-6f6f65ab19e6&sc_channel=ps&s_kwcid=AL!4422!3!614802967560!e!!g!!aws%20cloud%20security&ef_id=CjwKCAiAuaKfBhBtEiwAht6H7y0cpEY7-drZmPCfhisgX8A6ogdvzikiEwWk9Njz0F9HxvWJug8YIBoCGPYQAvD_BwE:G:s&s_kwcid=AL!4422!3!614802967560!e!!g!!aws%20cloud%20security)

🔐 Add MFA (if not deactivating root user) for the Root User since its the most powerful user in the AWS environment with access similar to domain admins in the on prem world!

🔐 [Disable regions you do not plan to use to reduce open ports susceptible to breach](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_examples_aws-enable-disable-regions.html)

🔐 [Create an Org Unit to centralize management of users/groups from here](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_tutorials_basic.html)

🔐 [Enable AWS Cloud Trail for data security api usage tracking, and residency for IR/Forensics audit logging](https://www.amazonaws.cn/en/cloudtrail/)

🔐 Create IAM Users with MFA's to not have to run day 2 operations using root user credentials, enable others in your organization using [principle of least privilege](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html) to leverage aws for cloud operations

🔐 Create IAM [Roles](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html) vs [Policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_identity-vs-resource.html)

🔐 Create Org-level [Service Control Policies (SCP)](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html)
## Homework Challenges

✅ [[Installed AWS CLI Latest version]((https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)) on GitPod Desktop with [env variables](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html)]
![CLI Installed on GP Desktop](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-AWS%20CLI%20Installed%20on%20GP%20Desktop.png)
![Env Variables](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-Env%20variables.png)
![Created Account ID Env Variable](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-Created%20AccountID%20Env%20Variable.png)
![GP Persistent Env Variables](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-GPEnvVariablesPersisting.png)
![Get Account Contact Information on GP](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-GP-Account-GetContactInformation.png)

✅ [Installed AWS CLI Command Prompter](https://docs.aws.amazon.com/cli/latest/userguide/cli-usage-parameters-prompting.html)
![Get Caller Identity](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-GetCallerIdentity.png)
![Get Account Contact Information](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-Account-GetContactInformation.png)

✅ [Destroy your root account](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user.html#id_root-user_manage_delete-key), [Set MFA](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_mfa_enable_virtual.html), [IAM role](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-user.html)
![MFA, IAM user](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-%20IAM%20Logged%20in.png)
![IAM user logging in](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-%20IAM%20Login.png)

✅ ![Created Org Unit](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-Org%20Unit%20Creation.png)

✅ [Set a billing alarm](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/monitor_estimated_charges_with_cloudwatch.html#turning_on_billing_metrics), [Set a AWS Budget](https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-create.html), [Set Budget Notifications using CLI](https://docs.aws.amazon.com/cli/latest/reference/budgets/create-budget.html)
![Billing Alert](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-Billing%20Alerts.png)
![Budget](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-Budget.png)

✅ [Applied Org-level Day0 SCP's](https://github.com/hashishrajan/aws-scp-best-practice-policies)
![SCP Created](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-SCP.png)

✅ Review all the questions of each pillars in the [Well Architected](https://aws.amazon.com/architecture/well-architected/) Tool (No specialized lens)

✅ Configured Cloud Trail ![Configure AWS Cloud Trail](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/6938a0f830393ac3cadfcc3baab3e2657fecd273/_docs/Week0-CloudTrailEnabled.png)

✅ Research the technical and [service limits](https://docs.aws.amazon.com/general/latest/gr/aws_service_limits.html) of specific services and how they could impact the technical path for technical flexibility

   👉 [Example](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Service%20Limit%20Checks.xlsx)

✅ Open a support ticket and request a service limit
![Ticket](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-SupportCase.png)

✅ [Use EventBridge to hookup Health Dashboard](https://docs.aws.amazon.com/health/latest/ug/cloudwatch-events-health.html#creating-event-bridge-events-rule-for-aws-health) to SNS and send notification when there is a service health issue
![EventBridge SNS Notification rule](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-EventBridge%20Alerts.png)
![SNS Notification Confirmation](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0-EventBridge%20SNS%20Alert%20Confirmation.png)

✅ Create an architectural diagram (to the best of your ability) the CI/CD logical pipeline in Lucid Charts
 ([HighLevel CI/CD Architecture Flow](https://lucid.app/lucidchart/8dd4bb31-a6b9-480b-986f-65f8256dc229/edit?invitationId=inv_743505e2-23ee-42d6-84dc-aabcde24a6d3))
![HighLevel CI/CD Architecture Dgm](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/bbdd9533c80553702b5305f7fff7db499751a2ad/_docs/Week0%20-%20CI_CD%20Architecture%20Diagram.png)
![Architecture Dgm](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023/blob/main/_docs/Week0%20-%20CI_CD%20Architecture%20Diagram%20(Andrew's%20walkthrough).png)
## Highlevel Architecture /CI CD Pipeline Considerations (Well Architecture Framework Inspired):
### To architect a Twitter Clone/Similar Microservice Application on AWS, the following steps should be considered:

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

### For the CI/CD pipeline the following steps should be considered (thought the actual implementation may vary based on the specific requirements of application):

👉 Set up the AWS environment: Create an AWS account, Set up an Amazon S3 bucket to store the application code and artifacts, Create an Amazon EC2 instance or an AWS Elastic Beanstalk environment to host the application

👉 Write the Code: Write the code for your Twitter application and store it in a code repository like GitHub

👉 Create a CodeBuild Project: Use AWS CodeBuild to automate the building and testing of code whenever a change is pushed to the repository

👉 Create a CodePipeline: Use AWS CodePipeline to automate the deployment of your application since it integrates with CodeBuild and S3 to continuously delivering code from the Github repository to the production environment

👉 Configure the CodePipeline Stages: The source stage pulls the code from the repository and stores it in S3 followed by the build stage uses CodeBuild to build and test the code sequenced by the deploy stage uses AWS Elastic Beanstalk to deploy the code to the production environment

👉 Test the Pipeline: Test the pipeline end-to-end to make sure it works as expected

👉 Monitor the Pipeline: Use Amazon CloudWatch to monitor the pipeline and receive alerts in case of any issues
