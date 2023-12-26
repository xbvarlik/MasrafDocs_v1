# Get Expenses

Use query filters to filter for status as pending or draft.

```HTTP
GET /expense
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
  "statusCode": 200,
  "data": [
    {
      "title": "string",
      "date": "dateOnly",
      "status": "string",
      "isTravel": "bool",
      "totalAmount": "decimal",
      "currency": "string"
    }
  ]
}
```
{collapsible="true"}