# commit message instructions

Follow the Conventional Commits format strictly for commit messages. Use the structure below:

```md
<type>(<optional scope>): <gitmoji> <description>

[optional body]

[optional footer(s)]
```

Guidelines:

1. **Types**
    - **`feat`**: Commits that add or remove a new feature to the API or UI.  
    - **`fix`**: Commits that fix a bug related to a previously introduced `feat`.
    - **`refactor`**: Commits that rewrite or restructure code without changing external behavior (no API or UI changes).
    - **`perf`**: Commits that improve performance without changing functionality (a type of `refactor`).
    - **`style`**: Commits that do not affect the code logic (e.g., formatting, white space, missing semicolons).
    - **`test`**: Commits that add missing tests or correct existing ones.
    - **`docs`**: Commits that affect only documentation (e.g., README, comments).
    - **`build`**: Commits that affect build system, dependencies, CI/CD pipeline, or versioning.
    - **`ops`**: Commits that relate to operational aspects like infrastructure, deployment, backups, etc.
    - **`chore`**: Miscellaneous commits, such as changes to `.gitignore`, updating metadata, or non-functional tooling.

2. **Scopes**
    - Describes the affected module or feature.
    - Don’t use issue IDs as scopes.
    - Example scopes (customize based on project):
        - **`ui`**
        - **`api`**
        - **`db`**
        - **`config`**
        - **`tests`**

3. **Gitmoji**
    - Include a relevant `gitmoji` that best represents the nature of the change.

4. **Description**
    - A concise summary of what the commit does.
    - Use **imperative, present tense**: “change” not “changed” or “changes”.
    - Think of it like: “This commit will...”
    - **Don’t** capitalize the first letter.
    - **No dot** (`.`) at the end.

5. **Body**
    - Explains the **motivation** behind the change.
    - Contrasts the new behavior with the **previous behavior**.
    - Use **imperative, present tense**: “change” not “changed” or “changes”.
    - Can include reasoning, edge cases, limitations, or decisions made.
    - Use **bullet points** (`*`) for clarity.
    - Clearly describe the motivation, context, or technical details behind the change, if applicable.

6. **Breaking Changes**
    - Should be indicated by an ! before the : in the subject line
    - Should be included in the footer section.

7. **Footer**
    - Reference related **issues**.
    - Place each entry on a **new line**.
    - **Breaking changes** should start with the phrase `BREAKING CHANGE:` followed by a clear explanation.
    - Avoid including non-functional or redundant information.

Commit messages should be clear, informative, and professional, aiding readability and project tracking.
