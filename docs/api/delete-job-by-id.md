---
layout: page
---

# Delete a dog job

Permanently remove a dog job record from the service.

## HTTP method

DELETE

## URL

```shell
{server_url}/dog_jobs/{id}
```

## Request headers

| Key | Value |
|---|---|
| Content-Type | application/json |

## Request body parameters

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `id`     | number | The dog job's unique record ID  |

## Example request body

```json
{
      "start_date": "2024-06-01",
      "end_date": "2024-06-06",
      "start_time": "0700",
      "end_time": "0900",
      "number_dogs": 3,
      "note": "can handle big dogs",
      "requirement": "walk and run dogs in the morning for 5 days in a row",
      "location_city": "Toronto",
      "location_area": "Eglington station",
      "pay": 20,
      "email": "jack@yopmail.com",
}
```

```

```bash
curl --location --request DELETE 'http://localhost:3000/shifts/1' \
--header 'Content-Type: application/json' \
--data '{
      "start_date": "2024-06-01",
      "end_date": "2024-06-06",
      "start_time": "0700",
      "end_time": "0900",
      "number_dogs": 3,
      "note": "can handle big dogs",
      "requirement": "walk and run dogs in the morning for 5 days in a row",
      "location_city": "Toronto",
      "location_area": "Eglington station",
      "pay": 20,
      "email": "jack@yopmail.com",
}'
```

## Return body

```js
{
      "start_date": "2024-06-01",
      "end_date": "2024-06-06",
      "start_time": "0700",
      "end_time": "0900",
      "number_dogs": 3,
      "note": "can handle big dogs",
      "requirement": "walk and run dogs in the morning for 5 days in a row",
      "location_city": "Toronto",
      "location_area": "Eglington station",
      "pay": 20,
      "email": "jack@yopmail.com",
}
```

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | Success | Requested data returned successfully |
| 404 | Error | Specified user record not found |
| ECONNREFUSED | N/A | Service is offline. Start the service and try again. |