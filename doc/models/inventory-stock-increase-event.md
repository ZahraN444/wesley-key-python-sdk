
# Inventory Stock Increase Event

*This model accepts additional fields of type Any.*

## Structure

`InventoryStockIncreaseEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `inventory_stock_increase_event_type` | `str` | Required, Constant | **Value**: `"stock.increase"` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "inventoryStockIncreaseEventType": "stock.increase",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

