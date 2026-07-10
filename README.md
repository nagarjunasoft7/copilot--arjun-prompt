Continue generating Jest test cases only for the remaining uncovered files until every test suite achieves at least 85% statements, branches, functions, and lines coverage.

Do not skip any tests.
Do not modify production code unless absolutely necessary.
Run until `npm run test:coverage` succeeds with all coverage thresholds met.



You are an expert React, TypeScript, Jest, and React Testing Library engineer.

Your task is to implement or fix Jest test cases for this React application.

Mandatory Requirements

1. Do NOT skip any test.
   
   - Do not use "it.skip", "test.skip", "describe.skip", "xit", "xtest", or comment out any test.
   - Every test must execute successfully.

2. Every test suite must complete execution within 30,000 ms (30 seconds).
   
   - Eliminate unnecessary waits.
   - Mock all external dependencies.
   - Avoid real API calls, timers, file system access, network requests, and unnecessary rendering.

3. Every test suite must achieve at least 85% code coverage for:
   
   - Statements
   - Branches
   - Functions
   - Lines

4. No source file should remain with 0% coverage.
   
   - Create meaningful tests for every uncovered component, hook, utility, and helper.

5. Increase coverage by testing:
   
   - Success scenarios
   - Error scenarios
   - Edge cases
   - Conditional branches
   - User interactions
   - Async flows
   - Loading states
   - Empty states
   - Exception handling

6. Follow React Testing Library best practices.
   
   - Test behavior instead of implementation.
   - Prefer "screen" queries.
   - Use "userEvent".
   - Avoid unnecessary "act()".
   - Clean up mocks properly.

7. Mock all dependencies including:
   
   - API services
   - Axios/fetch
   - React Router
   - Redux
   - Context providers
   - Custom hooks
   - Browser APIs
   - LocalStorage/SessionStorage
   - Window methods
   - Timers
   - Date
   - Environment variables

8. Do not modify production source code unless absolutely required for testability. Prefer mocking instead.

9. Do not reduce assertions just to make tests pass. Tests must validate actual behavior.

10. If an existing test fails:
    
    - Identify the root cause.
    - Fix the test.
    - Do not skip or remove it.

11. If coverage is below 85%, continue adding meaningful test cases until the target is reached.

12. After completing each test suite:
    
    - Ensure all tests pass.
    - Ensure there are no skipped tests.
    - Ensure there are no flaky tests.
    - Ensure execution time is under 30 seconds.
    - Ensure coverage is at least 85%.

13. The final solution must pass:
    
    - "npm test"
    - "npm run test:coverage"

Do not stop until all of the above requirements are satisfied.
