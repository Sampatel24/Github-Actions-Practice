# This is GitHub Actions Practice Repo

## Practice Workflows

- [First Github Action page Hello](.github/workflows/hello.yml)
- [CICD Demo](.github/workflows/cicd.yml)
- [Portfolio Website using GitHub Action](.github/workflows/portfolio-deploy.yml)
- [GitHub Action Matrix Strategy using Python Lint](.github/workflows/python-matrix.yml)
- [GitHub Action Docker Build & Push(CI) for flask app](.github/workflows/docker-built-push.yml)
- [GitHub Action Self-hosted Runner for flask app deployment(CD)](.github/workflows/deploy-app.yml)

## DevSecOps Pipeline
#### We will apply DevSecOps principles for above python flask app for security pipeline practice

### 1. CI (Continuous Integration with Security Scanning) 

#### Step-1: Code Quality Checks and Vulnerabilities Scan

- Lint and SAST [Check Code Quality using Flake and Bandit](.github/workflows/code-quality.yml)
- GitLeaks [Secrets Scan to check sensitive data using GitLeaks](.github/workflows/secrets-scan.yml)
- Pip Audit [Dependency Scan to check package vulnerablities using Pip Audit](.github/workflows/dependency-scan.yml)
- Hadolint [Scan Docker file to check errors using Hadolint](.github/workflows/docker-lint.yml)

#### Step-2: Build once the security scans are successfull

- [Docker Build and Push](.github/workflows/docker-built-push.yml)

#### Step-3: Scan built docker image

- Trivy [Scan docker image for CVEs using Trivy](.github/workflows/image-scan.yml)


### 2. CD (Continuous Deployment)

- Appleboy [Deploy to Production/Server(i.e AWS EC2 Instance) via SSH using Appleboy](.github/workflows/deploy-to-server.yml)


### 3. DevSecOps End To End Pipeline
#### This workflow defines a DevSecOps pipeline that will connects the other workflows together.

- [DevSecOps Pipeline](.github/workflows/devsecops-pipeline.yml)