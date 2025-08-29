# API

```python
client_controller = client.client
```

## Class Name

`APIController`

## Methods

* [Createanitem](../../doc/controllers/api.md#createanitem)
* [Getanitemby ID](../../doc/controllers/api.md#getanitemby-id)
* [Create O Auth Token](../../doc/controllers/api.md#create-o-auth-token)
* [Test Endpointwith Arrays](../../doc/controllers/api.md#test-endpointwith-arrays)


# Createanitem

Creates a new resource in the system.

```python
def createanitem(self,
                status,
                body=None)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `status` | [`Status11Enum`](../../doc/models/status-11-enum.md) | Template, Required | The status of the items to filter by. |
| `body` | [`Item`](../../doc/models/item.md) | Body, Optional | Custom model with additional properties |

## Response Type

`Any`

## Example Usage

```python
status = Status11Enum.ENUMVALUE3

body = Item(
    id='550e8400-e29b-41d4-a716-446655440000',
    name='John Doe',
    date=dateutil.parser.parse('2024-05-24').date(),
    date_time=dateutil.parser.parse('05/24/2024 12:00:00'),
    decimal=1234.56,
    long=1234567890123,
    bool=True,
    custom_enum=CustomEnum.VALUE3,
    json_object={"key1":"val1","key2":"val2"},
    animal=jsonpickle.decode('{"key1":"val1","key2":"val2"}'),
    map={
        'key0': Message(
            code=246,
            text='text4'
        ),
        'key1': Message(
            code=246,
            text='text4'
        )
    }
)

result = client_controller.createanitem(
    status,
    body=body
)
print(result)
```

## Example Response

```
{
  "match": "client_mac",
  "name": "cameras",
  "type": "match",
  "values": [
    "010203040506",
    "abcdef*"
  ]
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Bad Syntax | `APIException` |
| 401 | Unauthorized | `APIException` |
| 403 | Permission Denied | `APIException` |


# Getanitemby ID

```python
def getanitemby_id(self,
                  id,
                  value)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `str` | Template, Required | The ID of the item to retrieve |
| `value` | `str` | Query, Required | The value of the item to retrieve |

## Response Type

[`Item`](../../doc/models/item.md)

## Example Usage

```python
id = 'id0'

value = 'value2'

result = client_controller.getanitemby_id(
    id,
    value
)
print(result)
```


# Create O Auth Token

Generates a new OAuth token with the specified scopes.

```python
def create_o_auth_token(self,
                       body=None)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`TokensRequest`](../../doc/models/tokens-request.md) | Body, Optional | - |

## Response Type

`void`

## Example Usage

```python
client_controller.create_o_auth_token()
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Bad request | `APIException` |


# Test Endpointwith Arrays

This endpoint accepts a complex structure with multiple arrays.

```python
def test_endpointwith_arrays(self,
                            body=None)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`MultipleArraysRequest`](../../doc/models/multiple-arrays-request.md) | Body, Optional | - |

## Response Type

`void`

## Example Usage

```python
client_controller.test_endpointwith_arrays()
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 400 | Bad request | `APIException` |

