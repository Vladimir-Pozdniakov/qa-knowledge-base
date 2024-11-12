### Code Quality
1. - [ ] No code duplication `[CORE]`
1. - [ ] Interaction abstraction `[CORE]`
      - [ ] Interaction with GUI pages is extracted to page object classes `[CORE]`
      - [ ] Interaction with API is extracted to API object classes `[CORE]`
1. - [ ] Functions and methods are modular, handling a single responsibility `[CORE]`
1. - [ ] The code is easy to read and understand without excessive comments `[CORE]`
1. - [ ] Consistent naming conventions for files, classes, and variables `[CORE]`
1. - [ ] Avoids hard-coded values by using variables and configuration files `[CORE]`
1. - [ ] Functions and components are reusable across tests `[CORE]`
1. - [ ] Clear directory structure (e.g., /tests, /data, /config) that keeps test logic, data, and configuration organized and separated `[CORE]`
1. - [ ] Pre-commit hooks are set up to automatically run before code is committed `[CORE]`
1. - [ ] The linting tool is configured to catch syntax and style issues `[CORE]`

### Test Quality
1. - [ ] Test function names are descriptive and explain the purpose of the test `[CORE]`
1. - [ ] Test names are unique across the test suite `[CORE]`
1. - [ ] Tests are easy to read and understand without excessive comments `[CORE]`
1. - [ ] Pre/Post-condition fixtures are used to simplify and lower test code `[CORE]`
      - [ ] UI preconditions are created via API/DB `[CORE]`
      - [ ] API preconditions are created via DB `[CORE]`
1. - [ ] Tests only contain the steps to execute the test scenario (no data setup or helper logic) `[CORE]`
1. - [ ] Calculation logic or complex helper code is extracted to utility/helper functions `[CORE]`
1. - [ ] Soft assertions to gather all test checks (if more than one) `[CORE]`
1. - [ ] Tests are parameterized to run with different data sets without modifying the test code itself `[CORE]`

### Test Data Management
1. - [ ] Centralized test data storage for easy access `[CORE]`
1. - [ ] Isolated test data per test to avoid dependencies `[CORE]`
1. - [ ] Automated test data cleanup for environment stability `[CORE]`
1. - [ ] Dynamic test data generation to avoid hard-coding/pesticide paradox `[CORE]`
1. - [ ] Secure handling of sensitive test data (e.g., masking, encryption) `[CORE]`
1. - [ ] Allows using different datasets based on test configuration `[NICE TO HAVE]`

### Test Run Management
1. - [ ] Supports customization of the test run scope (e.g., smoke, regression, functional, E2E, etc.) `[CORE]`
1. - [ ] Supports tagging tests for selective execution `[NICE TO HAVE]`
1. - [ ] Execution flexibility for the local environment `[NICE TO HAVE]`
1. - [ ] Execution flexibility for CI/CD environment `[CORE]`
1. - [ ] Filters test runs based on environment or configuration `[NICE TO HAVE]`
1. - [ ] No hard-coded sensitive data `[CORE]`

### Scalability & Performance
1. - [ ] Data used in tests is loaded only when necessary, avoiding heavy operations in setup/teardown `[CORE]`
1. - [ ] Optimized test execution time for fast feedback `[NICE TO HAVE]`
1. - [ ] Supports and configures parallel test execution `[NICE TO HAVE]`
1. - [ ] Tests are isolated (do not rely on or impact each other’s state), allowing independent runs `[CORE]`
1. - [ ] Uses mocks/stubs for running tests in an isolated environment `[NICE TO HAVE]`

### Error Handling & Logging
1. - [ ] Generates detailed and readable logs with contextual information `[CORE]`
1. - [ ] Logs output is attached to a test reporting tool `[CORE]`
1. - [ ] Retry mechanism for handling flaky tests `[NICE TO HAVE]`
1. - [ ] Tests have meaningful assertions with clear and descriptive error messages for quick diagnosis `[CORE]`
1. - [ ] Handles unexpected failures gracefully without halting the suite `[CORE]`
1. - [ ] Configurable logging levels (e.g., debug, info, error) `[NICE TO HAVE]`
1. - [ ] Automatic screenshots or data dumps on failure (for UI tests or API responses) `[CORE]`

### Environment Configuration
1. - [ ] Utilize a strategy to manage environment-specific configurations (e.g., Dev, QA, Production - if applicable) `[CORE]`
1. - [ ] Centralized configuration files for managing settings and environments `[CORE]`
1. - [ ] Supports running tests in multiple environments, cross-platform testing (if applicable) `[NICE TO HAVE]`
1. - [ ] Configuration is environment-independent and adaptable `[NICE TO HAVE]`
1. - [ ] Uses environment variables to handle sensitive data `[CORE]`
1. - [ ] Includes a Dockerfile to create a repeatable environment for testing `[CORE]`
1. - [ ] Logs are configured to output to the console, allowing Docker logs to be captured and reviewed easily `[CORE]`
1. - [ ] docker-compose.yml file (if multiple containers are needed) `[CORE]`
      - [ ] Health check in docker-compose.yml to verify all dependencies are running before tests start `[CORE]`
      - [ ] Supports volume mounting to easily update and run tests without rebuilding the container `[CORE]`

### Test Results Reports
1. - [ ] Integration with HTML test reporting tools (e.g., Allure, Playwright Reporter) `[CORE]`
1. - [ ] Detailed reporting output with insights for each test execution `[CORE]`
1. - [ ] Historical test run result data is handled `[CORE]`
1. - [ ] Each test has a link to a related test case in TCM `[CORE]`
1. - [ ] Test report is available for all team members and stakeholders `[CORE]`
1. - [ ] The status of the test results is sent to the messenger (e.g., slack, discord, email) `[NICE TO HAVE]`
1. - [ ] Test results are integrated with TCM test runs to track execution `[NICE TO HAVE]`
1. - [ ] Test report must contain a SUT build version (for mobile/tv/automotive apps) or code version hash commit (for front-end/back-end) `[NICE TO HAVE]`

### CI/CD
1. - [ ] The test pipeline can be run manually by any development team member `[NICE TO HAVE]`
1. - [ ] The test pipeline can be run on a specific schedule `[NICE TO HAVE]`
1. - [ ] The test pipeline is triggered by any related development project by a merge commit `[CORE]`
1. - [ ] The test pipeline jobs are parallelized (if possible) `[NICE TO HAVE]`

### Documentation & Maintainability
1. - [ ] Comprehensive setup and usage documentation `[CORE]`
1. - [ ] Detailed guides for adding new tests and components `[NICE TO HAVE]`
1. - [ ] Test formed in a dedicated branch (feature / fix / maintenance) `[CORE]`
1. - [ ] Commits are small, focused, and well-documented `[CORE]`
1. - [ ] Changes are submitted through pull requests that others can review before merging `[CORE]`
1. - [ ] Examples demonstrate framework setup and usage `[NICE TO HAVE]`
1. - [ ] Documentation is regularly updated and up to date `[CORE]`
1. - [ ] The project's library packages are regularly updated `[CORE]`
	
