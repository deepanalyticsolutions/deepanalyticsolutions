# Commit Message Guidelines

This document explains the conventions we follow for commit messages in this repository.

---

## **Commit Message Format**

Each commit message should follow this structure:

1. **Type**: The category of the commit. Examples:
   - `feat`: Adding a new feature.
   - `fix`: Fixing a bug.
   - `docs`: Updating documentation.
   - `style`: Code style changes (e.g., formatting).
   - `refactor`: Code changes without altering behavior.
   - `test`: Adding or updating tests.
   - `chore`: Routine tasks like dependency updates or CI/CD maintenance.

2. **Scope** (Optional): A brief context of the affected code (e.g., `api`, `auth`, `build`).

3. **Subject**: A short summary of the change (max. 50 characters, written in the present tense).

4. **Body** (Optional): A detailed description of the change. Line width should not exceed 72 characters. Explain the *what*, *why*, and *how*.

5. **Footer** (Optional): References to related issues or breaking changes.

---

## **Template**

Use the following template for all commit messages:

```plaintext
<type>(<scope>): <subject>

<body>

<footer>
```

---

## **Examples**

1. **Adding a new feature**

```plaintext
feat(user-auth): add login functionality

Implemented login functionality with email and password validation.
This completes phase one of the user authentication system.

Resolves #123
```

2. **Fixing a bug**

```plaintext
fix(api): resolve timeout issue in fetch requests

Updated fetch request implementation to include proper timeout handling
using AbortController. This prevents hanging requests on slow networks.

Closes #456
```

3. **Updating documentation**

```plaintext
docs(readme): add setup instructions

Added a new section in the README detailing how to set up
the project locally. Included information about dependencies and configuration.
```

4. **Refactoring code**

```plaintext
refactor(database): optimize SQL query handling in users table

Optimized SQL queries for faster execution.
No changes to external APIs.
```

---

## **Notes**

- **Be concise**: Avoid unnecessary details in the subject line.
- **Use imperative mood**: Write as if giving a command (e.g., "Add feature" instead of "Added feature").
- **Link issues**: Always include relevant issue numbers in the footer (`Resolves #<issue_number>`).
- **Follow line limits**:
  - Subject: max. 50 characters.
  - Body: lines of max. 72 characters.
