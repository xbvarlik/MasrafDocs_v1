# Get Tags

To fill the drop-down menu at YeniKlasorOlustur screen called Kategori

```HTTP
GET /tags
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