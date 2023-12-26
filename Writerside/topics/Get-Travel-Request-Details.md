# Get Travel Request Details

```HTTP
GET /approval/request/travel/{id}
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
  "data": {
    "id": "guid",
    "title": "string",
    "startDate": "dateOnly",
    "endDate": "dateOnly",
    "countryCode": "string",
    "city": "string",
    "status": "string",
    "details": {
      "expenseCenterId(masrafTuru)": "int",
      "expenseCenterObjectId(secilenProje)": "guid",
      "travelTypeId(seyahatTuru)": "int",
      "description": "string"
    }
  }
}
```
{collapsible="true"}