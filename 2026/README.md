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

**Mentors**: Shubham Jain, Asish Kumar 

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


### 2. Keploy Blog Website Refactoring, Redesign & Performance Improvements

**Mentors**: Neha Gupta, TBD

The Keploy blog is a key channel for sharing technical knowledge and community contributions. As the blog continues to grow, there is an opportunity to **refactor existing code, redesign the user experience, and improve overall performance and maintainability** to better serve both readers and contributors.

Several improvement opportunities already exist as GitHub issues in the Keploy repository. Contributors are also encouraged to propose enhancements by taking inspiration from modern open-source and developer-focused blogs.

---

### **Description**

This project focuses on **refactoring and redesigning the Keploy blog website** to improve **UI/UX, performance, accessibility, and contributor experience**, while keeping the platform scalable and easy to maintain.

Contributors will work across both the frontend and backend/content management workflows of the blog. The project encourages hands-on ownership—students will pick existing issues, suggest improvements, and drive features from ideation through implementation.

---

### **Focus Areas**

- UI/UX redesign and visual consistency
- Performance optimization and Core Web Vitals
- Backend and API improvements
- Documentation and contributor experience
- DevOps and deployment enhancements

---

### **Tasks**

1. Audit the existing blog website for UI, performance, and architectural improvements.
2. Pick and resolve at least one existing issue from the Keploy repository.
3. Refactor and redesign UI components:
   - Layout, typography, and readability
   - Navigation and content discoverability
   - Mobile responsiveness and accessibility
4. Optimize performance:
   - Improve page load time and Lighthouse scores
   - Optimize images, scripts, and caching strategies
5. Enhance backend and CMS workflows (WordPress):
   - Improve content management and publishing flow
   - Enhance APIs or integrations if applicable
6. Propose and implement new features inspired by modern developer blogs:
   - Search and filtering
   - SEO improvements
   - Related posts and engagement features
7. Improve documentation and onboarding for blog contributors.

---

### **Tech Stack**

- TypeScript
- JavaScript
- WordPress
- Tailwind CSS

---

### **Skills Required**

- Frontend development (JavaScript, TypeScript, CSS)
- UI/UX fundamentals
- WordPress or CMS-based development
- Web performance optimization
- Open-source collaboration

---

### **References**

- Keploy blog repository issues:  
  https://github.com/keploy/keploy/issues?q=is%3Aissue%20is%3Aopen%20label%3Ablog-website

**Time Estimate**: 350 hours  
**Difficulty**: Medium

---


## Good First Issues for GSoC Aspirants

Here is a curated list of **Good First Issues** for GSoC aspirants. You can pick any issue from the list below and start contributing to Keploy:

👉 https://github.com/keploy/keploy/issues?q=is%3Aissue%20state%3Aopen%20label%3A%22Good%20First%20Issue%22
