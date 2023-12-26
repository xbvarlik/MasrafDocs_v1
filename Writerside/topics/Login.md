# Login

```HTTP
POST /login
```

### Request

```json
{
  "Headers": {
    "Authorization": "Bearer token"
  },
  "Body": {
    "email": "string",
    "password": "string"
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
    "access-token": "string",
    "refresh-token": "string"
  }
}
```
{collapsible="true"}