# Defining Model Schema

## What is a Model Schema ?

**Model schema** is a structured and organized set of rules, specifications, and definitions that define how data should be organized, stored, and managed within a software application or database. It serves as a blueprint that outlines the structure, data types, relationships, and constraints for the information that the application handles.

## Supported Data types in Model Schema

1. **ObjectID**: An ObjectID is a unique identifier often used in databases, particularly in MongoDB. It's a 12-byte identifier typically represented as a hexadecimal string. ObjectIDs are used to uniquely identify documents in a collection.

2. **Boolean**: A boolean data type represents two possible values: True or False. Booleans are often used to express binary decisions or states.

3. **String**: A string data type represents text. It can contain letters, numbers, symbols, and spaces. Strings are used to store textual information.

4. **Integer**: An integer data type represents whole numbers, both positive and negative, without decimal points. Integers are used for counting and calculations that involve whole quantities.

5. **Float**: A float data type represents decimal numbers. Unlike integers, floats can have fractional parts. They are used for calculations involving real numbers.

6. **Dict**: A dictionary is a collection of key-value pairs. Each key in the dictionary maps to a corresponding value. Dictionaries are used to store structured data and provide quick access to values based on their keys.

7. **Nested**: The "Nested" type typically refers to nested or embedded structures within a data model. This could involve nesting one set of attributes within another to represent more complex data relationships.

8. **Array**: An array is a collection of elements of the same data type, ordered by an index. Arrays are used to store multiple values in a single variable.

## Schema Layout

Let us assume we have a student data with given Schema that we need to store in database :

```json
{
    "id":{
        "type":"objectId",
        "required":true,
    },
    "name":{
       "type":"string",
       "required":true,
    },
    "age":{
        "type":"number",
        "required":true,
    },
    "subjects":{
        "type":"string[]",
        "required":true,
    },
    "address":{
        "city":{
            "type":"string",
            "required":true,
        },
        "state":{
            "type":"string",
            "required":true,
        }
    }

}
```

Schema given above would appear something like this in our user interface  

!["Student Model"](/assets/model/schema.png)
