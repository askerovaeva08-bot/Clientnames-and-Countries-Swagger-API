# GET /users Test Cases

## Positive Test Cases

### TC-01: Get User List with a Valid Token

Precondition: User is authorized with a valid token.

Steps:
1. Open Swagger UI.
2. Authorize with a valid token.
3. Execute the GET /users request.

Expected Result:
- Status Code: 200 OK
- The list of users is returned.
- Response body is not empty.

---

### TC-02: Verify Response Structure

Precondition: User is authorized.

Steps:
1. Execute the GET /users request.

Expected Result:
- Status Code: 200 OK
- Response contains user data fields (e.g., id, name, email).
- Response structure matches the API documentation.

---

### TC-03: Verify Response Format

Precondition: User is authorized.

Steps:
1. Execute the GET /users request.

Expected Result:
- Status Code: 200 OK
- Response format is application/json.
- User data is returned in a valid JSON structure.

---

## Negative Test Cases

### TC-04: Get Users Without Authorization Token

Steps:
1. Remove the authorization token.
2. Execute the GET /users request.

Expected Result:
- Status Code: 401 Unauthorized
- Error message indicating authorization is required.

---

### TC-05: Get Users with an Invalid Token

Steps:
1. Authorize using an invalid token.
2. Execute the GET /users request.

Expected Result:
- Status Code: 401 Unauthorized
- Error message indicating an invalid token.
