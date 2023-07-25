# Query Param Models
These models, as understood, are used to define the schema of query params to pass while calling an API. These can only be used in API's `Query Params` option.

As they are passed in the URL, there are limited types of fields you can define in these types of models - mainly native types such as **String**, **Integers**, **Boolean**, **Floats** and **ObjectIds**(passed as strings). Complex field types such as *Nested*, *Dict* and *List* are not allowed.

## Query Params Validation

Any API that has a Query Params attached to it, will validate the same when invoked at run time. Any errors pertaining to the validation of the Query Params will throw a `400 - Bad Request` with the appropriate error messages.

Sample error messages can look like - 

```json
{
    "detail": [
        {
            "loc": [
                "params",
                "name"
            ],
            "msg": "value is not a valid string",
            "type": "type_error.string"
        }
    ]
}
```