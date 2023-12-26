# Get Expense Collections (Klasorler)

```HTTP
GET /expenseCollection
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
      "id": "guid",
      "title": "string"
    }
  ]
}
```
{collapsible="true"}