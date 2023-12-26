# Get Expense Requests

If separation of data according to status is desired, use query filters to achieve it.

```HTTP
GET /approval/request/expense
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
      "title": "string",
      "user": {
        "id": "guid",
        "name": "string"
      },
      "date": "dateOnly",
      "isTravel": "bool",
      "travelRequestId": "guid"
    }
  ]
}
```
{collapsible="true"}