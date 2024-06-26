---
layout: page
---

# Get a dog job by city

Get a dog job by the location (city).

## HTTP method

GET

## URL

```shell
{server_url}/dog_jobs?location_city={value}
```

## Request headers

| Key | Value |
|---|---|
| Content-Type | application/json |

## Request body parameters

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `location_city` | string | The city where the dog owner is located |

## Example request body

```json
{
    "location_city": "Toronto"
}
```

```bash
curl --location --request GET 'http://localhost:3000/dog_jobs?location_city=Toronto' \
--header 'Content-Type: application/json' \
--data '{
    "location_city": "Toronto"
}'
```

## Return body

```js
[
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
        "id": "1"
    },
    {
        "start_date": "2024-06-07",
        "end_date": "2024-06-09",
        "start_time": "0700",
        "end_time": "1800",
        "number_dogs": 2,
        "note": "must house sit for two nights",
        "requirement": "24 hour care for two days",
        "location_city": "Toronto",
        "location_area": "North York",
        "pay": 30,
        "email": "mary@yopmail.com",
        "id": "2"
    },
    {
        "start_date": "2024-06-10",
        "end_date": "2024-06-11",
        "start_time": "0600",
        "end_time": "1800",
        "number_dogs": 2,
        "note": "must house sit for 12 hours",
        "requirement": "must be free two walk in the morning and early evening",
        "location_city": "Toronto",
        "location_area": "Queens park",
        "pay": 30,
        "email": "james@yopmail.com",
        "id": "3"
    },
    {
        "start_date": "2024-06-14",
        "end_date": "2024-06-19",
        "start_time": "0600",
        "end_time": "1800",
        "number_dogs": 1,
        "note": "big dog weighs 35 kgs",
        "requirement": "come to my house for morning and evening walks",
        "location_city": "Toronto",
        "location_area": "Lakeshore West",
        "pay": 35,
        "email": "jamie@yopmail.com",
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