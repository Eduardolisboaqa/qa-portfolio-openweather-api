# OpenWeather API - Test Summary

## Project Overview

This project was created to practice API testing using Postman and the OpenWeather API.

The main objective was to validate functional API behavior, HTTP status codes, response body structure and error handling.

## Scope

The following scenarios were tested:

- Get current weather by valid city name
- Get weather using an invalid city name
- Request without API key
- Request with invalid API key
- Validate important response fields

## Tools Used

- Postman
- OpenWeather API
- GitHub

## Test Results

| Test Case | Description | Expected Status Code | Status |
|----------|-------------|----------------------|--------|
| TC001 | Get weather by valid city name | 200 | Passed |
| TC002 | Invalid city name | 404 | Passed |
| TC003 | Missing API key | 401 | Passed |
| TC004 | Invalid API key | 401 | Passed |
| TC005 | Response field validation | 200 | Passed |

## Conclusion

The tested scenarios behaved according to the expected results.

This project helped reinforce API testing fundamentals, including request execution, response validation, status code analysis, error handling and test documentation.
