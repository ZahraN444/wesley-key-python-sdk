
# Order

*This model accepts additional fields of type Any.*

## Structure

`Order`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `int` | Optional | - |
| `pet_id` | `int` | Optional | - |
| `quantity` | `int` | Optional | - |
| `ship_date` | `datetime` | Optional | - |
| `status` | [`OrderStatus`](../../doc/models/order-status.md) | Optional | Order Status |
| `complete` | `bool` | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "id": 180,
  "petId": 220,
  "quantity": 136,
  "shipDate": "2016-03-13T12:52:32.123Z",
  "status": "placed",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

