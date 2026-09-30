```markdown
# first-contributions Development Patterns

> Auto-generated skill from repository analysis

## Overview

This skill introduces the development and contribution patterns of the `first-contributions` repository, a TypeScript-based project designed to help new contributors make their first open source contribution. The repository emphasizes simple, clear workflows for adding contributors, updating translations, and maintaining documentation. It follows consistent coding conventions and encourages collaborative, beginner-friendly practices.

## Coding Conventions

- **File Naming:**  
  Files are named using kebab-case.  
  _Example:_  
  ```
  add-contributor.ts
  contributors-list.test.ts
  ```

- **Import Style:**  
  Relative imports are used throughout the codebase.  
  _Example:_  
  ```typescript
  import { addContributor } from './add-contributor';
  ```

- **Export Style:**  
  Named exports are preferred.  
  _Example:_  
  ```typescript
  export function addContributor(name: string) { ... }
  ```

- **Commit Messages:**  
  Commit messages are freeform (no enforced prefix), averaging around 51 characters.  
  _Example:_  
  ```
  Add John Doe to Contributors.md
  ```

## Workflows

### Add Contributor to List
**Trigger:** When someone wants to add themselves or another person to the list of contributors.  
**Command:** `/add-contributor`

1. Open `Contributors.md`.
2. Add a new line with the contributor's name (optionally with a link or additional info).
   ```markdown
   - John Doe
   ```
3. Commit the change with a message referencing the addition.
   ```
   Add John Doe to Contributors.md
   ```
4. Open a pull request for review or auto-merge.

---

### Add or Update README Translation
**Trigger:** When someone wants to contribute a new translation or update an existing translation of the README.  
**Command:** `/add-readme-translation`

1. Edit or create `docs/translations/README.[lang].md` for the target language.
   ```
   docs/translations/README.es.md
   ```
2. Optionally, update `Contributors.md` to credit the translator.
3. Commit the changes with a message referencing the translation.
   ```
   Add Spanish translation for README
   ```
4. Open a pull request.

---

### Fix Contributors List Formatting
**Trigger:** When someone notices formatting issues, duplicate names, or syntax errors in `Contributors.md`.  
**Command:** `/fix-contributors-formatting`

1. Open `Contributors.md`.
2. Fix formatting, remove duplicates, or correct syntax.
   ```markdown
   - Jane Doe
   - John Doe
   ```
3. Commit the change with a message referencing the fix.
   ```
   Fix duplicate entries in Contributors.md
   ```
4. Open a pull request.

---

### Merge Branch or Pull Request
**Trigger:** When a feature, fix, or contributor addition branch is ready to be merged into main.  
**Command:** `/merge-branch`

1. Merge the feature/contributor/translation branch into `main`.
2. Resolve any merge conflicts if present.
3. Commit the merge.
4. Push to the repository.

---

## Testing Patterns

- **Test File Naming:**  
  Test files use the pattern `*.test.*`.  
  _Example:_  
  ```
  add-contributor.test.ts
  ```

- **Testing Framework:**  
  The specific testing framework is not detected, but standard TypeScript test patterns apply.

- **Test Example:**  
  ```typescript
  import { addContributor } from './add-contributor';

  test('adds a contributor', () => {
    expect(addContributor('Jane Doe')).toContain('Jane Doe');
  });
  ```

## Commands

| Command                     | Purpose                                                        |
|-----------------------------|----------------------------------------------------------------|
| /add-contributor            | Add a new contributor to Contributors.md                       |
| /add-readme-translation     | Add or update a README translation in docs/translations        |
| /fix-contributors-formatting| Fix formatting or duplicates in Contributors.md                |
| /merge-branch               | Merge a feature, fix, or contributor branch into main          |
```
