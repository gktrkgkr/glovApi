# glovApi

This project provides an endpoint for Glov API.

## Endpoint

The endpoint for this API lives at:
https://us-central1-glov-97db9.cloudfunctions.net/api/glovApi/

## Parameters

### stream
- **Type:** String
- **Values:** "true" or "false"
- **Description:** Determines whether streaming is enabled or not.

Example usage:
https://us-central1-glov-97db9.cloudfunctions.net/api/glovApi/?stream=true

### Authorization Header
- **Type:** Bearer Token
- **Format:** Bearer USER{xxx} where xxx is a three-digit integer.
- **Description:** Provides access authorization to the API.

Example:
Authorization: Bearer USER123

## Usage

To use this endpoint, make HTTP requests to the provided URL with appropriate parameters and headers.

### Example using cURL

```bash
curl -X GET \
  'https://us-central1-glov-97db9.cloudfunctions.net/api/glovApi/?stream=true' \
  -H 'Authorization: Bearer USER123'
