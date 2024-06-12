---
layout: page
---
# `dog jobs` resource

Base endpoint:

```shell
{server_url}/dog_jobs
```

Contains information about the dog job details posted by the dow owners in the service.

## Resource properties

Sample `dog jobs` resource

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
      "id": "1"
}
```

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

## Operations

The `dog jobs` resource supports these operations.

### READ (GET)

* Get all dog jobs
* Get a dog job by ID
* Get a dog job by city
* Get a dog job by area
* Get a dog job by start date
* Get a dog job by number of dogs

### CREATE (POST)

* Create a new dog job

### UPDATE (PUT/PATCH)

* Update dog job date
* Update dog job time
* Update dog job note
* Update dog job requirement


### DELETE

* Delete a dog job by ID