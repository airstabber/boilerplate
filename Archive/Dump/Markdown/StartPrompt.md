## **`StartPrompt.md` (Template for Project Initiation, Version: 1.0)**

**INSTRUCTION FOR AI ASSISTANT (Claude/ChatGPT/etc.):**  
**Please read this entire StartPrompt document carefully. Once you have processed it,  
confirm that you understand the overall goal (MVP for [Project Name]) and the key components.  
Then, please WAIT for me to ask for guidance on specific steps from the "To start (MVP Implementation):" section below.  
Do NOT provide a lengthy summary or try to guide through all steps at once. We will proceed step-by-step at my pace.**

---

Let's begin building the **[Project Name]**.

This project will utilize the **[Primary Stack Choice, e.g., T3 Stack (via `create.t3.gg`)]** as the foundation  
for a **[Application Type, e.g., Next.js]** application deployed on **[Hosting Platform, e.g., Cloudflare Pages]**.  
During initialization, we will include **[ORM Choice, e.g., Prisma]** as the ORM, selecting **[Local DB, e.g., SQLite]**  
for local database persistence and targeting **[Production DB, e.g., Cloudflare D1]** for production.  
 **[Authentication Solution, e.g., NextAuth.js]** will be integrated for authentication.  
 For the UI, we'll use **[UI Component Library, e.g., `shadcn/ui`]** components.

**The core initial goal (MVP):** To establish [describe the core functionality of the MVP concisely].  
For example: "a robust, invite-only, gatekept authentication system."  
[Provide key details about the MVP's core mechanism, e.g., "Access is granted via an administrator-provided unique `inviteToken`..."]  
[Mention any key supporting technologies for the MVP, e.g., "Secure, short-lived cookies (e.g., via `iron-session`) will be used for..."]  
_All application features beyond this core MVP are considered Phase 2 and will be detailed in `TODO.md` and subsequent `TODO-Example.md` documents._

**Key components for this MVP:**

1.  **Data Persistence ([Production DB] & [ORM Choice]):**

    - **Primary Table(s) for MVP:** [e.g., `AppUser`, `LinkedOAuthAccount`]
      - Fields for Table1: `id` (PK), `fieldA` (Type, constraints), `fieldB` (Type, constraints)...
      - Fields for Table2: ...
      - Key relationships and constraints (`@@unique`, foreign keys).
    - **Integration with [Authentication Solution, if applicable]:**
      - [e.g., "NextAuth.js will be configured with its Prisma Adapter..."]
      - [e.g., "How the project's core user model relates to the auth solution's user model..."]

2.  **User Interaction Flow & UI (MVP - [Application Type] & [UI Component Library]):**

    - **Key Page(s) / View(s) for MVP:** [e.g., `/invite/[token]`, `/dashboard`]
      - Brief description of each page's purpose and key UI elements for the MVP.
    - **Core User Actions for MVP:** [e.g., "Claim invite, link OAuth account, view dashboard, logout"].

3.  **Backend Logic (MVP - [Backend Tech, e.g., tRPC] on [Hosting Platform Functions]):**

    - **Core API Endpoint(s) / Procedure(s):** [e.g., `auth.validateInviteToken`]
      - Brief description of input, primary logic, and output for each.
      - Mention key interactions with the database or other services.
    - **Authentication/Authorization Logic (if applicable):**
      - [e.g., "NextAuth.js `signIn`, `jwt`, `session` callbacks logic..."]

4.  **Administrator/System Pre-requisite (MVP, if any):**
    - [e.g., "Manual population of `AppUser` table with `inviteToken`s."]
    - [e.g., "No specific admin prerequisites for a simple notes app MVP."]

### **To start (MVP Implementation):**

_(This section outlines the high-level steps to build the MVP. These steps will be expanded in Phase 1 of `TODO.md`)_

1.  Initializing [Primary Stack Choice] project...
2.  Initializing Git...
3.  Setting up [UI Component Library]...
4.  Defining initial Prisma schema for [Primary MVP Tables]...
5.  Configuring [Authentication Solution] Prisma Adapter (if applicable)...
6.  Running initial local database migrations...
7.  Setting up basic UI components for [Key MVP Pages/Views]...
8.  Creating tRPC procedures for [Core MVP Backend Logic]...
9.  Configuring [Authentication Solution] with one provider/method and implementing core callbacks...
10. Initial [Hosting Platform] setup, [Production DB] adapter configuration, applying migrations to [Production DB],  
    and configuring bindings/environment variables for a test deployment.
