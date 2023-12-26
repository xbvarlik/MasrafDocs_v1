# Expense Request Details

```HTTP
GET /approval/request/expense/{id}
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
    "user": {
      "id": "guid",
      "name": "string"
    },
    "status": "string",
    "date": "dateOnly",
    "totalAmount": "decimal",
    "currency": "string",
    "expenseCenter(masrafTuru)": "string",
    "expenseCenterObject(secilenProje)": "string",
    "costType": "string",
    "institutionName": "string",
    "documentNumber": "int",
    "paymentMethod": "string",
    "vatRate": "decimal",
    "vatAmount": "decimal",
    "description": "string",
    "isTravel": "bool",
    "travelRequestId": "guid"
  }
}
```
{collapsible="true"}