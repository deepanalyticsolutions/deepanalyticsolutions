# Commit Message Guidelines

This document explains the conventions we follow for commit messages in this repository.

---

## **Commit Message Format**

Each commit message should follow this structure:

1. **Type**: The category of the commit. Examples include:
   - `feat`: A new feature.
   - `fix`: A bug fix.
   - `docs`: Documentation updates.
   - `style`: Code style changes (e.g., formatting).
   - `refactor`: Code changes without altering behavior.
   - `test`: Adding or updating tests.
   - `chore`: Routine tasks like updates to dependencies or CI.

2. **Scope**: (Optional) A brief context of the code affected (e.g., `api`, `auth`, `build`).

3. **Subject**: A short summary of the change (max 50 characters, written in the present tense).

4. **Body**: (Optional) A detailed description of the change. Line width should not exceed 72 characters. Explain the *what*, *why*, and *how*.

5. **Footer**: (Optional) References to related issues or breaking changes.

---

## **Template**

Use the following template for all commit messages:
    <type>(<scope>): <subject>
    <body> <footer>

---

## **Exemples**

1. **Example 1**: Adding a New Feature
    feat(user-auth): add login functionality

    Implemented login functionality with email and password validation.
    This completes phase one of the user authentication system.

    Resolves #123


2. **Example 2**: Fixing a Bug
    fix(api): resolve timeout issue in fetch requests

    Updated fetch request implementation to include proper timeout handling
    using AbortController. This prevents hanging requests on slow networks.

    Closes #456


3. **Example 3**: Updating Documentation
    docs(readme): add setup instructions

    Added a new section in the README detailing how to set up the project locally.
    Included information about dependencies and configuration.


4. **Example 4**: Refactoring Code
    refactor(database): optimize query handling in users table

    Optimized SQL queries in the users table for faster execution.
    No changes to external APIs.

---

**Notes**:
    Be concise: Avoid unnecessary details in the subject line.
    Use imperative mood: Write as if giving a command, e.g., "Add feature" rather than "Added feature."
    Link issues: Always include relevant issue numbers in the footer (Resolves #<issue_number>).
    Follow line limits: Keep the subject under 50 characters and body lines under 72 characters.