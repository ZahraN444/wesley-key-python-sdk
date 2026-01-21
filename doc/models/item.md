
# Item

## Structure

`Item`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `uuid\|str` | Required | - |
| `name` | `str` | Required | - |
| `date` | `date` | Required | - |
| `date_time` | `datetime` | Required | - |
| `decimal` | `float` | Required | - |
| `long` | `int` | Required | - |
| `bool` | `bool` | Required | - |
| `custom_enum` | [`CustomEnum`](../../doc/models/custom-enum.md) | Required | - |
| `status` | [`StatusEnum`](../../doc/models/status-enum.md) | Optional | - |
| `json_object` | `Any` | Required | A generic JSON object |
| `animal` | `Any` | Required | - |
| `map` | [`Dict[str, Message]`](../../doc/models/message.md) | Required | - |

## Example (as JSON)

```json
{
  "id": "550e8400-e29b-41d4-a716-446655440000",
  "name": "John Doe",
  "date": "2024-05-24",
  "dateTime": "05/24/2024 12:00:00",
  "decimal": 1234.56,
  "long": 1234567890123,
  "bool": true,
  "CustomEnum": "VALUE3",
  "jsonObject": {
    "key1": "val1",
    "key2": "val2"
  },
  "Animal": {
    "key1": "val1",
    "key2": "val2"
  },
  "Map": {
    "key0": {
      "code": 246,
      "text": "text4"
    },
    "key1": {
      "code": 246,
      "text": "text4"
    },
    "key2": {
      "code": 246,
      "text": "text4"
    }
  },
  "status": "active"
}
```

