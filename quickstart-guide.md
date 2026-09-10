# Weather API Developer Quickstart Guide

Welcome to the Weather API Developer Guide. This document details how to authenticate and fetch current weather data using standard HTTP requests.

## Base URL
`https://api.weather.com/v1`

## Authentication
Pass your API key in the request header for every API request:
`Authorization: Bearer YOUR_API_KEY`

---

## Endpoint: Get Current Weather
`GET /current`

### Request Parameters
| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `city` | String | **Yes** | The target city name (e.g., `Hyderabad`). |
| `units` | String | No | Unit system: `metric` (default) or `imperial`. |

---

### Code Examples

#### cURL Request
```bash
curl -X GET "[https://api.weather.com/v1/current?city=Hyderabad&units=metric](https://api.weather.com/v1/current?city=Hyderabad&units=metric)" \
     -H "Authorization: Bearer YOUR_API_KEY"
