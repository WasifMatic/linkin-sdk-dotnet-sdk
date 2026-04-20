
# Universal Product Code

The Universal Product Code of the item.

*This model accepts additional fields of type JsonValue.*

## Structure

`UniversalProductCode`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Type` | [`UpcType`](../../doc/models/upc-type.md) | Required | The Universal Product Code type.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `5`, *Pattern*: `^[0-9A-Z_-]+$` |
| `Code` | `string` | Required | The UPC product code of the item.<br><br>**Constraints**: *Minimum Length*: `6`, *Maximum Length*: `17`, *Pattern*: `^[0-9]{0,17}$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "type": "UPC-E",
  "code": "code2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

