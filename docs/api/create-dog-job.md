---
layout: page
---

# Create a dog job

Create a new dog job.

## HTTP method

POST

## URL

```shell
{server_url}/dog_jobs
```

## Request headers

| Key | Value |
|---|---|
| Content-Type | application/json |

## Request body parameters

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `start_date` | string | The start date of the dog sitting job |
| `end_date` | string | The end date of the dog sitting job |
| `start_time` | string | The start time of the start date |
| `end_time` | string | The end date of the end date  |
| `number_dogs` | number | The number dogs to be taken care of |
| `note` | string | The job description |
| `requirement` | string | The necessary condition that a dog sitter should meet |
| `location_city` | string | The city where the dog owner is located |
| `location_area` | string | The specific area within the city |
| `id` | number | The dog job's unique record ID |

## Example request body

```json
{
      "start_date": "2024-09-08",
      "end_date": "2024-09-08",
      "start_time": "0800",
      "end_time": "2200",
      "number_dogs": 1,
      "note": "small dog with skin allergy that needs to be house sit",
      "requirement": "must follow the allergy treament notes",
      "location_city": "Toronto",
      "location_area": "Yorkville",
      "pay": 40,
      "email": "congee@yopmail.com"
}
```

```bash
curl --location 'http://localhost:3000/dog_jobs' \
--header 'Content-Type: application/json' \
--data '{
      "start_date": "2024-09-08",
      "end_date": "2024-09-08",
      "start_time": "0800",
      "end_time": "2200",
      "number_dogs": 1,
      "note": "small dog with skin allergy that needs to be house sit",
      "requirement": "must follow the allergy treament notes",
      "location_city": "Toronto",
      "location_area": "Yorkville",
      "pay": 40,
      "email": "congee@yopmail.com"
}'
```

## Return body

```js
 {
      "start_date": "2024-09-08",
      "end_date": "2024-09-08",
      "start_time": "0800",
      "end_time": "2200",
      "number_dogs": 1,
      "note": "small dog with skin allergy that needs to be house sit",
      "requirement": "must follow the allergy treament notes",
      "location_city": "Toronto",
      "location_area": "Yorkville",
      "pay": 40,
      "email": "congee@yopmail.com",
      "id": 5
 }
```

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | Success | Requested data returned successfully |
| 404 | Error | Specified user record not found |
| ECONNREFUSED | N/A | Service is offline. Start the service and try again. |