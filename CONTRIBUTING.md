# Contributing

Thank you for considering a contribution to the Commerce DevKit website! Please
follow the guidelines below to keep the project history clean.

---

## Conventional Commits

All commits **must** follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification:

```
<type>(<optional scope>): <description>

[optional body]

[optional footer(s)]
```

### Commit Types

| Type       | When to use                                             |
| ---------- | ------------------------------------------------------- |
| `feat`     | A new feature or component input                        |
| `fix`      | A bug fix                                               |
| `docs`     | Documentation changes only                              |
| `refactor` | Code change that neither fixes a bug nor adds a feature |
| `ci`       | Changes to CI/CD pipeline configuration                 |
| `chore`    | Maintenance tasks (dependency updates, tooling, etc.)   |
| `test`     | Adding or updating tests                                |
| `perf`     | Performance improvements                                |
| `revert`   | Reverts a previous commit                               |

---

## Branch Naming

| Pattern                       | Purpose             |
| ----------------------------- | ------------------- |
| `feature/<short-description>` | New features        |
| `fix/<short-description>`     | Bug fixes           |
| `release/<version>`           | Release preparation |
| `chore/<short-description>`   | Maintenance/tooling |
| `docs/<short-description>`    | Documentation only  |

---

## Workflow

1. Fork the repository.
1. Branch from `main` in your fork.
1. Make your changes following the commit conventions above.
1. Open a Pull Request targeting `main` in the upstream repository.

---

## Pull Request Guidelines

- Keep PRs focused — one concern per PR.
- Reference related issues in the PR description (e.g. `Closes #12`).
- Squash commits when merging unless individual commit history is meaningful.
- All pipeline checks must pass before merging.
