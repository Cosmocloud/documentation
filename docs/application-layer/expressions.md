# Expressions

While writing expresseions is nodes such as `Build JSON` and `Merge JSON`, you would have to write the expression as a JSON object which would be evaluated to a value.

When you open the editor, to write the expressions, sample expression would look like -

```json
{
    "$add": [
        1, 2, { "$multiply": [1, 2] }, { "$subtract": [10, 5] }
    ]
}
```

The result of the above scenario would result to `10`.

You can use these expressions to do mathematical operations in your worklows.

## Examples

Lets say you need to calculate the total price of a product, which is calculated as `price * quantity` while building a JSON object in the flow (using `Build JSON` or `Merge JSON`)

```json
{
    "totalPrice":{
        "$multiply": [
            "$.request.body.price",
            "$.request.body.quantity",
            1.18                          // multiply TAX probably
        ]
    }
}
```

## Available Operators

- **$add**: Add all the values in the array
- **$subtract**: Subtract `value[0]` from `value[1]`
- **$multiply**: Multiply all the values in the array
- **$divide**: Divide `value[0]` by `value[1]`