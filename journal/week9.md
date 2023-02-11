# Week 9 — CI/CD with CodePipeline, CodeBuild and CodeDeploy

## Technical Tasks
In the class, we are going to:

👉 Write a [buildspec.yml](https://docs.aws.amazon.com/codebuild/latest/userguide/build-spec-ref.html) to build new images from our GitHub repository

👉 Test [AWS CodeBuild](https://docs.aws.amazon.com/codebuild/latest/userguide/create-project.html) is building and tagging our images correctly

👉 Write an [appspec.yml](https://docs.aws.amazon.com/codedeploy/latest/userguide/reference-appspec-file.html#appspec-reference-ecs) with multiple lambda for steps

👉 Manually trigger a deploy with [CodeDeploy](https://docs.aws.amazon.com/AmazonECS/latest/userguide/create-blue-green.html) to Fargate

👉 Create a [CodePipeline](https://docs.aws.amazon.com/codepipeline/latest/userguide/welcome.html) that will trigger CodeBuild and CodeDeploy when code changes are pushed to our GitHub repository

## Business Scenario
```
The fractional CTO has had a talk with the CEO about the pace of feature development and the fact that its a manually and messy process to push changes since we have yet to automated, and we risk keeping up with feature development.

The CEO agrees with the CTO and has allowed us to focus on improving the automation around deployments.

The CTO has chosen that we use AWS CodePipeline simply due to leveraging more of the AWS ecosystem and the interoperability between services.

```
## Weekly Outcome
```
✅ Configuring and running a build server to bake container images and push to private repo
✅ Configure deployment controller for server containers
✅ Implement Continuous Deployment for backend and frontend applications

```
## [Possible Spend Considerations](https://docs.google.com/document/d/10Hec7Or1ZUedl0ye-05mVPhYFR5-ySh2K8ZbFqTxu1w/edit#bookmark=id.kgk7xd394kyy)
```
👉 Detail Codebuild costs
👉 Detail Codedeploy costs
👉 Detail CodePipeline cost

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
``` 
✅ Create a build server that will run the test suite for the backend code
- Add the test server step to CodePipeline

```