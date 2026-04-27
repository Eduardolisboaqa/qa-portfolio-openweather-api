# OpenWeather API Testing Project

## Project Overview

This project demonstrates API testing using Postman with the OpenWeather API.

The objective was to validate API behavior, HTTP status codes, response body structure, authentication errors and basic response data validation.

## API Tested

OpenWeather API - Current Weather Data

## Tools Used

- Postman
- GitHub
- OpenWeather API

## Test Scope

The following scenarios were tested:

- Get current weather by valid city name
- Get weather using an invalid city name
- Request without API key
- Request with invalid API key
- Validate response body fields
- Validate HTTP status codes

## HTTP Method Used

- GET

## Test Cases

| ID | Scenario | Expected Status | Status |
|----|----------|----------------|--------|
| TC001 | Get weather by valid city name | 200 OK | Passed |
| TC002 | Get weather using invalid city name | 404 Not Found | Passed |
| TC003 | Request without API key | 401 Unauthorized | Passed |
| TC004 | Request with invalid API key | 401 Unauthorized | Passed |
| TC005 | Validate response fields | 200 OK | Passed |

## Validations Performed

The following fields were validated in the API response:

- City name
- Temperature
- Humidity
- Weather description
- Wind speed
- Status code
- Error messages

## Repository Structure

```text
qa-portfolio-openweather-api/
│
├── README.md
├── postman-collection/
├── test-cases/
├── bug-reports/
├── evidence/
└── test-summary/
```

## Security Note

The API key used in this project was removed for security reasons.

In Postman, the API key should be stored as an environment variable:

{{api_key}}

## Evidence

Screenshots of the test executions are available in the /evidence folder.

## Postman Collection

The exported Postman collection is available in the /postman-collection folder.

## Test Summary

The final test execution summary is available in the /test-summary folder.

 ## Conclusion

This project helped me practice API testing fundamentals, including endpoint validation, status code verification, response body analysis, error handling and technical documentation.
