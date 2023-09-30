**As a** Backend Developer

**I need** to add REST APIs for reading, updating, deleting, and listing customer accounts to the existing Python Flask-based REST API.

**So that** the account microservice can fully manage customer accounts and provide a well-formed REST API for other microservices to interact with.

### Details and Assumptions
- The database model for customer accounts has already been developed.
- The existing Python Flask-based REST API has an endpoint to create a customer account.

### Acceptance Criteria
Given the existing Python Flask-based REST API with an endpoint to create a customer account,
When I implement the additional REST APIs for reading, updating, deleting, and listing customer accounts,
Then the following conditions should be met:

1. Given a valid customer ID,
   When I send a GET request to `/api/customers/{customer_id}`,
   Then I should receive a JSON representation of the customer's data, and the response status code should be 200.

2. Given a valid customer ID and updated customer data in JSON format,
   When I send a PUT request to `/api/customers/{customer_id}`,
   Then the customer's data should be updated accordingly, and the response status code should be 200.

3. Given a valid customer ID,
   When I send a DELETE request to `/api/customers/{customer_id}`,
   Then the customer account should be deleted, and the response status code should be 204.

4. When I send a GET request to `/api/customers`,
   Then I should receive a JSON array of customer objects, and the response status code should be 200.
