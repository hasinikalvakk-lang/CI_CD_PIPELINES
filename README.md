# CI/CD Pipeline Basics

## Project Overview
This project demonstrates the fundamentals of Continuous Integration and Continuous Deployment (CI/CD) using GitHub Actions.

The workflow automatically runs whenever code is pushed to the main branch, helping ensure that the project files are validated and the build process executes successfully.

## Technologies Used
- HTML
- CSS
- JavaScript
- GitHub Actions
- Git

## Project Structure

ci-cd-demo/
│
├── index.html
├── style.css
├── script.js
└── .github/
    └── workflows/
        └── ci.yml

## CI/CD Workflow

The GitHub Actions workflow performs the following steps:

1. Trigger on push to the main branch
2. Checkout repository code
3. Verify project files
4. Display a success message

## Workflow File

Location:

.github/workflows/ci.yml

## How to Run

1. Clone the repository:
   ```bash
   git clone <repository-url>
