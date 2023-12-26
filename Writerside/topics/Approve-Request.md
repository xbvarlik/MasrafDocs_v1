# Approve Request

```HTTP
PUT /approval/request/{id}/approve
```

### Request

```json
{
  "Headers": {
    "Authorization": "Bearer token"
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