# Get Projects

To fill the bottom sheet at ProjeSec screen.

```HTTP
GET /project
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
      "name": "string"
    }
  ]
}
```
{collapsible="true"}