# OpenWeather API - Test Cases

## TC001 - Get current weather by valid city name

**Endpoint:** `/data/2.5/weather`  
**Method:** GET  
**Parameter:** `q=London`  
**Expected Status Code:** 200  

**Expected Result:**
- The API should return weather data for the selected city.
- The response body should include city name, temperature, humidity and weather description.

**Status:** Passed

---

## TC002 - Get weather using an invalid city name

**Endpoint:** `/data/2.5/weather`  
**Method:** GET  
**Parameter:** `q=InvalidCityTest123`  
**Expected Status Code:** 404  

**Expected Result:**
- The API should return an error message indicating that the city was not found.

**Status:** Passed

---

## TC003 - Request without API key

**Endpoint:** `/data/2.5/weather`  
**Method:** GET  
**Parameter:** `q=London`  
**Expected Status Code:** 401  

**Expected Result:**
- The API should return an authentication error.

**Status:** Passed

---

## TC004 - Request with invalid API key

**Endpoint:** `/data/2.5/weather`  
**Method:** GET  
**Parameter:** `q=London&appid=invalid_key`  
**Expected Status Code:** 401  

**Expected Result:**
- The API should return an invalid API key error.

**Status:** Passed

---

## TC005 - Validate response fields

**Endpoint:** `/data/2.5/weather`  
**Method:** GET  
**Parameter:** `q=London`  
**Expected Status Code:** 200  

**Expected Result:**
The response body should contain:
- `name`
- `main.temp`
- `main.humidity`
- `weather[0].description`
- `wind.speed`

**Status:** Passed
