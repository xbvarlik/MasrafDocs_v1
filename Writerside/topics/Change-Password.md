# Change Password

```HTTP
PATCH /change-password
```

### Request

```json
{
  "Headers": {
    "Authorization": "Bearer token"
  },
  "Body": {
    "oldPassword": "string",
    "newPassword": "string"
  }
}
```
{collapsible="true"}

### Success Response

```json
{
  "isSuccess": true,
  "statusCode": 204,
  "data": null
}
```
{collapsible="true"}