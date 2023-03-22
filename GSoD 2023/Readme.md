# WELCOME TO KEPLOY

Hello! We are thrilled to announce that **Keploy** will be applying as a **GSoD** mentoring org for 2023! We are excited to welcome all technical writers to apply for contributing towards ***Keploy's Docs*** during this season! We love mentoring folks and help them get involved in the field of Open Source, tech and docs. If Keploy gets accepted for `GSoD 2023`, we would create task lists and basis of that select folks to contribute during the period. And even without `GSoD`, we always welcome folks to get involved ❤️!

**Keep an eye out on this page as we update with more project ideas.**


## Table of Contents:

* [About Keploy](#about-keploy)
* [About GSoD](#about-gsod)
* [Keploy's Participation](#keploy's-participation)
* [Projects](#projects)
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

1. Work on [Good First Issues](https://github.com/keploy/docs/issues).

    1.1 Review the list of Good First Issues in the project's repository and select the issues you want to work on.

    1.2 Set up the development environment by cloning the repository and ensuring that the project builds and runs locally.

    1.3 Connect with mentors or community members for guidance and support during the development process. This can include asking questions, seeking feedback, or pair programming.


2. Work on sample app creation for various integrations that Keploy offers. This would include creating sample apps and documenting how they work with sample test case and mock gnerations and test results. Here are a few ideas for some sample apps:
    2.1 https://github.com/keploy/keploy/issues/422
    2.2 https://github.com/keploy/keploy/issues/420
    2.3 https://github.com/keploy/keploy/issues/423
    2.3 https://github.com/keploy/keploy/issues/421
    2.5 https://github.com/keploy/keploy/issues/414
    2.6 https://github.com/keploy/keploy/issues/417
    2.7 https://github.com/keploy/keploy/issues/425

    You are also free to suggest sample apps on your own! You can refer to [this](https://github.com/keploy/samples-go/tree/main/echo-sql) to understand how to document your sample app.


3. Add 'Supported JWT Middlewares' to [Go Docs](https://github.com/keploy/docs/tree/main/docs/go). The reference can be taken from https://pkg.go.dev/github.com/keploy/go-sdk#readme-supported-jwt-middlewares and you can add the same to the Go Docs in the docs repo.

4. Improve Contribution Guide for Keploy SDK. 
Currently, the conrtibution guide for Keploy's SDK just has a video refernce to Keploy and an HLD for Java. 
You can take reference from the exisitng video and diagrams and construct a guided contribution guide based for the [SDK repo](https://github.com/keploy/keploy).



**Keep an Eye Out 👀 as we add more Projects! We would be happy to review any ideas that you may have to improve our docs!**

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

## Community

Join the Keploy community and connect with mentors and other members through our Slack channel. 

[![Join Keploy on Slack!](https://img.shields.io/badge/Join%20Us%20On-Slack-orange)](https://keploy.slack.com/)
 
Follow us on Twitter and LinkedIn to stay up-to-date with the latest news and announcements:

[![Twitter Follow](https://img.shields.io/twitter/follow/keploy?style=social)](https://twitter.com/keployio)

[![LinkedIn Follow](https://img.shields.io/badge/Connect%20On-LinkedIn-blue)](https://www.linkedin.com/company/keploy/)

You can also reach out to us via email at info@keploy.com.

We look forward to hearing from you and helping you get involved with the Keploy community!

## Code Of Conduct
Contributors to this project are expected to conduct themselves in a respectful way.
See the [CNCF Community Code of Conduct](https://github.com/cncf/foundation/blob/master/code-of-conduct.md) as a reference.

