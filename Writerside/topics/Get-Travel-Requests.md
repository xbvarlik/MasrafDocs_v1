# Get Travel Requests

```HTTP
GET /approval/request/travel
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
      "startDate": "dateOnly",
      "endDate": "dateOnly",
      "countryCode": "string",
      "city": "string",
      "status": {
        "id": "int",
        "name": "string"
      }
    }
  ]
}
```
{collapsible="true"}