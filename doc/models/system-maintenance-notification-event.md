
# System Maintenance Notification Event

*This model accepts additional fields of type Any.*

## Structure

`SystemMaintenanceNotificationEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `system_maintenance_notification_event_type` | `str` | Required, Constant | **Value**: `"system.maintenance"` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "systemMaintenanceNotificationEventType": "system.maintenance",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

