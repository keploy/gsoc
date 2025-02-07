# Google Summer of Code'25 Participant Guide

## **Communication**

Welcome to the Keploy GSoC'25 projects page. We encourage candidates to come up with their own project idea. Join our [Slack Channel](https://keploy.slack.com/join/shared_invite/zt-2poflru6f-_VAuvQfCBT8fDWv1WwSbkw) and stay tuned for updates.

Use our **[Template](https://docs.google.com/document/d/1yRWf5pXuUij-UwlXB9knDKqk9VYvV5GrNf865p77Y1U/edit?usp=sharing)** for the proposal. We recommend the use of google docs for the proposal.


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

The goal of this project is to elevate the Keploy Playground by:
1. **Expanding Language Support:** Adding robust support for multiple programming languages such as Java and Python.
2. **Integrating Test & Mock Support:** Providing comprehensive functionalities to generate tests and simulate mocks seamlessly.
3. **Improving User Onboarding:** Redesigning the user experience, especially the onboarding process, to ensure a smooth introduction to Keploy’s capabilities.

**Goals & Ideas**
1. **Interactive Demo Environment:** Build a dynamic playground where users can interact with live demos, generate tests, and see real-time results.
2. **Automated Test Generation from URL Input**: Allow users to provide a URL, then automatically scrape the frontend to generate a sitemap, identify API calls, and create tests based on the discovered endpoints using ATG
3. **Multi-Language Testing Support:** Implement a flexible backend architecture that supports testing across multiple languages, making Keploy a versatile tool for a diverse range of applications.

**Skills Required**
1. Next.js
2. Golang, Java, Python

**Refs**
1. [Keploy Playground](https://keploy.io/playground)
2. [Meshery Playground](https://play.meshery.io)

**Time Estimate** : 350 hours

**Difficulty** : Medium


### 2. Contract Testing - using Keploy
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
1. The goal of this project is to build a PR Agent Dashboard that provides interactive visualizations, metrics, and insights for pull request activities. 
2. The dashboard should support dynamic updates and be backed by a Go web server to process and serve data.
3. Structure the application to be easily extensible, enabling straightforward addition of new metrics or charts in the future.

**Goals & Ideas**
1. Dynamic Dashboard: Develop a frontend that dynamically displays PR-related metrics, using visual elements such as graphs and charts.
2. Template-Based PR Insights: Enable users to create and use templates for PR analysis, allowing customized views for different teams and workflows.
3. Scalable & Modular Design: Ensure the system is modular, allowing for easy integration of new metrics, charts, or data sources.

**Skills Required**
1. React/Next.js, Charting Libraries(e.g., Chart.js, Recharts, D3.js)
2. Golang
3. MongoDB

**Refs**
1. Grafana – For inspiration on dashboard design and real-time data visualization.
2. GitHub API Docs – To fetch and process PR data effectively.
3. Golang 

**Time Estimate** : 350 Hours

**Difficulty** : Medium

### 4. Code Review GitHub App (Using GitHub Action)
**Mentors**: Hermione, Gourav, Yash

**Goals & Ideas:**

1. Develop a GitHub App integrated with GitHub Actions triggering a pipeline on Azure/HyperExecute to provide automated code review feedback, analyzing pull requests for coding style, security vulnerabilities, and best practices.
2. Research about exisiting code review agents and setup a comparison between them by creating a PR using those agents, also create a GitHub Discussion on Keploy displaying the results
3. Read about other open source agents and understand the flow of these agents

**Tasks:**
1. Utilize GitHub API to retrieve PRs, integrate with linting tools like ESLint/Prettier (JavaScript) or GolangCI-Lint (Go), and implement static analysis tools for automated feedback.
2. Create a GitHub App which can triggger a Github Action 

**Skills Required**
1. GitHub Actions & GitHub API
2. REST APIs & Webhooks
3. Golang
4. JavaScript/TypeScript, Node.js
5. Static Code Analysis Tools (ESLint, GolangCI-Lint)

**Refs**
1. [GitHub Actions Documentation](https://docs.github.com/en/actions/) 
2. [GitHub REST API Guide](https://docs.github.com/en/rest?apiVersion=2022-11-28/)
3. [ESLint: Pluggable JavaScript Linter](https://pactflow.io/blog/what-is-contract-testing/)
4. [GolangCI-Lint](https://golangci-lint.run/)

**Time Estimate** : 350 hours

**Difficulty** : Medium 


### 5. Code Indexer

**Mentors**: Shivam, Charan, Sarthak

**Goals & Ideas**
1. Integrate UTG with the RAG indexer.

**Skills Required**
1. Experience with RAG (Retrieval Augmented Generation) architectures.
2. Knowledge of vector databases (e.g., Pinecone, FAISS, Weaviate, etc.).
3. Understanding of graph databases and their integration with AI systems.
4. Familiarity with indexing strategies for efficient code retrieval.
5. Proficiency in Python/Golang for backend development.

**Refs**
1. Research papers on RAG and GRAG models.
2. Documentation for vector and graph databases.

**Tasks** 
1. Integrate the existing RAG bot with a vector database.
2. Explore dynamic indexing techniques to improve efficiency.
3. Research methodologies for leveraging GRAGs to enhance retrieval.
4. Test OSS UTG with OSS Repos.
5. Integrate Gemini with UTG. 

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

**Skills Required**
1. Scripting Languages such as Python, Bash.
2. Golang

**Tasks**
1. Implement Idempotency Check for GET Requests in Postman
2. Denoise the un-expected Parameters (timestamp, headers, token's, change in body response) from Keploy Testcases
3. Create a basic report template using Allure or Extent Reports.

**Time Estimate** : 350 hours

**Difficulty** : Medium
