# Get Expense Types

To fill the bottom sheet at MasrafTuruSec screen.

```HTTP
GET /expenseType
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
      "id": "int",
      "name": "string"
    }
  ]
}
```
{collapsible="true"}