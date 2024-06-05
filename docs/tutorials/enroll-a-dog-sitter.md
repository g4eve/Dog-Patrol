---
layout: page
---

# Tutorial: Enroll a new dog sitter

In this tutorial, you learn how to entroll a new dog sitter into the service with the `POST` METHOD. 

Expect this tutorial to take about 15 minutes to complete.

## Before you start

Make sure you've completed the [Before you start a tutorial](before-you-start-a-tutorial) topic on the development system you'll use for the tutorial.

## Enroll a new dog sitter
You can enroll a new user in the To-Do service. To do so, `POST` a new [`dog sitter`](../api/dog-sitter.md) resource containing the dog sitter's details.

1. If your local service is not running, start it.

    ```shell
    cd <your-github-workspace>/dog-patrol/api
    # Run the service and monitor its database file for updates
    json-server -w dog-db-source.json
    ```
2. Open the Postman app on your desktop.
3. In the Postman app, create a new request with these values:
    * **METHOD**: POST
    * **URL**: `{{base_url}}/dog-sitter`
    * **Headers**:
        * `Content-Type: application/json`
    * **Request body**:
        You can change the values of each property as you'd like.

        ```js
        {
            "last_name": "Mae",
            "first_name": "Bennett",
            "email": "m.bennett@example.com",
            "phone":"226-414-9876",
            "city": "North York",
            "available day": "weekend"
            "available time": "morning"
        }
        ```
4. In the Postman app, select **Send** to make the request.
5. Watch for the response body, which should look something like this. Note that the names should be the same as you used in your **Request body** and the response should include the new user's `id`.

    ```js
    {
        "last_name": "Mae",
        "first_name": "Bennett",
        "email": "m.bennett@example.com",
        "phone":"226-414-9876",
        "city": "North York",
        "available day": "weekday"
        "available time": "morning"
        "id": 6
    }
    ```

## Related Topics

* [Dog sitter resource](../api/dog-sitter.md)
