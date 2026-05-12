
# System Alert Notification Event

*This model accepts additional fields of type Any.*

## Structure

`SystemAlertNotificationEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `system_alert_notification_event_type` | `str` | Required, Constant | **Value**: `"system.alert"` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "systemAlertNotificationEventType": "system.alert",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

