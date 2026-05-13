
# User

*This model accepts additional fields of type Any.*

## Structure

`User`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `int` | Optional | - |
| `username` | `str` | Optional | - |
| `first_name` | `str` | Optional | - |
| `last_name` | `str` | Optional | - |
| `email` | `str` | Optional | - |
| `password` | `str` | Optional | - |
| `phone` | `str` | Optional | - |
| `user_status` | `int` | Optional | User Status |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "id": 82,
  "username": "username6",
  "firstName": "firstName8",
  "lastName": "lastName0",
  "email": "email0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

