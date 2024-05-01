# Tool Rental API Collection

This repository contains a Postman collection for the Tool Rental API. It provides a set of endpoints to manage tools, orders, and authentication.

## Documentation

Please refer to the [documentation](https://github.com/vdespa/quick-introduction-to-postman/blob/main/README.md) for additional information about the Tool Rental API.

## Collection Structure

The collection consists of several folders, each representing a different category of requests:

1. **Authentication**: Contains requests related to authentication, such as registering an API client and obtaining an access token.

2. **Status - 200**: Contains a sanity test to verify that the API endpoint is working as expected.

3. **Tools**: Requests to manage tools, including getting all tools, getting a single tool by ID, and updating tools.

4. **Orders**: Requests to manage orders, including creating, updating, retrieving, and deleting orders.

## Environment Variables

The collection uses environment variables to store base URLs, access tokens, generated IDs, and other dynamic values. These variables are defined in the collection and can be configured based on your environment.

### Base URL
- **baseUrl**: The base URL of the Tool Rental API.

### Authentication
- **accessToken**: Access token used for authentication.

### Tools
- **toolId**: ID of the tool used in various requests.

### Orders
- **randomUserName**: Randomly generated user name used in creating orders.
- **orderId**: ID of the order used in various requests.

## Tests and Pre-request Scripts

The collection includes tests and pre-request scripts to verify the behavior of the API endpoints and generate dynamic data. These scripts are written in JavaScript and executed automatically during request execution.

## Usage

To use this collection:
1. Import the collection into Postman.
2. Set up the required environment variables.
3. Execute the requests to interact with the Tool Rental API.

# Running Tests with Newman

## Prerequisites
Before running the tests, ensure that Node.js and npm are installed on your system. If not, download and install them from the official Node.js website: [Node.js Downloads](https://nodejs.org/en/download/).

## Installation
To install Newman globally, open a terminal and run the following command:
`npm install -g newman`

On Mac os, install "brew install newman"

Once installed, verify the installation by running:
`newman -v`

## Running Tests
To execute all the tests, run the following command in your terminal:
`newman run postman_collection.json`
