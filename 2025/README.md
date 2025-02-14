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

### 1. AI-Powered Open-Source Code Review Agent (Using any CI/CD workflow)
**Mentors**: Hermione, Gourav, Yash, Shubham

Develop an AI-driven, open-source code review agent that integrates with version control platforms and CI/CD pipelines to provide automated feedback on coding style, security vulnerabilities, and best practices. Use any CI/CD runners and open-source static analysis tools to improve the developer experience in open-source projects.

**Goals & Ideas:**

1. Develop a application integrated that can be integrated to CI/CD workflows triggering a pipeline on GCP/HyperExecute to provide automated code review feedback, analyzing pull requests for coding style, security vulnerabilities, and best practices.
2. Utilize version control APIs (such as Git-based platforms) to retrieve code changes, integrate with linting tools like ESLint/Prettier (JavaScript) or GolangCI-Lint (Go), and implement AI/ML-based static analysis for automated feedback.
3. Train an AI/ML model on public open-source repositories to identify common coding issues and suggest improvements. Use Google's Vertex AI or an open-source ML model like CodeBERT, DeepSeek, Ollama to provide AI-powered code reviews.
4. Web dashboard for analytics and insights.

**Tasks:**
1. Explore the architecture and workflows of various open-source code review systems to understand their impact and areas for improvement and build a matrix comparing them based on features such as accuracy, language support, ease of integration, and performance
2. Build a modular webhook-based system to allow easy integration with various platforms.
3. Integrate OWASP Dependency-Check or Google’s Open Source Insights (deps.dev API) to detect vulnerable dependencies.
4. Export review results in JSON, Markdown, or PDF formats for offline analysis.

**Skills Required:**
- CI/CD workflows & automation
- REST APIs & Webhooks
- Golang
- JavaScript/TypeScript, Node.js
- Static Code Analysis Tools (ESLint, GolangCI-Lint)
- AI/ML for automated code review - Vertex AI (Optional but beneficial)

