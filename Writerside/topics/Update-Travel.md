# Update Travel

Same endpoint will be used for updating draft travel and pending travel.
If expense status is pending, backend will abort the previous request and create a new one.
Else if it is a draft, same request object will sustain.
Fill whatever needs to be updated and leave null to the rest.

```HTTP
PATCH /travel/{id}
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
  "statusCode": 204,
  "data": null
}
```
{collapsible="true"}