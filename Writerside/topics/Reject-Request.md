# Reject Request

```HTTP
PUT /approval/request/{id}/reject
```

### Request

```json
{
  "Headers": {
    "Authorization": "Bearer token"
  },
  "Body": {
    "explanation": "string"
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