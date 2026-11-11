# API Testing with Postman

## Project Overview
This project documents practical API testing using Postman. It demonstrates GET and POST requests, JSON responses, and query parameters using public APIs.

## 1. JSONPlaceholder – GET Request

**Endpoint:** `https://jsonplaceholder.typicode.com/posts/1`

**HTTP Method:** GET

**Purpose:** Retrieve an existing blog post from the API.

**Response:**
- User ID: 1
- Post ID: 1
- Title: sunt aut facere repellat provident occaecati excepturi optio reprehenderit
- Body: Blog post content returned by the server.

**Observation:** The API successfully returned structured JSON data.

## 2. Postman Echo – POST Request

**Endpoint:** `https://postman-echo.com/post`

**HTTP Method:** POST

**Purpose:** Submit student information as JSON.

**Request Body:**
```json
{
  "name": "Khalid",
  "course": "Information Technology",
  "university": "ARDHI University",
  "level": "Fourth Year"
}
```

**Observation:** The API successfully received and returned the submitted JSON data. The response included request headers, data, and URL.

## 3. Open-Meteo – GET Request

**Endpoint:** `https://api.open-meteo.com/v1/forecast`

**HTTP Method:** GET

**Query Parameters:**
- latitude: -6.7924
- longitude: 39.2083
- current: temperature_2m, relative_humidity_2m

**Purpose:** Retrieve current weather information for Dar es Salaam.

**Observed Response:**
- Temperature: 30.1 °C
- Relative humidity: 66%
- Elevation: 62 metres
- Measurement interval: 900 seconds

**Observation:** The API returned weather information in JSON format using query parameters. No API key was required for this request.

## 4. HTTPBin – Testing Attempt

**Endpoints:**
- `https://httpbin.org/get`
- `https://httpbin.org/post`

**HTTP Methods:** GET and POST

**Observation:** Both requests encountered HTTP 429 (Too Many Requests) due to rate limiting. Alternative services were used to complete the practical demonstrations.

## 5. Key Lessons Learned

- GET is used to retrieve information.
- POST is used to submit information.
- JSON represents structured data.
- API responses contain data and status information.
- Query parameters provide additional input to API requests.
- HTTP 429 indicates that a request limit has been exceeded.
- API keys must be protected and must not be published on GitHub.

## Tools Used
- Postman Web
- Ubuntu Linux
- Public REST APIs
- Git and GitHub
