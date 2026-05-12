
# Payment Completed Event

*This model accepts additional fields of type Any.*

## Structure

`PaymentCompletedEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `event_type` | [`EventType1`](../../doc/models/event-type-1.md) | Optional | - |
| `payment_id` | `int` | Required | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "paymentId": 91,
  "eventType": "payment.completed",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

