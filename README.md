# Checklist for Functional UI Testing - Tallinn Delivery App (Login)
## Homework17
Form Validation:

Verify that all input fields (username and password) are present and displayed correctly.
Check the presence and functionality of the "Login" button when entering data.
Incorrect Data Validation:

Validate error messages for attempting login without filling in the required fields.
Verify error messages for entering invalid login credentials.
Check for error messages when using unauthorized characters.
Login Functionality:

Test successful login with valid credentials.
Verify that the user is redirected to the correct page after login.
Logout Functionality:

Test the correct logout process and redirection to the login page.
Password Recovery:

Check for the presence and functionality of the password recovery feature.
Verify the receipt of an email with instructions for password recovery.

### Web Elements List for Functional Testing

| No | Web Element Description   | Xpath                        |
|----|---------------------------|------------------------------|
| 1  | Username Input Field      | //input[@name="username"]    |
| 2  | Password Input Field      | //input[@name="password"]    |
| 3  | Login Button              | //button[@type="submit"]     |
| 4  | Error Message Display     | //div[@class="error-message"]|
| 5  | Password Recovery Link    | //a[@href="/forgot-password"]|



# Homework10

## Project Description
This project is a collection of automated API tests that verify the functionality and reliability of an API interface. The tests are written in Java using the RestAssured framework.

## Tested Functionality
The following table provides an overview of the tested functionality and their status:

| Number | Check Name                                 | Check Description                                       | Status  |
|--------|--------------------------------------------|---------------------------------------------------------|---------|
| 1      | simplePositiveTestGet                 | Integer IDs with values {1, 5, 10} to get response 200 OK | Passed  |
| 2      | simpleNegativeTestGet                 | Integer IDs with values {0, 11} to get response 400 Bad Request | Passed  |
| 3      | simplePositiveTestPost                     | Create an order with random generated data (ID) to get response 200 OK | Passed  |
| 4      | simpleNegativeTestPost                     | Create an order with random generated data (ID) to get response 415 Unsupported Media Type | Passed  |
| 5      | simplePositiveTestResponseBodyStatusOpenGet| Check the response body for status "OPEN" to get response 200 OK | Passed  |
| 6      | simpleGetOrderById	                        | Check the Verifies the successful retrieval of an order by its ID from the Pet Store API. to get response 200 OK| Passed  |
| 7      | simpleGetOrderById	                        | Check the Verifies the successful retrieval of an order by its ID from the Pet Store API. to get response 404| Passed  |
## Tools Used
- Programming Language: Java
- API Testing Framework: RestAssured
- Build System: Maven
- Integrated Development Environment (IDE): IntelliJ IDEA
