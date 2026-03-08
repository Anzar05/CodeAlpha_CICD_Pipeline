# CI/CD Pipeline using GitHub Actions

## CodeAlpha DevOps Internship – CI/CD Task

This project demonstrates a simple Continuous Integration (CI) pipeline using GitHub Actions. The pipeline automatically runs whenever code is pushed to the repository.

------------------------------------------------------------

## Project Objective

The objective of this project is to understand how CI/CD pipelines automate the process of building and running applications.

Main goals:
- Learn Continuous Integration concepts
- Create a CI pipeline using GitHub Actions
- Automatically run code when changes are pushed
- Understand workflow automation

------------------------------------------------------------

## Technologies Used

GitHub  
GitHub Actions  
Python  
CI/CD Pipeline  

------------------------------------------------------------

## Project Structure

CodeAlpha_CICD_Pipeline
│
├── app.py
├── README.md
└── .github
    └── workflows
        └── ci.yml

------------------------------------------------------------

## Application Code

app.py

print("Hello from CodeAlpha CI/CD Pipeline!")

------------------------------------------------------------

## GitHub Actions Workflow

File Location:

.github/workflows/ci.yml

Workflow Code:

name: CI Pipeline

on:
  push:
    branches:
      - main

jobs:
  build:

    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Setup Python
        uses: actions/setup-python@v4
        with:
          python-version: '3.10'

      - name: Run Script
        run: python app.py

------------------------------------------------------------

## How the Pipeline Works

1. Developer pushes code to the GitHub repository
2. GitHub Actions detects the push event
3. The CI workflow is triggered automatically
4. Python environment is prepared
5. The script is executed

------------------------------------------------------------

## Output

Hello from CodeAlpha CI/CD Pipeline!

------------------------------------------------------------

## Key Learnings

- Basics of Continuous Integration
- Workflow automation using GitHub Actions
- Creating CI pipelines
- Running applications automatically after code changes

------------------------------------------------------------

## Internship Information

Internship Provider: CodeAlpha  
Domain: DevOps  
Task: CI/CD Pipeline Implementation

------------------------------------------------------------

## Author

Shaik Mahamood Anzar

DevOps Intern – CodeAlpha
