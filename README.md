# Task: Add SonarQube Scan with Jest Code Coverage to a React + TypeScript UI Application

You are an expert in configuring SonarQube for React and TypeScript applications and integrating it into GitHub Actions.

Objective

Configure SonarQube analysis for the existing React + TypeScript UI application and enforce a Quality Gate based on Jest test coverage.

Requirements

1. GitHub Actions
   
   - Add a new step named "SonarQube Scan - Jest Test Coverage" to the existing GitHub Actions workflow.
   - The new step should integrate seamlessly with the current workflow and must not modify or break any existing deployment steps.
   - Follow the same implementation pattern used in "deployment.yml", specifically the existing Sonar Scan step (if present), so the implementation remains consistent across workflows.

2. Jest Coverage
   
   - Use the existing Jest test cases and generated coverage reports.
   - Configure SonarQube to consume the Jest coverage report (LCOV format).
   - Ensure the workflow generates the coverage report before executing the SonarQube scan.

3. Quality Gate
   
   - Configure SonarQube so that the Quality Gate enforces a minimum 80% code coverage.
   - The GitHub workflow should fail if the SonarQube Quality Gate fails (including coverage below 80%).

4. Project Configuration
   
   - Read the existing "package.json".
   - Add only the required dependencies and scripts for SonarQube integration.
   - Create or update any required configuration files (such as "sonar-project.properties") using SonarQube best practices for a React + TypeScript project.
   - Ensure the coverage path and source paths are configured correctly.

5. Deliverables
   
   - List all files that need to be created or modified.
   - Show the complete changes for each file.
   - Explain why each change is required.
   - Ensure the solution follows industry best practices and does not impact the existing CI/CD pipeline.

Do not change any existing deployment logic unless it is strictly required for the SonarQube integration.
