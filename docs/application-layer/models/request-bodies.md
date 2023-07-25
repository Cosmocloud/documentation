# Request Body Models
These models, as the name suggests, are required when you need to pass a `Request Body` in an API. These APIs should have a request method as **POST**, **PUT**, **PATCH**, **DELETE** but not GET.

This is very similar to `Database Collection` model, where you can define nested models and entities, but can **only be used** in API's Request Body option.

!!! info "Info"

    Request Body has an option set as `extra_fields=forbid`` which makes your request bodies strict. Any extra field passed while calling the API, would lead to 400 Bad Request with appropriate error message.

## Request Body Validation

Any API that has a request body attached to it, will validate the same when invoked at run time. Any errors pertaining to the validation of the Request Body will throw a `400 - Bad Request` with the appropriate error messages.

Sample error messages can look like - 

```json
{
    "detail": [
        {
            "loc": [
                "body",
                "name"
            ],
            "msg": "value is not a valid string",
            "type": "type_error.string"
        }
    ]
}
```