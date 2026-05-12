
# User Action Notification Event

*This model accepts additional fields of type Any.*

## Structure

`UserActionNotificationEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_action_notification_event_type` | `str` | Required, Constant | **Value**: `"user.action"` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "userActionNotificationEventType": "user.action",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

