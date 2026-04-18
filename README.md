# CI/CD Final Project

## Project Name: Build and Deploy a CI/CD Pipeline with GitHub Actions, Tekton, and OpenShift

This project demonstrates building a complete CI/CD pipeline using:
- **GitHub Actions** for continuous integration (linting and unit testing)
- **Tekton** for task management and pipeline orchestration
- **OpenShift** for container deployment

## Project Details

- **Student:** G Srujan (Srujan5114)
- **Course:** IBM DevOps and Software Engineering - Continuous Integration and Delivery (CI/CD)
- **Platform:** IBM Skills Network / Coursera

## Repository Structure

- `.github/workflows/workflow.yml` - GitHub Actions CI workflow (lint with flake8, unit tests with nose)
- `.tekton/tasks.yml` - Tekton tasks (cleanup, nose test, git-clone, buildah, deploy)
- `labs/` - Lab reference files for each pipeline stage
- `service/` - Application source code (Flask Python service)
- `tests/` - Unit tests

## CI/CD Pipeline Overview

### GitHub Actions Workflow
- Lint service code with flake8
- Run unit tests with nosetests

### Tekton Pipeline
- cleanup: Clean workspace
- git-clone: Clone repository
- flake8: Lint code
- nose: Run unit tests
- buildah: Build container image
- deploy: Deploy to OpenShift

## Labs Completed

- Lab 1: Build an empty Pipeline
- Lab 2: Adding GitHub Triggers
- Lab 3: Use Tekton CD Catalog
- Lab 4: Integrate Unit Test Automation
- Lab 5: Building an Image
- Lab 6: Deploy to Kubernetes/OpenShift
