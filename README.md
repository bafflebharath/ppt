Hi Team,

I would like to share a quick update on the development approach we are currently adopting and the progress made on our ongoing use case.

**1. AI-Driven Development for CSP Implementation**
Our team has started leveraging an end-to-end AI-assisted development approach for CSP implementation. Using tools such as Copilot and coding agents, we are able to generate the first level of code (including separate JS and CSS files for a page) within **10–20 minutes**. After this, we perform unit testing and address any minor issues identified.

Using the same `.md` prompt/agent configuration in Codex, we are also able to generate **10–20 pages in a single run**. Additionally, the same prompts can generate **.docx documentation**, which can be used as a base for **end-to-end Unit Testing (UT) documentation**.

We have documented this approach and supporting details in a Confluence page (link attached).

**2. Architecture Approach for the Current Use Case**
Our application is currently built using JSP with tightly coupled Java code. To improve modularity and future scalability, we introduced a **Servlet-based API layer** similar to REST.

This enables us to:

* Expose application data through APIs
* Maintain a **loosely coupled architecture**
* Develop and deploy **Frontend and Backend independently**
* Reuse the same APIs if we migrate the application to **Spring REST** in the future

**3. Prototype Built Using Exposed APIs**
Using the APIs exposed from the RAM application, we developed a **simple Angular prototype**, which includes:

* A **login screen** integrated with the RAM application
* Authentication using the **session nonce generated from the application**
* A **User List page** that consumes **live data** from the RAM application APIs

Notably, the **entire first-level implementation was generated using AI**, leveraging Copilot, agent-based prompting, and AI-assisted coding practices. By providing clear acceptance criteria and well-defined use cases, we are able to generate high-quality baseline code in the initial attempt.

Thank you for your time and support.

Best regards,
Bharath Kumar
