# API Quickstart

<!-- This document describes how to start using your API: authorization, authentication, accessing API resources. -->
In this section, you'll find a step-by-step guide to quickly start using the API.

## Authentication

You can authenticate using login endpoint of the api.

```http
POST /login HTTP 1.1
Host: https://app-masraf-bff-api-dev-001.azurewebsites.net/api
```

## Response Handling

Responses from this api will be in format given below.

```json
{
  "isSuccess": "bool",
  "statusCode": "int",
  "data": "content you requested"
}
```

## Next Steps
Read specific descriptions for endpoints and payloads.