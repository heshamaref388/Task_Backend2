# Task Backend

## Description

This project is a backend service for managing exchanges, metadata, and candle data using Express and MongoDB.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/heshamaref388/Task_Backend2.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Task_Backend2
   ```
3. Install the dependencies:
   ```bash
   npm install
   ```

## Usage

### API Endpoints

#### Exchanges

- **GET /exchanges**: Retrieve all exchanges.
- **POST /exchanges**: Create a new exchange.
- **GET /exchanges/:id**: Retrieve a single exchange by ID.
- **PUT /exchanges/:id**: Update an exchange by ID.
- **DELETE /exchanges/:id**: Delete an exchange by ID.

#### Metadata

- **GET /metadata**: Retrieve all metadata.
- **POST /metadata**: Create a new metadata entry.
- **GET /metadata/:id**: Retrieve a single metadata entry by ID.
- **PUT /metadata/:id**: Update a metadata entry by ID.
- **DELETE /metadata/:id**: Delete a metadata entry by ID.

#### Candles

- **GET /candle**: Retrieve all candles.
- **POST /candle**: Create a new candle entry.
- **GET /candle/:id**: Retrieve a single candle entry by ID.
- **PUT /candle/:id**: Update a candle entry by ID.
- **DELETE /candle/:id**: Delete a candle entry by ID.

### Environment Variables

- **MONGODB_URI**: The connection string for MongoDB. Set this in your environment variables.

## How the API Works

The API is built using Express.js and connects to a MongoDB database. It follows a RESTful architecture, allowing clients to perform CRUD (Create, Read, Update, Delete) operations on resources.

### Request and Response Format

- **Request Format**: All requests should be made to the appropriate endpoint using the specified HTTP method (GET, POST, PUT, DELETE).
- **Response Format**: The API responds with JSON data. Successful responses will return a status code of 200 (OK) or 201 (Created) along with the requested data. Errors will return appropriate status codes (e.g., 400 for bad requests, 404 for not found).

### Authentication

Currently, the API does not require authentication for accessing the endpoints. However, this can be implemented in the future.

### Error Handling

The API provides meaningful error messages in the response body. Common error responses include:

- **400 Bad Request**: The request was invalid or cannot be served.
- **404 Not Found**: The requested resource could not be found.
- **500 Internal Server Error**: An unexpected error occurred on the server.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the ISC License.
