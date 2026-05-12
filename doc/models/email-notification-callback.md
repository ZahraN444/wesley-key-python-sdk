
# Email Notification Callback

*This model accepts additional fields of type Any.*

## Structure

`EmailNotificationCallback`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `message_id` | `str` | Optional | - |
| `recipient_email` | `str` | Optional | - |
| `status` | [`Status1`](../../doc/models/status-1.md) | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "messageId": "msg_001",
  "recipientEmail": "user@example.com",
  "status": "sent",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

