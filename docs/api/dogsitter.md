---
layout: page
---
# `dog sitter` resource

Base endpoint:

```shell
{server_url}/dog_sitter
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

* [Get all dog sitters](get-all-dog-sitters.md)
* [Get a dog sitter by ID](get-sitter-by-id.md)
* [Get a dog sitter by city](get-sitter-by-city.md)
* [Get a dog sitter by first name](get-sitter-by-first-name.md)

### CREATE (POST)

* [Enroll a new dog sitter](../docs/tutorials/enroll-a-dog-sitter.md)
* [Enroll a new dog sitter](/docs/tutorials/enroll-a-dog-sitter.md)
* [Enroll a new dog sitter](docs/tutorials/enroll-a-dog-sitter.md)
* [Enroll a new dog sitter](tutorials/enroll-a-dog-sitter.md)
* [Enroll a new dog sitter](..tutorials/enroll-a-dog-sitter.md)
* [Enroll a new dog sitter](../tutorials/enroll-a-dog-sitter.md)

### UPDATE (PUT/PATCH)

* [Change a dog sitter property by ID](update-sitter-by-id.md)

### DELETE

* [Delete a dog sitter by ID](delete-sitter-by-id.md)