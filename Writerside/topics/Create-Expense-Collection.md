# Create Expense Collection

```HTTP
POST /expenseCollection
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
  "statusCode": 201,
  "data": {
    "id": "guid",
    "title": "string",
    "tagId": "guid"
  }
}
```
{collapsible="true"}