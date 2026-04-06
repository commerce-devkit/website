# AGENTS.md

## Purpose

This repository uses the Hugo static site generator. Agents (human or AI) contributing here must follow consistent structure, content practices, and commit conventions to keep the project maintainable and readable.

---

## Repository Overview

- Static site built with Hugo
- Content lives in `/content`
- Layouts in `/layouts`
- Static assets in `/static`
- Configuration in `hugo.toml` (or `.yaml` / `.json`)

---

## General Guidelines

- Prefer clarity over cleverness
- Keep content and templates simple and maintainable
- Avoid introducing unnecessary dependencies or build complexity
- Follow existing patterns before introducing new ones
- Ensure generated output builds without warnings

---

## Hugo-Specific Practices

- Use front matter consistently (`title`, `date`, `draft`, etc.)
- Keep content in Markdown unless there is a strong reason otherwise
- Use archetypes when creating new content
- Do not commit generated `/public` files unless explicitly required
- Validate changes with:

  ```bash
  hugo server
  ```

- Ensure no broken links or missing assets

---

## Conventional Commits

All commits MUST follow the Conventional Commits specification:

```
<type>(optional scope): <short summary>
```

### Allowed Types

- `feat` — new content, feature, or page
- `fix` — corrections (typos, broken links, config issues)
- `docs` — documentation-only changes
- `style` — formatting, whitespace, no content change
- `refactor` — restructuring without changing output
- `perf` — performance improvements
- `build` — build system or dependency changes
- `ci` — CI/CD changes
- `chore` — maintenance tasks

### Scope (Optional)

Use scope when helpful:

- `content`
- `layout`
- `theme`
- `config`
- `assets`
- `seo`

Example:

```
feat(content): add article on static site performance
```

---

## Commit Message Style (50/72 Rule)

### Structure

```
<type>(scope): <subject line>

<body>
```

### Subject Line

- Max **50 characters**
- Imperative mood ("add", not "added")
- No trailing period
- Be specific and concise

### Body

- Wrap at **72 characters**
- Explain _why_, not just _what_
- Use full sentences and paragraphs
- Write for humans, not machines
- Include context, tradeoffs, and intent when useful

---

## Example Commit

```
feat(content): add guide on Hugo image optimization

This introduces a new guide explaining how to optimize images
in Hugo using built-in processing features. It focuses on
practical examples and avoids external tooling to keep the
workflow simple.

The goal is to improve page load performance while keeping
the authoring experience straightforward for contributors.
```

---

## What to Avoid

- One-line commits with no context (unless trivial)
- Vague messages like "update stuff" or "fix things"
- Overly long subject lines
- Mixing unrelated changes in a single commit
- Auto-generated or machine-style commit messages

---

## Pull Request Expectations

- Keep PRs focused and small
- Include a clear description of changes
- Reference related issues if applicable
- Ensure the site builds successfully
- Preview changes locally before submitting

---

## Agent-Specific Instructions

- Always infer appropriate commit type and scope
- Rewrite commit messages to match this standard if needed
- Prefer multiple small commits over one large commit
- When generating content, ensure it matches existing tone and structure
- Do not introduce breaking structural changes without explicit instruction

---

If you want, I can tailor this further (e.g., add multilingual content rules, SEO checklist, or CI integration).
