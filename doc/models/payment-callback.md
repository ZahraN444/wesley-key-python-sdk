
# Payment Callback

*This model accepts additional fields of type Any.*

## Structure

`PaymentCallback`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `order_id` | `str` | Required | - |
| `payment_status` | [`PaymentStatus`](../../doc/models/payment-status.md) | Required | - |
| `transaction_id` | `str` | Required | - |
| `amount` | `float` | Optional | - |
| `currency` | `str` | Optional | - |
| `timestamp` | `datetime` | Optional | - |
| `failure_reason` | `str` | Optional | Reason for payment failure (if applicable) |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "orderId": "order_789",
  "paymentStatus": "success",
  "transactionId": "txn_abc123",
  "amount": 59.98,
  "currency": "USD",
  "timestamp": "09/19/2025 10:35:00",
  "failureReason": "failureReason0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

