# Remove Expenses From Collection

```HTTP
PATCH /expenseCollection/{id}
```

### Request

```json
{
  "Headers": {
    "Authorization": "Bearer token"
  },
  "Body": {
    "expenseIds": ["guid"]
  }
}
```
{collapsible="true"}

### Success Response

```json
{
  "isSuccess": true,
  "statusCode": 204,
  "data": {
    "id": "guid",
    "title": "string",
    "tag": "string",
    "expenses": [
      {
        "title": "string",
        "status": "string",
        "date": "dateOnly",
        "amount": "decimal",
        "currency": "string"
      }
    ]
  }
}
```
{collapsible="true"}