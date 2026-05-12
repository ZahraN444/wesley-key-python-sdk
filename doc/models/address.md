
# Address

*This model accepts additional fields of type Any.*

## Structure

`Address`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `street` | `str` | Required | - |
| `city` | `str` | Required | - |
| `zip` | `str` | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "street": "123 Main St",
  "city": "New York",
  "zip": "10001",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

