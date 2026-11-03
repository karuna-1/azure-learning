# Day 3 – GitHub Actions and Automated Testing

## Automated Testing

Automated testing uses code to test applications
without manually checking every feature.

## Why Use Automated Testing?

- Detect bugs early.
- Reduce manual work.
- Improve application reliability.
- Prevent broken code from reaching production.

## CI/CD Testing Flow

1. Developer pushes code to GitHub.
2. GitHub Actions starts the workflow.
3. Dependencies are installed.
4. Automated tests are executed.
5. If tests pass, the pipeline can continue.
6. If tests fail, deployment should be stopped.

## Important Concept

Test first, deploy only if tests pass.