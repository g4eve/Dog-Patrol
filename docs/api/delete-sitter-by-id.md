---
layout: page
---

# Delete a dog sitter

Permanently remove a dog sitter record from the service.

## HTTP method

DELETE

## URL

```shell
{server_url}/dog_sitter/{id}
```

## Request headers

| Key | Value |
|---|---|
| Content-Type | application/json |

## Request body parameters

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `id`     | number | The dog sitter's unique record ID  |

## Example request body

```json
{
      "last_name": "Smith",
      "first_name": "Ferdinand",
      "email": "f.smith@example.com",
      "phone": "416-555-1213",
      "city": "Toronto",
      "available_day": "weekday",
      "available_time": "morning"
}
```

```

```bash
curl --location --request DELETE 'http://localhost:3000/dog_sitter/1' \
--header 'Content-Type: application/json' \
--data '{
      "last_name": "Smith",
      "first_name": "Ferdinand",
      "email": "f.smith@example.com",
      "phone": "416-555-1213",
      "city": "Toronto",
      "available_day": "weekday",
      "available_time": "morning"
}'
```

## Return body

```js
{
      "last_name": "Smith",
      "first_name": "Ferdinand",
      "email": "f.smith@example.com",
      "phone": "416-555-1213",
      "city": "Toronto",
      "available_day": "weekday",
      "available_time": "morning"
}
```

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | Success | Requested data returned successfully |
| 404 | Error | Specified user record not found |
| ECONNREFUSED | N/A | Service is offline. Start the service and try again. |