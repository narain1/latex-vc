# latex-vc Control and Automation

Welcome to the LaTeX Version Control and Automation repository. This repository is designed to maintain version control for LaTeX projects, automatically compile them into PDFs upon each commit, and publish releases when updates are merged into the main branch.

## Features

- **Version Control**: Keep track of all changes to your LaTeX documents and revert back to previous versions whenever needed.
- **Automated PDF Building**: Automatically compile LaTeX files into PDFs with every commit using GitHub Actions.
- **Automatic Release Publishing**: Automatically create a new release and publish the compiled PDFs when changes are merged to the main branch.

## Getting Started

### Prerequisites

Ensure you have `git` installed on your system to clone the repository and handle version control. Visit [Git's official site](https://git-scm.com/) for installation instructions.

### Setup

`just fork the repository and start editing your latex file`

### Workflow

* Edit and Commit Changes
* Make changes to your LaTeX files and commit them:
* git push origin feature-branch-name

#### Open a Pull Request
Go to the repository on GitHub, and open a pull request from your feature branch to the main branch.

#### Automated Build and Review
Upon creating a pull request, GitHub Actions will compile the LaTeX files into a PDF, which you can review in the Actions tab.

#### Merge Pull Request and Publish Release
Once the pull request is approved and merged, GitHub Actions will automatically compile the final version of the PDF and publish a release with the PDF attached.

## GitHub Actions

This repository uses GitHub Actions for Continuous Integration and Continuous Deployment (CI/CD). Here’s what happens under the hood:

* Build LaTeX PDF: Every push triggers the LaTeX compilation action that builds the PDFs.
* Publish PDF: When changes are merged to the main branch, another action creates a GitHub release and uploads the compiled PDFs.

You can customize the workflows by editing the .github/workflows files.
