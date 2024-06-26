---
layout: page
---

# Change a dog job property value

Update any property of a specific dog job record. Enter the ID number followed by the property name and value in the request body.

## HTTP method

PATCH

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
| `id`     | number | The dog job's unique record ID |
| `end_time`  | string | The end time of the end date |

## Example request body

```json
{
        "end_time": "closed"
}
```

```bash
curl --location --request PATCH 'http://localhost:3000/dog_jobs/4' \
--header 'Content-Type: application/json' \
--data '{
    "end_time": "1900"
}'
```

## Return body

```js
    {
      "start_date": "2024-06-14",
      "end_date": "2024-06-19",
      "start_time": "0600",
      "end_time": "1900",
      "number_dogs": 1,
      "note": "big dog weighs 35 kgs",
      "requirement": "come to my house for morning and evening walks",
      "location_city": "Toronto",
      "location_area": "Lakeshore West",
      "pay": 35,
      "email": "jamie@yopmail.com",
      "id": "4"
    }
```

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | Success | Requested data returned successfully |
| 404 | Error | Specified user record not found |
|  ECONNREFUSED | N/A | Service is offline. Start the service and try again. |