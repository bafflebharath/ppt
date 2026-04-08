# ppt

Hi Team,

I wanted to share a quick update on the development approach we are currently adopting and the progress made on our ongoing use case.

**1. AI-Driven Development for CSP Implementation**
Our team has started using an end-to-end AI-assisted coding approach for CSP implementation. With tools like Copilot and coding agents, we are able to generate the initial level of code (including separate JS and CSS files for a page) within **10–20 minutes**.
After this, we perform unit testing and fix minor issues.

Using the same `.md` prompt/agent configuration in Codex, we are also able to generate **10–20 pages in a single run**.
We have documented the process and best practices in a Confluence page (link attached).

**2. Architecture Approach for Current Use Case**
Our application is currently built using JSP with tightly coupled Java code. To improve modularity, we have introduced a **Servlet-based API layer** (similar to REST).

This approach allows us to:

* Expose application data through APIs
* Keep the system **loosely coupled**
* Develop and deploy **Frontend and Backend independently**
* Reuse the same APIs in the future if we migrate to **Spring REST architecture**

**3. Prototype Built Using Exposed APIs**
Using the APIs exposed from the RAM application, we developed a **simple Angular prototype** which includes:

* A **Login screen** integrated with the RAM application
* Session login using the **generated nonce/session token**
* A **User List page** that consumes **live data** from the RAM application APIs

Notably, the **entire first-level implementation was generated using AI**, leveraging Copilot, vibe coding practices, and agent-based prompting. With **clear acceptance criteria and well-defined use cases**, we are able to generate high-quality baseline code in the first attempt.

Thank you for your time. Please feel free to reach out if you need any additional details.

Best regards,
Bharath
