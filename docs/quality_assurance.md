# Testing Strategy, Quality Assurance, and CI/CD Planning

## Overview

The goal of this workshop is to help students design and organize a professional testing and quality assurance strategy for their CAPSTONE software development projects.

Modern software projects require more than simply writing code. Teams must also establish reliable processes for:

- Verifying software quality
- Preventing regressions
- Automating testing
- Managing deployments
- Maintaining code reliability over time

In this workshop, students will plan and document the testing strategy for their project while also configuring Continuous Integration / Continuous Deployment (CI/CD) pipelines using GitHub Actions.

This workshop focuses on:

- Testing planning
- Quality assurance processes
- Automated testing
- GitHub-based CI/CD pipelines

## Learning Objectives

By the end of this workshop, students should be able to:

- Identify and explain different types of software testing
- Design a testing strategy appropriate for their CAPSTONE project
- Define quality assurance responsibilities within the team
- Configure automated CI/CD workflows using GitHub Actions
- Automatically run tests and linters during Pull Requests
- Understand the relationship between testing and professional software development workflows

---

## 1. Testing Strategy Document

Each group must create a Markdown document describing their quality assurance strategy for their CAPSTONE project.

Suggested filename:

```text
/docs/QA.md
```

## Required Sections

The document must contain the following sections.

### A. Testing Goals

Describe:

- Why testing is important for the project
- The risks the team is attempting to reduce
- What types of failures would be most critical

Examples:

- Authentication failures
- Data corruption
- AI hallucinations
- Incorrect calculations
- Security vulnerabilities
- API failures

### B. Planned Types of Testing

Students must explain how they plan to use multiple forms of testing.

#### Unit Testing

Explain:

- What components/functions will be unit tested
- Which testing framework will be used (examples: Jest, PyTest, etc.)
- Expected minimum coverage goals

#### Integration Testing

Explain:

- Which parts of the system require integration testing
- Which APIs or databases will be tested together

Examples:

- Authentication + Database
- Backend + AI APIs
- Frontend + Backend communication

#### End-to-End (E2E) Testing

Explain:

- Which complete user workflows should be tested

Examples:

- User registration
- Login
- Checkout/payment process
- AI prompt submission workflow

#### Manual Testing

Describe:

- What types of testing will still require manual verification
- How usability testing or visual verification will be performed

#### Performance / Load Testing

Explain:

- Whether the team plans to test scalability or performance
- Which components might become bottlenecks

Examples:

- AI API latency
- Database performance
- High traffic scenarios

#### Security Testing

Describe:

- Security concerns relevant to the project

Examples:

- SQL Injection
- Authentication weaknesses
- Rate limiting
- API key exposure
- Insecure user input handling

## C. Pull Request Quality Rules

Students must define quality rules for Pull Requests.

Examples:

- Pull Requests must pass all automated tests
- Pull Requests must be reviewed by another team member
- No direct pushes to `main`
- CI checks must succeed before merging

---

## 2. CI/CD Setup Using GitHub Actions

Each group must configure at least one GitHub Actions workflow.

The workflow must automatically execute whenever:

- A Pull Request is created
- Code is pushed to the repository

### Required CI/CD Features

The workflow must include at least:

#### Repository Checkout

Example:

```yaml
- name: Checkout repository
  uses: actions/checkout@v4
```

#### Dependency Installation

The workflow should install required dependencies.

Examples:

```yaml
npm install
```
or

```yaml
pip install -r requirements.txt
```

#### Automated Testing

The workflow must automatically execute tests.

Examples:

```yaml
npm test
```
or

```yaml
pytest
```

#### Linting or Static Analysis

Students must configure at least one quality verification tool.  (examples: ESLint, Pylint, Prettier, Markdownlint, etc.)

### Required Repository Structure

The workflow file must be stored in:

```text
/.github/workflows/
```

Example:

```text
/.github/workflows/ci.yml
```

---

## 3. Example GitHub Action Workflow

Students must include at least one working workflow file.

Example:

```yaml
name: CI Pipeline

on:
  pull_request:
  push:

jobs:
  test:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v4

      - name: Install dependencies
        run: npm install

      - name: Run tests
        run: npm test

      - name: Run linter
        run: npm run lint
```

Students are encouraged to customize and expand this workflow for their own project needs.

---

## 4. Testing Backlog Using GitHub Issues

Groups must create GitHub Issues related to testing and quality assurance.

Examples:

- Create authentication unit tests
- Configure ESLint
- Add Playwright E2E tests
- Configure GitHub Actions CI pipeline
- Create API integration tests

---

## Final PDF Submission

After completing the workshop, groups must generate a PDF document containing the following items in order:

1. Testing Strategy Document (**4.0 marks**)
2. GitHub Actions Workflow File (**3.0 marks**)
3. Screenshots of Successful CI/CD Runs (**1.0 marks**)
4. Testing-Related GitHub Issues (**2.0 marks**)

Additional **2.0 marks** will be allocated to professionalism, organization, and clarity.

---

## Submission Instructions

Submit a single PDF document containing all required artifacts and screenshots.

---

## Evaluation Criteria

Each item will be evaluated using the following performance levels:

| Performance Level | Percentage Range | Description |
| --- | --- | --- |
| Exemplary | 100% | The component is exceptionally detailed, professional, technically accurate, and demonstrates strong understanding of testing and CI/CD practices. |
| Proficient | 75% | The component is well completed and demonstrates good understanding with only minor omissions or weaknesses. |
| Satisfactory | 50% | The component demonstrates partial understanding but lacks detail, depth, consistency, or completeness in multiple areas. |
| Limited | 25% | The component is incomplete, poorly organized, or demonstrates minimal effort or understanding. |
| Not Submitted | 0% | The component was not submitted or does not provide sufficient evidence of completion. |

In addition, **3.0 marks** are allocated to presenting this Project Integration at our Scrum meeting. Marks will be allocated as per the table below:

| Performance Level | Percentage Range | Description |
| --- | --- | --- |
| Exemplary | 100% | The presentation is exceptionally clear, professional, and well organized. The speaker demonstrates strong mastery of the subject matter, communicates ideas confidently, and answers questions accurately and thoughtfully. Visual aids and explanations significantly enhance understanding. |
| Proficient | 75% | The presentation is clear and organized, with good understanding of the topic demonstrated throughout. Most questions are answered correctly and with reasonable detail. Minor issues with clarity, pacing, confidence, or depth may be present. |
| Satisfactory | 50% | The presentation communicates the basic ideas of the topic but lacks clarity, organization, confidence, or sufficient detail in multiple areas. Responses to questions demonstrate only partial understanding of the material. |
| Limited / Insufficient | 25% | The presentation is poorly prepared, unclear, incomplete, or difficult to follow. The speaker demonstrates limited understanding of the material and is unable to adequately answer questions related to the topic. |
---

# Important Notes

- All Markdown files must render correctly on GitHub
- CI/CD workflows must execute successfully
- Use professional naming conventions throughout the repository
- Teams are encouraged to automate as much testing as possible
- Documentation should clearly explain testing responsibilities and procedures
- Students are encouraged to continuously improve their workflows throughout the semester
