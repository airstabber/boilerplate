## **`TODO.md` (Template for Main Project Roadmap, Version: 1.0)**

**Phase 1: Core MVP Implementation (Aligns with "To start..." in StartPrompt.md for [Project Name])**

**I. Project Setup & Foundations:**

1.  **Initialize [Primary Stack Choice]:** (Details: T3 selections, project name).
2.  **Git Initialization:** Init repo, initial commit.
3.  **[UI Component Library] Setup:** Initialize and add basic components.
4.  **[Hosting Platform] Setup (Initial Placeholder):** Create project, link Git, configure build.

**II. Database Schema & Prisma Setup (Local):**

1.  **Define Custom Prisma Models for MVP:** (List key tables and refer to StartPrompt for fields).
2.  **Integrate [Authentication Solution] Prisma Adapter (If Applicable):** Add required models.
3.  **Local Database Migration:** (Command, verify tables).

**III. Backend Logic (MVP - [Backend Tech] & [Authentication Solution] Configuration):**

1.  **Core tRPC Procedure 1 (e.g., `module.procedureName`):**  
    (Brief description of purpose, input, core logic, output, key interactions e.g. with `iron-session` or other libraries).
2.  **Core tRPC Procedure 2 ...**
3.  **[Authentication Solution] Configuration:** (Key providers, environment variables).
4.  **[Authentication Solution] Callbacks Implementation (Core Logic):**  
    (Brief description of key logic for `signIn`, `jwt`, `session` etc. specific to MVP functionality).

**IV. Frontend UI (MVP - [Application Type] & [UI Component Library]):**

1.  **Key Page/Component 1 (e.g., `/invite/[token]/page.tsx` or `/notes/page.tsx`):**  
    (Brief description of functionality, tRPC calls made, conditional rendering).
2.  **Key Page/Component 2 ...**
3.  **Authenticated Area Shell (e.g., `/dashboard` or main app layout - Minimal):** (Protection, basic display, logout).
4.  **Basic Page Layout:** (Overall structure).

**V. Deployment & [Production DB] Integration (Initial):**

1.  **[Production DB] Creation:** (How to create).
2.  **Prisma [Production DB] Adapter Configuration:** (For production builds).
3.  **[Production DB] Migrations (Production):** (How to apply).
4.  **[Hosting Platform] Bindings & Environment Variables:** (Key bindings and env vars).
5.  **Deploy & Test MVP:** (Key flows to test).

---

**Transition Point: MVP Completion & Preparation for Phase 2**

_Once all items in Phase 1 are conceptually complete, request a summary from the AI assistant based on the work done.  
This summary will serve as the context for starting Phase 2 development, potentially in a new chat._

**Example AI Request for Summary:**  
"The MVP for [Project Name] as outlined in `StartPrompt.md` is conceptually complete.  
Could you provide a concise summary of what we've accomplished for this MVP,  
so that it can be used as context for Phase 2 from this `TODO.md`?"

## **(Placeholder for AI-Generated Summary - to be pasted here after AI generates it)**

### [AI to generate summary here based on conceptual completion of Phase 1]

---

**Phase 2: Enhancements & Future Features (High-Level List - Detailed in dedicated Feature TODO files)**

**I. [Category 1, e.g., User Profile & Account Management]:**

1.  Feature A _(Ref: `[Path/To/]TODO-ExampleA.md`)_
2.  Feature B _(Ref: `[Path/To/]TODO-ExampleB.md`)_

**II. [Category 2, e.g., Core Application Features]:**

1.  Feature C _(Ref: `[Path/To/]TODO-ExampleC.md`)_
2.  Feature D _(Ref: `[Path/To/]TODO-ExampleD.md`)_

**III. [Category 3, e.g., Platform Polish & DevOps]:**

1.  Feature E _(Ref: `[Path/To/]TODO-ExampleE.md`)_
2.  Feature F _(Ref: `[Path/To/]TODO-ExampleF.md`)_

_Note: Add more categories and features as needed.  
The `Ref:` paths should point to where the detailed `TODO-Example.md` files will reside._
