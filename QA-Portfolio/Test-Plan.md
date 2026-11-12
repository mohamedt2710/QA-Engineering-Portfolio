# Test Plan – JSONPlaceholder REST API

## 1. Objective
Validate core REST API behavior for the Posts resource, including successful retrieval, creation, update, and deletion.

## 2. Scope
**In scope**
- GET /posts
- GET /posts/{id}
- POST /posts
- PUT /posts/{id}
- PATCH /posts/{id}
- DELETE /posts/{id}
- HTTP status codes and response body structure

**Out of scope**
- Authentication and authorization (the practice API does not provide a real account flow)
- Production data persistence guarantees
- Load, security, and compatibility testing

## 3. Test approach
- Positive, negative, and boundary-oriented scenarios
- Validate status codes, response headers where relevant, JSON fields, and data types
- Use Postman collection assertions
- Execute requests independently and as a collection

## 4. Test data
Use the public practice service: https://jsonplaceholder.typicode.com  
Existing sample post ID: 1  
Nonexistent/invalid route: /invalid-resource

## 5. Entry criteria
- API base URL is reachable
- Postman is available
- Collection variables are configured

## 6. Exit criteria
- All planned cases have an execution result
- Failures include request details and reproducible evidence
- No defect is marked as confirmed without reproducing the mismatch

## 7. Risks and limitations
JSONPlaceholder is a mock API. Write operations simulate behavior and may not persist changes. Results can differ from a production API.

## 8. Deliverables
- Test cases
- Postman collection
- Execution evidence (to be added after running)
- Defect reports for confirmed failures only
