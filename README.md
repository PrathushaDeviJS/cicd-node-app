## CI/CD Implementation

This project implements a CI/CD pipeline using GitHub Actions, Docker, Trivy, and AWS ECR.

- Created a simple Node.js/Express web application with a `/health` endpoint.
- Dockerized the application using a Dockerfile.
- Tested the Docker container locally.
- Created a GitHub Actions workflow to automate the CI/CD process.
- Automated dependency installation and application testing.
- Automated Docker image building.
- Integrated Trivy to scan the Docker image for HIGH and CRITICAL vulnerabilities.
- Configured AWS authentication using GitHub Secrets.
- Created a private Amazon ECR repository.
- Automatically pushed the Docker image to ECR using the Git commit SHA as the image tag.

### Current Pipeline

GitHub Push → Install Dependencies → Run Tests → Docker Build → Trivy Scan → Push Image to Amazon ECR

### Current Status

The CI pipeline, security scanning, Docker build, and ECR image push have been successfully implemented and verified.

