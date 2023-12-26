# Create Expense (MasrafGiris)

Same endpoint will be used for create default expense (daily expense in previous setup) and travel expenses.
If travel expense, set isTravelExpense to true and fill travelId field and backend will add this expense in that travel's expense collection (klasor).
Else if it is a default expense, set isTravelExpense to false and leave travelId empty and backend will add this expense
in that user's default expense collection.

```HTTP
POST /expense
```

### Request

<warning style="">Given in json for readability, application type is actually in multipart/formdata</warning>
```json
{ 
  "Headers": {
    "Authorization": "Bearer token"
  },
  "Body": {
    "isTravelExpense": "bool",
    "travelId": "guid", //nullable
    "title": "string",
    "expenseCenterId(masrafTuru)": "int",
    "expenseCenterObjectId(secilenProje)": "guid",
    "costTypeId(giderTuru)": "int",
    "institutionName": "string",
    "documentNumber": "int",
    "documentDate": "dateOnly",
    "paymentMethodId": "int",
    "totalAmount": "decimal",
    "currencyId": "int",
    "vatRateId": "int",
    "description": "string" //nullable
  }
}
```
{collapsible="true"}

### Success Response

```json
{
  "isSuccess": true,
  "statusCode": 201,
  "data": null
}
```
{collapsible="true"}