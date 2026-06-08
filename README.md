# CI/CD Pipeline Basics using GitHub Actions

## Project Overview

This project demonstrates the fundamentals of Continuous Integration and Continuous Deployment (CI/CD) using GitHub Actions. The workflow is automatically triggered whenever code is pushed to the main branch. It performs basic validation steps and ensures that the project is successfully processed through an automated pipeline.

The purpose of this project is to understand DevOps automation concepts and gain hands-on experience with creating and managing CI/CD workflows.

---

## Objectives

- Understand the concepts of Continuous Integration (CI) and Continuous Deployment (CD).
- Create a basic automated workflow using GitHub Actions.
- Learn how pipelines are triggered automatically.
- Automate build verification steps.
- Gain practical experience with DevOps tools and workflows.

---

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Git
- GitHub
- GitHub Actions

---

## Project Structure

```text
CI_CD_PIPELINES/
│
├── index.html
├── style.css
├── script.js
├── README.md
│
└── .github/
    └── workflows/
        └── ci.yml
```

---

## CI/CD Workflow

The workflow is configured using GitHub Actions and is stored in:

```text
.github/workflows/ci.yml
```

### Workflow Steps

1. Trigger workflow on every push to the main branch.
2. Checkout repository code.
3. Verify project files.
4. Execute automated pipeline steps.
5. Display success message after completion.

---

## Workflow Configuration

```yaml
name: CI Pipeline

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Code
        uses: actions/checkout@v4

      - name: Check Files
        run: ls

      - name: Success Message
        run: echo "Pipeline Executed Successfully"
```

---

## How to Clone and Run

### Clone Repository

```bash
git clone https://github.com/hasinikalvakk-lang/CI_CD_PIPELINES.git
```

### Navigate to Project Folder

```bash
cd CI_CD_PIPELINES
```

### Open Project

Open `index.html` in your browser.

---

## Continuous Integration (CI)

Continuous Integration is the practice of automatically integrating code changes into a shared repository. Whenever code is pushed, the workflow automatically runs and verifies that everything is working correctly.

### Benefits

- Early error detection
- Faster development cycles
- Improved code quality
- Automated validation

---

## Continuous Deployment (CD)

Continuous Deployment automates the process of delivering software after successful validation and testing. It reduces manual effort and speeds up software delivery.

### Benefits

- Faster releases
- Reduced human errors
- Consistent deployments
- Improved productivity

---

## Workflow Execution

Whenever a developer pushes code to the repository:

```text
Developer Pushes Code
          ↓
GitHub Repository
          ↓
GitHub Actions Triggered
          ↓
Checkout Code
          ↓
Verify Files
          ↓
Build Successful
```

---

## Expected Output

The GitHub Actions workflow should complete successfully and display:

```text
Pipeline Executed Successfully
```

in the Actions logs.

---

## Learning Outcomes

Through this project, I learned:

- Basics of DevOps practices
- CI/CD concepts
- GitHub Actions workflow creation
- Pipeline automation
- Workflow execution monitoring
- Repository management using Git and GitHub

---

## Future Improvements

- Add automated testing.
- Add code quality checks.
- Deploy application automatically.
- Integrate notifications for workflow status.
- Implement multi-stage CI/CD pipelines.

---

## Author

**Hasini Kalva**

B.Tech Student | Aspiring Web Developer | DevOps Learner

GitHub: https://github.com/hasinikalvakk-lang

---

## Repository Link

https://github.com/hasinikalvakk-lang/CI_CD_PIPELINES
