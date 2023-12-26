# Password Reset Request

```HTTP
POST /password-reset-request
```

### Request

```json
{
  "Headers": {
    "Authorization": "Bearer token"
  },
  "Body": {
    "email": "string"
  }
}
```
{collapsible="true"}

### Success Response

```json
{
  "isSuccess": true,
  "statusCode": 200,
  "data": {
    "change-password-url": "string"
  }
}
```
{collapsible="true"}