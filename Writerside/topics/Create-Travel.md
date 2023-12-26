# Create Travel

```HTTP
POST /travel
```

### Request

```json
{
  "Headers": {
    "Authorization": "Bearer token"
  }, 
  "Body": {
    "title": "string",
    "expenseCenterId(masrafTuru)": "int",
    "expenseCenterObjectId(secilenProje)": "guid",
    "description": "string",
    "startDate": "dateOnly",
    "endDate": "dateOnly",
    "countryId": "int",
    "cityId": "int",
    "travelTypeId(seyahatTuru)": "int",
    "travelMethodId(vasita)": "int",
    "isAccommodationUsed(otel)": "bool",
    "isAdvancePaymentRequired": "bool",
    "advancePaymentAmount": "decimal",
    "advancePaymentCurrencyId": "int" 
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