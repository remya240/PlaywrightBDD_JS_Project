# Playwright BDD Automation Framework

## Overview

This project is a web UI automation framework built using Playwright, JavaScript, and Cucumber BDD. It uses readable feature files, reusable step definitions, the Page Object Model (POM), and Excel-based test data to support maintainable and scalable test automation.

## Tech Stack

- **Playwright** – Browser automation
- **JavaScript** – Programming language
- **Cucumber BDD** – Behavior-driven development
- **Excel and CSV** – Test data management
- **GitHub Actions** – Continuous integration and automated test execution

## Project Structure

```text
PlaywrightBDD_JS_Project/
├── .github/
│   └── workflows/       # GitHub Actions workflow
├── features/            # Cucumber feature files
├── fixtures/            # Reusable test fixtures
├── import/              # Import-related test data
├── pages/               # Page Object Model classes
├── setup/               # Authentication setup
├── steps/               # Cucumber step definitions
├── testData/            # Excel and CSV test data
├── utils/               # Reusable utility classes
├── cucumber.js          # Cucumber configuration
├── playwright.config.js # Playwright configuration
├── package.json         # Dependencies and npm scripts
├── package-lock.json    # Locked dependency versions
└── README.md            # Project documentation
```

## Getting Started

### Prerequisites

- Node.js and npm
- Git
- Visual Studio Code or another code editor

### Installation

Clone the repository and navigate to the project directory:

```bash
git clone https://github.com/remya240/PlaywrightBDD_JS_Project.git
cd PlaywrightBDD_JS_Project
npm ci
```

Install the required Playwright browsers:

```bash
npx playwright install
```

## Running Tests

Check `package.json` for the available npm scripts and use the appropriate command to execute the tests.

For example:

```bash
npm test
```

If the `test` script is not configured, run the Cucumber command specified in your project configuration.

## Test Data

Test data is maintained in Excel and CSV files to reduce hard-coded values and improve test maintainability.

## Reporting and Logging

Refer to the project configuration and available npm scripts for test reports and execution logs.

## CI/CD

GitHub Actions configuration is maintained under `.github/workflows/`. The workflow can install dependencies, execute configured tests, and upload test reports.

## Best Practices

- Keep credentials, passwords, and authentication tokens out of source control.
- Store sensitive configuration in environment variables.
- Exclude `.env` files and authentication state from Git.
- Use reusable page objects and step definitions.
- Keep feature files readable and focused on business behavior.
- Use external test data to minimize hard-coded values.
