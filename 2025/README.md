# Google Summer of Code'25 Participant Guide

## **Communication**

Welcome to the Keploy GSoC'25 projects page. We encourage candidates to come up with their own project idea. Join our [Slack Channel](https://keploy.slack.com/join/shared_invite/zt-2poflru6f-_VAuvQfCBT8fDWv1WwSbkw) and stay tuned for updates.

Use our **[Template](https://docs.google.com/document/d/1QSSs4vPvn_tPeJkhwDuJ9YLSXdtygob9cPc-5yXj3pY/edit?usp=sharing)** for the proposal. We recommend the use of google docs for the proposal.


## **General suggestions and warnings**
_________________

- **Project ideas describe the goals we want to achieve
  but may miss details that have to be defined during the project**:
  we expect students to do their own research, propose solutions and be
  ready to deal with uncertainty and solve challenges that
  will come up during the project

- **Code and prototypes are preferred over detailed
  documents and unreliable estimates**:
  rather than using your time to write a very long
  application document, we suggest to invest in writing a prototype
  (which means the code may be thrown out entirely) which will help you
  understand the challenges of the project you want to work on; your
  application should refer to the prototype or other Github contributions
  you made to Keploy that show you have the capability to succeed in the
  project idea you are applying for.

- **Students who have either shown to have or have shown to be
  fast learners for the required hard and soft skills by
  contributing to Keploy have a lot more chances of being accepted**:
  in order to get started contributing refer to the
  :doc:`Keploy Contributing Guidelines <keploy/keploy/contributing.md>`

- **Get trained in the projects you want to apply for**: once
  applicants have completed some basic training by
  :doc:`contributing to Keploy <keploy/keploy/contributing.md>`
  we highly suggest to start working on
  some aspects of the project they are
  interested in applying: all projects
  listed this year are improvements
  of existing modules so these modules
  already have a list of open issues
  which can be solved as part of your advanced training.
  It will also be possible to complete some of the tasks listed in
  the project idea right now before GSoC starts.
  We will list some easy tasks in the project idea for this purpose.

## **Projects List**

### 1. Enhance Keploy Playground

**Mentors**: Shivam, Tvisha, Manas

**Description**
1.
2.

**Goals & Ideas**
1.
2.

**Skills Required**
1.
2.

**Refs**
1.
2.

**Time Estimate** : 350 hours
**Difficulty** : Medium


### 2. Contract Testing - Multiple services using Keplot
**Mentors**: Gourav, Charan

**Description**: Contract testing is a method focused on verifying interactions between microservices, applications, or systems, ensuring correct communication through predefined contracts. It facilitates early issue identification and reduces complex end-to-end testing needs.

**Goals & Ideas**
1. Keploy Support: Integrate contract testing capabilities into Keploy to enable advanced testing functionalities, enhancing its ability to validate microservice interactions effectively.
2. Automated Change Management for API Chains: When using Keploy with services m1, m2, and m3, consider a scenario where m2 undergoes a change, such as the addition of a new field. When this change is incorporated into m2's test cases, it could potentially disrupt the mock interactions expected by m1, necessitating updates to m1's tests to align with the new behavior. This process ensures that mocks are consistently refreshed to reflect the most current service interactions. Keploy facilitates this dynamic updating mechanism, streamlining the maintenance of test cases and mocks across services. Consequently, it simplifies end-to-end (E2E) testing, making it more efficient and reducing the complexity typically associated with testing interconnected services.

**Skills Required**
1. Golang
2. REST APIs

**Refs**
1. [What is Contract Testing?](https://pactflow.io/blog/what-is-contract-testing/)
2. [Keploy Documentation](https://keploy.io/docs/)
3. [What is a REST API? - IBM](https://www.ibm.com/topics/rest-apis#:~:text=the%20next%20step-,What%20is%20a%20REST%20API%3F,representational%20state%20transfer%20architectural%20style.)
4. [A Tour of Go](https://go.dev/tour/)

**Time Estimate** : 350 hours
**Difficulty** : medium 

### 3. GitHub App Dashboard with Metrics and Chart
**Mentors**: Manas, Tvisha, Hermione

**Description**
1.
2.

**Goals & Ideas**
1.
2.

**Skills Required**
1.
2.

**Refs**
1.
2.

**Time Estimate** : 350 Hours
**Difficulty** : Medium

### 4. Code Review GitHub App (Using GitHub Action)
**Mentors**: Hermione, Gourav, Yash

**Goals & Ideas:**
1. 
2.

**Skills Required**
1. 
2.

**Refs**
1. 
2.

**Time Estimate** : 350 hours
**Difficulty** : Medium 


### 5. Code Indexer

**Mentors**: Shivam, Charan, Sarthak

**Goals & Ideas**
1.
2.

**Skills Required**
1.
2.

**Refs**
1.
2.

**Time Estimate** : 350 hours
**Difficulty** : Medium


### 6. TestSuite Idempotency Checker

**Mentors**: Animesh, Sarthak

**Description**: Ensuring idempotency in test suites is crucial for reliable and repeatable testing. This project focuses on analyzing test cases to identify operations that should be idempotent, it will help in detecting noisy parameters and inconsistencies which may lead to flaky tests.

**Goals & Ideas**
1. Identify Noisy Parameters – Automatically detect parameters in test cases that cause unnecessary variations, leading to non-idempotent behavior.
2. Validate CRUD Operations – Ensure that CRUD requests in test cases conform to idempotency rules by verifying their consistency across multiple executions.
3. HTML-based Test Verification – Check test cases that interact with HTML responses to ensure stable outputs and prevent unintended failures.
4. Automated Idempotency Reporting – Develop a reporting mechanism that flags test cases violating idempotency, with insights into potential fixes.

**Tasks**
1. Implement Idempotency Check for GET Requests in Postman
2. Denoise the un-expected Parameters (timestamp, headers, token's, change in body response) from Keploy Testcases
3. Create a basic report template using Allure or Extent Reports.

**Skills Required**
1.Scripting Languages

**Time Estimate** : 350 hours
**Difficulty** : Hard
