---
layout: page
---

# Quickstart guide

This Quickstart guide will help you get started quickly with integrating the Dog Patrol Service into your application.

## Setting up the Dog Patrol service

Follow these [prerequisite steps](../tutorials/before-you-start-a-tutorial.md) to install the tools and test your development system.

## About the Dog Patrol service

The Dog Patrol Service API is designed to facilitate connections between dog sitters and dog owners. Dog sitters can find job opportunities, and dog owners can post jobs to find suitable sitters. 

The service has two resources: [`dog sitter`](dogsitter.md) and [`dog jobs`](dogjobs.md). The [`dog sitter`](dogsitter.md) resource lists all dog sitters enrolled in the service and are looking for a dog sitting job. The [`dog jobs`](dogjobs.md) resource lists all dog sitting job information posted by dog owners.

## How to use the Dog Patrol service

To build your API call, you must have the following components:

* **A host.**  The {server_url} is set to `http://localhost:3000`.
* **A request.**  The service REST API enables CRUD operations via HTTP requests on database resources (`GET`, `POST`, `PUT`, `PATCH`, and `DELETE` methods). Request and response bodies are encoded as JSON.

### Supported endpoints

#### Dog Jobs

| HTTP Method | Endpoint |
| -------------- | -------------- |
| GET | [List all dog jobs](get-all-dog-jobs.md) |
| GET | [List dog jobs by ID](get-job-by-id.md) |
| GET | [List dog jobs by area](get-job-by-area.md)|
| GET | [List dog jobs by city](get-job-by-city.md)|
| GET | [List dog jobs by number of dogs](get-job-by-number-dogs.md)|
| GET | [List dog jobs by start date](get-job-by-strat-date.md)|
| POST | [Create a new dog jobs](create-dog-job.md)|
| PATCH | [Update dog job by ID](update-job-by-id.md) |
| DELETE | [Delete a dog job by ID](delete-job-by-id.md) |

#### Dog Sitter

| HTTP Method | Endpoint |
| -------------- | -------------- |
| GET | [List all dog sitters](get-all-dog-sitters.md) |
| GET | [Find a dog sitter by ID](get-sitter-by-id.md) |
| GET | [List dog sitters by city](get-sitter-by-city.md) |
| GET | [List dog sitters by first name](get-sitter-by-first-name.md) |
| POST | [Enroll a new dog sitter](../docs/tutorials/enroll-a-dog-sitter.md) |
| PATCH | [Change a dog sitter property by ID](update-sitter-by-id.md) |
| DELETE | [Delete a dog sitter by ID](delete-sitter-by-id.md)|

## Making your first API call – *List all dog jobs*

Let’s try making a test call to the [`Dog Jobs`](dogjobs.md) resource using cURL.

```bash
curl http://localhost:3000/dog_jobs
```

The response will be a list of dog jobs from the Dog Patrol service such as you see in this example:

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


```
