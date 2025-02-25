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

**Description**: The objective of this project is to enhance the Keploy Playground by introducing new functionalities, improving user experience, and expanding its capabilities. This includes:

1. **Expanding Language Support:** Adding robust support for multiple programming languages such as Java and Python.
2. **Integrating Test & Mock Support:** Providing comprehensive functionalities to generate tests and simulate mocks seamlessly.
3. **Improving User Onboarding:** Redesigning the user experience, especially the onboarding process, to ensure a smooth introduction to Keploy’s capabilities.

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
1. Integrate the existing RAG bot with a [Milvus](https://github.com/milvus-io/milvus).
  * Modify the existing RAG bot to store code snippets as vector embeddings in Milvus.
2. Explore dynamic indexing techniques to improve efficiency.
  * Research and compare different indexing techniques (HNSW, IVF, PQ, Flat Index) for faster retrieval.
3. Research methodologies for leveraging GRAGs to enhance retrieval.
  * Implement a prototype that combines vector search with graph-based retrieval to improve accuracy.
4. Test Open-Source [UTG (Unit Test Generation)](https://keploy.io/docs/running-keploy/unit-test-generator/) with OSS Repositories.
  * Run Keploy’s OSS Unit Test Generator (UTG) on real-world repositories and suggest optimizations for the UTG model based on results.
5. Use [Gemini AI](https://gemini.google.com/app) (Google’s LLM) to generate better test cases from indexed OSS codebases.

**Time Estimate** : 350 hours

**Difficulty** : Medium


### 3. TestSuite Idempotency Checker

**Mentors**: Animesh, Sarthak Shyngle, Neha Gupta

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

**Ref**
1. [idempotency and safety in REST APIs ](https://www.linkedin.com/advice/0/how-do-you-test-monitor-idempotency)
2. [How Idempotent REST APIs Boost Reliability and Error Handling](https://keploy.io/docs/concepts/reference/glossary/idempotency/)
3. [Idempotent Message Validator](https://docs.mulesoft.com/mule-runtime/latest/idempotent-message-validator)

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
**Mentors**: Gourav Kumar, Charan Kamarapu, Ahmed Lotfy, Shubham Jain

**Description**: The goal of this project is to enhance the functionality of contract testing by adding new features and improving existing capabilities. This includes better schema storage, consolidation, and validation, along with exploring a provider-driven approach as a future enhancement.

**Goals & Ideas**
1. **Schema Storage Enhancement**: Implement local storage support for schemas, functioning as a mock public registry (e.g., S3).
2. **Unified Schema Management**: Merge individual test/mock schemas into a comprehensive single schema for each service, consolidating all APIs
3. **Advanced Schema Comparison**: Design and improve schema validation between interconnected services to ensure consistency.
4. **Provider-Driven Architecture**: Develop and integrate a provider-driven contract testing model into Keploy, allowing service providers to define and manage contracts efficiently.

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
**Mentors**: Manas Manohar, Tvisha Raji, Hermione Dadheech, Neha Gupta

**Description**
1. The objective of this project is to create a console that provides interactive visualizations, metrics, and insights for code merges and test activities.
2. The console should support dynamic updates and be powered by a Go web server that processes and serves data.
3. It should be structured for easy extensibility, making it straightforward to add new metrics or charts in the future.

**Goals & Ideas**
1. Dynamic Dashboard: Develop a frontend that aggregates and displays real-time test reports using visual elements such as graphs and charts
2. Template-Based PR Insights: Allow users to create and utilize templates for code analysis, offering customizable views for different teams and workflows.
3. Scalable & Modular Design:  Ensure the system’s architecture is modular and can accommodate new metrics, charts, or data sources with minimal effort.

**Tasks:**
1. Build a web app that tracks multiple repositories and user activities, offering a customizable feed of test outcomes and analytics.
2. Research techniques for building modular dashboards, data processing, and integration with various version control or repository hosting services.

**Skills Required**
1. Next.js, Charting Libraries(e.g., Chart.js, Recharts, D3.js)
2. Golang
3. MongoDB

**Refs**
1. Grafana – For inspiration on dashboard design and real-time data visualization.
2. Golang Documentation – For best practices in building scalable Go services.

**Time Estimate** : 350 Hours

**Difficulty** : Medium

---
## Task List : Good First Issue for GSoC aspirants

| Projects | Good First Issue |
| -------- | ------- |
| update website themes  | https://github.com/keploy/keploy/issues/2536 </br> https://github.com/keploy/keploy/issues/2535 </br> https://github.com/keploy/keploy/issues/2534  | 
|Improve keploy console| https://github.com/keploy/keploy/issues/2551 </br> https://github.com/keploy/keploy/issues/2552|
| Integrate RAG Bot with a Vector Database  | https://github.com/keploy/keploy/issues/2533  |
| PR Analysis with Linting & Static Analysis in testGPT    | https://github.com/keploy/keploy/issues/2532    |
| Checking of HTML-Based Test Validation   | https://github.com/keploy/keploy/issues/2528    |
| a GitHub App to Trigger GitHub Actions    | https://github.com/keploy/keploy/issues/2531    |
| Denoise Unexpected Parameters in Keploy Testcases | https://github.com/keploy/keploy/issues/2527  |
| Implement Idempotency Check for GET Requests | https://github.com/keploy/keploy/issues/2526  |
| SON Diff viewer re-alignment to top | https://github.com/keploy/keploy/issues/2524 |
