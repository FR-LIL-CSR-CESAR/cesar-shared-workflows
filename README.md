# CESAR Reusable GitHub Workflows

This repository contains **reusable workflows** for GitHub Actions designed to be used across multiple projects. The goal is to centralize and standardize CI/CD automation for easier maintenance and evolution of workflows.

## 📌 How to Use These Workflows?

In your repository, you can call a workflow from this repository by adding an action in `.github/workflows/your_workflow.yml`:

```yaml
name: Example of Using a Reusable Workflow

on:
  push:
    branches:
      - main

jobs:
  call-workflow:
    uses: GITHUB_USERNAME/REPO_NAME/.github/workflows/WORKFLOW_NAME.yml@main
    with:
      parameter1: value1
      parameter2: value2
```
