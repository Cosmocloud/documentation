# Models

Models defines the various schema definitions in your project, where you would need to define the structure of the data. There are 3 types of Models in Cosmocloud right now -

## Database Collections

These models define the structure of your Database's collections (or tables) and define the various entities that live in your system. You can define entities as a First Class citizen of your app like Students, Orders, Payments, etc which live on it's own as a single record.

Cosmocloud is powered by MongoDB - a full featured document database, which lets you model the data in a very efficient manner - very different from how you do in a Relational World.

You can check the various  as given by MongoDB as well as check a dedicated series on various  you should follow while designing your system.

!!! info "Info"

    You can also reach out to Cosmocloud expert team to help in better designing and building your system's data models.

One important feature to note while creating these models is that, each record would implicitly have a **[_id](https://www.mongodb.com/docs/manual/core/document/)** field as **ObjectId** field, which will be auto generated when inserting records in the database. You do not have to explicitly define the _id field if you are not overriding the default behaviour.
!!! info "Info"
    
    _id field acts as an automatic Primary Key in MongoDB collections.

## Request Body
These models, as with the name, are required when you build non GET APIs, such as Create Students, Update Order, Delete record APIs.

This is very similar to Database collections, where you can define nested models and entities, but can only be used in API's Request Body option.

!!! info "Info"

    Request Body as an option set as extra_fields=forbid which makes your request bodies strict. Any extra field passed while calling the API, would lead to 400 Bad Request with appropriate error message.

## Query Params
These models, as understood, are used to define the schema of query params to pass while calling an API. These can only be used in API's Query Params option.

As they are passed in the URL, there are limited types of fields you can define in these types of models - maily native types such as String, Integers, Boolean, Floats and ObjectIds. Complex field types such as Nested, Dict and List are not allowed.