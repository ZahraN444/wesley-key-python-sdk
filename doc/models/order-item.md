
# Order Item

*This model accepts additional fields of type Any.*

## Structure

`OrderItem`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `product_id` | `str` | Required | - |
| `quantity` | `int` | Required | **Constraints**: `>= 1` |
| `price` | `float` | Required | **Constraints**: `>= 0` |
| `description` | `str` | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "productId": "prod_001",
  "quantity": 2,
  "price": 29.99,
  "description": "Premium Widget",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

