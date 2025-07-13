# Development Operations

## What is Devops?

### 🤔 Definition:

DevOps consists of practices and tools aimed at streamlining and automating the software development and operations lifecycle.

### 🧑‍🤝‍🧑 Collaboration:

It bridges the gap between development (Dev) and operations (Ops) teams, promoting better communication and teamwork.

### 🏎️ Continuous Processes:

Key practices include Continuous Integration (CI), Continuous Delivery (CD), and Continuous Deployment, enabling faster and more reliable software releases.

### 🤖 Automation:

DevOps automates tasks such as testing and deployment to improve efficiency and reduce human error.

### 🔭 Monitoring & Feedback:

Strong focus on monitoring applications and systems to gather feedback, ensure performance, and adapt quickly to changes.

## Other Options

Github, Azure Devops, GitLab, Jenkins, Bitbucket, CircleCI, TeamCity, Octopus deploy, Harness, Codefresh offer similar.

## Github or Azure Devops ?

### The Relationship Between GitHub and Azure DevOps

Rather than pick one or the other we can use them both.

🤝 Shared Ownership: Both platforms are owned and actively developed by Microsoft, which means they’re designed to complement each other rather than compete.

↘️ Integrated Workflows: You can link Azure Boards to GitHub commits, pull requests, and issues, enabling full traceability from planning to deployment.

⚔️ Cross-Platform CI/CD: Azure Pipelines can build and deploy code from GitHub repositories, and GitHub Actions can trigger Azure services, creating a hybrid DevOps pipeline.

🏳️‍🌈 Unified Licensing: GitHub Enterprise licenses now include Azure DevOps Basic usage rights, streamlining access across both platforms.

🪪 Security Synergy: GitHub Advanced Security features like secret scanning and code analysis are being integrated into Azure DevOps via GHAzDO (GitHub Advanced Security for Azure DevOps).

## They are Similar!

    - Aspect GitHub Azure DevOps
    - Version Control Git-based repositories Git or TFVC repositories
    - CI/CD GitHub Actions vs Azure Pipelines
    - Project Management GitHub Projects (lightweight) vs Azure Boards (Agile-focused)
    - Package Hosting GitHub Packages vs Azure Artifacts
    - Security Tools CodeQL, Dependabot, Secret Scanning GHAzDO (via GitHub integration)
    - IDE Integration with VS Code, Visual Studio, JetBrains etc

### 🔍 GitHub vs Azure DevOps: Main Feature Breakdown

| Feature                       | Description                                                  | Example                                         |             GitHub              |        Azure DevOps        |
| ----------------------------- | ------------------------------------------------------------ | ----------------------------------------------- | :-----------------------------: | :------------------------: |
| **Tags (Git)**                | Labels pointing to specific commits, often used for releases | `git tag v1.0.0`                                |               ✅                |             ✅             |
| **Git Hooks (Client-side)**   | Scripts triggered by Git events on local machines            | `pre-commit` hook to run linting before commits |               ✅                |  ❌ _(server-side only)_   |
| **Webhooks**                  | HTTP callbacks triggered by repo events                      | Trigger CI build when code is pushed            |               ✅                |             ✅             |
| **Service Hooks**             | Azure-specific integrations with external services           | Create Trello card when a work item is created  |               ❌                |             ✅             |
| **Branch Protection Rules**   | Enforce rules on branches to prevent unwanted changes        | Require PR reviews before merging to `main`     |               ✅                | ✅ _(via Branch Policies)_ |
| **Pull Request Templates**    | Predefined content for PR descriptions                       | Auto-fill checklist in every PR                 |               ✅                |             ✅             |
| **CI/CD Pipelines**           | Automate build, test, and deployment workflows               | Run tests and deploy on push to `main`          |      ✅ _(GitHub Actions)_      |   ✅ _(Azure Pipelines)_   |
| **Artifact Publishing**       | Store and share build outputs or packages                    | Publish NuGet package or Docker image           |     ✅ _(GitHub Packages)_      |   ✅ _(Azure Artifacts)_   |
| **Work Item Tracking**        | Manage tasks, bugs, and features                             | Create user story with tags and priority        |               ❌                |       ✅ _(Boards)_        |
| **Dashboard & Reporting**     | Visualize project metrics and progress                       | Burn-down charts, velocity reports              |               ❌                |             ✅             |
| **Feature Flags Integration** | Toggle features on/off without redeploying code              | Enable beta feature for select users            | ✅ _(via Actions or 3rd-party)_ |   ✅ _(via Extensions)_    |

[Return](https://github.com/uerbzr/course-devops)
