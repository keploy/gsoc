## Google Season Of Docs Proposal : Optimizing Go Repo User Experience: Improving JWT Middleware Documentation and SDK Contribution Guide
<hr/>

# WELCOME TO KEPLOY

Hello! We are thrilled to announce that **Keploy** will be applying as a **GSoD** mentoring org for 2023! We are excited to welcome all technical writers to apply for contributing towards ***Keploy's Docs*** during this season! We love mentoring folks and help them get involved in the field of Open Source, tech and docs. If Keploy gets accepted for `GSoD 2023`, we would create task lists and basis of that select folks to contribute during the period. And even without `GSoD`, we always welcome folks to get involved ❤️!

**Keep an eye out on this page as we update with more project ideas.**


## Table of Contents:

* [About Keploy](#about-keploy)
* [About GSoD](#about-gsod)
* [Keploy's Participation](#keploys-participation)
* [Projects](#projects)
* [Project Scope](#project-scope)
* [Measuring Project's Success](#measuring-projects-success)
* [Timeline](#timeline)
* [Project Budget](#project-budget)
* [Proposal Format](#proposal-format)
* [Community](#community)
* [Code Of Conduct](#code-of-conduct)

## About Keploy

Keploy is a functional testing toolkit for developers. It generates E2E tests for APIs (KTests) along with mocks or stubs(KMocks) by recording real API calls. KTests can be imported as mocks for consumers and vice-versa.

Merge KTests with unit testing libraries(like Go-Test, JUnit..) to track combined test-coverage.

KMocks can also be referenced in existing tests or use anywhere (including any testing framework). KMocks can also be used as tests for the server.

You can read more about Keploy from [here](https://docs.keploy.io/docs/keploy-explained/introduction).

## About GSoD
Google Season of Docs (GSoD) is a unique program that brings together technical writers and open source communities to work collaboratively on improving project documentation. It is an initiative by Google that aims to improve the state of documentation within the open source community.

During the program, technical writers are paired with open source communities that are looking to enhance their documentation. The writers collaborate with community mentors to identify areas of improvement, document new features, and provide better explanations of existing features. The program encourages collaboration and communication between technical writers and community members, fostering a strong relationship between the two.

GSoD provides an opportunity for open source communities to benefit from the skills and expertise of technical writers, who bring a fresh perspective to the project. Technical writers, in turn, gain valuable experience in open source software development and contribute to the greater good of the community.

The program runs for several months, during which time technical writers work closely with community members to complete documentation tasks. The ultimate goal is to improve the documentation of the project, making it more accessible to users and developers alike. Overall, GSoD helps to create a more vibrant and thriving open source community by promoting collaboration, improving documentation, and enhancing the user experience.

You can read more about Google Season Of Docs [here](https://developers.google.com/season-of-docs). 

## Keploy's Participation

We at Keploy believe that clear and comprehensive documentation is essential to the success of any open source project, as it helps users understand the project's features and functionalities, and how to contribute to it. Given Keploy is a developer tool, it becomes all the more essential to have a clear and concise documentation so that developers and testers can easily understand Keploy's core principals and can integrate and work with Keploy with ease. A better documentation becomes ever more important for us as we have a number of integrations and would definitely not want any developer or tester to sit back and keep scratching their heads to make Keploy work (not that it presently the case, but still better documentation is always better, right😅?)

We look to participate in Google Season of Docs (GSoD) because we recognize the value of technical writing as a critical aspect of the development process. By engaging with technical writers, we can benefit from their expertise and collaborate on improving our documentation, making it more user-friendly and accessible to a wider audience.

At Keploy, we believe that open source is more than just a software development model; it's a community-driven approach to building software. We see GSoD as an opportunity to strengthen our community by fostering collaboration between technical writers and Keploy community members. This will not only enhance our documentation but also help create a welcoming and inclusive environment that encourages contributions from all kinds of contributors.

In summary, participating in GSoD aligns with our values of open source, community engagement, and accessibility. We believe that working with technical writers will enhance our documentation, improve the user experience, and build a stronger community around our project. ***We are excited and hope to be part of this program and look forward to collaborating with technical writers to make Keploy an even better testing framework✨!***


## Projects

1. <b>Improve Documentation For Keploy SDK and Go Documentation</b>: 
    1.1 <b>Add References Page for Keploy Variables</b>. 
    Currently, the guide for Keploy's SDK just has no references to the Variables that user can set in addition to ``KEPLOY_MODE``. These Variables are mentioned under configs in [Server Code](https://github.com/keploy/keploy/blob/f9e65515e65a58dd18572564610cb41c55ee8de5/server/server.go#L53).
    1.2 <b>How Keploy handles authentication and authorization</b> - Add 'Supported JWT Middlewares' to [Go Docs](https://github.com/keploy/docs/tree/main/docs/go). The reference can be taken from https://pkg.go.dev/github.com/keploy/go-sdk#readme-supported-jwt-middlewares and you can add the same to the Go Docs in the docs repo.
    1.3 <b>Add to Documentation how to generate Mocks with generating test case</b> - Keploy supports mock generation without generating test cases. Currently this feature is not documented anywhere in the docs. You need to document this feature, also explaining its advantages (use case scenarios) and the process to achieve3. it.
    1.4 <b>Blog</b>:Write a blog on Mocks vs Stubs vs Real data (Real Database)
    1.5 <b>Blog</b>: How much assertions is good assertion?
   <i> Mentors: Sanskriti Harmukh, Diganta Kr Banik and Animesh Pathak</i>

2. <b>Improve Contribution Guide for Keploy SDK</b> - 
2.1 Currently, the contribution guide for Keploy's SDK just has a video refernce to Keploy and a HLD for Java. 
You can take reference from the exisitng video and diagrams and construct a guided contribution guide based for the [SDK repo](https://github.com/keploy/keploy).
<b>We also would like you to add readmes/guides/guides/blogs for the following topics</b>:
2.2 Add Adding test coverage to Keploy to Keploy's Contribution Guide
2.3 Adding Keploy Support for eBPF version of Keploy(both Readme as well as Docs)
2.4 Migration Guide from Keploy V1 to V2.
2.5 Blog on E2E vs Unit Testing (especially aimed for advanced developers)
2.6 Blog on Test Driven Development vs Behaviour Driven Development and how Keploy works with both.
<i>Mentors: Ankit Kumar and Jyotirmoy Roy</i>

3. <b> Add blogs, documentation and videos to educate developers around testing with Keploy</b><!-- We expect to improve developer experience and help developers understand how Keploy improves the process as well as the results (including code coverage) for testing. We aim to achive this by educating developers about current testing scenarios that would not only help experienced developers but also developers who are starting out with testing tools. We have jotted a few blog ideas down but would be open to more ideas from technical writers: -->
3.1 Karate vs REST-Assured vs Keploy
3.2 Adding documentation for integrating and adding to DSL version of Keploy
3.3 We expect the selected technical writer to make a video on how Keploy functions (would be better if animated) as it would help users understand more easily how Keploy works. 
<i>Mentors:  Ankit Kumar, Jyotirmoy Roy, Sanskriti Harmukh, Diganta Kr Banik and Animesh Pathak</i>
**Keep an Eye Out 👀 as we add more Projects! We would be happy to review any ideas that you may have to improve our docs!**

## Project Scope

<!-- 1. <b>Scope for Adding 'Supported JWT Middlewares' to Go Docs</b>: The project would  explain the integration , which is lacking in case of the original doc in pkg.go.dev. Out of scope for this would include simply copying the entire documentation from pkg.go.dev and adding it to our docs.

2. <b>Scope for improving contribution guide for Keploy SDK</b>: The scope includes a detailed guide to install Keploy on local machine and then tackle the issue to be solved (step by step guide would also include what problems one might face while setting up the environment and known methods to tackle the common errors). Out of Scope for this project would include adding more video content to explain the working of the SDK. -->

1. <b>Improve Documentation For Keploy SDK and Go Documentation</b>: The project aims to improve the documentation for Keploy SDK and Go documentation. The specific tasks that can be undertaken as part of the project are:
    - Adding a References page for Keploy Variables: The objective is to create a new page in the Keploy SDK guide that lists all the Keploy variables that can be set in addition to KEPLOY_MODE, along with a brief description of each.
    - Adding Supported JWT Middlewares to Go Docs: The objective is to create a new page in the Go documentation that lists the JWT middlewares that Keploy supports, along with a brief description of each.
    - Adding Documentation for Mock Generation: The objective is to create a new section in the Keploy SDK guide that explains the process for generating mocks in Keploy <i>without recording test cases</i>, along with its advantages and use cases.
    - Writing a Blog on Mocks vs Stubs vs Real Data: The objective is to write a blog post that explains the differences between mocks, stubs, and real data, along with the pros and cons of each approach and when to use each one.
    - Writing a Blog on Good Assertion Practices: The objective is to write a blog post that provides tips for writing effective assertions in unit tests, along with examples and use cases.

2. <b>Improve Contribution Guide for Keploy SDK</b>: The project aims to improve the contribution guide for Keploy SDK and add new documentation to the SDK repo. The specific tasks that can be undertaken as part of the project are:
    - Improving the Contribution Guide: The objective is to create a new contribution guide that is comprehensive and includes detailed instructions on how to contribute to Keploy SDK.
    - Adding Test Coverage to Keploy's Contribution Guide: The objective is to add a new section to the contribution guide that explains how to add test coverage to Keploy SDK.
    - Adding eBPF Support to Keploy: The objective is to add a new readme and documentation to the Keploy SDK that explains how to use eBPF with Keploy. 
    - Migration Guide from Keploy V1 to V2: The objective is to create a new migration guide that explains how to migrate from Keploy V1 to V2. 
    - Blog on E2E vs Unit Testing: The objective is to write a blog post that explains the differences between end-to-end testing and unit testing, and when to use each approach. The post should include examples and use cases, and should be aimed towards advanced users.
    - Blog on Test Driven Development vs Behavior Driven Development: The objective is to write a blog post that explains the differences between test-driven development and behavior-driven development, and how Keploy can be used to support both approaches. The post should include examples and use cases, and provide tips for using Keploy in a TDD or BDD workflow.

3. <b> Add blogs, documentation and videos to educate developers around testing with Keploy</b>: The scope for the third idea includes:
    - Karate vs REST-Assured vs Keploy: The objective is to write a blog post that compares the three testing frameworks Karate, REST-Assured, and Keploy, highlighting their differences and advantages. The post should include examples and use cases for each framework.
    - Adding documentation for integrating and adding to DSL version of Keploy: The objective is to add new documentation to the Keploy SDK that explains how to integrate and add to the domain-specific language (DSL) version of Keploy.
    - Video on how Keploy works: The objective is to create an animated video that explains how Keploy works, including its architecture, main components, and how it can be used for testing and deployment. The video should be informative and engaging, and should help users understand the key features and benefits of Keploy.

## Measuring Project's Success
We will measure the success of projects in two halves. 
Firstly, we will use git's workflow issue(if technical writers want to add any) followed by pull requrest followed by discussions on the pull request and then finally merging. 
For the second half, we will try to get user reviews as to if they found the changes helpful and if they were able to get their tasks done following the documenttion. To do this we would leverage our slack channel and try to get reviews from our users.

## Timeline

The project considering the three ideas, on a whole is expected to be completed within four months. The first few weeks would be used to help the technical writers get accustomed with Keploy and understand what Keploy does so that they can use the information while preparing and updating the documentations. Once the technical writers are selected for our project, we expect them to suggest a timeline within which they expect to complete their tasks.

## Project Budget
If our project proposal is accepted, we will have seven mentors who will work across all three project ideas. In order to support our team, we would like to request a total grant of USD 14000 from Google. We plan to distribute USD 4500 of this grant among the technical writers working on each project, and allocate an additional USD 500 towards awarding swags to the technical writers as a token of appreciation.

| Budget item      | Total Amount (in USD) | 
| ---------------- | --------------- |
| Technical Writer achieves the task of improving Documentation For Keploy SDK and Go Documentation| 4500|
| Technical Writer achieves the task of improving Contribution Guide for Keploy SDK | 4500         |
|Technical writer adds blogs, documentation and videos to educate developers around testing with Keploy | 4500 |
| Swags/T-Shirts   | 500             |
| TOTAL            |     14000          |


### Proposal Format
A Google Season Of Docs usually consists of a Statement Of Interest. Your Statement Of Interest should generally contain about 1,000 words (**But don't consider this as a constraint**). Here's a guide of what you can include in your Statement Of Interest:

1. Introduction: Introduce yourself and your background. Explain your interest in participating in the GSoD program and what you hope to gain from it.
2. Project Description: Provide a brief description of the project you want to work on. Include the project goals, technologies involved, and any relevant information that will help the selection committee understand the project's scope.
3. Relevant Experience: Highlight any relevant experience you have in the project's domain or technical writing/documentation. Describe past contributions to similar projects and provide links to relevant work.
4. Proposed Plan: Explain your proposed plan for completing the project within the given timeline. Outline the steps you will take to achieve the project goals and how you will collaborate with the project team and mentor.
5. Impact: Describe how your project will benefit the community and users of the technology. This can include improving the quality of documentation, increasing accessibility, or adding new features.
6. Proposed Total Budget: If applicable, provide an estimated budget for completing the proposed project, including any necessary resources or tools.
7. Conclusion: Summarize your statement of interest and express your enthusiasm for the project.

You can also go through [GSoD Tech Writer Guide](https://developers.google.com/season-of-docs/docs/tech-writer-guide) and [Creating a Statement of Interest](https://developers.google.com/season-of-docs/docs/tech-writer-statement) to get a better idea of how to construct your Statement of Interest. But remember, at the end of the day, this is just a suggestive list. ***Do add your creativity and provide us with any other information that you feel we should know!***

## About Mentors

Our mentors Animesh Pathak, Sanskriti Harmukh, Ankit Kumar, Diganta Kr Banik, and Jyotirmoy Roy are also members of this year's `Google Summer Of Code`. Keploy is one of the projects that has been selected under `GSoC 2023` and we hope that we can provide participants seemless experience during the event. We also hope to follow our GSoC Success and participate in this year's `Google Season Of Docs`.
## Community

Join the Keploy community and connect with mentors and other members through our Slack channel. 

[![Join Keploy on Slack!](https://img.shields.io/badge/Join%20Us%20On-Slack-orange)](https://keploy.slack.com/)
 
Follow us on Twitter and LinkedIn to stay up-to-date with the latest news and announcements:

[![Twitter Follow](https://img.shields.io/twitter/follow/keploy?style=social)](https://twitter.com/keployio)

[![LinkedIn Follow](https://img.shields.io/badge/Connect%20On-LinkedIn-blue)](https://www.linkedin.com/company/keploy/)

You can also reach out to us and submit your Statement Of Interests via email at support@keploy.io.

We look forward to hearing from you and helping you get involved with the Keploy community!

## Code Of Conduct
Contributors to this project are expected to conduct themselves in a respectful way.
See the [CNCF Community Code of Conduct](https://github.com/cncf/foundation/blob/master/code-of-conduct.md) as a reference.

