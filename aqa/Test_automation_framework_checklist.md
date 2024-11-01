### Code Quality
- [ ] No code duplication `[CORE]`
- [ ] Interaction abstraction `[CORE]`
  - [ ] Interaction with GUI pages is extracted to page object classes `[CORE]`
  - [ ] Interaction with API is extracted to API object classes `[CORE]`
- [ ] Functions and methods are modular, handling a single responsibility `[CORE]`
- [ ] The code is easy to read and understand without excessive comments `[CORE]`
- [ ] Consistent naming conventions for files, classes, and variables `[CORE]`
- [ ] Avoids hard-coded values by using variables and configuration files `[CORE]`
- [ ] Functions and components are reusable across tests `[CORE]`
- [ ] Clear directory structure (e.g., /tests, /data, /config) that keeps test logic, data, and configuration organized and separated `[CORE]`
- [ ] Pre-commit hooks are set up to automatically run before code is committed `[CORE]`
- [ ] The linting tool is configured to catch syntax and style issues `[CORE]`

### Test Quality
- [ ] Test function names are descriptive and explain the purpose of the test `[CORE]`
- [ ] Test names are unique across the test suite `[CORE]`
- [ ] Tests are easy to read and understand without excessive comments `[CORE]`
- [ ] Pre/Post-condition fixtures are used to simplify and lower test code `[CORE]`
  - [ ] UI preconditions are created via API/DB `[CORE]`
  - [ ] API preconditions are created via DB `[CORE]`
- [ ] Tests only contain the steps to execute the test scenario (no data setup or helper logic) `[CORE]`
- [ ] Calculation logic or complex helper code is extracted to utility/helper functions `[CORE]`
- [ ] Soft assertions to gather all test checks (if more than one) `[CORE]`
- [ ] Tests are parameterized to run with different data sets without modifying the test code itself `[CORE]`

### Test Data Management
- [ ] Centralized test data storage for easy access `[CORE]`
- [ ] Isolated test data per test to avoid dependencies `[CORE]`
- [ ] Automated test data cleanup for environment stability `[CORE]`
- [ ] Dynamic test data generation to avoid hard-coding/pesticide paradox `[CORE]`
- [ ] Secure handling of sensitive test data (e.g., masking, encryption) `[CORE]`
- [ ] Allows using different datasets based on test configuration `[NICE TO HAVE]`

### Test Run Management
- [ ] Supports configuring test run scope (e.g., smoke, regression, functional, E2E, etc.) `[CORE]`
- [ ] Supports tagging tests for selective execution `[NICE TO HAVE]`
- [ ] Execution flexibility for the local environment `[NICE TO HAVE]`
- [ ] Execution flexibility for CI/CD environment `[CORE]`
- [ ] Filters test runs based on environment or configuration `[NICE TO HAVE]`
- [ ] No hard-coded sensitive data `[CORE]`

### Scalability & Performance
- [ ] Data used in tests is loaded only when necessary, avoiding heavy operations in setup/teardown `[CORE]`
- [ ] Optimized test execution time for fast feedback `[NICE TO HAVE]`
- [ ] Supports and configures parallel test execution `[NICE TO HAVE]`
- [ ] Tests are isolated (do not rely on or impact each other’s state), allowing independent runs `[CORE]`
- [ ] Uses mocks/stubs for running tests in an isolated environment `[NICE TO HAVE]`

### Error Handling & Logging
- [ ] Generates detailed and readable logs with contextual information `[CORE]`
- [ ] Logs output is attached to a test reporting tool `[CORE]`
- [ ] Retry mechanism for handling flaky tests `[NICE TO HAVE]`
- [ ] Tests have meaningful assertions with clear and descriptive error messages for quick diagnosis `[CORE]`
- [ ] Handles unexpected failures gracefully without halting the suite `[CORE]`
- [ ] Configurable logging levels (e.g., debug, info, error) `[NICE TO HAVE]`
- [ ] Automatic screenshots or data dumps on failure (for UI tests or API responses) `[CORE]`

### Environment Configuration
- [ ] Utilize a strategy to manage environment-specific configurations (e.g., Dev, QA, Production - if applicable) `[CORE]`
- [ ] Centralized configuration files for managing settings and environments `[CORE]`
- [ ] Supports running tests in multiple environments, cross-platform testing (if applicable) `[NICE TO HAVE]`
- [ ] Configuration is environment-independent and adaptable `[NICE TO HAVE]`
- [ ] Uses environment variables to handle sensitive data `[CORE]`
- [ ] Includes a Dockerfile to create a repeatable environment for testing `[CORE]`
- [ ] Logs are configured to output to the console, allowing Docker logs to be captured and reviewed easily `[CORE]`
- [ ] docker-compose.yml file (if multiple containers are needed) `[CORE]`
  - [ ] Health check in docker-compose.yml to verify all dependencies are running before tests start `[CORE]`
  - [ ] Supports volume mounting to easily update and run tests without rebuilding the container `[CORE]`

### Test Results Reports
- [ ] Integration with HTML test reporting tools (e.g., Allure, Playwright Reporter) `[CORE]`
- [ ] Detailed reporting output with insights for each test execution `[CORE]`
- [ ] Historical test run result data is handled `[CORE]`
- [ ] Each test has a link to a related test case in TCM `[CORE]`
- [ ] Test report is available for all team members and stakeholders `[CORE]`
- [ ] The status of the test results is sent to the messenger (e.g., slack, discord, email) `[NICE TO HAVE]`
- [ ] Test results are integrated with TCM test runs to track execution `[NICE TO HAVE]`

### CI/CD
- [ ] The test pipeline can be run manually by any development team member `[NICE TO HAVE]`
- [ ] The test pipeline can be run on a specific schedule `[NICE TO HAVE]`
- [ ] The test pipeline is triggered by any related development project by a merge commit `[CORE]`
- [ ] The test pipeline jobs are parallelized (if possible) `[NICE TO HAVE]`

### Documentation & Maintainability
- [ ] Comprehensive setup and usage documentation `[CORE]`
- [ ] Detailed guides for adding new tests and components `[NICE TO HAVE]`
- [ ] Test formed in a dedicated branch (feature / fix / maintenance) `[CORE]`
- [ ] Commits are small, focused, and well-documented `[CORE]`
- [ ] Changes are submitted through pull requests that others can review before merging `[CORE]`
- [ ] Examples demonstrate framework setup and usage `[NICE TO HAVE]`
- [ ] Documentation is regularly updated and up to date `[CORE]`
- [ ] Regularly scheduled updates for dependencies and maintenance `[CORE]`
	
