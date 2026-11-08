# JSONPlaceholder API — Test Cases

## Project Overview

API: JSONPlaceholder
Base URL: https://jsonplaceholder.typicode.com
Testing Tool: Postman
Test Types: Positive, Negative, Response Validation

---

## API-TC-001 — Retrieve a Valid Post

**Endpoint:** GET /posts/1

**Test Type:** Positive

**Test Objective:**
Verify that the endpoint returns HTTP 200 and a JSON
response containing the expected post ID, a numeric user ID, 
and non-empty string title and body.

**Preconditions:**
- The API is accessible.

**Test Steps:**
1. Open the GET /posts/1 request in Postman.
2. Send the request.
3. Examine the response and test results.

**Expected Results:**
1. HTTP status is 200 OK.
2. Post ID equals 1.
3. userId is numeric.
4. title is a non-empty string.
5. body is a non-empty string.

**Actual Result:**
All corresponding Postman assertions passed.

**Status:** PASS

---

## API-TC-002 — Retrieve a Nonexistent Post

**Endpoint:** GET /posts/9999

**Test Type:** Negative

**Test Objective:**
Verify that requesting a nonexistent post returns HTTP 404 Not Found and an empty JSON object {}.

**Preconditions:**
- The API is accessible.
- Post ID 9999 does not exist.

**Test Steps:**
1. Open the GET /posts/9999 request in Postman.
2. Send the request.
3. Examine the response and test results.

**Expected Results:**
1. HTTP status is 404 Not Found.
2. Response body is an empty JSON object `{}`.

**Actual Result:**
All corresponding Postman assertions passed

**Status:** PASS

---

## API-TC-003 — Retrieve All Posts

**Endpoint:** `GET /posts`

**Test Type:** Positive

**Test Objective:**
Verify that the GET /posts endpoint successfully returns an array containing 100 posts.
The 100 posts begin with post ID 1, and each post contains valid IDs and non-empty string titles and bodies.

**Preconditions:**
- The API is accessible.

**Test Steps:**
1. Open the GET /posts request in Postman.
2. Send the request.
3. Examine the response and test results.

**Expected Results:**
1. HTTP status is 200 OK.
2. Response body is a JSON array.
3. The array contains exactly 100 posts.
4. The first post has an ID of 1.
5. Every post's id is an integer.
6. Every title is a non-empty string.
7. Every body is a non-empty string.

**Actual Result:**
All corresponding Postman assertions passed.

**Status:**PASS

---
