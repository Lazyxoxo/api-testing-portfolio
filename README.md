# JSONPlaceholder API Testing Portfolio

## Project Overview

This project uses the JSONPlaceholder API, Postman, and JavaScript to practice automated API testing.

The project currently includes two positive test cases and one negative test case, executed through three HTTP GET requests. JavaScript assertions are used to validate HTTP status codes, JSON response structures, and individual response fields.

## Tools & Technologies

- **JSONPlaceholder:** A public mock REST API used as the system under test.
- **Postman:** An API testing application used to send HTTP GET requests, inspect responses, and execute automated test assertions.
- **JavaScript:** The programming language used to write assertions that validate HTTP status codes and JSON response data.

## Test Coverage

| Test Case ID | Endpoint | Test Scenario | Result |
|---|---|---|---|
| API-TC-001 | `GET /posts/1` | Retrieve a valid post | PASS |
| API-TC-002 | `GET /posts/9999` | Retrieve a nonexistent post | PASS |
| API-TC-003 | `GET /posts` | Retrieve all posts | PASS |

Detailed test steps, expected results, and execution outcomes are documented in [test-cases.md](test-cases.md).

## How to Run the Tests

1. Open Postman.
2. Download the Postman collection `.json` file from this GitHub repository.
3. In Postman, click **Import** and select the downloaded JSON file.
4. Open the imported collection and select one of the saved GET requests.
5. Click **Send** to execute the request.
6. Open the **Test Results** tab in the response panel.
7. Review the automated assertion results to determine whether the tests passed or failed.

## Test Results and Evidence

All three API test cases were executed successfully in Postman, with **17 of 17 automated assertions passing**.

| Test Case ID | Endpoint | Assertions Passed | Evidence |
|---|---|---|---|
| API-TC-001 | `GET /posts/1` | 6/6 | [View Screenshot](evidence/API-TC-001.png) |
| API-TC-002 | `GET /posts/9999` | 2/2 | [View Screenshot](evidence/API-TC-002.png) |
| API-TC-003 | `GET /posts` | 9/9 | [View Screenshot](evidence/API-TC-003.png) |

**Overall Result:** PASS — 17/17 assertions passed.

The screenshots show the HTTP request, response status, and automated assertion results for each test case.
