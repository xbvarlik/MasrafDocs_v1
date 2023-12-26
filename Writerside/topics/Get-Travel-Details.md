# Get Travel Details

```HTTP
GET /travel/{id}
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
    },
    "expenses": [
      {
        "id": "guid",
        "title": "string",
        "date": "dateOnly",
        "amount": "decimal",
        "currency": "string",
        "status": "string"
      }
    ]
  }
}
```
{collapsible="true"}