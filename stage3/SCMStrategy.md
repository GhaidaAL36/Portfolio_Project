## SCM Strategy (Source Code Management)

### Version Control & Branching
Madar will use **Git** as the main version control system, with a remote repository hosted on **GitHub**.

We will follow a **feature-based branching model**:

| Branch | Purpose |
| --- | --- |
| `main` | Production-ready and stable version of the application |
| `development` | Integration branch where completed features are merged and tested together |
| `feature/` | Each new feature or module is developed in a separate branch |

### Workflow Process

1. A team member creates a feature branch from `development`
2. Implements the assigned task
3. Commits changes frequently with clear commit messages
4. Pushes the code to the repository
5. A code review is performed by another team member
6. After approval, the code is merged into `development`
7. Once stable, `development` is merged into `main` for release

### Code Quality Rules

- No direct commits to `main`
- Mandatory code review before merging
- Consistent commit messages (e.g., `feat: add AI task generator`)

---

## QA Strategy (Quality Assurance)

We will use a combination of the following testing approaches:

| Testing Type | Description |
| --- | --- |
| **Unit Testing** | Tests individual functions and components in isolation |
| **Integration Testing** | Ensures that different modules work together correctly |
| **End-to-End Testing** | Simulates real user behavior across the full system |

### API & AI Validation

- **Postman** will be used for testing API requests and responses
- Validation of AI-generated output format, consistency, and correctness will be performed to ensure reliable task simulations
