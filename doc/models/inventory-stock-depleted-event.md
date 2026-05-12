
# Inventory Stock Depleted Event

*This model accepts additional fields of type Any.*

## Structure

`InventoryStockDepletedEvent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `inventory_stock_depleted_event_type` | `str` | Required, Constant | **Value**: `"stock.depleted"` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "inventoryStockDepletedEventType": "stock.depleted",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

