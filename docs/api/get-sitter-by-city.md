---
layout: page
---

# Get a dog sitter by city

Find a dog sitter by location (city).

## HTTP method

GET

## URL

```shell
{server_url}/dog_sitter?city={value}
```

## Request headers

| Key | Value |
|---|---|
| Content-Type | application/json |

## Request body parameters

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `city` | string | The dog sitter's geographical location |

## Example request body

```json
{
    "city": "Toronto"
}
```

```bash
curl --location --request GET 'http://localhost:3000/dog_sitter?city=Toronto' \
--header 'Content-Type: application/json' \
--data '{
    "city": "Toronto"
}'
```

## Return body

```js
[
    {
      "last_name": "Smith",
      "first_name": "Ferdinand",
      "email": "f.smith@example.com",
      "phone": "416-555-1213",
      "city": "Toronto",
      "available day": "weekday",
      "available time": "morning",
      "id": "1"
    },
    {
      "last_name": "Jones",
      "first_name": "Jill",
      "email": "j.jones@example.com",
      "phone": "416-555-1212",
      "city": "Toronto",
      "available day": "weekday",
      "available time": "night",
      "id": "2"
    },
    {
      "last_name": "Martinez",
      "first_name": "Marty",
      "email": "m.martinez@example.com",
      "phone": "416-555-1214",
      "city": "Toronto",
      "available day": "weekend",
      "available time": "afternoon",
      "id": "3"
    },
    {
      "last_name": "Bailey",
      "first_name": "Bill",
      "email": "b.bailey@example.com",
      "phone": "416-555-1215",
      "city": "Toronto",
      "available day": "both",
      "available time": "all",
      "id": "4"
    }
]
```

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | Success | Requested data returned successfully |
| 404 | Error | Specified user record not found |
| ECONNREFUSED | N/A | Service is offline. Start the service and try again. |