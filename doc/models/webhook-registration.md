
# Webhook Registration

*This model accepts additional fields of type Any.*

## Structure

`WebhookRegistration`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `url` | `str` | Required | The endpoint URL that will receive webhook events |
| `events` | [`List[Event]`](../../doc/models/event.md) | Required | List of events to subscribe to |
| `secret` | `str` | Optional | Secret key for webhook signature verification |
| `active` | `bool` | Optional | Whether the webhook is active<br><br>**Default**: `True` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "url": "https://merchant.example.com/webhooks/events",
  "events": [
    "order.created",
    "payment.completed"
  ],
  "secret": "webhook_secret_key_123",
  "active": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

