
# Audit Log Event

*This model accepts additional fields of type Any.*

## Structure

`AuditLogEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `event_type` | [`EventType3`](../../doc/models/event-type-3.md) | Optional | - |
| `actor` | `str` | Optional | - |
| `action` | `str` | Optional | - |
| `context` | `Any` | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "eventType": "audit.log",
  "actor": "actor0",
  "action": "action2",
  "context": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

