# Week 10 — CloudFormation Part 1

## Technical Tasks
In the class, we are going to : work on [CFN's](https://aws.amazon.com/cloudformation/resources/templates/)
```
👉 Write a CFN template for our Cluster and Load Balancer
👉 Deploy CFN template
👉 Update CFN template

```
## Business Scenario
```
The CEO went on a trip with our primary investor to Singapore to see how they can break into the APAC (Asian Pacific region). 

The CTO has taken this indication that CEO might turn around at any moment and ask for us to prepare to launch in APAC and since there are no active feature requests by the company we take this opportunity to write our Infrastructure as Code (IaC)

CloudFormation has been chosen since nearly all of our infrastructure lives in AWS (with the exception of our GitHub Git Repositories and Momento Caching Layer),

We do not expect to be changing our IaC often due to our small team and since we are likely entering a long feature development cycle. So relying on yaml files requires zero future maintenance since CFN specification rarely changes. 

```
## Weekly Outcome
```
✅ Write Declarative Infrastructure as Code for a three-tier architecture
✅ Deploy infrastructure via IaC service that manages the remote state
```

## [Possible Spend Considerations](https://docs.google.com/document/d/10Hec7Or1ZUedl0ye-05mVPhYFR5-ySh2K8ZbFqTxu1w/edit#bookmark=id.pc57r5n8uv1)
```
👉 AWS CloudFormation is free, but the resources it can provision may not be. Review the overall cost of what we are provisioning
```

## Alternatives and Considerations
```
📎 In the business scenario we are suggesting the “right solution” is to implement Multi-region, there are other options that would have reduced complexity and improved performance such as us utilizing AWS Global Accelerator, Amazon CloudFront. 
📎 Other reasons why we would want to use CloudFormation (CFN) is to be explicit about what we expect the state of our infrastructure should be, this is good for security, and determining misconfiguration. If we (and we should) commit our CFN to a repo we can keep track of different interactions of our infrastructure, and this allows us possibly to rollback to the previous IaC state.

```

## Security Considerations
```
TBD
```

## Homework Challenges 
``` 
✅ 
```