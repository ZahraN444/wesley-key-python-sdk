
# Payment Status Created Event

*This model accepts additional fields of type Any.*

## Structure

`PaymentStatusCreatedEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `payment_status_created_id` | `str` | Required | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "paymentStatusCreatedId": "ps_123",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

