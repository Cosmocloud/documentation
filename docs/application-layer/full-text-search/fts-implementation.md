# Implement full-text search in your application

Full-text search is a complex topic. It requires a good amount of expertise to set up correctly. Using a fully integrated solution such as MongoDB Atlas Search makes it easy for your team to add those features to your application in a matter of minutes.

Cosmocloud comes with a built-in feature to add full-text search in your application in a few minutes. It internally uses Atlas Search to implement full-text search but it is very less complicated than atlas search.

!!! info
    Cosmocloud Full Text Search is powered by MongoDb Atlas Search and hence, it requires MongoDb Atlas Configuration to implement full-text search in your application.

    [Setup MongoDB Atlas Database Config](/getting-started/account-setup/database-setup)

## Adding Full-Text search in your application
- In order to incorporate full-text search functionality in your application, you must create search indexes. These indexes serve as a unique definition for a database model, specifying which fields should be indexed and which analyzers should be used for processing those specific fields.

- You can create a Search index on a single field or on multiple fields. We recommend that you index the fields that you regularly use to sort or filter your data in order to quickly retrieve the documents that contain the relevant data at query time.

- When creating search indexes for fields, you have the option to utilize the built-in analyzers provided by Atlas Search, or you can create custom analyzers to tailor the indexing process according to your specific requirements.

- Each Database Collection model allows for the creation of a single search index. Within that model, you can choose between using built-in or custom analyzers for each field, based on the specific processing needs of that particular field.

!!! info

    You cannot create more than:

    - 3 indexes on M0 clusters.
    - 5 indexes on M2 clusters.
    - 10 indexes on M5 clusters.
    
    There are no limits to the number of indexes you can create on M10+ clusters.