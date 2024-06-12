---
layout: page
---

# Change a dog sitter property value

Update any property of a specific dog sitter record. Enter the ID followed by the property name and value in the request body.

## HTTP method

PATCH

## URL

```shell
{server_url}/dog_sitter/{id}
```

Sample request body.

```js
{
    "available day": "weekday",
    "available time": "morning",
}
```