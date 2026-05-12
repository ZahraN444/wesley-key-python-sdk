
# Webhook Update

*This model accepts additional fields of type Any.*

## Structure

`WebhookUpdate`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `url` | `str` | Optional | - |
| `events` | `List[str]` | Optional | - |
| `secret` | `str` | Optional | - |
| `active` | `bool` | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "url": "url6",
  "events": [
    "events8",
    "events9"
  ],
  "secret": "secret2",
  "active": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

