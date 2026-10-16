# Playwright BDD Automation Framework

## Overview
This project is a web UI automation framework built using Playwright, JavaScript, and Cucumber BDD. It uses readable feature files, reusable page objects, and Excel-based test data to support maintainable and scalable automation.

## Tech Stack
- **Playwright** – Browser automation
- **JavaScript** – Programming language
- **Cucumber BDD** – Behavior-driven testing
- **Excel** – Test data management
- **GitHub Actions** – CI/CD workflow

## Project Structure

```text
PalywrightBDD_JS/
├── .github/workflows/   # CI workflow configuration
├── features/            # BDD feature files
├── fixtures/            # Test fixtures
├── import/              # Import test data
├── pages/               # Page Object Model classes
├── setup/               # Authentication setup
├── steps/               # Step definitions
├── testData/            # Excel test data
├── utils/               # Reusable utilities
├── cucumber.js          # Cucumber configuration
├── playwright.config.js  # Playwright configuration
└── package.json         # Dependencies and scripts
```

## Getting Started

### Prerequisites
- Node.js and npm
- Git

### Installation

Clone the repository and navigate to the project directory:

```bash
git clone https://github.com/remya240/PlaywrightBDD_JS_Project.git
cd PlaywrightBDD_JS_Project
npm install
```

Install the required Playwright browsers if needed:

```bash
npx playwright install
```

## Running Tests

Check `package.json` for the available test scripts. Run the appropriate script, for example:

```bash
npm test
```

If no `test` script is configured, use the command defined for your Cucumber and Playwright BDD setup.

## Test Data
Test data is maintained in Excel and CSV files to reduce hard-coded values and make test scenarios easier to maintain.

## Reporting
The framework can be configured to generate test execution reports. Refer to the project configuration for the available reporting commands.

## CI/CD
A GitHub Actions workflow is included under `.github/workflows/` for running automation through CI.

## Notes
- Keep credentials and authentication tokens out of source control.
- Configure environment variables and authentication state before running tests, as required by the project.
