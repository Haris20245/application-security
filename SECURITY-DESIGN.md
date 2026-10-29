
# Application Security Pipeline Design

## Project
This project demonstrates automated security checks in a CI pipeline.

## Pipeline steps
1. Download the source code.
2. Install the required Python tools.
3. Scan the source code with Bandit.
4. Check Python dependencies with pip-audit.
5. Run unit tests with pytest.
6. Save the test report as an artifact.

## Security controls
- Bandit detects potentially insecure Python code.
- pip-audit checks dependencies for known vulnerabilities.
- Unit tests verify expected application behavior.
- The pipeline fails when a required security check or test fails.
- GitHub Actions uses read-only repository permissions.
- Secrets should not be stored directly in source code.

## Test results
Three unit tests passed:
- Addition
- Division
- Division by zero

## Limitations
Automated checks cannot guarantee that an application is completely secure.
