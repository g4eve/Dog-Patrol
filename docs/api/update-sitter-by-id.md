---
layout: page
---

# Change a dog sitter property value

Update any property of a specific dog sitter record. Enter the ID followed by the property name and value in the request body.

## HTTP method

PATCH

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
| `id`     | number | The dog sitter's unique record ID |
| `available_day`  | string | The days that the dog sitter is available (weekday, weekend, or both) |

## Example request body

```json
{
        "available_day": "weekend"
}
```

```bash
curl --location --request PATCH 'http://localhost:3000/dog_sitter/2' \
--header 'Content-Type: application/json' \
--data '{
    "available_day": "weekend"
}'
```

## Return body

```js
    {
      "last_name": "Jones",
      "first_name": "Jill",
      "email": "j.jones@example.com",
      "phone": "416-555-1212",
      "city": "Toronto",
      "available_day": "weekend",
      "available_time": "night",
      "id": "2"
    }
```

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | Success | Requested data returned successfully |
| 404 | Error | Specified user record not found |
|  ECONNREFUSED | N/A | Service is offline. Start the service and try again. |