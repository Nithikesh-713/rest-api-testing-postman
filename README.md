# rest-api-testing-postman
# REST API Testing Using Postman

## Project Overview

This personal QA practice project demonstrates REST API testing using Postman, JavaScript assertions, and documented test cases.

The project uses [JSONPlaceholder](https://jsonplaceholder.typicode.com/), a public mock REST API for learning and testing.

## Tools and Technologies

- Postman
- REST APIs and HTTP methods
- JSON
- JavaScript
- Microsoft Excel
- GitHub

## API Testing Scenarios

| Test Scenario | Method | Endpoint | Expected Status |
|---|---|---|---|
| Fetch an existing post | GET | `/posts/1` | 200 OK |
| Fetch a non-existing post | GET | `/posts/9999` | 404 Not Found |
| Create a post | POST | `/posts` | 201 Created |
| Update a post | PUT | `/posts/1` | 200 OK |
| Delete a post | DELETE | `/posts/1` | Verify actual response |

## Testing Activities

- Sent API requests using GET, POST, PUT, and DELETE.
- Created JavaScript assertions to validate status codes and response data.
- Practiced positive and negative API testing.
- Validated JSON response fields.
- Documented test scenarios and expected results in Excel.
- Prepared a PDF test-case report.

## Project Files

- `REST_API_Test_Cases.xlsx` — Test scenarios and expected results.
- `REST_API_Test_Case_Report.pdf` — Test-case report.
- `REST_API_Testing_Postman_Collection.json` — Importable Postman collection.

## How to Run

1. Download the Postman collection JSON file from this repository.
2. Open Postman and click **Import**.
3. Select the downloaded JSON file.
4. Open each request and click **Send**.
5. Review the response and test results.
6. Record the actual results in the test-case workbook.

## Important Note

JSONPlaceholder is a mock API. POST, PUT, and DELETE simulate changes and do not permanently modify the service's stored data. Test results should be recorded only after executing the requests.

## Author

**Nithikesh H**

GitHub: https://github.com/Nithikesh-713
