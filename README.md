# FREE AWS Cloud Project Bootcamp
```
- Application: Cruddur
- Cohort: 2023-A1
```
- [Youtube Playlist](https://www.youtube.com/playlist?list=PLBfufR7vyJJ609vhGNS4I9wRCL8aI59Rd)
- [Discord](https://discord.com/channels/1055552619441049660/1069062377766666300)
- [AWS Cloud Project Bootcamp Outline](https://docs.google.com/document/d/19XMyd5zCk7S9QT2q1_Cg-wvbnBwOge7EgzgvtVCgcz0/edit?usp=sharing)
- [AWS Cloud Project Bootcamp FAQs](https://docs.google.com/document/d/1VEs2i_tm1FxUatu1ZfUZH8EEVlhN9XWpVDvqg7GYeKM/edit?usp=sharing) 
- [AWS Cloud Project Bootcamp Spending Considerations](https://docs.google.com/document/d/10Hec7Or1ZUedl0ye-05mVPhYFR5-ySh2K8ZbFqTxu1w/edit#heading=h.sfgk2xkezrng)
- [AWS Cloud Bootcamp Grading Rubric (Individual vs Team)](https://docs.google.com/document/d/1ib98SsYYwWlqkGWZ_s9u0KFFovn_GtLsEV3JJaJ1890/edit)
- [AWS Cloud Project Bootcamp Surveys](https://docs.google.com/document/d/1XWuCvo2HkCUhqMpJiv0K5fJDKWkkO6AoXP8rnT39vkk/edit?usp=sharing)
- [AWS Cloud Project Bootcamp Codes of Conduct](https://docs.google.com/document/d/1Rutvjt1uBtq_SbDg-0cmImjHqq5IvGK8FIzW1L-9FDk/edit?usp=sharing)
- [AWS Cloud Project Bootcamp Sponsorship Package](https://docs.google.com/document/d/1FpVI2fZaji-q2xPj8BIxOWjUjnd7wsYZfxqFc1aa0VY/edit?usp=sharing)
- [AWS Ontario Virtual User Group Meetup Page](https://www.meetup.com/aws-ontario-virtual-user-group/)
- [Discounted Training Deals - LIMITED TIME ONLY!](https://docs.google.com/spreadsheets/d/1EDxIryZ11maOC-P8f3wPlI_fQv6gTnBc0sbDL_wojIY/edit#gid=0) 
- Pre-requisites: Github, Gitpod, AWS Free Accounts

This is the starting codebase that will be used in the [FREE AWS Cloud Project Bootcamp 2023](https://student.cloudprojectbootcamp.com/profile)

![Cruddur Graphic](_docs/assets/cruddur-banner.jpg)

![Cruddur Screenshot](_docs/assets/cruddur-screenshot.png)

## Instructions

👉 At the start of the bootcamp you need to create [a new Github Repository from this template](https://github.com/DionneNoellaBarretto/aws-bootcamp-cruddur-2023).

## Learning Outcomes
```
✅ To learn how to containerize a frontend and backend web application 
 👉 eg. Docker
✅ To learn how to work with multiple serverless containers 
 👉 eg. AWS Fargate, Amazon ECR
✅ To learn how to abstract API call with GraphQL 
 👉 eg. AWS AppSync
✅ To learn basic data modeling for NoSQL databases 
 👉 eg. Amazon DynamoDB
✅ To learn basic data modeling for SQL databases
 👉 eg. Amazon RDS
✅ To learn aside-caching to improve database performance
 👉 eg. Momento
✅ To learn how to set up a CI/CD pipeline 
 👉 eg. CodeBuild, CodeDeploy, CodePipeline
✅ To learn how to use Infrastructure as Code (IaC)
 👉 eg. CloudFormation
✅ To learn how to offload background jobs to serverless functions
✅ To learn how to setup hosted zones
 👉 Route53
```

## Journaling Homework

The `/journal` directory contains

- [X] [Week 0](journal/week0.md)
- [ ] [Week 1](journal/week1.md)
- [ ] [Week 2](journal/week2.md)
- [ ] [Week 3](journal/week3.md)
- [ ] [Week 4](journal/week4.md)
- [ ] [Week 5](journal/week5.md)
- [ ] [Week 6](journal/week6.md)
- [ ] [Week 7](journal/week7.md)
- [ ] [Week 8](journal/week8.md)
- [ ] [Week 9](journal/week9.md)
- [ ] [Week 10](journal/week10.md)
- [ ] [Week 11](journal/week11.md)
- [ ] [Week 12](journal/week12.md)
- [ ] [Week 13](journal/week13.md)

## Project Scenario

```
A startup company has decided to build their own micro-blogging platform and has hired you to be its first cloud engineer.

The company paid a web-development firm to translate their wireframe designs into a mock web-application for the purpose of demoing to raise capital.

After a successful round of funding, you [the cloud engineer] have been tasked with taking the mock web-application and making it production ready at scale.

The startup company consulted a fractional CTO to help choose some of the technical requirements to place the company on a good technical roadmap:

✅ The frontend application should be written in Javascript using React (functional components).
✅ The backend application should be written in Python using Flask
✅ Since we plan to be API only
✅ Since we want to choose a popular framework API only framework
✅ Since we want a micro-framework because we are offloading as much to the cloud as possible to avoid be a monolithic application
✅ Since we don’t want an ORM because the CTO considers it an anti-pattern
✅ Since Python is the most popular language being learned for cloud right now
✅ That an API specification be defined detailing the exact endpoints required.

The web application:
✅ Shall be deployed to AWS.
✅ Takes advantage of modern-applications cloud services.

The startup company has spent the majority of their funding on hiring you for the next 6 months (but mostly spent the money on marketing and buying a really cool domain) and so you also need to ensure you keep the cloud provider costs as low as possible.

Good Luck! 😂
```

## Project Description

### Pitching Cruddur to Customers
```

Introducing a new micro-blogging platform that emphasizes privacy and the present moment. 

Our platform allows users to post updates, thoughts, and photos that automatically expire after a period of time, ensuring that your personal information and conversations stay relevant and in the moment. 

Perfect for busy professionals, students and anyone who wants to stay connected without the pressure of maintaining a permanent online presence. 

Sign up now and experience the freedom of ephemeral social media.
```

### Pitching Cruddur to Investors
```
What are the largest hurdles for long-term success and largest liability for social media platforms? Trust and Safety Issues

A micro-blogging platform with expiring posts can help reduce trust and safety issues that are common on most social media platforms in several ways:
📝 Reduces the amount of personal information available online: By having posts automatically expire, users are less likely to share sensitive personal information that could be used for identity theft or other malicious purposes.
📝 Decreases the potential for cyberbullying and harassment: With ephemeral content, there is less of a chance for negative or harmful posts to be saved and shared, reducing the potential for bullying and harassment.
📝 Improves the overall user experience: By allowing users to focus on the present moment, rather than worrying about the long-term impact of their posts, the platform can provide a more positive and enjoyable experience for users.
📝 Increases the sense of community: By focusing on the present, the platform's users are more likely to engage in conversations and build relationships, rather than just passively scrolling through old content.
📝 Increases trust and safety: With less personal information and harmful content available, users will feel more secure in using the platform and be more likely to trust the platform with their personal information.
```
In summary, a micro-blogging platform with expiring posts can:
🗹 reduce trust and safety issues by limiting the amount of personal information online, 
🗹 decreasing the potential for cyberbullying and harassment, 
🗹 and improving the overall user experience. 

Additionally, it will increase sense of community and increase trust and safety among users.

What is the hardest challenge for micro-blogging platforms? Monetizing their platform for long terms sustainability and a strong exit strategy?
```
A micro-blogging platform with expiring posts can be great for monetization in several ways:
📎 Increases user engagement: With expiring posts, users are more likely to be active and engaged on the platform, as they have a sense of urgency to view and interact with content before it disappears. This increased engagement can lead to more opportunities for monetization, such as through advertising or sponsored content.
📎 Encourages user-generated content: By limiting the lifespan of posts, the platform can create an environment where users are more likely to create and share new content, rather than just scrolling through old posts. This user-generated content can be monetized through advertising or sponsored content.
📎 Creates a sense of exclusivity: Expiring posts can create a sense of exclusivity and scarcity, making users more likely to engage with the platform and view sponsored content.
📎 Enhances the platform's ability to target ads: An ephemeral platform can enhance the platform's ability to target ads, as the platform can gather data on users' interests, preferences, and conversations that are currently relevant. This allows for more effective and relevant targeting of ads, which can increase the value of the platform for advertisers.
📎 Provides opportunities for in-platform transactions: An ephemeral platform allows for the platform to enable in-platform transactions, such as purchasing access to certain content or exclusive feature, which can be monetized.
```

In summary, a micro-blogging platform with expiring posts can be great for monetization as it:
```
🗹  increases user engagement, 
🗹  encourages user-generated content, 
🗹  creates a sense of exclusivity, 
🗹  enhances the platform's ability to target ads, 
🗹  and provides opportunities for in-platform transactions.
```

All of these features can increase the value of the platform for advertisers and lead to more revenue opportunities.

```
How is Cruddur different from to existing competitors:

🎯 Snapchat has ephemeral features but is focused on being private 1-to-1 or group chat. Snapchat lost trust with users because their private conversations turned out to not be ephemeral. Cruddur is focused on being a public-facing micro blogging platform similar to Twitter
🎯 Twitter is a micro-blogging platform but ephemeral posts have to be implemented through third-party applications and it not how Twitter is used. Twitter had Twittter Stories but removed the feature since it was a bolted on feature as opposed to the whole platform being ephemeral-first.
🎯 Instagram is a platform focused around photo-sharing and while they do have Instagram Stories, an ephemeral feature for posts to expire, its not the primary way of interacting on the platform.

Cruddur will succeed by being a true ephemeral-first micro-blogging platform.

```