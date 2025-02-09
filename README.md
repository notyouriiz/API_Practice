# Mock API Practice with Mocki.io

This repository provides examples and practice exercises for calling APIs using Mocki.io, a service that allows you to quickly generate mock APIs for development and testing.

## What is Mocki.io?

Mocki.io is a tool that simplifies API development and testing by providing instant, customizable mock APIs [1][3][5]. It allows you to simulate API endpoints, define responses, and test your application without relying on a live backend. Mocki.io helps to:

*   Simulate errors
*   Remove dependencies on backend
*   Generate custom data
*   Avoid unstable external services
*   Create proof of concepts

## Setup

1.  **Create an account:** Visit [Mocki.io](https://mocki.io) and sign up for a free account.
2.  **Create a Mock API:** Use the Mocki.io interface to create a new API. You can define your own data model or import an existing OpenAPI specification.
3.  **Get the API Endpoint:** Once your mock API is created, Mocki.io will provide you with a unique endpoint URL.

## Examples

### Example 1: Basic GET Request

This example demonstrates how to make a simple GET request to a Mocki.io endpoint.
```
import requests

url = "YOUR_MOCKI_IO_ENDPOINT" # Replace with your Mocki.io endpoint URL
response = requests.get(url)

if response.status_code == 200:
data = response.json()
print(data)

else:
print(f"Request failed with status code: {response.status_code}")
text

```
Replace `"YOUR_MOCKI_IO_ENDPOINT"` with the actual URL provided by Mocki.io.

### Example 2: POST Request

This example demonstrates how to send a POST request to a Mocki.io endpoint.

```
import requests
import json

url = "YOUR_MOCKI_IO_ENDPOINT" # Replace with your Mocki.io endpoint URL
headers = {'Content-type': 'application/json'}

data = {
"key1": "value1",
"key2": "value2"
}

response = requests.post(url, data=json.dumps(data), headers=headers)

if response.status_code == 200:
print("POST request successful")
print(response.json())

else:
print(f"POST request failed with status code: {response.status_code}")
text

```
Remember to replace `"YOUR_MOCKI_IO_ENDPOINT"` with your actual Mocki.io endpoint.

## Practice Exercises

1.  **Create a Mock API with multiple endpoints:** Use Mocki.io to create an API with different endpoints for users and todos.
2.  **Simulate Errors:** Configure your Mock API to return error responses for specific requests.
3.  **Implement different HTTP methods:** Practice using GET, POST, PUT, and DELETE requests with your Mock API.
4.  **Dynamic Responses:** Explore how to set up dynamic responses based on request parameters.
