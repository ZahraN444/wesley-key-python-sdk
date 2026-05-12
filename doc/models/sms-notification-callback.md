
# Sms Notification Callback

*This model accepts additional fields of type Any.*

## Structure

`SmsNotificationCallback`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `message_id` | `str` | Optional | - |
| `phone_number` | `str` | Optional | - |
| `status` | [`Status2`](../../doc/models/status-2.md) | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "messageId": "sms_002",
  "phoneNumber": "+15551234567",
  "status": "delivered",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

