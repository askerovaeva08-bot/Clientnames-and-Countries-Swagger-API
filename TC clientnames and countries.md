TC01 — Create All Clients via GET Request

ID: TC01

Title: To create all clients by the GET request

Description: To create clients with mandatory fields.

Pre-condition: Authorize with Bearer Token.

Steps
Send a GET request to the Swagger API endpoint.
Include the Bearer Token for authorization.
Data
[
  {
    "age": 0,
    "id": 0,
    "name": "string",
    "phone": "string",
    "surname": "string"
  }
]

Expected Result

Response code is 200 OK.
