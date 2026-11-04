# Day 4 – Docker and Continuous Integration

## 1. Docker Images
- Docker images package application code, dependencies, and configuration.
- They are used to create containers.

## 2. Docker Commands
- `docker build -t day9-api ./day9-api` – Builds API image.
- `docker build -t day9-web ./day9-web` – Builds Web image.
- `docker images` – Lists available images.
- `docker pull python:3.12` – Downloads a base image.

## 3. GitHub Actions
- GitHub's automation platform for CI/CD.
- Workflows are written in YAML.
- Workflow files are stored in `.github/workflows/`.

## 4. Important Concepts
- Workflow: Complete automation process.
- Job: Group of tasks.
- Step: Individual task.
- Runner: Machine that executes jobs.
- Trigger: Event that starts a workflow.

## 5. Workflow Triggers
- `push`: Runs when code is pushed.
- `pull_request`: Runs on pull request events.
- `workflow_dispatch`: Starts a workflow manually.

## 6. Our Docker CI Pipeline
1. Developer pushes code to GitHub.
2. GitHub Actions starts the workflow.
3. Repository code is checked out.
4. API Docker image is built.
5. Web Docker image is built.
6. Build results are displayed.

## 7. CI/CD Concepts
- **Continuous Integration (CI):** Automatically integrates, builds, and tests code.
- **Continuous Delivery:** Keeps code ready for production; deployment may require manual approval.
- **Continuous Deployment:** Automatically deploys successfully tested code to production.

## 8. Practical Work Completed
- Inspected API and Web Dockerfiles.
- Built both Docker images locally.
- Created a GitHub Actions workflow.
- Automated Docker image builds.
- Pushed the workflow to GitHub.
- Verified successful execution with a green tick.

## Key Takeaway
GitHub Actions automates Docker image building, reduces manual work, and helps detect build errors early.