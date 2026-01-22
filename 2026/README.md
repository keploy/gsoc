# Google Summer of Code'26 Participant Guide

## **Communication**

Welcome to the Keploy GSoC'26 projects page. We encourage candidates to come up with their own project idea. Join our [Slack Channel]() and stay tuned for updates.

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

## **Projects List (GSoC 2026)**

### 1. MCP Server for Keploy (Model Context Protocol Integration)

**Mentors**: TBD

As AI-assisted developer tools and agents become increasingly common, there is a growing opportunity to standardize how project context, APIs, and workflows are shared with AI models. Introducing a dedicated Model Context Protocol (MCP) server for Keploy would enable AI agents, IDE copilots, and automation tools to interact with Keploy in a structured, secure, and extensible way.

This project offers contributors the chance to design and build this MCP integration from the ground up, helping Keploy become more accessible to next-generation AI-powered developer tooling.

#### **Description**

This project focuses on designing and implementing an MCP server that acts as a bridge between Keploy and AI-powered tools. The server will expose structured context such as APIs, test results, schemas, and project metadata, allowing AI agents to reason about and operate on Keploy-managed projects more effectively.

#### **Tasks**
1. Study the Model Context Protocol (MCP) specification and reference implementations.
2. Design MCP-compatible schemas for:
   - Test cases and reports  
   - Mock definitions  
   - API schemas and traffic metadata  
   - Project configuration and metadata
3. Implement the MCP server using **TypeScript / Node.js**.
4. Expose core MCP endpoints for context discovery and retrieval.
5. Implement authentication and authorization mechanisms.
6. Validate compatibility with MCP clients or AI agents.
7. Write comprehensive documentation and usage examples.

#### **Skills Required**
- TypeScript / JavaScript
- Node.js backend development
- REST APIs & JSON schemas
- Basic understanding of AI/LLM tooling
- Open-source development workflows

