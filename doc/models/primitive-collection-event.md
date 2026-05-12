
# Primitive Collection Event

*This model accepts additional fields of type Any.*

## Structure

`PrimitiveCollectionEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `event_type` | [`EventType2`](../../doc/models/event-type-2.md) | Optional | - |
| `ids` | `List[int]` | Required | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "eventType": "primitive.variant",
  "ids": [
    77,
    78,
    79
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

