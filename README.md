# Regular Exam – 23 February 2025

This repository contains my solution for the **Regular Exam** in the _DevOps for Developers_ module @ SoftUni.

## Project Description

The project is based on a simple .NET application with unit and integration tests. The goal of the exam was to apply core DevOps practices, including CI/CD configuration with GitHub Actions and Jenkins, working with Git branches, and managing pull requests between environments.

---

## Tasks Completed

### 1. Resource Setup
- Forked the original repository provided by SoftUni.
- Cloned the forked repository to my local environment.
- Opened the solution and verified that the application builds correctly without errors.

### 2. Git & GitHub
- Worked with Git and GitHub to manage branches and commits.
- Created a feature branch following Git Flow principles.

### 3. GitHub Actions CI/CD Pipeline
- Set up a GitHub Actions workflow with the following behavior:
  - **On push to `develop` branch:** Runs all **unit tests**.
  - **On push to `staging` branch:** Triggers **integration tests**.
- The pipeline includes steps for:
  - Checkout
  - Build
  - Test (unit/integration depending on branch)

### 4. Branching Strategy
- Created and worked in a feature branch named: `feature-ci-pipeline`.
- Implemented the GitHub Actions configuration in this branch.

### 5. Jenkins CI Pipeline
- Configured a **Jenkins pipeline** to build the app and run all tests.
- The Jenkins pipeline is triggered on changes pushed to the `feature-ci-pipeline` branch.
- The setup includes:
  - Build stage
  - Test execution
  - Console output to verify success

### 6. Pull Requests Workflow
- Created a Pull Request from `feature-ci-pipeline` to `develop` (for peer review and merging).
- Created a Pull Request from `develop` to `staging` to simulate promotion to staging environment.
- Finally, created a Pull Request from `staging` in the forked repo to the original repository’s `staging` branch.

---

## Technologies Used

- Git & GitHub
- GitHub Actions
- Jenkins
- .NET
- Unit & Integration Testing

---

## Notes

The exam was designed to simulate a real-world CI/CD pipeline setup using both GitHub Actions and Jenkins. The project helped reinforce key DevOps skills including:
- Automation of builds and tests
- Multi-environment workflows
- Infrastructure as Code (via CI pipelines)
- Branching strategies and team collaboration practices

---
