# Get Approved Travels

To fill the bottom sheet at SeyahatSec screen.

```HTTP
GET /travel/approved
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
      "startDate": "dateOnly",
      "endDate": "dateOnly"
    }
  ]
}
```
{collapsible="true"}