# 🚀 GitHub Actions – Zero to Advanced

![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-blue?logo=githubactions&logoColor=white)
![YAML](https://img.shields.io/badge/YAML-Configuration-red?logo=yaml)
![DevOps](https://img.shields.io/badge/Domain-DevOps-orange)
![Status](https://img.shields.io/badge/Status-Learning%20%26%20Practice-success)

## 📌 About This Project

This repository contains my hands-on learning and practical implementation of **GitHub Actions**, from beginner to advanced level.

The main objective is to understand how GitHub Actions automates software development workflows through Continuous Integration (CI) and Continuous Delivery/Deployment (CD).

I am exploring different workflow configurations, YAML syntax, automation techniques, multi-job pipelines, security practices, and Docker image publishing.

## 🎯 Learning Objectives

- Understand CI/CD concepts and GitHub Actions architecture.
- Learn YAML syntax and workflow configuration.
- Automate build, test, and deployment processes.
- Implement single-job and multi-job workflows.
- Understand workflow triggers, runners, and environments.
- Manage secrets, variables, and permissions.
- Implement matrix builds, caching, and artifacts.
- Build secure and reusable CI/CD pipelines.
- Integrate Docker with GitHub Actions.

## 📚 Learning Roadmap

### 📅 Day 1 – GitHub Actions Fundamentals
- Introduction to CI/CD
- Introduction to YAML
- Anatomy of a workflow
- Workflow triggers (`push`, `pull_request`, `workflow_dispatch`, `schedule`)
- GitHub-hosted runners
- `run` vs `uses`
- GitHub Marketplace Actions
- `actions/checkout`
- `actions/setup-node`

### 📅 Day 2 – Building CI/CD Pipelines
- Environment variables and scopes
- Contexts and expressions
- Secrets and repository variables
- First CI pipeline
- Parallel jobs
- Job dependencies (`needs`)
- Conditional execution (`if`)
- Status functions

### 📅 Day 3 – Advanced Workflow Management
- Job outputs
- Matrix builds
- Matrix `include` and `exclude`
- `fail-fast` and `max-parallel`
- Dependency caching
- Workflow artifacts
- Artifact merging
- Reusable workflows
- Composite actions

### 📅 Day 4 – Production Deployment
- GITHUB_TOKEN and permissions
- Least-privilege security
- GitHub Environments
- Deployment approvals
- Concurrency management
- Timeouts and error handling
- Self-hosted runners
- Production CI/CD pipeline

### 📅 Day 5 – Advanced GitHub Actions & Security
- Supply-chain security and SHA pinning
- CodeQL code scanning
- Secret scanning and push protection
- Pull request security
- OIDC cloud authentication
- Workflow chaining
- Monorepo change detection
- Docker image build and push to GHCR
- Custom JavaScript actions
- Custom Docker actions
- Debugging workflows using `act`
- Hardened CI/CD pipeline

## 🛠️ Technologies & Tools

| Category | Technologies |
|---|---|
| CI/CD | GitHub Actions |
| Version Control | Git, GitHub |
| Configuration | YAML |
| Containers | Docker |
| Container Registry | GitHub Container Registry (GHCR) |
| Security | CodeQL, Secret Scanning, SHA Pinning |
| Cloud Authentication | AWS OIDC |
| Automation | Bash, GitHub Workflows |
| Development | Node.js, npm |

## 📂 Repository Structure

```text
Dveops_GitHub_Action/
│
├── .github/
│   └── workflows/
│       └── CI-CD workflows
│
├── day-01/
│   ├── workflows/
│   └── actions/
│
├── day-02/
│   ├── workflows/
│   └── actions/
│
├── day-03/
│   ├── workflows/
│   └── actions/
│
├── day-04/
│   ├── workflows/
│   └── actions/
│
├── day-05/
│   ├── workflows/
│   └── actions/
│
├── sample-app/
│
└── README.md
```

*Note: This is the planned learning structure. Add the folders and files as you implement each exercise.*

## ⚙️ How GitHub Actions Works

```text
Developer
    |
    v
GitHub Repository
    |
    v
Workflow Trigger
    |
    v
GitHub Actions Runner
    |
    v
Build
    |
    v
Test
    |
    v
Deploy
    |
    v
Application Delivery
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/PurushothIT/Dveops_GitHub_Action.git
```

### 2. Navigate to the Project

```bash
cd Dveops_GitHub_Action
```

### 3. Create a Workflow

Create a YAML file inside:

```text
.github/workflows/
```

Example:

`hello-world.yml`

```yaml
name: My First GitHub Action

on:
  push:
    branches:
      - main

jobs:
  hello:
    runs-on: ubuntu-latest

    steps:
      - name: Print Message
        run: echo "Hello GitHub Actions!"
```

### 4. Push Changes to GitHub

```bash
git add .
git commit -m "Add GitHub Actions workflow"
git push origin main
```

### 5. Verify Workflow Execution

1. Open your GitHub repository.
2. Navigate to the Actions tab.
3. Select your workflow.
4. Check the execution logs.
5. Verify whether the workflow completed successfully.

## 📖 Key Concepts Learned

| Concept | Purpose |
|---|---|
| Workflow | Defines an automated process |
| Trigger | Defines when a workflow executes |
| Runner | Machine that executes workflow jobs |
| Job | Collection of workflow steps |
| Step | Individual task inside a job |
| Secrets | Securely stores sensitive information |
| Matrix | Executes jobs across multiple configurations |
| Artifacts | Stores and shares workflow files |
| Reusable Workflow | Reuses complete jobs |
| Composite Action | Reuses multiple steps |
| OIDC | Enables keyless cloud authentication |

## 🎯 Final Goal

Build a production-ready CI/CD pipeline using GitHub Actions with automated testing, Docker image creation, security scanning, and deployment automation.

## 👨‍💻 Author

**Purushoth G**

- GitHub: [@PurushothIT](https://github.com/PurushothIT)
- Repository: [Dveops_GitHub_Action](https://github.com/PurushothIT/Dveops_GitHub_Action)

---

⭐ If you find this repository useful, feel free to explore and learn from the workflows.

**Learning by Doing | Building Real-World DevOps Skills**
