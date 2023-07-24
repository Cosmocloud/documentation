# Conditions

While writing conditions is nodes such as `If Else`, `If Else v2`, `Switch Case`, you would have to write a condition with which these nodes would resolve into `true` or `false`.

When you open the editor, to write the condition, you would have to write a condition in a JSON way -

```json
{
    "$and": [
        {
            "name": {
                "$eq": "John"
            }
        },
        {
            "age": {
                "$gt": 18
            }
        }
    ]
}
```

In the above scenario, we have 2 expressions, both of which have to be true as they are inside an `$and` condition.

## Simple conditions

A simple condition can be of the form - 
```json
{
    <key>: {
        <operator>: <value>
    }
}
```
### Available operators in the system are -

- **$eq**: Equal to
- **$neq**: Not equal to
- **$gt**: Greater than
- **$gte**: Greater than or equal to
- **$lt**: Less than
- **$lte**: Less than or equal to

## Building Complex Queries

Complex queries can be formed by using multiple simple or other complex queries, and joining each of them with `$and` or `$or`  operators.

Example - 

```json
{
    "$and": [
        {
            "name": {
                "$eq": "John"
            }
        },
        {
            "$or": [
                {
                    "$lte": 20
                },
                {
                    "$ne": "Hello"
                }
            ]
        }
    ]
}
```