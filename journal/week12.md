# Week 12 — Modern APIs

## Technical Tasks
In the class, we are going to use GraphQL and [AppSync](https://docs.aws.amazon.com/appsync/latest/devguide/designing-a-graphql-api.html) to modernize our API:

```
👉 Implement Realtime Pub/Sub APIs
👉 Implementing WebSockets for front-end react application
👉 Custom Resolver for Lambda Authorizator with AuthN
👉 Use the Amplify Libraries for AppSync
👉 Design GraphQL Schema
👉 Custom Domain with AppSync

```
## Business Scenario
```
Implement a GraphQL API utilizing a NoSQL and SQL data source

The company is looking to hire a web-application developer to keep pace with our upcoming feature-developer cycle to work along your the Cloud Engineering team,

After reviewing hundreds of applicants it’s been hard to find web-application developers that complement writing raw SQL and next to none who know the DynamoDB API.

However, we notice many applicants know how to use React and also know how to use GraphQL. (Maybe there is a correlation between these open-source technologies built by Facebook)

The fractional CTO has asked you to investigate using AWS AppSync (a hosted version of GraphQL) and report back the effort to use maintain over a standard REST API.

```
## Weekly Outcome
```
✅
```
## [Possible Spend Considerations](https://docs.google.com/document/d/10Hec7Or1ZUedl0ye-05mVPhYFR5-ySh2K8ZbFqTxu1w/edit#bookmark=id.rrnte5qnq0rm)
```
👉 AppSync has a good free-tier limit -  $4M 

```
## Alternatives and Considerations
```
📎 Instead of AppSync for realtime we could have API Gateway for Realtime, some would suggest that AppSync is easier to use
📎 Alternatives to AppSync could be using open-source Apollo. You’d have to run Apollo on your compute such as Lambda, Apollo does not (at the time of writing document) Realtime Subscriptions

```

## Security Considerations
```
🎯 You can set AWS WAF (OWASP 10)
🎯 Authenication with Amazon Cognito
🎯 Enable Logging for CloudWatch
🎯 This would track request to the endpoints
🎯 not obfuscated in the logs (just like a Lambda function)
🎯 AppSync is Encypted by default
🎯 Identity-based Policies through IAM
🎯 API calls tracked through CloudTrail (GetGraphqlApi,CreateApikey) 
🎯 This does not track requests to the endpoints

```

## Homework Challenges 
``` 
✅ Convert an existing DynamoDB REST API endpoint to use AppSync GraphQL
✅ Convert an existing Postgres SQL REST API endpoint to use AppSync GraphQL
✅ Replace AuthN with Cognito as authentication system with AppSync


```