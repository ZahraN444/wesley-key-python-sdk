
# Multiple Arrays Request

## Structure

`MultipleArraysRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `array_1` | `List[str]` | Required | An array containing items of type string |
| `array_2` | `List[int]` | Optional | An array containing items of type integer |

## Example (as JSON)

```json
{
  "Array1": [
    "Array19",
    "Array10"
  ],
  "Array2": [
    99,
    98,
    97
  ]
}
```

