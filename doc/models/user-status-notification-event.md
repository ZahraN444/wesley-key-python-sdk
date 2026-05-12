
# User Status Notification Event

*This model accepts additional fields of type Any.*

## Structure

`UserStatusNotificationEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_status_notification_event_type` | `str` | Required, Constant | **Value**: `"user.status"` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "userStatusNotificationEventType": "user.status",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

