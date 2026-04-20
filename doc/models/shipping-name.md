
# Shipping Name

The name of the party.

*This model accepts additional fields of type JsonValue.*

## Structure

`ShippingName`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `FullName` | `string` | Optional | When the party is a person, the party's full name.<br><br>**Constraints**: *Maximum Length*: `300` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "full_name": "full_name6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

