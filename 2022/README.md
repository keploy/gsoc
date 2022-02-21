# GSoC'22 Participant Guide

## **Communication**

Welcome to the Keploy GSoC projects page. We encourage candidates to come up with their own project idea.

Join our [Slack Channel](https://join.slack.com/t/keploy/shared_invite/zt-12rfbvc01-o54cOG0X1G6eVJTuI_orSA) and stay tuned for updates.

Use our [Template](https://docs.google.com/document/d/1QSSs4vPvn_tPeJkhwDuJ9YLSXdtygob9cPc-5yXj3pY/edit?usp=sharing) for the proposal. We recommend the use of google docs for the proposal.


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

### 1. Keploy Typescript/Javascript SDK 
**Mentors**: Neha Gupta, Ritik Jain, Rajat Sharma.

**Goals & Ideas**
* Create Typescript SDK to enable JS/TS application servers to use the keploy ecosystem similar to the [Go SDK](https://github.com/keploy/go-sdk).
* Create integration framework to easily add routers/web-frameworks or external dependencies similar to the [Go Integrations package](https://github.com/keploy/go-sdk/tree/main/integrations)
* Use the integrations package to add support for top 2 web frameworks/routers, http client, mysql/postgres and mongo support.
* Document the integration for users interested in adding support for more libraries.
* Package and publish the SDK to npm registry.
* Add support for running the SDK through the Mocha or Jest testing frameworks. 
* Create a sample nodejs application server to demonstrate the functionalities of the ts/js SDK.  

**Skills Required**
* Typescript/Javascript
* Rest APIs
* Unit testing

**Refs**
* https://github.com/keploy/go-sdk
* https://jestjs.io
* https://mochajs.org
* https://github.com/keploy/example-url-shortener


### 2. Keploy Java SDK
**Mentors**: Shubham Jain, Ritik Jain, Saurabh Nigam.

**Goals & Ideas**
* Create Java SDK to enable Java application servers to use the keploy ecosystem similar to the [Go SDK](https://github.com/keploy/go-sdk).
* Create integration framework to easily add routers/web-frameworks or external dependencies similar to the [Go Integrations package](https://github.com/keploy/go-sdk/tree/main/integrations)
* Use the integrations package to add support for top 2 web frameworks/routers (likely spring boot and Quarkus), mysql/postgres and mongo support.
* Document the integration for users interested in adding support for more libraries.
* Package and publish the SDK to maven central. 
* Add support for running the SDK through the JUnit testing framework.
* Create a sample spring boot application to demonstrate the functionalities of the Java SDK.

**Skills Required**
* Java
* Rest APIs
* Unit testing

**Refs**
* https://github.com/keploy/go-sdk
* https://junit.org/junit5
* https://github.com/keploy/example-url-shortener

### 3. Autogenerate test cases
Mentors: Shubham Jain, Neha Gupta, Sarthak

**Goals & Ideas**
* Use fuzz testing approach to generate new testcases from existing testcases. We can take inspiration from [Go Fuzzing](https://go.dev/doc/fuzz)
* Define and capture testcases coverage and other useful metrics (KPIs) about the effectiveness of testcases. 
* Avoid adding testcases that don't meaningfully impact any of the testing KPIs.
* Use the API schemas and data types to ensure various potential edge cases are generated. 
* Create a demo application to demonstrate the test case generation capability. 
* Add the feature to generate extra testcases for the keploy server.

**Skills Required**
* Go
* Rest APIs
* Unit testing

**Refs**
* https://go.dev/doc/fuzz
* https://github.com/keploy/keploy/issues/25
* https://github.com/keploy/keploy/issues/24

### 4. Add prioritization to deduplication algorithm
Mentors: Shubham Jain, Neha Gupta

**Goals & Ideas**
* The current deduplication algorithm lacks any kind of prioritization for testcases.
* For highly distributed or complex applications the amount of testcases captured from traffic could make the testcases too noisy. 
* The idea is to prioritize top N testcases based on predefined KPI templates.
* Create a demo application to demonstrate the test prioritization feature.
* Publish benchmark results to show the baseline performances of the deduplication algorithms.

**Skills Required**
* Go
* Rest APIs
* Unit testing

**Refs**
* https://github.com/keploy/keploy/issues/27