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
| `end_time` | string | The end time of the end date |
| `number_dogs` | number | The number dogs to be taken care of |
| `note` | string | The job description |
| `requirement` | string | The necessary condition that a dog sitter should meet |
| `location_city` | string | The city where the dog owner is located |
| `location_area` | string | The specific area within the city |
| `pay` | number | The hourly rate in CAD |
| `email` | string | The email address of the dog owner |
| `id` | number | The dog job's unique record ID |

## Operations

The `dog jobs` resource supports these operations.

### READ (GET)

* [Get a dog job by city (Complete)](get-job-by-city.md)
* [Get all dog jobs](get-all-dog-jobs.md)
* [Get a dog job by ID](get-job-by-id.md)
* [Get a dog job by area](get-job-by-area.md)
* [Get a dog job by start date](get-job-by-strat-date.md)
* [Get a dog job by number of dogs](get-job-by-number-dogs.md)

### CREATE (POST)

* [Create a new dog job (Complete)](create-dog-job.md)

### UPDATE (PUT/PATCH)

* [Update dog job by ID (Complete)](update-job-by-id.md)

### DELETE

* [Delete a dog job by ID (Complete)](delete-job-by-id.md)