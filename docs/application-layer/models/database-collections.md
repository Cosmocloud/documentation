# Database Collections

These models define the structure of your Database's collections (or tables) and define the various **entities** that live in your system. You can define entities as a First Class citizen of your app like **Students**, **Orders**, **Payments**, etc which live on it's own as a **single record**.

Cosmocloud is powered by [MongoDB](https://mongodb.com) - a full featured document database, which lets you model the data in a very efficient manner - very different from how you do in a Relational World.

!!! warning "Warning"
    
    You can check the `Database Collection` model naming convention [here](https://www.mongodb.com/docs/manual/reference/limits/#mongodb-limit-Restriction-on-Collection-Names). You can easily define these as strings containing [a-zA-Z0-9_] characters and ***cannot*** begin with numbers or underscore.

You can check the various [Data Modelling Concepts](https://www.mongodb.com/docs/manual/core/data-modeling-introduction/) as given by MongoDB as well as check a dedicated series on various [Data Modelling Patterns](https://www.mongodb.com/blog/post/building-with-patterns-a-summary) you should follow while designing your system.

!!! info "Info"

    You can also reach out to Cosmocloud expert team to help in better designing and building your system's data models.

One important feature to note while creating these models is that, each record would implicitly have an `_id` ([check docs](https://www.mongodb.com/docs/manual/core/document/)) field as **ObjectId** field, which will be **auto generated** when inserting records in the database. You do not have to explicitly define the `_id` field if you are not overriding the default behaviour.
!!! info "Info"
    
    `_id` field acts as an automatic Primary Key in MongoDB collections, as well as MongoDB automatically creates a unique index on `_id`.