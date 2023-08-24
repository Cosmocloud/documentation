# Creating a Search Index

!!! info
    Make sure that your Database config is configured with MongoDB Atlas configuration, otherwise, you will not be able to create/view the search indexes.

- Browse to **Full Text Search** --> **Search Indexes** and you will see a list of search indexes if there will be any.

    ![Search Index List](/assets/fts/search-index/search_index_list.webp) 

- On the top right corner of this page, click on **Create Search Index** button to create a search index. 

- It will open a form to create the search index. Select the model for which you want to create the search index and give a name to your search index. ( By default it will take the model name as the search index name) 

    ![Create Search Index](/assets/fts/search-index/create_search_index.webp) 

- Click on the **Next** button after filling in the search index details.
- The next stage is to **Define Field Mappings**, which can be done in two ways:
    - **Dynamic Field Mapping**: Use dynamic mappings if your schema changes regularly, is unknown, or when experimenting with Full-text Search.

    ![Dynamic Field Mapping](/assets/fts/search-index/dynamic_field_mapping.webp) 

    - **Static Field Mapping**: Use static mappings to configure index options for fields that you don't want to be indexed dynamically, or to configure a single field independently from others in an index. 

        For static field mapping toggle Dynamic to False, and you will get the option to add mappings for the fields you want to be indexed.
    
    ![Static Field Mapping](/assets/fts/search-index/static_field_mapping.webp) 

    - Now select the field that you want to be indexed and select the analyzer that you want to be used to process the data of that field and clicking on **Create** button will create a search index for that model.