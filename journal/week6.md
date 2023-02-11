# Week 6 — Deploying Containers

## Technical Tasks
In the class, we are going to:


👉 Create an [Elastic Container Repository - ECR](https://docs.aws.amazon.com/AmazonECR/latest/userguide/repository-create.html)

👉 Push our container images to ECR

👉 Write an [ECS Task Definition](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definitions.html) file for Fargate

👉 Launch our [Fargate services](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/AWS_Fargate.html) via CLI

👉 Test that our services individually work

👉 Play around with Fargate desired capacity

👉 How to push new updates to your code update Fargate running tasks

👉 Test that we have a [Cross-origin Resource Sharing (CORS)](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing) issue

## Business Scenario
```
Our primary investor emailed our CEO asking when the web-application will be online to show to their extended private network.

The CEO asked if we could get the web-application up on a domain, and they agreed on a timeline of two weeks.

There are many options to deploy our containers to AWS, and ECS Fargate was chosen because its:
✅  Serverless containers (fewer moving parts to worry about, pay for value), 
✅  We might want to migrate to (Kubernetes) K8s in the future (EKS can use Fargate as worker nodes)

The CTO wants us to deploy the frontend and backend as separate containers, to ensure we avoid building a monolithic application
```
## Weekly Outcome
```
✅ Being able to push and tag container images to remote repository 
✅ Practical knowledge of deploying, configuring and updating a serverless container
✅ Basic knowledge of working with a cloud CLI

```
## [Possible Spend Considerations](https://docs.google.com/document/d/10Hec7Or1ZUedl0ye-05mVPhYFR5-ySh2K8ZbFqTxu1w/edit#bookmark=id.cxxxocsnwv9z)
```
👉 Elastic Container Repository spend
👉 Fargate Compute Spend
👉 CloudWatch Logs pricing
👉 Transfer charges (hidden costs)?

```
## Alternatives and Considerations
```
📎 AWS Copilot CLI could have been used to deploy Fargate services, but it abstracts away a lot of the components, and it will take considerable learning opportunities. The AWS Copilot CLI generates will generate out CloudFormation code. While it can be customized, it's an additional layer we must work through.
📎 AWS AppRunner could have been used and poses similar issues that adopting AWS Copilot CLI in that it abstracts away a lot of our learning opportunities. For a startup, AWS AppRunner is an ideal choice but only for a small amount of containers.
📎 If we had time, I would have had multiple weeks to:
- deploy to AppRunner
- then migrate to using AWS Copilot CLI 
- then use Fargate with CFN (this is our bootcamp focus)
- then a final migration to Fargate with Kubernetes
📎 The front-end application could have beenhosted on Amplify Hosting or hosted using a static S3 website with CloudFront as the CDN and in many cases this would be “ideal way” to host your frontend.
- The reason we didn’t use CloudFront is because creating a distrubtion takes a long time to create and troubleshooting a distribution has a long wait time to update

```

## Security Considerations
```
TBD
```

## Homework Challenges 
``` 
✅ Try and host your frontend application on Static Website Hosting with CloudFront
- This challenge could count for both Week 4 and 5 because you will have to deal with CORS as well.

```