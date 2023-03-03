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
**Mentors**: Neha Gupta, Ritik Jain, Sanskriti Harmukh, Ankit Kumar

**Goals & Ideas**
* Add support for `Get` curl command for the test case.
* Add support to `Run` individual test case.
* Add support for commands in Keploy CLI, for eg: `show [test_id];` will 
show that specific test case among various testcases, `show [test_run_id];` will show the info related to it.
* Rename test files and mock files to method_endpoint.
* Add comment to keploy generated test file and mocks basically KMocks and KTests.
* Pipe the server logs from SDK to Keploy Server. (Ritik to make GFI)
* Add the static link to serve the test report genenerated at end of log.

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


**Task List** : 

| Tasks | Repo | Actionable By | <GitHub_ID> |
|-------|-----------|-----------|-----------|
|  Setup Keploy Locally with a Sample Go Application      |      Samples-go     |           |          <PR_ID>|  
|  Use Keploy to increase test cases coverage      |  Keploy         |    [ISSUE LINK](https://github.com/keploy/keploy/issues/333)     |           |           |
|  Add a vertical line separator in CLI   |       Keploy    |      [ISSUE LINK](https://github.com/keploy/keploy/issues/334)   |           |           |
|  Add support for `Get TC` to display test-cases from yaml   |    Keploy     |    [ISSUE LINK](https://github.com/keploy/keploy/issues/337)     |           |           |
|  Update Keploy UI with new way of working Keploy    |    UI     |    [ISSUE LINK](https://github.com/keploy/keploy/issues/335)    |           |           |

### 2. Keploy Java SDK
**Mentors**: Sarthak Shyngle, Gourav Kumar, Charan Kamarapu, Barkatul Mujauddin.

**Goals & Ideas**
* Add support for `MongoDB` database.
* Add support for `Apache Kafka`.
* Add support for java Native HttpClient.
* Add support for `RabbitMQ`.
* Add support for `Google Cloud Platform` & `Azure` SDKs. 
* Add Mock Library `Redis` and `KSQL` Support.

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

**Task List** : 

| Tasks | Repo | Actionable By | <GitHub_ID> |
|-------|-----------|-----------|-----------|
|  Setup Keploy Locally with a Sample Java Application (Use as many dependencies you can)    |    Samples-Java       |           |      <PR_ID>|     |
|  Create a github action for running java based linters in pipeline     |    Java-SDK       |   [ISSUE LINK](https://github.com/keploy/java-sdk/issues/129)        |           |
|  Create a github action for publishing sdk to maven central    |    Java-SDK         |     [ISSUE LINK](https://github.com/keploy/java-sdk/issues/127)       |           |
|  Write the test-cases for JAVA-SDK (for Integrations)     |    Java-SDK     |    [ISSUE LINK](https://github.com/keploy/java-sdk/issues/131)   |           |           |
| Creating Sample Java Application using JWT Token         |   Java-SDK   |     [ISSUE LINK](https://github.com/keploy/samples-java/issues/34)      |           |
| Creating Interceptors and Advice for different jwt objects   |   Java-SDK   |    [ISSUE LINK](https://github.com/keploy/java-sdk/issues/132)      |           |           |


### 3. Keploy Typescript/Javascript SDK
**Mentors**: Charan Kamarapu, Ritik Jain, Shubham Jain, Nishant Mishra, Diganta Kr Banik.

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

**Task List** : 

| Tasks | Repo | Actionable By | <GitHub_ID> |
|-------|-----------|-----------|-----------|
| Setup Keploy Locally with a Sample TS Application   |    Samples-Typescript       |           |     <PR_ID>      |
| Empty response for node-fetch http call     |    Typescript-SDK       |     [ISSUE LINK](https://github.com/keploy/typescript-sdk/issues/49)        |           |           |
| Linting action is failing in CI of TS-SDK       |    Typescript-SDK       |       [ISSUE LINK](https://github.com/keploy/typescript-sdk/issues/50)     |           |           |
| Add a sample unit test for mocking/stubbing calls in unit-tests      |     Samples-Typescript      |      [ISSUE LINK](https://github.com/keploy/samples-typescript/issues/10)     |           |           |
| Write the test-cases for TS-SDK (for Integrations)       |     Typescript-SDK      |      Ritik (To Create GFI)    |           |           |
| Add check to not record testcases during test mode | Typescript-SDK | [ISSUE LINK](https://github.com/keploy/typescript-sdk/issues/42) | | |
| Add log statement in keploy and mock module to log mode | Typescript-SDK | [ISSUE LINK](https://github.com/keploy/typescript-sdk/issues/45) | [#45](https://github.com/keploy/typescript-sdk/pull/48) | |
| Remove cp cmd from build script | Typescript-SDK | [ISSUE LINK](https://github.com/keploy/typescript-sdk/issues/51) | [#51](https://github.com/keploy/typescript-sdk/pull/53) | |
| Add filter for headers during recording | Typescript-SDK | [ISSUE LINK](https://github.com/keploy/typescript-sdk/issues/44) | | |

### 4. Autogenerate test cases
Mentors: Shubham Jain, Neha Gupta, Sarthak, Jyotirmoy Roy, Pranshu Srivastava

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

**Task List** : 
| Tasks | Repo | Actionable By | <GitHub_ID> |
|-------|-----------|-----------|-----------|
| Create a REST-Api in Golang using any router and one database supported by Keploy                 |           |     [Issue Link](https://github.com/keploy/samples-go/issues/40)      |      <PR_ID>     |  
| Short list different ideas to generate more than one testcase using api schema and response provided |           |       [Issue Link](https://github.com/keploy/keploy/issues/338)    |           |      
| Add Go-fuzz tests for the application created                                               |           |    [Issue Link](https://github.com/keploy/samples-go/issues/40)       |           | 
|     TBA more      |           |     Shubham (To be Added)      |           | 

### 5. eBPF based Keploy Integration
Mentors: Shubham Jain, Sarthak Shyngle, Gourav Kumar, Animesh Pathak

<!--
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
-->
