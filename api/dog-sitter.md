---
layout: page
---
# `dog sitter` resource

Base endpoint:

```shell
{server_url}/dog-sitter
```

Contains information about the dog sitters enrolled in the service.

## Resource properties

Sample `dog sitter` resource

```js
{
      "last_name": "Smith",
      "first_name": "Ferdinand",
      "email": "f.smith@example.com",
      "phone":"416-555-1213",
      "city": "Toronto",
      "available day": "weekday",
      "available time": "morning",
      "id": 1
}
```

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `last_name` | string | The dog sitter's last name |
| `first_name` | string | The dog sitter's first name |
| `email` | string | The dog sitter's email address |
| `phone` | string | The dog sitter's phone number |
| `city` | string | The dog sitter's geographical location |
| `available day` | string | The days that the dog sitter is available (weekday, weekend, or both)|
| `available time` | string | The time that the dog sitter is available (morning, afteroon, night, or all) |
| `id` | number | The dog sitter's unique record ID |

## Operations

The `dog sitter` resource supports these operations.

### READ (GET)

* Get all dog sitters
* Get a dog sitter by ID
* Get a dog sitter by Email
* Get a dog sitter by first name

### CREATE (POST)

* [Enroll a new dog sitter](../docs/enroll-a-dog-sitter)

### UPDATE (PUT/PATCH)

* Change dog sitter property

### DELETE

* Delete a dog sitter by ID