# Metaflow CI/CD: Kubernetes Integration Testing with GitHub Actions

## Overview
This repository contains the implementation of **Metaflow CI/CD integration tests on Kubernetes** using **GitHub Actions**. The project automates running Metaflow flows against a production-like Kubernetes environment, ensuring seamless testing, faster PR validation, and reliable CI/CD pipelines.

The system leverages:
- **Metaflow Dev Stack** (Kind + Argo Workflows)
- **GitHub Actions** for automation
- **Pytest** for test result aggregation
- **Runner & Deployer APIs** for programmatic flow execution

---

## Key Features
- Automated **Kubernetes integration tests** for every PR
- **Reusable GitHub Actions workflow** for CI/CD
- Multi-backend **test result aggregation**
- **PR status reporting** via GitHub check runs
- Selective test execution with **pytest markers**
- Documentation for running tests locally

---

## Why This Matters
- **Early detection of integration bugs** before merging
- **Confidence in contributions** on production-like infrastructure
- **Faster release cycles** with reduced manual QA
- Strengthened **Metaflow ecosystem** for developers

---

## Architecture
[CI/CD Pipeline] -> [GitHub Actions] -> [Metaflow Dev Stack on Kubernetes] -> [Runner/Deployer API] -> [Test Results Aggregation]

- **Dynamic integration testing** ensures every PR is validated against a real Kubernetes environment.
- **Modular design** allows adding new test backends easily.
