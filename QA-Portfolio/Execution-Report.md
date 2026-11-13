# API Test Execution Report – JSONPlaceholder

## 1. Execution status

**Status: Not Run**

The Postman collection and test cases have been prepared, but no execution results have been recorded yet. This report intentionally does not claim that requests or assertions have passed.

| Metric | Current value |
|---|---:|
| Planned test cases | 10 |
| Executed | 0 |
| Passed | 0 |
| Failed | 0 |
| Blocked / Not Run | 10 |
| Confirmed defects | 0 |

## 2. Environment

- **API:** JSONPlaceholder
- **Base URL:** https://jsonplaceholder.typicode.com
- **Tool:** Postman
- **Collection:** [JSONPlaceholder – QA API Testing](./JSONPlaceholder-API.postman_collection.json)
- **Test data:** Existing post ID 1; invalid ID format `abc`; unsupported route `/invalid-resource`

## 3. Test coverage and execution record

| Test Case | Request / Coverage | Execution status | Actual result |
|---|---|---|---|
| API-001 | GET /posts – retrieve all posts | Not Run | Not recorded |
| API-002 | GET /posts/1 – retrieve existing post | Not Run | Not recorded |
| API-003 | GET /posts/abc – invalid ID format | Not Run | Not recorded |
| API-004 | GET /invalid-resource – unsupported route | Not Run | Not recorded |
| API-005 | POST /posts – create post | Not Run | Not recorded |
| API-006 | PUT /posts/1 – replace post | Not Run | Not recorded |
| API-007 | PATCH /posts/1 – partial update | Not Run | Not recorded |
| API-008 | DELETE /posts/1 – delete post | Not Run | Not recorded |
| API-009 | GET /posts/1 – response content type | Not Run | Not recorded |
| API-010 | GET /posts/1 – response field types | Not Run | Not recorded |

## 4. Collection assertion coverage

The collection contains 8 requests. Some requests validate more than one test condition:
- GET all posts: status code and non-empty array
- GET existing post: status code, required fields/types, and JSON content type
- GET invalid ID: response is handled without a server error and content type is JSON or empty
- Unsupported route: 404 status
- POST: 201 status and returned submitted data/generated ID
- PUT: 200 status and returned updated fields
- PATCH: 200 status and returned patched title
- DELETE: successful 200 or 204 status

## 5. Execution instructions

1. Import the collection JSON file into Postman.
2. Open the collection and confirm the `baseUrl` variable is `https://jsonplaceholder.typicode.com`.
3. Select **Run** / **Run collection**.
4. Run all 8 requests and retain the run summary.
5. Review any failed request's response, assertion message, and Postman console before classifying it as an API defect.

## 6. Notes and limitations

- JSONPlaceholder is a mock API. POST, PUT, PATCH, and DELETE responses simulate write operations; changes are not persisted as they would be in a production database.
- A failed assertion is not automatically a confirmed product defect. Reproduce the behavior and compare it with the documented expectation first.
- Update this report only with observed status codes, assertion results, and evidence from an actual run.

---
*This report records test preparation only. Execution results are pending.*
