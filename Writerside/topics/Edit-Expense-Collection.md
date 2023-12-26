# Edit Expense Collection

```HTTP
PATCH /expenseCollection/{id}/edit-collection
```

### Request

```json
{
  "Headers": {
    "Authorization": "Bearer token"
  },
  "Body": {
    "title": "string",
    "tagName(kategori)": "string"
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
    
  }
}
```
{collapsible="true"}