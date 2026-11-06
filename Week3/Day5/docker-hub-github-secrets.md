# Day 5 – Docker Hub and GitHub Secrets

## 1. Docker Hub

Docker Hub is a cloud-based registry used to store and share Docker images.

## 2. Important Docker Commands

- `docker build`: Builds a Docker image.
- `docker tag`: Assigns a name to an image.
- `docker push`: Uploads an image to Docker Hub.
- `docker pull`: Downloads an image from Docker Hub.
- `docker login`: Authenticates with Docker Hub.

## 3. GitHub Secrets

GitHub Secrets securely stores sensitive information used by GitHub Actions workflows.

Examples:
- Docker Hub username.
- Docker Hub access token.
- API keys.
- Deployment credentials.

Never write passwords or tokens directly in workflow files.

## 4. Docker Hub Authentication

Our GitHub repository uses two secrets:

- `DOCKER_USERNAME`: Docker Hub username.
- `DOCKER_TOKEN`: Docker Hub access token.

GitHub Actions accesses them using:

`${{ secrets.DOCKER_USERNAME }}`
`${{ secrets.DOCKER_TOKEN }}`

## 5. Docker CI/CD Pipeline

1. Developer pushes code to GitHub.
2. GitHub Actions starts the workflow.
3. Repository code is checked out.
4. GitHub Actions logs in to Docker Hub.
5. API Docker image is built.
6. Web Docker image is built.
7. Both images are pushed to Docker Hub.

## 6. Practical Work Completed

- Created Docker Hub repositories: `day9-api` and `day9-web`.
- Generated a Docker Hub personal access token.
- Added GitHub repository secrets.
- Configured Docker Hub login in GitHub Actions.
- Automated API and Web image builds.
- Automated image publishing to Docker Hub.
- Verified successful workflow execution.

## 7. Important Security Practices

- Never commit access tokens to GitHub.
- Use GitHub Secrets for sensitive credentials.
- Give tokens only the permissions they require.
- Rotate or revoke exposed tokens.

## Key Takeaway

GitHub Actions can automatically build and publish Docker images to Docker Hub using securely stored GitHub Secrets.