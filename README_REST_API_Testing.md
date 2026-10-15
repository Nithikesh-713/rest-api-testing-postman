# REST API Testing Using Postman

## Overview
A beginner QA portfolio project practicing REST API requests and automated response assertions using Postman and JSONPlaceholder.

## Tools
- Postman Web
- JSONPlaceholder: https://jsonplaceholder.typicode.com/
- JavaScript-based Postman test scripts

## Coverage
- GET: retrieve a post and validate response fields
- Negative GET: request a nonexistent post
- POST: validate simulated resource creation
- PUT: validate simulated update response
- DELETE: validate simulated deletion response
- Status-code, response-body, field-value, and response-time assertions

## Example endpoints
- `GET /posts/1`
- `GET /posts/9999`
- `POST /posts`
- `PUT /posts/1`
- `DELETE /posts/1`

Base URL: `https://jsonplaceholder.typicode.com`

## Example test script
```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Post ID is 1", function () {
    const data = pm.response.json();
    pm.expect(data.id).to.eql(1);
});
```

## Important limitations
JSONPlaceholder is a practice API. POST, PUT, and DELETE simulate changes and do not permanently modify stored data. Document observed behavior and don't report a defect unless it conflicts with a stated requirement.

## How to reproduce
1. Open Postman.
2. Create requests using the endpoints above.
3. Add relevant scripts under **Scripts → After response**.
4. Send each request and record actual status, response, and test results.
5. Save requests in a collection and export the collection.

## Evidence checklist
- [ ] Exported Postman collection JSON
- [ ] Screenshot of passing GET tests
- [ ] Screenshot of negative GET result
- [ ] Screenshot of POST tests
- [ ] Screenshot of PUT and DELETE tests
- [ ] Completed test-case spreadsheet

## Resume project bullet (use after verifying your collection)
**REST API Testing Using Postman** — Practiced GET, POST, PUT, and DELETE requests against a public test API; wrote JavaScript assertions to validate status codes, response fields, and response bodies; documented positive and negative test scenarios.
