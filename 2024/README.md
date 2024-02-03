# Google Summer of Code'24 Participant Guide

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

### 1. Add support for macOS native networking - code from mitmproxy
**Mentors**:

**Goals & Ideas**

**Skills Required**

**Refs**

**Time Estimate** : 

**Difficulty** :

**Task List** : 
| S.No | Tasks | Repo | Actionable By | 
|------|-------|-----------|-----------|
|      |       |       |            |

### 2. denoising + docker extension
**Mentors**:

**Goals & Ideas**

**Skills Required**

**Refs**

**Time Estimate** : 

**Difficulty** :

**Task List** : 
| S.No | Tasks | Repo | Actionable By | 
|------|-------|-----------|-----------|
|      |       |       |            |

### 3. Multiple services using keploy (API chaining)
**Mentors**:
[Gourav Kumar](https://github.com/gouravkrosx)

**Description**
- In Keploy, testing multiple services via API chaining emphasizes enabling contract testing to ensure seamless interactions among services. This ensures that all communications across services meet predefined expectations, enhancing the reliability of interconnected systems.
- Contract testing is a method focused on verifying interactions between microservices, applications, or systems, ensuring correct communication through predefined contracts. It facilitates early issue identification and reduces complex end-to-end testing needs.

**Goals & Ideas**
1. Keploy Support: Integrate contract testing capabilities into Keploy to enable advanced testing functionalities, enhancing its ability to validate microservice interactions effectively.
2. One-Go Testing: Implement functionality within Keploy for recording tests and mocks for all related microservices simultaneously. This feature would capture both ingress and egress traffic, utilizing process identification (PID) for filtering. The primary goal is to ensure that tests and mocks remain synchronized across all services, thereby maintaining consistency and accuracy in testing environments.
3. Automated Change Management for API Chains: When using Keploy with services m1, m2, and m3, consider a scenario where m2 undergoes a change, such as the addition of a new field. When this change is incorporated into m2's test cases, it could potentially disrupt the mock interactions expected by m1, necessitating updates to m1's tests to align with the new behavior. This process ensures that mocks are consistently refreshed to reflect the most current service interactions. Keploy facilitates this dynamic updating mechanism, streamlining the maintenance of test cases and mocks across services. Consequently, it simplifies end-to-end (E2E) testing, making it more efficient and reducing the complexity typically associated with testing interconnected services.
4. Both HTTP test and HTTP mock share the same [spec](https://github.com/keploy/samples-go/blob/main/gin-redis/keploy/test-set-0/tests/test-1.yaml).

**Skills Required**
1. Golang
2. REST APIs
3. Contract Testing
4. E2E Testing

**Refs**
1. [What is Contract Testing?](https://pactflow.io/blog/what-is-contract-testing/)
2. [Keploy Documentation](https://keploy.io/docs/)
3. [What is a REST API? - IBM](https://www.ibm.com/topics/rest-apis#:~:text=the%20next%20step-,What%20is%20a%20REST%20API%3F,representational%20state%20transfer%20architectural%20style.)
4. [A Tour of Go](https://go.dev/tour/)

**Time Estimate** : 350 Hours

**Difficulty** : Medium

**Task List** : 
| S.No | Tasks | Repo | Actionable By | 
|------|-------|-----------|-----------|
|      |       |       |            |

### 4. vs code and other editors extension
**Mentors**:

**Goals & Ideas**

**Skills Required**

**Refs**

**Time Estimate** : 

**Difficulty** :

**Task List** : 
| S.No | Tasks | Repo | Actionable By | 
|------|-------|-----------|-----------|
|      |       |       |            |


### 5. Add support for Windows native
**Mentors**:

**Goals & Ideas**

**Skills Required**

**Refs**

**Time Estimate** : 

**Difficulty** :

**Task List** : 
| S.No | Tasks | Repo | Actionable By | 
|------|-------|-----------|-----------|
|      |       |       |            |
