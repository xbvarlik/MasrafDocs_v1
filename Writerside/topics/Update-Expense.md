# Update Expense

Same endpoint will be used for updating draft expenses and pending expenses.
If expense status is pending, backend will abort the previous request and create a new one.
Else if it is a draft, same request object will sustain.
Fill whatever needs to be updated and leave null to the rest.

```HTTP
PATCH /expense/{id}
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
        "description": "string"
    }
}
```
{collapsible="true"}

### Success Response

```json
{
  "isSuccess": true,
  "statusCode": 204,
  "data": null
}
```
{collapsible="true"}