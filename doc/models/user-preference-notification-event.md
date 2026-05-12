
# User Preference Notification Event

*This model accepts additional fields of type Any.*

## Structure

`UserPreferenceNotificationEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `user_preference_notification_event_type` | `str` | Required, Constant | **Value**: `"user.preference"` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "userPreferenceNotificationEventType": "user.preference",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

