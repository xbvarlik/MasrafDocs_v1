# Home
```HTTP
GET /home
```

### Success Response
```json
{
  "isSuccess": true,
  "statusCode": 200,
  "data": {
    "pendingRequestCount": "int",
    "draftRequestCount": "int",
    "lastOperation": "string",
    "currentTravel": {
      "country": {
        "id": "int",
        "name": "string"
      },
      "city": {
        "id": "int",
        "name": "string"
      },
      "title": "string,",
      "description": "string",
      "startDate": "dateOnly",
      "endDate": "dateOnly",
      "totalExpenseInTravel": {
        "amount": "decimal",
        "currency": {
          "id": "int",
          "name": "string"
        }
      }
    },
    "monthlyExpenses": {
      "date": "dateOnly",
      "currency": {
        "id": "int",
        "name": "string"
      },
      "costTypeExpenses": [
        {
          "costType": "string",
          "amount": "decimal"
        }
      ]
    }
  }
}
```
{collapsible="true"}