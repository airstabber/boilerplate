**`/[Path/To/File/TODO-Example.md]` (Draft v1.0)**

> _Note: Refer to `FolderStructure.md` to define the file path above  
> & move this file into its correct location according to the defined structure._

## TODO: [Clear, Descriptive Title of the Feature]

### 1. Core Purpose

_Concisely describe the primary goal of this feature. What problem does it solve for the user or the system?_

### 2. MVP Scope

_Define the absolute minimum set of functionalities that make up the first shippable/testable version of  
**this specific feature**. Be very specific about what's IN and what's OUT for the MVP of this feature._

- Functionality 1...
- Functionality 2...
- NOT included in MVP: X, Y, Z (these go to Future Enhancements).

### 3. Future Enhancements

_List potential improvements, additional functionalities, or advanced capabilities  
for **this specific feature** that are beyond its initial MVP._

- Enhancement 1...
- Enhancement 2...

### 4. Dependencies

_List any other features, modules, libraries, external services, or data that **this specific feature**  
depends on to function correctly. Also note if other features depend on this one._

- Requires [Library X] for [purpose].
- Depends on completion of [TODO-OtherFeature.md].
- Data from [Specific Prisma Model / API].

### 5. URL Structure & Routing (If Applicable)

_Detail any new web pages, routes, or API endpoint structures specific to **this feature**._

- New Page: `/[app_path]/[feature_route]`
- New API Endpoint (if not solely tRPC): `api/[feature_endpoint]`
- Relevant tRPC procedures will be defined in Section 8.

### 6. User Experience Flow / Key User Stories

_Describe how users will interact with **this feature**. Use user stories if helpful._

- As a [type of user], I want to [perform an action related to this feature] so that I can [achieve a goal].
- Step-by-step flow for key interactions.
- Consider happy paths and common alternative flows.

### 7. UI Components (`shadcn/ui` & Custom)

_List the key UI components needed to build the interface for **this feature**.  
Differentiate between existing `shadcn/ui` components and custom components you'll need to build._

- **Page/View: [Name of Page/View for this feature]**
  - `shadcn/ui:Button` for [action].
  - `shadcn/ui:Input` for [data entry].
  - Custom Component: `[MyFeatureSpecificComponent]` for [purpose].
- **Modal: [Name of Modal for this feature]**
  - ...

### 8. Backend Logic & Requirements ([Backend Tech] / Prisma / [Prod DB] / [Relevant Libraries])

_Detail the server-side logic required for **this feature**.  
Specify tRPC procedures, their inputs, core logic, outputs, and interactions with the database or other services._  
**A. tRPC Procedure: `module.procedureNameForFeature`**

- **Input:** (Define expected input parameters and types)
- **Authentication/Authorization:** (Specify if procedure requires auth, and any specific roles/permissions)
- **Logic:**
  1.  Step 1: (e.g., Validate input).
  2.  Step 2: (e.g., Interact with Prisma models - `prisma.model.create(...)`).
  3.  Step 3: (e.g., Perform business logic).
  4.  Return: (Define success/error response structure).
- **Security Considerations:** (Any specific security notes for this endpoint).

**B. Other Backend Components/Services (If any)** - (e.g., Interaction with Cloudflare KV, R2, external APIs)

### 9. Prisma Schema Additions/Considerations

_List any new Prisma models, fields, relations, enums, or modifications to existing schemas that are required specifically for **this feature**._

- **New Table: `[NewFeatureTable]`**
  - `id Int @id @default(autoincrement())`
  - `fieldForFeature String`
  - `appUserId Int` (if user-specific)
  - `appUser AppUser @relation(fields: [appUserId], references: [id])`
- **Modifications to `AppUser` (or other existing tables):**
  - Add `newFieldForFeature: Boolean @default(false)`

### 10. Error Handling & Edge Cases

_Identify potential errors, edge cases, and how they should be handled for **this specific feature** (both frontend and backend)._

- Invalid user input.
- Database errors (creation/update/deletion failures).
- Authorization failures.
- Network issues during tRPC calls.
- Specific edge cases related to the feature's logic.
