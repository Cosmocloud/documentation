# Full Text Search

## What is Full-Text Search?

Full-text search is a specialized search technique that allows users to search for text within large amounts of textual data and retrieve relevant documents or records that contain the queried words or phrases. Unlike traditional search, which typically requires an exact match, full-text search enables users to find relevant information even if the search terms are not an exact match.

Traditional databases are primarily designed for structured data storage and retrieval, where queries are usually based on specific fields or values. While traditional databases can handle some text-based searching using techniques like wildcard or pattern matching, they are not optimized for efficient full-text search across extensive text data.

## Understanding full text search with an example

Let's assume we have a collection of students with various attributes such as name, age, email, student ID, height, and address. We want to query the students based on their names.

First, we need to index the collection by creating an index specifically for the name attribute. The index allows us to quickly locate documents that contain specific names without traversing the entire collection.

Here's an example of the initial collection of 4 students:

```
Alice (age: 20, email: alice@example.com, student ID: 1234, height: 165 cm, address: 123 Main St)
Bob (age: 22, email: bob@example.com, student ID: 5678, height: 170 cm, address: 456 Elm St)
Henry (age: 19, email: henry@example.com, student ID: 4321, height: 160 cm, address: 321 Pine St)
Bob (age: 21, email: bob2@example.com, student ID: 9876, height: 175 cm, address: 789 Oak St)
```

Once the indexing is completed, we would have separate indexes for each student's name:

```
Alice: [(age: 20, email: alice@example.com, student ID: 1234, height: 165 cm, address: 123 Main St)]
Bob: [
  Bob (age: 22, email: bob@example.com, student ID: 5678, height: 170 cm, address: 456 Elm St),
  Bob (age: 21, email: bob2@example.com, student ID: 9876, height: 175 cm, address: 789 Oak St)
]
Henry: [
  (age: 19, email: henry@example.com, student ID: 4321, height: 160 cm, address: 321 Pine St)
]
```

Now, when a user queries the students based on their names, we can utilize the name as an index to directly retrieve the relevant documents without having to traverse the entire collection. For example, if the user searches for the name "Bob," we can quickly access the collections associated with the name "Bob" through the corresponding index.

This approach significantly improves search performance as it avoids the need to scan every document in the collection. Instead, it leverages the index to pinpoint the relevant documents efficiently.

> However, indexing require some disk space and can consume a lot of resources when created and this was very basic example of indexing.

## Understanding the full-text search indexing process

Indexing is a crucial step in full-text search that allows for efficient retrieval of information from a collection of documents. While the previous example provided a basic understanding of indexing by focusing on indexing the "name" attribute, it's important to note that there are various indexing techniques available, each with its strengths and considerations.

The indexing process in full-text search is determined by the analyzer used. An analyzer is a component responsible for tokenizing the text, applying various transformations, and generating indexed terms.
[How to Create a Search Index?](/application-layer/full-text-search/create-search-index/)

## Processing data with Analyzers

Analyzers in Atlas Search are composed of a tokenizer, which extracts tokens from the text, and filters that you define. These filters are applied to the tokens, enabling the creation of indexable terms that account for variations in punctuation, capitalization, filler words, and more.

By configuring the analyzer for a specific field, you can define how the data is processed and transformed during the indexing process. This allows you to handle common challenges in full-text searches, such as case insensitivity, stop word removal, stemming, and more. The combination of tokenizer and filters in the analyzer ensures that the indexed terms accurately reflect the search requirements and provide relevant search results.
[How to Create a Custom Analyzer?](/application-layer/full-text-search/create-custom-analyzer/)
