# Weather API Testing (Postman + Newman)

## Overview
API test collection validating current weather endpoint: status codes, schema basics, and negative scenarios.

## Tools
- Postman
- Newman (CLI) for automated runs
- Node.js (to install Newman)

## How to Run
1. Install newman: `npm install -g newman`
2. Run: `newman run Postman-Collection/WeatherAPI.postman_collection.json -r cli,html --reporter-html-export Reports/WeatherAPI_Newman_Report.html`

## Scope
- 200 OK for valid city
- 404/400 for invalid city or missing params
- Response time check
