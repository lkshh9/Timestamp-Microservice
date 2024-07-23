# Back End Development and APIs Projects


# Project 1 : Timestamp Microservice

This is the boilerplate code for the Timestamp Microservice project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/timestamp-microservice

## FreeCodeCamp Project Completed 

This is a simple timestamp microservice built with Node.js and Express. The application provides endpoints to parse date strings and Unix timestamps, returning the date in both Unix timestamp and UTC string formats.

## Features

- Parse and format date strings and Unix timestamps
- Handle invalid dates gracefully
- Return current date and time in Unix and UTC formats

## API Endpoints

### GET `/api/:date`

This endpoint takes a date parameter (either a date string or Unix timestamp) and returns a JSON object with the Unix timestamp and UTC date string.

- **Date String Input**: `/api/2024-07-23`
  - Response:
    ```json
    {
      "unix": 1721798400000,
      "utc": "Tue, 23 Jul 2024 00:00:00 GMT"
    }
    ```

- **Unix Timestamp Input**: `/api/1627084800000`
  - Response:
    ```json
    {
      "unix": 1627084800000,
      "utc": "Wed, 23 Jul 2021 00:00:00 GMT"
    }
    ```

- **Invalid Date Input**: `/api/invalid-date`
  - Response:
    ```json
    {
      "error": "Invalid Date"
    }
    ```

### GET `/api`

This endpoint returns the current date and time in both Unix timestamp and UTC string formats.

- **Example**:
  - Response:
    ```json
    {
      "unix": 1627084800000,
      "utc": "Wed, 23 Jul 2021 00:00:00 GMT"
    }
    ```



