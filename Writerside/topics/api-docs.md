# API Overview

<!-- This document provides an introduction into your API. -->

## Introduction

This is the API for backend of app XPens. It provides endpoints for XPens Mobile App.

## What you can do using <API name>

You can access the endpoints that are specifically designed for a client app, 
you can not access the actual endpoints in the back.

## Authentication

At this point, application has a basic authentication that authenticates and authorizes user via a JWT.
In the future, app to app SSO will be introduced int the api.

## API Base URL

<a href="https://app-masraf-bff-api-dev-001.azurewebsites.net/api"></a>

## Swagger URL

<a href="https://app-masraf-bff-api-dev-001.azurewebsites.net/swagger/index.html"></a>

## Error Handling

The error response will be a json object which look like this:

```json
{
  "isSuccess": "bool",
  "statusCode": "int",
  "errorResponse": "string/error-details"
}
```

| Status Code | Explanation           |
|-------------|-----------------------|
| 400         | Bad Request           |
| 401         | Unauthorized          |
| 403         | Forbidden             |
| 404         | Not Found             |
| 500         | Internal Server Error |

If error response status code starts with 4, it means there is a problem with how the request is sent. 
Check your payload and headers and see inner exception in the errorResponse part. Specific meanings of 
inner exceptions are given below.

| Exception Code            | What it means?                                                                      | What to do?                                                                                   |
|---------------------------|-------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| NttForbiddenException     | Current logged in user has not permission to access the requested route.            | Log in with a different user that has requested permission.                                   |
| NttNotFoundException      | Content looking for is not found.                                                   | Check parameters in payload and path.                                                         |
| NttNullException          | Some not nullable field in the request is null.                                     | Check parameters in payload and path.                                                         |
| NttAlreadyExistsException | Content with the same value for some unique field is already exist in the database. | Check unique fields in the payload.                                                           |
| NttBusinessException      | General response for outlier business exceptions.                                   | Check message to see what's wrong. Even then can't figure out, contact with the backend team. |
| NttValidationException    | Some validation error occurred.                                                     | Check parameters in payload and path.                                                         |
| NttOperationalException   | General response for operational exceptions.                                        | Check parameters and if you see nothing is wrong, contact with the backend team.              |
| NttUnauthorizedException  | Current user is not logged in and try to access a protected route.                  | Log in with a user and try again.                                                             |
| NttDatabaseException      | Something is wrong with database transactions.                                      | Contact with the backend team.                                                                |
| NttSystemException        | Internal server error. Something is not going as expected in the backend.           | Contact with the backend team.                                                                |

<seealso>

<!--List any additional resources, such as tutorials or guides, that can help users understand and use the API effectively.-->

</seealso>
