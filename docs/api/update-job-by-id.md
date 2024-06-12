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

Sample request body.

```js
{
    "end_time": "2100",
    "pay": 23,
}
```