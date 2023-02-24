# GSoC'23 Participant Guide

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

### 1. Keploy CLI Refactoring 
**Mentors**: Neha Gupta, Ritik Jain

**Goals & Ideas**
* Add support for `Get` curl command for the test case.
* Add support to `Run` individual test case.
* On the CLI add a vertical line separator to show differences in the test cases 
(show complete tests info on both sides, only highlight differences with different color)
* Add support for commands in Keploy CLI, for eg: `show [test_id];` will 
show that specific test case among various testcases, `show [test_run_id];` will show the info related to it.
* Rename test files and mock files to method_endpoint.
* Add comment to keploy generated test file and mocks basically Kmocks and Ktests.

**Skills Required**
* Golang
* Rest APIs

**Refs**
* https://github.com/keploy/keploy
* https://github.com/keploy/example-url-shortener
* https://docs.keploy.io/docs/devtools/server-contrib-guide
* https://docs.keploy.io/

**Time Estimate** : 175 hours

**Difficulty** : Medium


### 2. Keploy Java SDK
**Mentors**: Sarthak Shyngle, Gourav Kumar, Charan Kamarapu.

**Goals & Ideas**
* Add support for `MongoDB` database.
* Add support for `Apache Kafka`.
* Add support for java Native HttpClient.
* Add support for `RabbitMQ`.
* Add support for `Google Cloud Platform` & `Azure` SDKs. 

**Skills Required**
* Java
* Rest APIs
* Unit testing

**Refs**
* https://github.com/keploy/java-sdk
* https://github.com/keploy/go-sdk
* https://github.com/keploy/samples-java
* https://junit.org/junit5
* https://github.com/keploy/example-url-shortener
* https://docs.keploy.io/

**Time Estimate** : 350 hours

**Difficulty** : Medium

### 3. Keploy Typescript/Javascript SDK
**Mentors**: Charan Kamarapu, Ritik Jain, Shubham Jain.

**Goals & Ideas**
* Add support for `Httpclients` in typescript. 
    - This sdk currently supports `node-fetch` httpClient, to support other httpclients like `axios`, `http`, etc. You can take the 1st ref below which intercepts other popular httpClients.
* Add support for popular `Sql` databases. For eg: `PostgreSQL`, `MySQL`, etc. By adding support for `Sequelize`.
* Add support for `MongoDB` database.
* Add support for `Amazon S3`, `DynamoDB`, `Azure Blob Storage`, and `Google Cloud Storage` using the HTTP Client.
* Add support for `Redis` & `Elasticsearch`.


**Skills Required**
* Typescript/Javascript
* Rest APIs
* Unit testing

**Refs**
* https://www.npmjs.com/package/@mswjs/interceptors
* https://sequelize.org/
* https://github.com/keploy/go-sdk
* https://jestjs.io
* https://mochajs.org
* https://github.com/keploy/example-url-shortener
* https://docs.keploy.io/

**Time Estimate** : 350 hours

**Difficulty** : Hard

### 4. Autogenerate test cases
Mentors: Shubham Jain, Neha Gupta, Sarthak, TBD

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
* https://docs.keploy.io/

**Time Estimate** : 175 hours

**Difficulty** : Medium

### 5. Time Simulation in Java SDK
Mentors: Sarthak Shyngle, Gourav Kumar, Animesh Pathak

**Goals & Ideas**
* To capture time based tokens like jwt and recreate that session during test-mode (Already implemented for go-sdk).
* Basically record the time and save it with testcase in form of yamls.
* Identify the methods which mainly return Time object used inside JSON Web Tokens (JWTs).
* Override the Time object to return the recorded time at the time of test run by reading it from testcases which will mock time which was set to be expired. 
* Create a demo application which uses jwt token based authentication . 
* It will good if there are minimum changes required in user API for that runtime ASM instrumentation libraries like bytebuddy can be used.

**Skills Required**
* Java
* Rest APIs
* Unit testing

**Refs**
* https://github.com/keploy/java-sdk
* https://github.com/keploy/samples-java
* https://junit.org/junit5
* https://github.com/keploy/go-sdk
* https://www.baeldung.com/java-json-web-tokens-jjwt

**Time Estimate** : 175 hours

**Difficulty** : Medium