**Refs**
1. [ESLint: Pluggable JavaScript Linter](https://pactflow.io/blog/what-is-contract-testing/)
2. [GolangCI-Lint](https://golangci-lint.run/)

**Time Estimate** : 350 hours

**Difficulty** : Hard

### 2. OSS Code Indexer for Efficient Retrieval

**Mentors**: Shivam, Charan, Sarthak, Shubham Jain

**Goals & Ideas**
Develop an efficient code indexing system that enables fast and scalable code search and retrieval. The system will integrate  open source unit test geneartion with a Retrieval-Augmented Generation (RAG) indexer, utilizing vector and graph databases to improve query efficiency and relevance. The goal is to create a robust and scalable solution that can handle large open-source codebases and enable better code discovery, navigation, and reuse. 

- Integrate the existing RAG bot with a vector database.
- Explore dynamic indexing techniques to improve efficiency.
- Research methodologies for leveraging GRAGs to enhance retrieval.
- Test OSS UTG with OSS Repos.
- Integrate Gemini with UTG.

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


### 3. TestSuite Idempotency Checker

**Mentors**: Animesh, Sarthak, Neha Gupta

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
4. Handling noisy parameters of big payloads(10k or more lines) in the cli-diff viewer.

**Skills Required**
1. Scripting Languages such as Python, Bash.
2. Golang
3. Logical Reasoning + DSA
   
**Time Estimate** : 350 hours

**Difficulty** : Medium


### 4. Improve Keploy Open-Source Playground console

**Mentors**: Aditya Sharma, Shivam Jha, Tvisha Raji, Manas, Neha Gupta

**Description**

The goal of this project is to elevate the open-source Keploy Playground for the contributors to understand record-replay. Few of the features requests b community includes:
1. **Expanding Language Support:** Adding support for more languages such as Java, Python, Node.
2. **Integrating Test & Mock Support:** Adding support to fetch generated tests from the keploy server and simulated mocks which can be editable on the playground.
3. **Improving User Onboarding:** Currently the playground lags if the payload is big, or in case of AI/ML genrated tests, the idea is to improve performance of the react console so that other community members can experience it well.

**Goals & Ideas**
1. **Currently Loading Structure Loading is Fragile:** Improve the user experience by fixing the performance issues and handling edge cases.
2. **Interactive Demo Environment:** Build a dynamic playground console where users can interact with live demos, generate tests, and see real-time results.
3. **Automated Test Generation from URL Input**: Allow users to provide a URL, then automatically scrape the frontend to generate a sitemap, identify API calls, and create tests based on the discovered endpoints using ATG
4. **Multi-Language Testing Support:** Implement a flexible backend architecture that supports testing across multiple languages, making Keploy a versatile tool for a diverse range of applications.

**Skills Required**
1. Next.js, React, typescript
2. API call handling
3. Golang, Java, Python
4. [optional] AI/ML 

**Refs**
1. [source code] - https://github.com/keploy/website/tree/main/app/(default) 
2. [Meshery Playground](https://play.meshery.io)

**Time Estimate** : 350 hours

**Difficulty** : Medium


### 5. API contract matching - Adding Features and Platform support
**Mentors**: Gourav Kumar, Charan Kamarapu, Shubham Jain

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

**Tasks**
1. [Implement Microservices Architecture with HTTP APIs & Validate Keploy Contract Testing](https://github.com/keploy/keploy/issues/2541)
2. [Identify and Resolve Issues in Keploy Contract Testing Implementation](https://github.com/keploy/keploy/issues/2543) 

**Time Estimate** : 350 hours

**Difficulty** : medium 

### 6.  App Dashboard with Metrics and Chart
**Mentors**: Manas, Tvisha, Hermione, Neha

**Description**
1. The goal of this project is to build a PR Agent Dashboard that provides interactive visualizations, metrics, and insights for pull request activities. 
2. The dashboard should support dynamic updates and be backed by a Go web server to process and serve data.
3. Structure the application to be easily extensible, enabling straightforward addition of new metrics or charts in the future.

**Goals & Ideas**
1. Dynamic Dashboard: Develop a frontend that dynamically displays PR-related metrics, using visual elements such as graphs and charts.
2. Template-Based PR Insights: Enable users to create and use templates for PR analysis, allowing customized views for different teams and workflows.
3. Scalable & Modular Design: Ensure the system is modular, allowing for easy integration of new metrics, charts, or data sources.

**Tasks:**
1. Develop a web app that enables users to track GitHub organizations, repositories, and user activity, providing a customizable feed and insights.
2. Research about GitHub APIs, Building Modular Dashboards, Data Processing and Integration

**Skills Required**
1. Next.js, Charting Libraries(e.g., Chart.js, Recharts, D3.js)
2. Golang
3. MongoDB

**Refs**
1. Grafana – For inspiration on dashboard design and real-time data visualization.
2. GitHub API Docs – To fetch and process PR data effectively.
3. Golang 

**Time Estimate** : 350 Hours

**Difficulty** : Medium

---
## Task List : Good First Issue for GSoC aspirants

| Projects | Good First Issue |
| -------- | ------- |
| update website themes  | https://github.com/keploy/keploy/issues/2536 </br> https://github.com/keploy/keploy/issues/2535 </br> https://github.com/keploy/keploy/issues/2534  |
| Integrate RAG Bot with a Vector Database  | https://github.com/keploy/keploy/issues/2533  |
| PR Analysis with Linting & Static Analysis in testGPT    | https://github.com/keploy/keploy/issues/2532    |
| Checking of HTML-Based Test Validation   | https://github.com/keploy/keploy/issues/2528    |
| a GitHub App to Trigger GitHub Actions    | https://github.com/keploy/keploy/issues/2531    |
| Denoise Unexpected Parameters in Keploy Testcases | https://github.com/keploy/keploy/issues/2527  |
| Implement Idempotency Check for GET Requests | https://github.com/keploy/keploy/issues/2526  |
| SON Diff viewer re-alignment to top | https://github.com/keploy/keploy/issues/2524 |