#### **References**
- [Model Context Protocol (MCP) specification](https://modelcontextprotocol.io/)
- [Keploy documentation](https://docs.keploy.io/)

**Time Estimate**: 350 hours  
**Difficulty**: Medium–Hard  


### 2. Keploy Blog Website Revamp & Performance Enhancement

**Mentors**: TBD


The Keploy blog is a key channel for sharing technical knowledge and community contributions. However, the current blog website has several limitations:
- UI/UX inconsistencies
- Performance and page load issues
- Limited contributor-friendly workflows
- Missing features common in modern developer blogs

Several improvement opportunities already exist as GitHub issues in the Keploy repository, and additional enhancements can be proposed by analyzing best-in-class open-source and developer-focused blogs.

#### **Description**

Revamp the **Keploy Blog Website** to improve **UI/UX, performance, accessibility, and contributor experience**, while keeping the platform scalable and easy to maintain.

This project focuses on improving both the frontend experience and the backend/content management workflows of the Keploy blog. Contributors will work on existing issues, propose new improvements, and implement features inspired by high-quality developer blogs.

Contributors are encouraged to take ownership by identifying gaps, creating new issues, and driving features from ideation to implementation.

#### **Focus Areas**

- UI/UX improvements
- Performance optimization
- Backend/API development
- Documentation and contributor experience
- DevOps and deployment improvements

#### **Tasks**

1. Audit the existing blog website for UI, performance, and architectural issues.
2. Pick and solve at least one existing issue from the Keploy repository.
3. Improve UI/UX:
   - Layout, typography, and readability
   - Navigation and discoverability
   - Mobile responsiveness and accessibility
4. Optimize performance:
   - Improve page load time and Lighthouse scores
   - Optimize images, scripts, and caching
5. Enhance backend and CMS workflows (WordPress):
   - Improve content management and publishing flow
   - Enhance APIs or integrations if applicable
6. Propose and implement new features inspired by modern developer blogs:
   - Better search and filtering
   - SEO enhancements
   - Related posts and engagement features
7. Improve documentation and contributor onboarding for the blog.

#### **Tech Stack**
- TypeScript
- JavaScript
- WordPress
- Tailwind CSS

#### **Skills Required**
- Frontend development (JavaScript, TypeScript, CSS)
- UI/UX fundamentals
- WordPress or CMS-based development
- Web performance optimization
- Open-source collaboration

#### **References**

- Keploy blog repository issues [https://github.com/keploy/keploy/issues?q=is%3Aissue%20is%3Aopen%20label%3Ablog-website]

**Time Estimate**: 350 hours  
**Difficulty**: Medium  


### **3. Test Suite Management Dashboard**

**Mentors**: TBD

#### **Problem Statement**

As test suites grow across services and repositories, managing tests efficiently becomes increasingly complex. Developers often struggle with test prioritization, visibility into failures, tracking regressions, and linking test results to real-world bugs. Existing workflows are fragmented across tools like CI pipelines, issue trackers, and version control systems.

A centralized, developer-friendly test management dashboard can significantly improve productivity, test reliability, and release confidence.

#### **Project Goal**
Build a comprehensive **Test Suite Management Dashboard** for Keploy that provides visibility, prioritization, and control over test suites, while integrating seamlessly with CI/CD pipelines and issue tracking systems.

#### **Description**
This project focuses on creating an interactive dashboard that helps teams manage, prioritize, and track tests effectively. The dashboard will integrate with popular developer tools and use test coverage and risk signals to guide smarter testing decisions.

#### **Tasks**
1. Design and implement a web-based test management dashboard.
2. Integrate Jira and/or Linear for:
   - Automatic bug creation from failing tests
   - Linking test failures to tracked issues
3. Build a Kanban-style board for:
   - Test prioritization
   - Tracking test status (new, flaky, critical, fixed)
4. Implement Git-based version control for test cases:
   - Track test history
   - Show diffs between test changes
5. Integrate with CI/CD systems:
   - GitHub Actions
   - GitLab CI
   - Jenkins
6. Implement smart risk-based test prioritization using:
   - Code coverage metrics
   - Historical failure data

#### **Skills Required**
- TypeScript / JavaScript
- Frontend frameworks (React or similar)
- REST APIs
- CI/CD pipelines
- Git workflows
- Basic understanding of testing strategies

**Time Estimate**: 350 hours  
**Difficulty**: Medium–Hard  



### **4. PII Detection & Sanitization Engine**

**Mentors**: TBD

#### **Problem Statement**
When recording production traffic for test generation, sensitive data such as emails, phone numbers, credit card details, or personal identifiers may unintentionally appear in test artifacts. This introduces privacy risks and compliance concerns, especially in regulated environments.

There is a strong need for automated, reliable mechanisms to detect and sanitize sensitive data during test capture and execution.

#### **Project Goal**
Build a **PII Detection & Sanitization Engine** that automatically identifies, masks, or anonymizes sensitive data in recorded traffic and test artifacts, helping teams adopt Keploy safely in production-like environments.

#### **Description**
This project involves creating a real-time PII detection and sanitization layer that integrates directly into Keploy’s traffic capture and test workflows. The system should be configurable, extensible, and capable of generating compliance reports.

#### **Tasks**
1. Implement real-time PII detection for:
   - Emails
   - Phone numbers
   - Credit card numbers
   - Government identifiers (SSN, etc.)
2. Build configurable masking and anonymization strategies:
   - Partial masking
   - Tokenization
   - Full anonymization
3. Integrate sanitization at capture time to prevent sensitive data storage.
4. Flag tests and artifacts that may contain sensitive data.
5. Generate compliance-ready reports aligned with:
   - GDPR
   - HIPAA
6. Integrate seamlessly with existing Keploy test suites.

#### **Skills Required**
- Golang or TypeScript
- Regular expressions and pattern matching
- Data privacy fundamentals
- Secure system design
- Testing frameworks

**Time Estimate**: 350 hours  
**Difficulty**: Hard  



### **5. AI Model Testing Framework**

**Mentors**: TBD

#### **Problem Statement**
Testing AI and LLM-based applications introduces new challenges such as nondeterministic outputs, hallucinations, prompt regressions, and quality evaluation. Traditional testing frameworks are not well-suited to validate AI-driven behavior consistently.

There is a growing need for a structured testing framework tailored specifically for AI and LLM-powered applications.

#### **Project Goal**
Build an **AI Model Testing Framework** that enables developers to test, evaluate, and benchmark AI-driven applications with confidence.

#### **Description**
This project focuses on creating a testing and evaluation toolkit for AI applications. The framework will support multiple AI providers, detect regressions caused by prompt changes, and measure response quality using meaningful metrics.

#### **Tasks**
1. Design a testing framework for AI/LLM applications.
2. Add support for multiple model providers:
   - OpenAI
   - Anthropic
   - Local and open-source models
3. Implement regression detection for prompt changes.
4. Measure hallucination rates and response accuracy.
5. Define and compute response quality metrics.
6. Add benchmarking capabilities across models and prompts.
7. Support voice agent and conversational AI testing workflows.

#### **Skills Required**
- Python or TypeScript
- Understanding of LLMs and AI systems
- Testing frameworks and evaluation metrics
- API integrations
- Prompt engineering fundamentals

**Time Estimate**: 350 hours  
**Difficulty**: Medium–Hard  



### **6. Test Migration Tool**

**Mentors**: TBD

#### **Problem Statement**
Many teams already have extensive test suites built using tools like Postman, Selenium, and JMeter. Migrating these tests to Keploy often requires manual effort, slowing adoption and increasing the learning curve.

A unified migration tool can significantly reduce friction and accelerate onboarding to Keploy.

#### **Project Goal**
Build a **one-click Test Migration Tool** that enables seamless migration of existing tests from popular testing platforms into Keploy-compatible tests.

#### **Description**
This project involves building a unified migration platform that parses test definitions from different tools and converts them into Keploy test artifacts while preserving intent, assertions, and workflows.

#### **Tasks**
1. Analyze test formats from:
   - Postman
   - Selenium
   - JMeter
2. Design a unified intermediate test representation.
3. Implement converters to transform existing tests into Keploy tests.
4. Build a CLI or UI-based one-click migration workflow.
5. Validate migrated tests and generate migration reports.
6. Document migration steps and limitations.

#### **Skills Required**
- Golang or TypeScript
- Test automation tools
- Parsing and data transformation
- CLI or UI development
- Developer tooling experience

**Time Estimate**: 350 hours  
**Difficulty**: Medium  


### **7. Trace-Based Testing**

**Mentors**: TBD

#### **Problem Statement**
Modern distributed systems generate rich tracing data, but this information is rarely used directly for testing. Traces can provide valuable insights into real execution paths, dependencies, and system behavior that traditional tests often miss.

Leveraging traces for testing can significantly improve test accuracy and coverage.

#### **Project Goal**
Enable **Trace-Based Testing** in Keploy by generating and validating tests using distributed tracing data.

#### **Description**
This project focuses on using trace data (such as OpenTelemetry traces) to automatically derive test scenarios, validate service interactions, and detect behavioral regressions in distributed systems.

#### **Tasks**
1. Integrate distributed tracing data into Keploy workflows.
2. Extract request flows and dependencies from traces.
3. Generate test cases based on real execution paths.
4. Validate traces against expected behavior during test runs.
5. Detect deviations and regressions using trace comparisons.
6. Support popular tracing standards and tools.

#### **Skills Required**
- Distributed systems fundamentals
- Tracing tools (OpenTelemetry or similar)
- Golang or TypeScript
- Testing and observability concepts
- Backend system design

**Time Estimate**: 350 hours  
**Difficulty**: Hard  

---
## Task List : Good First Issue for GSoC aspirants

| Projects | Good First Issue |
| -------- | ------- |

|Add New Quickstarts for More Languages | https://github.com/keploy/keploy/issues/3521 | 
| IP not found error when run with docker compose up  | https://github.com/keploy/keploy/issues/3360  |

| Enhance the testimonial marquee UI on the blog homepage | https://github.com/keploy/keploy/issues/3440 |

| Beautify tags on blog reading posts | https://github.com/keploy/keploy/issues/3437 |

| Fix blog navbar dropdown ui on mobile devices | https://github.com/keploy/keploy/issues/3431 |

| Fix new blog navbar alignment on scroll and shrink | https://github.com/keploy/keploy/issues/3429 |

| Fix blog navbar alignment on desktop | https://github.com/keploy/keploy/issues/3428 |

|  Fix Blog navbar Logo on shrink | https://github.com/keploy/keploy/issues/3427 |

| Remove inclusion of delay time in the test run summary | https://github.com/keploy/keploy/issues/3351 |

| Add skeleton loaders in the blog website for better user experience | https://github.com/keploy/keploy/issues/3293 |

| Ignore mockery generated files from go coverage calculation | https://github.com/keploy/keploy/issues/3219 | 


| Add Modern UI Components to Blog Landing Page | https://github.com/keploy/keploy/issues/3084 |

| Add Dark/Light Mode Support with Toggle | https://github.com/keploy/keploy/issues/3083 |

| Redesign Testimonials Section (Blog Website) | https://github.com/keploy/keploy/issues/3082 |

| Create Writers Page with Cards for Contributors | https://github.com/keploy/keploy/issues/3074 |

| Add Resources Page for Writers program | https://github.com/keploy/keploy/issues/3076 |

| Add Dark/Light Mode Support with Toggle for Devrel website | https://github.com/keploy/keploy/issues/3078 |

| Add Blog Publishing Flow Documentation Page | https://github.com/keploy/keploy/issues/3077 |

| SEO, Open Graph, Sitemap, and Performance Optimizations | https://github.com/keploy/keploy/issues/3079 |

| Add Search Functionality in blog website navbar | https://github.com/keploy/keploy/issues/3081 |

| Redesign and Implement Navbar Using TailwindCSS or UI Library | https://github.com/keploy/keploy/issues/2769 |

| Improve Keploy docs website mobile-friendly | https://github.com/keploy/keploy/issues/2998 |

| Redesign DevRel website | https://github.com/keploy/keploy/issues/3066 |

| Add Navbar, Footer, and new UI components for Devrel website | https://github.com/keploy/keploy/issues/3067 |

| Migrate Writers site to Next.js 15 + TypeScript + Tailwind | https://github.com/keploy/keploy/issues/3069 |

| Improve Typography, Fonts, and Information Hierarchy for Writers program website | https://github.com/keploy/keploy/issues/3070 |

| Modern UI Components for Key Sections in Writers program website | https://github.com/keploy/keploy/issues/3071 |

| Modern Navigation and Layout for Writers program website | https://github.com/keploy/keploy/issues/3072 |


---

## Task List: Good First Issues for GSoC Aspirants

| Project / Area | Good First Issue |
|---------------|-----------------|
| Add New Quickstarts for More Languages | https://github.com/keploy/keploy/issues/3521 |
| IP not found error when running with Docker Compose | https://github.com/keploy/keploy/issues/3360 |
| Enhance the testimonial marquee UI on the blog homepage | https://github.com/keploy/keploy/issues/3440 |
| Beautify tags on blog reading posts | https://github.com/keploy/keploy/issues/3437 |
| Fix blog navbar dropdown UI on mobile devices | https://github.com/keploy/keploy/issues/3431 |
| Fix new blog navbar alignment on scroll and shrink | https://github.com/keploy/keploy/issues/3429 |
| Fix blog navbar alignment on desktop | https://github.com/keploy/keploy/issues/3428 |
| Fix blog navbar logo on shrink | https://github.com/keploy/keploy/issues/3427 |
| Remove inclusion of delay time in the test run summary | https://github.com/keploy/keploy/issues/3351 |
| Add skeleton loaders in the blog website for better UX | https://github.com/keploy/keploy/issues/3293 |
| Ignore mockery-generated files from Go coverage calculation | https://github.com/keploy/keploy/issues/3219 |
| Add modern UI components to blog landing page | https://github.com/keploy/keploy/issues/3084 |
| Add dark/light mode support with toggle (Blog) | https://github.com/keploy/keploy/issues/3083 |
| Redesign testimonials section (Blog Website) | https://github.com/keploy/keploy/issues/3082 |
| Create writers page with cards for contributors | https://github.com/keploy/keploy/issues/3074 |
| Add resources page for Writers Program | https://github.com/keploy/keploy/issues/3076 |
| Add dark/light mode support with toggle (DevRel Website) | https://github.com/keploy/keploy/issues/3078 |
| Add blog publishing flow documentation page | https://github.com/keploy/keploy/issues/3077 |
| SEO, Open Graph, sitemap, and performance optimizations | https://github.com/keploy/keploy/issues/3079 |
| Add search functionality in blog website navbar | https://github.com/keploy/keploy/issues/3081 |
| Redesign and implement navbar using Tailwind CSS or UI library | https://github.com/keploy/keploy/issues/2769 |
| Improve Keploy docs website mobile-friendliness | https://github.com/keploy/keploy/issues/2998 |
| Redesign DevRel website | https://github.com/keploy/keploy/issues/3066 |
| Add navbar, footer, and new UI components for DevRel website | https://github.com/keploy/keploy/issues/3067 |
| Migrate Writers site to Next.js 15 + TypeScript + Tailwind | https://github.com/keploy/keploy/issues/3069 |
| Improve typography, fonts, and information hierarchy (Writers site) | https://github.com/keploy/keploy/issues/3070 |
| Modern UI components for key sections (Writers site) | https://github.com/keploy/keploy/issues/3071 |
| Modern navigation and layout for Writers site | https://github.com/keploy/keploy/issues/3072 |
