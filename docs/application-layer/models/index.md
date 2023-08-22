# Model Types

Models defines the various schema definitions in your project, where you would need to define the structure of the data. There are 3 types of Models in Cosmocloud right now -

### Database Collection Models

These define and mirror the database collections (tables / entities) in the system. The name of these models should be exactly the same as the underlying Database collection.

!!! warning "Warning"
    You can check the `Database Collection` model naming convention [here](https://www.mongodb.com/docs/manual/reference/limits/#mongodb-limit-Restriction-on-Collection-Names). You can easily define these as strings containing [a-zA-Z0-9_] characters and ***cannot*** begin with numbers or underscore.

### Query Params Models

Query param models, are structures or schemas that define the expected format and data types of query parameters used in API calls. They serve as a set of rules that guide how query parameters should be constructed and what types of values they should hold when making requests to an API.

### Request Body Models

A "Request Body Model" is a structured definition that outlines the format, structure, and data types expected in the payload of an HTTP request made to an API endpoint. It serves as a blueprint for using HTTP methods like POST, PUT, PATCH, and DELETE. Unlike GET requests that retrieve data, these methods involve sending data to the server for processing .

!!! info "Info"

    Request Body has an option set as `extra_fields=forbid`` which makes your request bodies strict. Any extra field passed while calling the API, would lead to 400 Bad Request with appropriate error message.
