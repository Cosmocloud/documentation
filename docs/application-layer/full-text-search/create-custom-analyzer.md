# Creating a Custom Analyzer

- Browse to **Full Text Search** --> **Custom Analyzers** and you will see a list of custom analyzers if there will be any.

    ![Custom Analyzers list](/assets/fts/search-index/dynamic_field_mapping.webp) 

- On the top right corner of this page, click on **Create Custom Analyzer** button to create a custom analyzer.

- It will open a form to create the custom analyzer. Provide a name for the analyzer and select the tokenizer type and also fill in the required tokenizer properties.

    A **Tokenizer** determines how Atlas Search splits up text into discrete chunks for indexing. Tokenizers require the type of tokenizer and some tokenizers have additional properties as well.

    [Read More about the tokenizers](https://www.mongodb.com/docs/atlas/atlas-search/analyzers/tokenizers/)

- After selecting the tokenizer type and filling in the tokenizer properties(if any), click on **Create** button to create the Custom Analyzer.

<iframe src="https://drive.google.com/file/d/1Bbq7DejV7Pwso-hLyyU0bfsTIEHfcWcH/preview" width="720" height="410" allow="autoplay"></iframe>